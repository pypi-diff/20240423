# Comparing `tmp/od_metrics-1.0.2.tar.gz` & `tmp/od_metrics-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "od_metrics-1.0.2.tar", last modified: Fri Apr 12 21:44:52 2024, max compression
+gzip compressed data, was "od_metrics-1.1.0.tar", last modified: Mon Apr 22 22:59:50 2024, max compression
```

## Comparing `od_metrics-1.0.2.tar` & `od_metrics-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.742132 od_metrics-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-12 21:44:42.000000 od_metrics-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5463 2024-04-12 21:44:52.742132 od_metrics-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4939 2024-04-12 21:44:42.000000 od_metrics-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-12 21:44:42.000000 od_metrics-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-12 21:44:52.742132 od_metrics-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-12 21:44:42.000000 od_metrics-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.738132 od_metrics-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.738132 od_metrics-1.0.2/src/od_metrics/
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/constants.py
--rw-r--r--   0 root         (0) root         (0)    46882 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/od_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/utils.py
--rw-r--r--   0 root         (0) root         (0)    23245 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.742132 od_metrics-1.0.2/src/od_metrics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5463 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.742132 od_metrics-1.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)    12838 2024-04-12 21:44:42.000000 od_metrics-1.0.2/tests/test_odmetrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 22:59:50.352016 od_metrics-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-22 22:59:39.000000 od_metrics-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5463 2024-04-22 22:59:50.352016 od_metrics-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4939 2024-04-22 22:59:39.000000 od_metrics-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-22 22:59:39.000000 od_metrics-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-22 22:59:50.352016 od_metrics-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-22 22:59:39.000000 od_metrics-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 22:59:50.348016 od_metrics-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 22:59:50.348016 od_metrics-1.1.0/src/od_metrics/
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-22 22:59:39.000000 od_metrics-1.1.0/src/od_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-22 22:59:39.000000 od_metrics-1.1.0/src/od_metrics/constants.py
+-rw-r--r--   0 root         (0) root         (0)    47602 2024-04-22 22:59:39.000000 od_metrics-1.1.0/src/od_metrics/od_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     5538 2024-04-22 22:59:39.000000 od_metrics-1.1.0/src/od_metrics/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23245 2024-04-22 22:59:39.000000 od_metrics-1.1.0/src/od_metrics/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 22:59:50.352016 od_metrics-1.1.0/src/od_metrics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5463 2024-04-22 22:59:50.000000 od_metrics-1.1.0/src/od_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2024-04-22 22:59:50.000000 od_metrics-1.1.0/src/od_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 22:59:50.000000 od_metrics-1.1.0/src/od_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-22 22:59:50.000000 od_metrics-1.1.0/src/od_metrics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-22 22:59:50.000000 od_metrics-1.1.0/src/od_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 22:59:50.352016 od_metrics-1.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    16455 2024-04-22 22:59:39.000000 od_metrics-1.1.0/tests/test_odmetrics.py
```

### Comparing `od_metrics-1.0.2/LICENSE` & `od_metrics-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `od_metrics-1.0.2/PKG-INFO` & `od_metrics-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 1.0.2
+Version: 1.1.0
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 1.0.2 Summary: Object Detection
+Metadata-Version: 2.1 Name: od-metrics Version: 1.1.0 Summary: Object Detection
 metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
```

### Comparing `od_metrics-1.0.2/README.md` & `od_metrics-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `od_metrics-1.0.2/setup.cfg` & `od_metrics-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = od-metrics
-version = 1.0.2
+version = 1.1.0
 author = EMalagoli92
 author_email = emala.892@gmail.com
 description = Object Detection metrics.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EMalagoli92/OD-metrics
 classifiers =
