# Comparing `tmp/detectools-0.1.1.tar.gz` & `tmp/detectools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detectools-0.1.1.tar", last modified: Fri Apr 19 13:01:20 2024, max compression
+gzip compressed data, was "detectools-0.1.2.tar", last modified: Tue Apr 23 09:25:00 2024, max compression
```

## Comparing `detectools-0.1.1.tar` & `detectools-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.612008 detectools-0.1.1/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    34523 2024-04-17 14:19:07.000000 detectools-0.1.1/LICENSE.txt
--rw-r--r--   0 jbernigauds  (1000) jbernigauds  (1000)    41762 2024-04-19 13:01:20.612008 detectools-0.1.1/PKG-INFO
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1637 2024-04-19 12:53:28.000000 detectools-0.1.1/README.md
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      817 2024-04-17 14:23:50.000000 detectools-0.1.1/README_deployment.md
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1349 2024-04-17 14:17:38.000000 detectools-0.1.1/pyproject.toml
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)       38 2024-04-19 13:01:20.612008 detectools-0.1.1/setup.cfg
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      145 2024-04-19 12:53:28.000000 detectools-0.1.1/setup.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.592007 detectools-0.1.1/src/
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.596007 detectools-0.1.1/src/detectools/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2051 2024-04-19 13:01:00.000000 detectools-0.1.1/src/detectools/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2417 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/augmentation.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    10779 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/dataset.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.604008 detectools-0.1.1/src/detectools/formats/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     3989 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/formats/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    13184 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/formats/base.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     7159 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/formats/detection_format.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     7015 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/formats/mask.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     9732 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/formats/segmentation_format.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     6500 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/inference.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2209 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/metrics.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.608008 detectools-0.1.1/src/detectools/models/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      330 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/models/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2641 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/models/base.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    11002 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/models/mask2former.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    10950 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/models/yolo.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    16594 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/models/yolov8_seg.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     8112 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/trainer.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.608008 detectools-0.1.1/src/detectools/utils/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     3401 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/data_management.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     6207 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/inference.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2775 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/mask_utils.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    15905 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/metrics.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1202 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/trainer.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     4081 2024-04-19 12:53:28.000000 detectools-0.1.1/src/detectools/utils/visualisation.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-04-19 13:01:20.608008 detectools-0.1.1/src/detectools.egg-info/
--rw-r--r--   0 jbernigauds  (1000) jbernigauds  (1000)    41762 2024-04-19 13:01:20.000000 detectools-0.1.1/src/detectools.egg-info/PKG-INFO
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1016 2024-04-19 13:01:20.000000 detectools-0.1.1/src/detectools.egg-info/SOURCES.txt
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)        1 2024-04-19 13:01:20.000000 detectools-0.1.1/src/detectools.egg-info/dependency_links.txt
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      152 2024-04-19 13:01:20.000000 detectools-0.1.1/src/detectools.egg-info/requires.txt
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)       11 2024-04-19 13:01:20.000000 detectools-0.1.1/src/detectools.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1087 2024-03-21 13:04:40.000000 detectools-0.1.2/LICENSE.txt
+-rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-23 09:25:00.256460 detectools-0.1.2/PKG-INFO
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1637 2024-03-21 11:28:28.000000 detectools-0.1.2/README.md
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      599 2024-04-17 13:45:59.000000 detectools-0.1.2/README_deployment.md
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1442 2024-04-23 09:24:44.000000 detectools-0.1.2/pyproject.toml
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       38 2024-04-23 09:25:00.256460 detectools-0.1.2/setup.cfg
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      145 2024-03-21 13:29:41.000000 detectools-0.1.2/setup.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.252460 detectools-0.1.2/src/
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.252460 detectools-0.1.2/src/detectools/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2051 2024-04-23 09:14:32.000000 detectools-0.1.2/src/detectools/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2417 2024-04-17 12:26:22.000000 detectools-0.1.2/src/detectools/augmentation.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    10779 2024-04-18 14:52:14.000000 detectools-0.1.2/src/detectools/dataset.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools/formats/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3989 2024-03-21 11:28:28.000000 detectools-0.1.2/src/detectools/formats/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    13184 2024-04-19 11:34:07.000000 detectools-0.1.2/src/detectools/formats/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     7175 2024-04-23 07:27:53.000000 detectools-0.1.2/src/detectools/formats/detection_format.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     7057 2024-04-23 08:35:56.000000 detectools-0.1.2/src/detectools/formats/mask.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     9748 2024-04-23 07:27:33.000000 detectools-0.1.2/src/detectools/formats/segmentation_format.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     6555 2024-04-22 14:49:17.000000 detectools-0.1.2/src/detectools/inference.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2209 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/metrics.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools/models/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      330 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/models/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2641 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/models/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    11002 2024-04-17 09:16:04.000000 detectools-0.1.2/src/detectools/models/mask2former.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    10950 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/models/yolo.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    16594 2024-04-16 14:42:36.000000 detectools-0.1.2/src/detectools/models/yolov8_seg.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     8112 2024-04-16 07:53:15.000000 detectools-0.1.2/src/detectools/trainer.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools/utils/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)        0 2024-03-21 13:12:26.000000 detectools-0.1.2/src/detectools/utils/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3401 2024-04-16 11:03:27.000000 detectools-0.1.2/src/detectools/utils/data_management.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     6207 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/utils/inference.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2775 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/utils/mask_utils.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    15905 2024-04-16 11:21:48.000000 detectools-0.1.2/src/detectools/utils/metrics.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1202 2024-03-21 11:28:28.000000 detectools-0.1.2/src/detectools/utils/trainer.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     4708 2024-04-23 09:04:07.000000 detectools-0.1.2/src/detectools/utils/visualisation.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools.egg-info/
+-rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1016 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)        1 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      218 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       11 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/top_level.txt
```

### Comparing `detectools-0.1.1/README.md` & `detectools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/README_deployment.md` & `detectools-0.1.2/README_deployment.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,8 @@
 
 Source code  documentation will be accessible soon.
 
 ## Installation
 
 ```shell
 pip install detectools
-```
-
-## Citations
-
-detectools wrap several models from other sources. Please, if you use :
-- Yolo models : cite ultralytics
-- Mask2former : cite huggingface and transformers   (these are both open source python packages)
+```
```

