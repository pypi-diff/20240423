# Comparing `tmp/ehdg_pupil_detector-3.4.2.tar.gz` & `tmp/ehdg_pupil_detector-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.4.2.tar", last modified: Mon Apr 22 20:59:26 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.4.3.tar", last modified: Mon Apr 22 22:40:13 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.4.2.tar` & `ehdg_pupil_detector-3.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.902410 ehdg_pupil_detector-3.4.2/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.4.2/LICENSE
--rw-rw-rw-   0        0        0     4075 2024-04-22 20:59:26.901413 ehdg_pupil_detector-3.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.4.2/README.md
--rw-rw-rw-   0        0        0     1162 2024-04-22 20:54:05.000000 ehdg_pupil_detector-3.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 20:59:26.902410 ehdg_pupil_detector-3.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.867987 ehdg_pupil_detector-3.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.875969 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    23108 2024-04-22 20:56:03.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      312 2024-04-22 20:58:16.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    23738 2024-04-22 20:54:05.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opmtrack.py
--rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opmtrack_plot.json
-drwxrwxrwx   0        0        0        0 2024-04-22 20:59:26.900416 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4075 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 20:59:26.000000 ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.374622 ehdg_pupil_detector-3.4.3/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.4.3/LICENSE
+-rw-rw-rw-   0        0        0     4075 2024-04-22 22:40:13.373625 ehdg_pupil_detector-3.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.4.3/README.md
+-rw-rw-rw-   0        0        0     1162 2024-04-22 22:39:11.000000 ehdg_pupil_detector-3.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 22:40:13.374622 ehdg_pupil_detector-3.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.339219 ehdg_pupil_detector-3.4.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.348182 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    23108 2024-04-22 22:34:30.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      312 2024-04-22 22:37:43.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    23788 2024-04-22 22:29:58.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opmtrack.py
+-rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opmtrack_plot.json
+drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.371630 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4075 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.4.2/LICENSE` & `ehdg_pupil_detector-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.2/PKG-INFO` & `ehdg_pupil_detector-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.4.2
+Version: 3.4.3
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.4.2/README.md` & `ehdg_pupil_detector-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.2/pyproject.toml` & `ehdg_pupil_detector-3.4.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.4.2"
+version = "3.4.3"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.2", "numpy"]
 requires-python = ">=3.9"
```

### Comparing `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,24 +178,24 @@
                     middle_of_width = int(frame_width / 2)
                     middle_of_height = int(frame_height / 2)
                     min_max_area = (middle_of_width, middle_of_height)
                     if min_max_circle:
                         cv2.ellipse(
                             detected_frame,
                             min_max_area,
-                            (int(min_pupil_size), int(min_pupil_size)),
-                            90,
+                            (int(min_pupil_size / 2), int(min_pupil_size / 2)),
+                            int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             min_circle_color_tuple
                         )
                         cv2.ellipse(
                             detected_frame,
                             min_max_area,
-                            (int(max_pupil_size), int(max_pupil_size)),
-                            90,
+                            (int(max_pupil_size / 2), int(max_pupil_size / 2)),
+                            int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             max_circle_color_tuple
                         )
 
                 v_writer.write(detected_frame)
 
                 pupil_data = {}
```

### Comparing `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.4.2
+Version: 3.4.3
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.4.2/src/ehdg_pupil_detector.egg-info/SOURCES.txt` & `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