```

### Comparing `od_metrics-1.0.2/src/od_metrics/constants.py` & `od_metrics-1.1.0/src/od_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `od_metrics-1.0.2/src/od_metrics/od_metrics.py` & `od_metrics-1.1.0/src/od_metrics/od_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from functools import reduce, partial
 from collections import defaultdict
 import operator
 from typing import Literal, Any, Callable, cast
 import numpy as np
 
 from .constants import DEFAULT_COCO, _STANDARD_OUTPUT
-from .utils import get_indexes, get_suffix, _Missing
+from .utils import get_indexes, get_suffix, _Missing, to_xyxy
 from .validators import ConstructorModel, ComputeModel, MeanModel
 
 
 class ODMetrics:
     """
     ODMetrics class.
 
@@ -479,15 +479,16 @@
         y_pred_boxes = [yp["bbox"] for yp in y_pred_]
         iscrowd = [yt["iscrowd"] for yt in y_true_]
 
         # Compute IoU between each prediction and ground truth region
         ious = iou(
             y_true=y_true_boxes,
             y_pred=y_pred_boxes,
-            iscrowd=iscrowd
+            iscrowd=iscrowd,
+            box_format="xywh",
             )
         return ious
 
     def _evaluate_image(  # pylint: disable=R0912
             self,
             y_true: defaultdict,
             y_pred: defaultdict,
@@ -1046,21 +1047,19 @@
         return output
 
 
 def iou(
         y_true: np.ndarray | list,
         y_pred: np.ndarray | list,
         iscrowd: np.ndarray | list[bool] | list[int] | None = None,
+        box_format: Literal["xyxy", "xywh", "cxcywh"] = "xywh",
         ) -> np.ndarray:
     """
     Calculate IoU between bounding boxes.
 
-    Single bounding boxes must be in `"xywh"` format, i.e.
-        [xmin, ymin, width, height]
-
     The standard iou of a ground truth `y_true` and detected
     `y_pred` object is:
 
     $$iou(\\text{y_true}, \\text{y_pred}) =
         \\frac{\\text{y_true} \\bigcap \\text{y_pred}}
         {\\text{y_true}\\bigcup \\text{y_pred}}$$
 
@@ -1092,14 +1091,31 @@
         `np.ndarray` with shape `(B1, 4)`, `B1` `y_true` batch size.
     y_pred : np.ndarray | list
         `np.ndarray` with shape `(B2, 4)`, `B2` `y_pred` batch size.
     iscrowd : np.ndarray | list[bool] | list[int] | None
         Whether `y_true` are crowd regions.
         If `None`, it will be set to `False` for all `y_true`.
         The default is `None`.
+    box_format: Literal["xyxy", "xywh", "cxcywh"], optional
+        Bounding box format.
+        Supported formats are:<br>
+            - `"xyxy"`: boxes are represented via corners,
+                    x1, y1 being top left and x2, y2
+                    being bottom right.<br>
+            - `"xywh"`: boxes are represented via corner,
+                    width and height, x1, y2 being top
+                    left, w, h being width and height.
+                    This is the default format; all
+                    input formats will be converted
+                    to this.<br>
+            - `"cxcywh"`: boxes are represented via centre,
+                    width and height, cx, cy being
+                    center of box, w, h being width
+                    and height.<br>
+        The default is `"xywh"`.
 
     Returns
     -------
     np.ndarray
         IoU vector of shape `(B2, B1)`.
     """
     if len(y_pred) == 0 or len(y_true) == 0:
@@ -1107,28 +1123,22 @@
     # iscrowd
     if iscrowd is not None:
         if len(iscrowd) != len(y_true):
             raise ValueError("`iscrowd` and `y_true` should have the same "
                              "length.")
     else:
         iscrowd = [False]*len(y_true)
-    # To np.ndarray
-    if not isinstance(y_pred, np.ndarray):
-        y_pred = np.array(y_pred)
-    if not isinstance(y_true, np.ndarray):
-        y_true = np.array(y_true)
+    # To np.ndarray and xyxy box format
+    y_true = np.array([to_xyxy(bbox_, box_format) for bbox_ in y_true])
+    y_pred = np.array([to_xyxy(bbox_, box_format) for bbox_ in y_pred])
 
     # pylint: disable-next=W0632
-    xmin1, ymin1, width1, height1 = np.hsplit(y_pred, 4)
+    xmin1, ymin1, xmax1, ymax1 = np.hsplit(y_pred, 4)
     # pylint: disable-next=W0632
-    xmin2, ymin2, width2, height2 = np.hsplit(y_true, 4)
-    xmax1 = xmin1 + width1
-    xmax2 = xmin2 + width2
-    ymax1 = ymin1 + height1
-    ymax2 = ymin2 + height2
+    xmin2, ymin2, xmax2, ymax2 = np.hsplit(y_true, 4)
 
     # Intersection
     xmin_i = np.maximum(xmin1.T, xmin2).T
     ymin_i = np.maximum(ymin1.T, ymin2).T
     xmax_i = np.minimum(xmax1.T, xmax2).T
     ymax_i = np.minimum(ymax1.T, ymax2).T
     inter_area = (np.maximum((xmax_i - xmin_i), 0)
```