### Comparing `detectools-0.1.1/pyproject.toml` & `detectools-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,21 @@
     ]
 
 dynamic = ["version"]
 requires-python = ">=3.10.12"
 
 dependencies = [
     "computervisiontools",
+    "matplotlib==3.8.2",
     "torch==2.1.0",
     "torchvision==0.16.0",
+    "pandas==2.1.4",
     "tensorboard==2.15.1",
+    "XlsxWriter==3.1.9",
+    "seaborn==0.13.0",
     "pycocotools==2.0.7",
     "torchmetrics==1.3.0",
     "ultralytics==8.1.7",
     "transformers==4.39.2"
 ]
 
 license = {file = "LICENSE.txt"}
@@ -40,8 +44,8 @@
 Homepage = "https://forgemia.inra.fr/ue-apc/librairies/python/detectools"
 Issues = "https://forgemia.inra.fr/ue-apc/librairies/python/detectools/-/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
-version = {attr = "detectools.__version__"}
+version = {attr = "detectools.__version__"}
```

### Comparing `detectools-0.1.1/src/detectools/__init__.py` & `detectools-0.1.2/src/detectools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Torch prebuild functions to train, evaluate and use models in production."""
 import json
 import os
 import sys
 from pathlib import Path
 from typing import Any, Dict, Literal, Union
 
-__version__ = "0.1.1" # change detectools version here
+__version__ = "0.1.2" # change detectools version here
 
 IMAGE_FOLDER = "images"
 ANNOTATION_FILE = "coco_annotations.json"
 
 COLORS = [
     (0, 102, 204),
     (51, 255, 51),
```

### Comparing `detectools-0.1.1/src/detectools/augmentation.py` & `detectools-0.1.2/src/detectools/augmentation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/dataset.py` & `detectools-0.1.2/src/detectools/dataset.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/formats/__init__.py` & `detectools-0.1.2/src/detectools/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/formats/base.py` & `detectools-0.1.2/src/detectools/formats/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/formats/detection_format.py` & `detectools-0.1.2/src/detectools/formats/detection_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
     def get_object(self, indice: int) -> DetectionAnnotation:
         """Return a DetectionAnnotation object at position indice."""
         single_object_format = self[indice]
         bbox, label = single_object_format.get("boxes", "labels")
         detection_object = DetectionAnnotation(self.spatial_size, label, bbox.squeeze())
         if "scores" in single_object_format:
-            detection_object.score = self.get("scores")
+            detection_object.score = single_object_format.get("scores")
 
         return detection_object
 
     # Methods that changes internal states of Formats
     # override
     def crop(self, top: int, left: int, height: int, width: int):
         """Crop boxes and update spatial size."""
```

### Comparing `detectools-0.1.1/src/detectools/formats/mask.py` & `detectools-0.1.2/src/detectools/formats/mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             indexes = torch.tensor(list(range(self.n_objects))[indexes])
 
         if indexes.dtype == torch.bool:
             indexes = indexes.nonzero().flatten()
         
         assert torch.sum(indexes > self.n_objects) == 0, f"Some indexes are higher than the number of objects in mask: indexes {indexes} & number of objects: {self.n_objects}"
         get_mask = DetectMask(self._mask)
-        retrieve_mask = torch.isin(get_mask._mask, indexes + 1) # 1 to avoid background 0
+        retrieve_mask = torch.isin(get_mask._mask, indexes.to(get_mask.device) + 1) # 1 to avoid background 0
         get_mask = DetectMask(torch.where(retrieve_mask, get_mask._mask, 0))
         get_mask.reindex()
 
         return get_mask
     
     def __iter__(self):
         """Iterate over Mask return binary mask for each value in 1-N range with N objects. Do not iter over
