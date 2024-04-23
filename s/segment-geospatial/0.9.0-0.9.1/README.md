# Comparing `tmp/segment-geospatial-0.9.0.tar.gz` & `tmp/segment-geospatial-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.9.0.tar", last modified: Sun Aug  6 19:29:17 2023, max compression
+gzip compressed data, was "segment-geospatial-0.9.1.tar", last modified: Tue Aug 15 03:46:51 2023, max compression
```

## Comparing `segment-geospatial-0.9.0.tar` & `segment-geospatial-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:17.059663 segment-geospatial-0.9.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96991 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/samgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/text_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 03:46:51.046851 segment-geospatial-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-15 03:46:51.046851 segment-geospatial-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 03:46:51.046851 segment-geospatial-0.9.1/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99553 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33893 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/samgeo/hq_sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 03:46:51.046851 segment-geospatial-0.9.1/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-15 03:46:50.000000 segment-geospatial-0.9.1/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-15 03:46:50.000000 segment-geospatial-0.9.1/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-15 03:46:50.000000 segment-geospatial-0.9.1/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 03:46:50.000000 segment-geospatial-0.9.1/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-15 03:46:50.000000 segment-geospatial-0.9.1/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-15 03:46:50.000000 segment-geospatial-0.9.1/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-15 03:46:51.046851 segment-geospatial-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-15 03:46:42.000000 segment-geospatial-0.9.1/setup.py
```

### Comparing `segment-geospatial-0.9.0/LICENSE` & `segment-geospatial-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.9.0/PKG-INFO` & `segment-geospatial-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.9.0
+Version: 0.9.1
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -44,15 +44,15 @@
 ## Citations
 
 -   Qiusheng Wu, & Lucas Osco. (2023). samgeo: A Python package for segmenting geospatial data with the Segment Anything Model (SAM). Zenodo. <https://doi.org/10.5281/zenodo.7966658>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
