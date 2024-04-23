# Comparing `tmp/aau_label-0.1.0.tar.gz` & `tmp/aau_label-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_label-0.1.0.tar", last modified: Fri Apr 19 18:40:30 2024, max compression
+gzip compressed data, was "aau_label-0.2.0.tar", last modified: Tue Apr 23 07:35:25 2024, max compression
```

## Comparing `aau_label-0.1.0.tar` & `aau_label-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1099 2024-04-19 06:41:14.792161 aau_label-0.1.0/LICENSE
--rw-r--r--   0        0        0       39 2024-04-19 06:41:14.792161 aau_label-0.1.0/README.md
--rw-r--r--   0        0        0      433 2024-04-19 18:40:30.642980 aau_label-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 06:48:29.759738 aau_label-0.1.0/src/aau_label/__init__.py
--rw-r--r--   0        0        0      436 2024-04-19 09:08:42.325514 aau_label-0.1.0/src/aau_label/errors.py
--rw-r--r--   0        0        0     6605 2024-04-19 13:44:29.221383 aau_label-0.1.0/src/aau_label/label_handler.py
--rw-r--r--   0        0        0      527 2024-04-19 09:47:02.266837 aau_label-0.1.0/src/aau_label/model.py
--rw-r--r--   0        0        0       84 2024-04-19 07:33:02.610343 aau_label-0.1.0/src/aau_label/parsers/__init__.py
--rw-r--r--   0        0        0     1787 2024-04-19 13:34:34.968818 aau_label-0.1.0/src/aau_label/parsers/darknet_parser.py
--rw-r--r--   0        0        0     2113 2024-04-19 13:34:28.738871 aau_label-0.1.0/src/aau_label/parsers/pascal_parser.py
--rw-r--r--   0        0        0      279 2024-04-19 13:32:13.802087 aau_label-0.1.0/src/aau_label/parsers/protocol.py
--rw-r--r--   0        0        0        0 2024-04-19 06:48:29.760738 aau_label-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 aau_label-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-19 06:41:14.792161 aau_label-0.2.0/LICENSE
+-rw-r--r--   0        0        0       39 2024-04-19 06:41:14.792161 aau_label-0.2.0/README.md
+-rw-r--r--   0        0        0      434 2024-04-23 07:35:25.458826 aau_label-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6621 2024-04-23 07:33:05.270267 aau_label-0.2.0/src/aau_label/__init__.py
+-rw-r--r--   0        0        0      436 2024-04-19 09:08:42.325514 aau_label-0.2.0/src/aau_label/errors.py
+-rw-r--r--   0        0        0      586 2024-04-23 07:30:45.330748 aau_label-0.2.0/src/aau_label/model.py
+-rw-r--r--   0        0        0      131 2024-04-23 07:31:36.565873 aau_label-0.2.0/src/aau_label/parsers/__init__.py
+-rw-r--r--   0        0        0     1830 2024-04-23 07:27:21.866796 aau_label-0.2.0/src/aau_label/parsers/darknet_parser.py
+-rw-r--r--   0        0        0     2145 2024-04-23 07:28:02.404302 aau_label-0.2.0/src/aau_label/parsers/pascal_parser.py
+-rw-r--r--   0        0        0      496 2024-04-23 07:30:41.492504 aau_label-0.2.0/src/aau_label/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-19 06:48:29.760738 aau_label-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 aau_label-0.2.0/PKG-INFO
```

### Comparing `aau_label-0.1.0/LICENSE` & `aau_label-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aau_label-0.1.0/src/aau_label/label_handler.py` & `aau_label-0.2.0/src/aau_label/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable
 
 from pandas import DataFrame
 from PIL import Image as PILImage
 
 from .errors import LabelError
-from .model import COCOInfo, COCOLicense, Label, LabelImage
+from .model import AAULabel, AAULabelImage, COCOInfo, COCOLicense
 from .parsers import DarknetParser, PascalParser
+from .protocols import Label, LabelImage
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Sequence
     from PIL.Image import Image
-    from .parsers.protocol import LabelParser
+    from .protocols import LabelParser
 
 import dataclasses
 import logging
 from datetime import datetime
 
 logger = logging.getLogger(__name__)
 
@@ -27,24 +28,24 @@
     label_images = []
     with open(filepath, "r") as file:
         data = json.load(file)
 
         for element in data:
             labels: list[Label] = []
             for label_dict in element["labels"]:
-                label = Label(
+                label = AAULabel(
                     label_dict["x"],
                     label_dict["y"],
                     label_dict["width"],
                     label_dict["height"],
                     label_dict["classifier"],
                 )
                 labels.append(label)
 
-            label_image = LabelImage(
+            label_image = AAULabelImage(
                 path=element["path"],
                 width=element["width"],
                 height=element["height"],
                 labels=labels,
             )
             label_images.append(label_image)
 
@@ -89,19 +90,19 @@
 
     for img_path, label_path in pairs:
         image: Image = PILImage.open(img_path)
         width, height = image.size
         labels: Sequence[Label] = []
 
         try:
-            labels = parser.parse(label_path.as_posix(), image)
+            labels = parser.parse(label_path, image)
         except (FileNotFoundError, ValueError, LabelError) as error:
             logger.warning(error)
         else:
-            yield LabelImage(img_path.as_posix(), width, height, labels)
+            yield AAULabelImage(img_path, width, height, labels)
 
 
 def from_pascal_dir(img_dir: str | Path, label_dir: str | Path) -> Iterable[LabelImage]:
     return from_dir(img_dir, label_dir, PascalParser())
 
 
 def from_darknet_dir(
@@ -114,15 +115,15 @@
     with open(filepath, "w") as file:
         json.dump(label_images, file, indent=2)
 
 
 def __get_unique_classifiers(label_images: Iterable[LabelImage]) -> Dict[str, int]:
     classifiers = set()
     for label_image in label_images:
-        classifiers.update(label.classifier for label in label_image.labels)
+        classifiers.update(label.name for label in label_image.labels)
     return {classifier: i for i, classifier in enumerate(classifiers)}
 
 
 def to_coco(
     label_images: Iterable[LabelImage], license: COCOLicense, info: COCOInfo
 ) -> Dict[str, Any]:
     logger.info("Extracting unique labels from LabelImage objects")
@@ -151,15 +152,15 @@
             }
         )
         for label in label_image.labels:
             annotations.append(
                 {
                     "id": label_id,
                     "image_id": image_id,
-                    "category_id": classifier_db[label.classifier],
+                    "category_id": classifier_db[label.name],
                     "bbox": [label.x, label.y, label.width, label.height],
                     "iscrowd": 0,
                 }
             )
             label_id += 1
 
     return {
@@ -185,30 +186,30 @@
                 "path": label_image.path,
                 "image_width": label_image.width,
                 "image_height": label_image.height,
                 "label_width": label.width,
                 "label_height": label.height,
                 "x": label.x,
                 "y": label.y,
-                "classifier": label.classifier,
+                "classifier": label.name,
             }
             for label in label_image.labels
         )
     return DataFrame(rows)
 
 
 def from_dataframe(df: DataFrame) -> Iterable[LabelImage]:
     for (path, width, height), group in df.groupby(
         ["path", "image_width", "image_height"]
     ):
         labels: Sequence[Label] = [
-            Label(
+            AAULabel(
                 label["x"],
                 label["y"],
                 label["label_width"],
                 label["label_height"],
                 label["classifier"],
             )
             for _, label in group.iterrows()
         ]
 
-        yield LabelImage(path, width, height, labels)
+        yield AAULabelImage(path, width, height, labels)
```

### Comparing `aau_label-0.1.0/src/aau_label/parsers/darknet_parser.py` & `aau_label-0.2.0/src/aau_label/parsers/darknet_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import os
+from pathlib import Path
 from typing import List, Optional
 
 from PIL.Image import Image
 
 from ..errors import ClassFileNotFoundError
-from ..model import Label
-from .protocol import LabelParser
+from ..model import AAULabel
+from ..protocols import Label, LabelParser
 
 
 class DarknetParser(LabelParser):
     file_extension = ".txt"
 
     def __init__(self):
         self.current_directory: Optional[str] = None
@@ -22,28 +23,28 @@
 
         class_index = int(class_index)
         width = round(float(width) * img_width)
         height = round(float(height) * img_height)
         x = round(float(x) * img_width - width / 2)
         y = round(float(y) * img_height - height / 2)
 
-        return Label(x, y, width, height, self.label_map[class_index])
+        return AAULabel(x, y, width, height, self.label_map[class_index])
 
-    def parse(self, label_file: str, image: Image) -> List[Label]:
+    def parse(self, label_file: Path, image: Image) -> List[Label]:
         self.__load_class_file(label_file)
 
         with open(label_file, "r") as file:
             width, height = image.size
 
             try:
                 return [self.__parse_row(row, width, height) for row in file]
             except ValueError:
                 raise ValueError(f"Badly formatted label file: {label_file}")
 
-    def __load_class_file(self, label_file: str):
+    def __load_class_file(self, label_file: Path):
         filepath, _ = os.path.split(label_file)
 
         if self.current_directory == filepath:
             return
 
         self.current_directory = filepath
         classfile = os.path.join(filepath, "classes.txt")
```

### Comparing `aau_label-0.1.0/src/aau_label/parsers/pascal_parser.py` & `aau_label-0.2.0/src/aau_label/parsers/pascal_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from dataclasses import dataclass
-from typing import ClassVar, List
+from pathlib import Path
+from typing import List
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element, ParseError
 
 from PIL.Image import Image
 
 from aau_label.errors import PascalParseError
 
-from ..model import Label
-from .protocol import LabelParser
+from ..model import AAULabel
+from ..protocols import Label, LabelParser
 
 
 @dataclass
 class BoundingBox:
     xmin: int
     ymin: int
     xmax: int
     ymax: int
 
 
 class PascalParser(LabelParser):
     file_extension = ".xml"
 
-    def parse(self, label_file: str, image: Image) -> List[Label]:
+    def parse(self, label_file: Path, image: Image) -> List[Label]:
         root = ElementTree.parse(label_file).getroot()
         try:
             return [
                 self.__parse_object(child) for child in root if child.tag == "object"
             ]
         except ParseError as e:
             raise PascalParseError(label_file) from e
@@ -37,15 +38,15 @@
 
         for child in element:
             if child.tag == "name":
                 classifier = child.text or ""
             elif child.tag == "bndbox":
                 bounding_box = self.__parse_bounding_box(child)
 
-        return Label(
+        return AAULabel(
             bounding_box.xmin,
             bounding_box.ymin,
             bounding_box.xmax - bounding_box.xmin,
             bounding_box.ymax - bounding_box.ymin,
             classifier,
         )
```