@@ -151,22 +151,22 @@
         _, indices = torch.sort(merged_scores)
         merged_mask = DetectMask(torch.zeros(mask._mask.shape, device=mask.device).long())
         value = 1
         valid_indices = []
 
         for i in indices:
             if i > torch.max(mask._mask):
-                indice_mask = other_mask._mask[i] * value
+                indice_mask = (other_mask._mask == i + 1) * value
             else:
-                indice_mask = mask[i]._mask * value
+                indice_mask = (mask._mask == i + 1) * value
             # do not add empty masks
             if indice_mask.sum() == 0:
                 continue
             
-            merged_mask._mask[indice_mask > 0] = indice_mask[indice_mask > 0]
+            merged_mask._mask[indice_mask > 0] = indice_mask[indice_mask > 0].int()
 
             value += 1
             valid_indices.append(i)
 
         return merged_mask, torch.tensor(valid_indices)
```

### Comparing `detectools-0.1.1/src/detectools/formats/segmentation_format.py` & `detectools-0.1.2/src/detectools/formats/segmentation_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         """Return a SegmentationAnnotation object at position indice."""
         single_object_format = self[indice]
         bbox, label, mask = single_object_format.get("boxes", "labels", "masks")
         segmentation_object = SegmentationAnnotation(
             self.spatial_size, label, bbox.squeeze(), mask._mask
         )
         if "scores" in single_object_format:
-            segmentation_object.score = self.get("scores")
+            segmentation_object.score = single_object_format.get("scores")
 
         return segmentation_object
 
     # Methods that changes internal states of Formats
     def crop(self, top: int, left: int, height: int, width: int):
         """Crop boxes and mask and update spatial size."""
         self.spatial_size = (height, width)
```

### Comparing `detectools-0.1.1/src/detectools/inference.py` & `detectools-0.1.2/src/detectools/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from math import ceil
 from typing import Callable, List, Literal, Tuple, Union
 
 import detectools.utils.inference as I
+import torch
 from computervisiontools import load_image, save_image
 from computervisiontools.preprocessing import build_preprocessing
 from detectools.formats import Format
 from detectools.models.base import BaseModel
 from detectools.utils.visualisation import visualisation
 from torch import Tensor
 from torch.utils.data import DataLoader, TensorDataset
@@ -109,17 +110,18 @@
 
         Args:
             batch_patchs (Tensor):Batch of image patches.
 
         Returns:
             List[Format]: Patches predictions.
         """
-        predictions = self.model.get_predictions(batch_patchs)
-        # split in N predictions for N == batch size (avoid forgetting empty predictions)
-        return predictions.split()
+        with torch.no_grad():
+            predictions = self.model.get_predictions(batch_patchs)
+            # split in N predictions for N == batch size (avoid forgetting empty predictions)
+            return predictions.split()
 
     def predict(
         self, image: Union[Tensor, str], visualisation_path: str = ""
     ) -> Format:
         """Predict a segmentation mask from RGB image.
 
         Args:
```

### Comparing `detectools-0.1.1/src/detectools/metrics.py` & `detectools-0.1.2/src/detectools/metrics.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/models/base.py` & `detectools-0.1.2/src/detectools/models/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/models/mask2former.py` & `detectools-0.1.2/src/detectools/models/mask2former.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/models/yolo.py` & `detectools-0.1.2/src/detectools/models/yolo.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/models/yolov8_seg.py` & `detectools-0.1.2/src/detectools/models/yolov8_seg.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/trainer.py` & `detectools-0.1.2/src/detectools/trainer.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/utils/data_management.py` & `detectools-0.1.2/src/detectools/utils/data_management.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/utils/inference.py` & `detectools-0.1.2/src/detectools/utils/inference.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/utils/mask_utils.py` & `detectools-0.1.2/src/detectools/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/utils/metrics.py` & `detectools-0.1.2/src/detectools/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/utils/trainer.py` & `detectools-0.1.2/src/detectools/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.1/src/detectools/utils/visualisation.py` & `detectools-0.1.2/src/detectools/utils/visualisation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import List, Union, Tuple
 
 from detectools import COLORS
 from detectools.formats import BaseFormat, BaseAnnotation, SegmentationAnnotation, SegmentationFormat
 from torch import Tensor
 from torchvision.transforms.v2 import ConvertBoundingBoxFormat
 from torchvision.utils import draw_bounding_boxes, draw_segmentation_masks
