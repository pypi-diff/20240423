# Comparing `tmp/ehdg_pupil_detector-3.4.1.tar.gz` & `tmp/ehdg_pupil_detector-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.4.1.tar", last modified: Mon Apr 22 11:39:38 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.4.2.tar", last modified: Mon Apr 22 20:59:26 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.4.1.tar` & `ehdg_pupil_detector-3.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 11:39:38.632957 ehdg_pupil_detector-3.4.1/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.4.1/LICENSE
--rw-rw-rw-   0        0        0     4075 2024-04-22 11:39:38.631960 ehdg_pupil_detector-3.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.4.1/README.md
--rw-rw-rw-   0        0        0     1162 2024-04-22 11:35:28.000000 ehdg_pupil_detector-3.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 11:39:38.633955 ehdg_pupil_detector-3.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 11:39:38.601521 ehdg_pupil_detector-3.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 11:39:38.608502 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    23108 2024-04-18 01:34:44.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      312 2024-04-22 05:49:11.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    23705 2024-04-22 11:34:42.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/opmtrack.py
--rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/opmtrack_plot.json
-drwxrwxrwx   0        0        0        0 2024-04-22 11:39:38.631960 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4075 2024-04-22 11:39:38.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-04-22 11:39:38.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 11:39:38.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-22 11:39:38.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-22 11:39:38.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 11:39:38.000000 ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.902410 ehdg_pupil_detector-3.4.2/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.4.2/LICENSE
+-rw-rw-rw-   0        0        0     4075 2024-04-22 20:59:26.901413 ehdg_pupil_detector-3.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.4.2/README.md
+-rw-rw-rw-   0        0        0     1162 2024-04-22 20:54:05.000000 ehdg_pupil_detector-3.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 20:59:26.902410 ehdg_pupil_detector-3.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.867987 ehdg_pupil_detector-3.4.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.875969 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    23108 2024-04-22 20:56:03.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      312 2024-04-22 20:58:16.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    23738 2024-04-22 20:54:05.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opmtrack.py
+-rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opmtrack_plot.json
+drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.900416 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4075 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.4.1/LICENSE` & `ehdg_pupil_detector-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.1/PKG-INFO` & `ehdg_pupil_detector-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.4.1/README.md` & `ehdg_pupil_detector-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.1/pyproject.toml` & `ehdg_pupil_detector-3.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.4.1"
+version = "3.4.2"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.2", "numpy"]
 requires-python = ">=3.9"
```

### Comparing `ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import csv
+import math
 import os
 import argparse
 import importlib.metadata
 from importlib.resources import files
 import cv2
 import commentjson
 from ehdg_pupil_detector import ehdg_pupil_detector
@@ -147,32 +148,32 @@
 
                 center_of_pupil = (int(center_of_pupil_x), int(center_of_pupil_y))
                 detected_frame = np.copy(frame)
                 if center_of_pupil != (0, 0):
                     cv2.ellipse(
                         detected_frame,
                         center_of_pupil,
-                        (int(major_axis), int(minor_axis)),
+                        (math.ceil(major_axis), math.ceil(minor_axis)),
                         int(angle_of_pupil),
                         0, 360,  # start/end angle for drawing
                         pupil_circle_color_tuple
                     )
                     if min_max_circle:
                         cv2.ellipse(
                             detected_frame,
                             center_of_pupil,
-                            (int(min_pupil_size), int(min_pupil_size)),
+                            (int(min_pupil_size/2), int(min_pupil_size/2)),
                             int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             min_circle_color_tuple
                         )
                         cv2.ellipse(
                             detected_frame,
                             center_of_pupil,
-                            (int(max_pupil_size), int(max_pupil_size)),
+                            (int(max_pupil_size/2), int(max_pupil_size/2)),
                             int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             max_circle_color_tuple
                         )
                 else:
                     middle_of_width = int(frame_width / 2)
                     middle_of_height = int(frame_height / 2)
```

### Comparing `ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.4.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt` & `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