### Comparing `od_metrics-1.0.2/src/od_metrics/utils.py` & `od_metrics-1.1.0/src/od_metrics/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 __all__ = [
     "_Missing",
     "get_indexes",
     "get_suffix",
+    "to_xywh",
+    "to_xyxy",
     ]
 
 from typing import Literal
 import numpy as np
 
 
 class _Missing:
@@ -120,14 +122,95 @@
         return cxcywh_xywh(bbox)
     raise ValueError(  # pragma: no cover
         "`box_format` can be `'xyxy'`, `'xywh'`, `'cxcywh'`. "
         f"Found {box_format}"
         )
 
 
+def xywh_xyxy(bbox: list[float]) -> list[float]:
+    """
+    Change bounding box format from `xywh` to `xyxy`.
+
+    Parameters
+    ----------
+    bbox : list[float]
+        Input bounding box.
+
+    Returns
+    -------
+    list[float]
+        Bounding box in `"xyxy"` format.
+    """
+    return [
+        bbox[0],
+        bbox[1],
+        bbox[0] + bbox[2],
+        bbox[1] + bbox[3]
+        ]
+
+
+def cxcywh_xyxy(bbox: list[float]) -> list[float]:
+    """
+    Change bounding box format from `cxcywh` to `xyxy`.
+
+    Parameters
+    ----------
+    bbox : list[float]
+        Input bounding box.
+
+    Returns
+    -------
+    list[float]
+        Bounding box in `"xyxy"` format.
+    """
+    return [
+        bbox[0] - bbox[2] / 2,
+        bbox[1] - bbox[3] / 2,
+        bbox[0] + bbox[2] / 2,
+        bbox[1] + bbox[3] / 2
+        ]
+
+
+def to_xyxy(
+        bbox: list[float],
+        box_format: Literal["xyxy", "xywh", "cxcywh"],
+        ) -> list[float]:
+    """
+    Change bounding box format to `"xyxy"`.
+
+    Parameters
+    ----------
+    bbox : list[float]
+        Input bounding box.
+    box_format : Literal["xyxy", "xywh", "cxcywh"]
+        Input bounding box format.
+        It can be `"xyxy"`, `"xywh"` or `"cxcywh"`.
+
+    Raises
+    ------
+    ValueError
+        If `box_format` not one of `"xyxy"`, `"xywh"`, `"cxcywh"`.
+
+    Returns
+    -------
+    list[float]
+        Bounding box in `"xyxy"` format.
+    """
+    if box_format == "xywh":
+        return xywh_xyxy(bbox)
+    if box_format == "xyxy":
+        return bbox
+    if box_format == "cxcywh":
+        return cxcywh_xyxy(bbox)
+    raise ValueError(
+        "`box_format` can be `'xyxy'`, `'xywh'`, `'cxcywh'`. "
+        f"Found {box_format}"
+        )
+
+
 def get_suffix(
         iou_threshold: np.ndarray,
         area_range_key: np.ndarray,
         max_detection_threshold: np.ndarray,
         ) -> str:
     """
     Create metric's suffix.
```

### Comparing `od_metrics-1.0.2/src/od_metrics/validators.py` & `od_metrics-1.1.0/src/od_metrics/validators.py`

 * *Files identical despite different names*

### Comparing `od_metrics-1.0.2/src/od_metrics.egg-info/PKG-INFO` & `od_metrics-1.1.0/src/od_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 1.0.2
+Version: 1.1.0
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 1.0.2 Summary: Object Detection
+Metadata-Version: 2.1 Name: od-metrics Version: 1.1.0 Summary: Object Detection
 metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
```

### Comparing `od_metrics-1.0.2/tests/test_odmetrics.py` & `od_metrics-1.1.0/tests/test_odmetrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from __future__ import annotations
 
 import unittest
 import copy
 from typing import Any, Literal
 from functools import partial
+from itertools import product
 import numpy as np
 from parameterized import parameterized, parameterized_class
 
 from src.od_metrics import ODMetrics, iou
 from src.od_metrics.constants import DEFAULT_COCO
+from src.od_metrics.utils import to_xywh
 from tests.utils import annotations_generator, pycoco_converter, \
     test_equality, rename_dict, xywh_to, apply_function
 from tests.config import TESTS
 
 try:
     import pycocotools
     from pycocotools import mask as maskUtils
@@ -327,14 +329,73 @@
             y_pred=y_pred,
             iscrowd=iscrowd
             )
         pycoco_ious = maskUtils.iou(y_pred, y_true, iscrowd_pycoco)
 
         self.assertTrue(test_equality(od_metrics_ious, pycoco_ious))
 
+    @parameterized.expand(list(product(
+        ["random", None], ["xyxy", "xywh", "cxcywh", "error"])))
+    def test_box_formats(
+            self,
+            iscrowd_mode: Literal["random", None],
+            box_format: Literal["xyxy", "xywh", "cxcywh"],
+            ) -> None:
+        """Test `box_format` argument."""
+        if iscrowd_mode == "random":
+            iscrowd = list(map(
+                bool,
+                np.random.randint(
+                    low=0,
+                    high=2,
+                    size=[self.SIZE]
+                    ).tolist()
+                )
+            )
+            iscrowd_pycoco = iscrowd
+        else:
+            iscrowd = None
+            iscrowd_pycoco = [False] * self.SIZE
+        y_pred = np.random.randint(
+            low=1,
+            high=self.HIGH,
+            size=[self.SIZE, 4]
+            )
+
+        y_true = np.random.randint(
+            low=1,
+            high=self.HIGH,
+            size=[self.SIZE, 4]
+            )
+
+        if box_format in ["xyxy", "xywh", "cxcywh"]:
+            od_metrics_ious = iou(
+                y_true=y_true,
+                y_pred=y_pred,
+                iscrowd=iscrowd,
+                box_format=box_format,
+                )
+
+            y_true_pycoco = np.array([to_xywh(bbox_, box_format)
+                                      for bbox_ in y_true])
+            y_pred_pycoco = np.array([to_xywh(bbox_, box_format)
+                                      for bbox_ in y_pred])
+            pycoco_ious = maskUtils.iou(y_pred_pycoco, y_true_pycoco,
+                                        iscrowd_pycoco)
+
+            self.assertTrue(test_equality(od_metrics_ious, pycoco_ious))
+        else:
+            with self.assertRaises(ValueError):
+                od_metrics_ious = iou(
+                    y_true=y_true,
+                    y_pred=y_pred,
+                    iscrowd=iscrowd,
+                    box_format=box_format,
+                    )
+
     def test_length_exception(self) -> None:
         """Test exception `iscrowd` and `y_true` different length."""
         iscrowd = list(map(
             bool,
             np.random.randint(
                 low=0,
                 high=2,
@@ -356,10 +417,59 @@
         with self.assertRaises(ValueError):
             iou(
                 y_true=y_true,
                 y_pred=y_pred,
                 iscrowd=iscrowd,
                 )
 
+    @parameterized.expand(list(product(
+        ["random", None], ["xyxy", "xywh", "cxcywh"])))
+    def test_not_valid_boxes(
+            self,
+            iscrowd_mode: Literal["random", None],
+            box_format: Literal["xyxy", "xywh", "cxcywh"],
+            ) -> None:
+        """Test equivalence for not valid (negative values) boxes."""
+        if iscrowd_mode == "random":
+            iscrowd = list(map(
+                bool,
+                np.random.randint(
+                    low=0,
+                    high=2,
+                    size=[self.SIZE]
+                    ).tolist()
+                )
+            )
+            iscrowd_pycoco = iscrowd
+        else:
+            iscrowd = None
+            iscrowd_pycoco = [False] * self.SIZE
+        y_pred = np.random.randint(
+            low=-10,
+            high=1,
+            size=[self.SIZE, 4]
+            )
+        y_true = np.random.randint(
+            low=-10,
+            high=1,
+            size=[self.SIZE, 4]
+            )
+
+        od_metrics_ious = iou(
+            y_true=y_true,
+            y_pred=y_pred,
+            iscrowd=iscrowd,
+            box_format=box_format,
+            )
+
+        y_true_pycoco = np.array([to_xywh(bbox_, box_format)
+                                  for bbox_ in y_true])
+        y_pred_pycoco = np.array([to_xywh(bbox_, box_format)
+                                  for bbox_ in y_pred])
+        pycoco_ious = maskUtils.iou(y_pred_pycoco, y_true_pycoco,
+                                    iscrowd_pycoco)
+
+        self.assertTrue(test_equality(od_metrics_ious, pycoco_ious))
+
 
 if __name__ == "__main__":
     unittest.main()  # pragma: no cover
```