--   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Segment GeoTIFF files using the Segment Anything Model ([SAM](https://github.com/facebookresearch/segment-anything)) and [HQ-SAM](https://github.com/SysCV/sam-hq)
 -   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
```

### Comparing `segment-geospatial-0.9.0/README.md` & `segment-geospatial-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ## Citations
 
 -   Qiusheng Wu, & Lucas Osco. (2023). samgeo: A Python package for segmenting geospatial data with the Segment Anything Model (SAM). Zenodo. <https://doi.org/10.5281/zenodo.7966658>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
--   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Segment GeoTIFF files using the Segment Anything Model ([SAM](https://github.com/facebookresearch/segment-anything)) and [HQ-SAM](https://github.com/SysCV/sam-hq)
 -   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
```

### Comparing `segment-geospatial-0.9.0/samgeo/common.py` & `segment-geospatial-0.9.1/samgeo/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,78 @@
                 zip_ref.extractall(output)
             else:
                 zip_ref.extractall(os.path.dirname(output))
 
     return os.path.abspath(output)
 
 
-def download_checkpoint(url=None, output=None, overwrite=False, **kwargs):
+def download_checkpoint(model_type="vit_h", checkpoint_dir=None, hq=False):
+    """Download the SAM model checkpoint.
+
+    Args:
+        model_type (str, optional): The model type. Can be one of ['vit_h', 'vit_l', 'vit_b'].
+            Defaults to 'vit_h'. See https://bit.ly/3VrpxUh for more details.
+        checkpoint_dir (str, optional): The checkpoint_dir directory. Defaults to None, "~/.cache/torch/hub/checkpoints".
+        hq (bool, optional): Whether to use HQ-SAM model (https://github.com/SysCV/sam-hq). Defaults to False.
+    """
+
+    if not hq:
+        model_types = {
+            "vit_h": {
+                "name": "sam_vit_h_4b8939.pth",
+                "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
+            },
+            "vit_l": {
+                "name": "sam_vit_l_0b3195.pth",
+                "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
+            },
+            "vit_b": {
+                "name": "sam_vit_b_01ec64.pth",
+                "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
+            },
+        }
+    else:
+        model_types = {
+            "vit_h": {
+                "name": "sam_hq_vit_h.pth",
+                "url": "https://drive.google.com/file/d/1qobFYrI4eyIANfBSmYcGuWRaSIXfMOQ8/view?usp=sharing",
+            },
+            "vit_l": {
+                "name": "sam_hq_vit_l.pth",
+                "url": "https://drive.google.com/file/d/1Uk17tDKX1YAKas5knI4y9ZJCo0lRVL0G/view?usp=sharing",
+            },
+            "vit_b": {
+                "name": "sam_hq_vit_b.pth",
+                "url": "https://drive.google.com/file/d/11yExZLOve38kRZPfRx_MRxfIAKmfMY47/view?usp=sharing",
+            },
+            "vit_tiny": {
+                "name": "sam_hq_vit_tiny.pth",
+                "url": "https://huggingface.co/lkeab/hq-sam/resolve/main/sam_hq_vit_tiny.pth",
+            },
+        }
+
+    if model_type not in model_types:
+        raise ValueError(
+            f"Invalid model_type: {model_type}. It must be one of {', '.join(model_types)}"
+        )
+
+    if checkpoint_dir is None:
+        checkpoint_dir = os.environ.get(
+            "TORCH_HOME", os.path.expanduser("~/.cache/torch/hub/checkpoints")
+        )
+
+    checkpoint = os.path.join(checkpoint_dir, model_types[model_type]["name"])
+    if not os.path.exists(checkpoint):
+        print(f"Model checkpoint for {model_type} not found.")
+        url = model_types[model_type]["url"]
+        download_file(url, checkpoint)
+    return checkpoint
+
+
+def download_checkpoint_legacy(url=None, output=None, overwrite=False, **kwargs):
     """Download a checkpoint from URL. It can be one of the following: sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
 
     Args:
         url (str, optional): The checkpoint URL. Defaults to None.
         output (str, optional): The output file path. Defaults to None.
         overwrite (bool, optional): Overwrite the file if it already exists. Defaults to False.
```

### Comparing `segment-geospatial-0.9.0/samgeo/samgeo.py` & `segment-geospatial-0.9.1/samgeo/hq_sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """
-The source code is adapted from https://github.com/aliaksandr960/segment-anything-eo. Credit to the author Aliaksandr Hancharenka.
+Segment remote sensing imagery with HQ-SAM (High Quality Segment Anything Model).
+See https://github.com/SysCV/sam-hq
 """
 
 import os
 import cv2
 import torch
 import numpy as np
-from segment_anything import sam_model_registry, SamAutomaticMaskGenerator, SamPredictor
+from segment_anything_hq import sam_model_registry, SamAutomaticMaskGenerator, SamPredictor
 
 from .common import *
 
 
 class SamGeo:
     """The main class for segmenting geospatial data with the Segment Anything Model (SAM). See
     https://github.com/facebookresearch/segment-anything for details.
     """
 
     def __init__(
         self,
         model_type="vit_h",
-        checkpoint=None,
         automatic=True,
         device=None,
+        checkpoint_dir=None,
+        hq=False,
         sam_kwargs=None,
+        **kwargs,
     ):
         """Initialize the class.
 
         Args:
             model_type (str, optional): The model type. It can be one of the following: vit_h, vit_l, vit_b.
                 Defaults to 'vit_h'. See https://bit.ly/3VrpxUh for more details.
-            checkpoint (str, optional): The path to the model checkpoint. It can be one of the following:
-                sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
-                Defaults to None. See https://bit.ly/3VrpxUh for more details.
             automatic (bool, optional): Whether to use the automatic mask generator or input prompts. Defaults to True.
                 The automatic mask generator will segment the entire image, while the input prompts will segment selected objects.
             device (str, optional): The device to use. It can be one of the following: cpu, cuda.
                 Defaults to None, which will use cuda if available.
+            hq (bool, optional): Whether to use the HQ-SAM model. Defaults to False.
+            checkpoint_dir (str, optional): The path to the model checkpoint. It can be one of the following:
+                sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
+                Defaults to None. See https://bit.ly/3VrpxUh for more details.
             sam_kwargs (dict, optional): Optional arguments for fine-tuning the SAM model. Defaults to None.
                 The available arguments with default values are listed below. See https://bit.ly/410RV0v for more details.
 
                 points_per_side: Optional[int] = 32,
                 points_per_batch: int = 64,
                 pred_iou_thresh: float = 0.88,
                 stability_score_thresh: float = 0.95,
@@ -50,49 +54,23 @@
                 crop_overlap_ratio: float = 512 / 1500,
                 crop_n_points_downscale_factor: int = 1,
                 point_grids: Optional[List[np.ndarray]] = None,
                 min_mask_region_area: int = 0,
                 output_mode: str = "binary_mask",
 
         """
-        # Download the checkpoint if it does not exist
-        CACHE_PATH = os.environ.get(
-            "TORCH_HOME", os.path.expanduser("~/.cache/torch/hub/checkpoints")
-        )
-
-        model_types = {
-            "vit_h": "sam_vit_h_4b8939.pth",
-            "vit_l": "sam_vit_l_0b3195.pth",
-            "vit_b": "sam_vit_b_01ec64.pth",
-        }
-
-        if model_type not in model_types:
-            raise ValueError(
-                f"Model type {model_type} is not supported. It must be one of the following: {model_types}."
-            )
-
-        checkpoints = {
-            "sam_vit_h_4b8939.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
-            "sam_vit_l_0b3195.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
-            "sam_vit_b_01ec64.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
-        }
-
-        if checkpoint is None:
-            url = checkpoints[model_types[model_type]]
-            checkpoint = model_types[model_type]
-        else:
-            url = None
 
-        if not os.path.exists(checkpoint):
-            basename = os.path.basename(checkpoint)
-            checkpoint = os.path.join(CACHE_PATH, basename)
+        hq = True  # Using HQ-SAM
+        if "checkpoint" in kwargs:
+            checkpoint = kwargs["checkpoint"]
             if not os.path.exists(checkpoint):
-                print(f"Checkpoint {checkpoint} does not exist.")
-                download_checkpoint(url=url, output=checkpoint)
-        self.checkpoint = checkpoint
+                checkpoint = download_checkpoint(model_type, checkpoint_dir, hq)
+            kwargs.pop("checkpoint")
+        else:
+            checkpoint = download_checkpoint(model_type, checkpoint_dir, hq)
 
         # Use cuda if available
         if device is None:
             device = "cuda" if torch.cuda.is_available() else "cpu"
             if device == "cuda":
                 torch.cuda.empty_cache()
```

### Comparing `segment-geospatial-0.9.0/samgeo/text_sam.py` & `segment-geospatial-0.9.1/samgeo/text_sam.py`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.9.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.9.1/segment_geospatial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.9.0
+Version: 0.9.1
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -44,15 +44,15 @@
 ## Citations
 
 -   Qiusheng Wu, & Lucas Osco. (2023). samgeo: A Python package for segmenting geospatial data with the Segment Anything Model (SAM). Zenodo. <https://doi.org/10.5281/zenodo.7966658>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
--   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Segment GeoTIFF files using the Segment Anything Model ([SAM](https://github.com/facebookresearch/segment-anything)) and [HQ-SAM](https://github.com/SysCV/sam-hq)
 -   Segment remote sensing imagery with text prompts
 -   Create foreground and background markers interactively
 -   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
```

### Comparing `segment-geospatial-0.9.0/setup.py` & `segment-geospatial-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.9.0',
+    version='0.9.1',
     zip_safe=False,
 )
```