+import random as rd
 
 
-def draw_object(image: Tensor, obj: BaseAnnotation, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS) -> Tensor:
+def draw_object(image: Tensor, obj: BaseAnnotation, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS,  color_objects: bool=False) -> Tensor:
     """Draw bounding boxe & mask to image.
 
     Args:
         image (Tensor): Tensor image (uint8 & RGB)
         obj (Union[Annotation]): Annotation to draw.
         classes ( List[str]) : Names of classes to draw.  Defaults to [].
         colors (List[Tuple[int, int, int]]): List of colors for visualisations.
+        color_objects (bool): If True a random color is applied to each object instead of one color/label.
 
     Returns:
         Tensor: Image with object box drawed on.
     """
     # convert box for torch drawing bb
     format_converter = ConvertBoundingBoxFormat("XYXY")
     # wrap in object data in list
@@ -39,22 +41,23 @@
     if isinstance(obj, SegmentationAnnotation):
         image = draw_segmentation_masks(image, obj.masks)
 
 
     return image
 
 
-def draw_objects(image: Tensor, objects: BaseFormat, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS):
+def draw_objects(image: Tensor, objects: BaseFormat, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS, color_objects: bool=False):
     """Draw all bounding boxes of an object on image.
 
     Args:
         image (Tensor): Tensor image (uint8 & RGB)
         objects (DetectionTarget): DetectionTargets to draw.
         classes (List[str], optional): Names of classes to draw. Defaults to [].
         colors (List[Tuple[int, int, int]]): List of colors for visualisations.
+        color_objects (bool): If True a random color is applied to each object instead of one color/label.
 
 
     Returns:
         Tensor: Image with objects boxes drawed on.
     """
     # convert boxes format
     labels, boxes = objects.get("labels", "boxes")
@@ -69,44 +72,50 @@
     if "scores" in objects:
         new_upstrings = []
         scores = objects.get("scores")
         for i, string in enumerate(upstring):
             new_upstrings.append(f"{string} - {round(scores[i].item(), 2)}")
         upstring = new_upstrings
     # set COLORS according to classes
-    import random as rd
-    colors = [colors[rd.randint(0, len(colors)-1)] for label in labels]
+    if color_objects:
+        colors = [colors[rd.randint(0, len(colors)-1)] for label in labels]
+    else:
+        colors = [colors[label] for label in labels]
     # draw objects on image
     image = draw_bounding_boxes(image, boxes, upstring, colors, width=6)
 
     if isinstance(objects, SegmentationFormat) and objects.size != 0:
+        image.to("cpu") # limit GPU memory usage by switching to CPU
+        objects.set_device("cpu")
         masks = objects.get("masks").to_binary_masks()
         image = draw_segmentation_masks(image, masks.bool(), colors=colors, alpha=0.5)
 
     return image
 
 
 def visualisation(
     image: Tensor,
     target: Union[BaseFormat, SegmentationFormat],
     classes: List[str] = [],
-    colors: List[Tuple[int, int, int]]=COLORS
+    colors: List[Tuple[int, int, int]]=COLORS,
+    color_objects: bool = False
 ) -> Tensor:
     """Draw boxe(s) on image from DetectionTarget or DetectionObject.
 
     Args:
         image (Tensor): _description_
         objects (Union[DetectionTarget, DetectionObject]): _description_
         classes (List[str], optional): _description_. Defaults to [].
         colors (List[Tuple[int, int, int]]): List of colors for visualisations.
+        color_objects (bool): If True a random color is applied to each object instead of one color/label.
     Returns:
         Tensor: Image with objects boxes drawed on.
     """
 
     if isinstance(target, BaseAnnotation):
         image = draw_object(image, target, classes, colors)
 
     if isinstance(target, BaseFormat):
         if target.size > 0:
-            image = draw_objects(image, target, classes, colors)
+            image = draw_objects(image, target, classes, colors, color_objects=color_objects)
 
     return image
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `detectools-0.1.1/src/detectools.egg-info/SOURCES.txt` & `detectools-0.1.2/src/detectools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

