# Comparing `tmp/ehdg_pupil_detector-3.4.3.tar.gz` & `tmp/ehdg_pupil_detector-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.4.3.tar", last modified: Mon Apr 22 22:40:13 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.5.0.tar", last modified: Tue Apr 23 03:55:04 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.4.3.tar` & `ehdg_pupil_detector-3.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.374622 ehdg_pupil_detector-3.4.3/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.4.3/LICENSE
--rw-rw-rw-   0        0        0     4075 2024-04-22 22:40:13.373625 ehdg_pupil_detector-3.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.4.3/README.md
--rw-rw-rw-   0        0        0     1162 2024-04-22 22:39:11.000000 ehdg_pupil_detector-3.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 22:40:13.374622 ehdg_pupil_detector-3.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.339219 ehdg_pupil_detector-3.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.348182 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    23108 2024-04-22 22:34:30.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      312 2024-04-22 22:37:43.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    23788 2024-04-22 22:29:58.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opmtrack.py
--rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opmtrack_plot.json
-drwxrwxrwx   0        0        0        0 2024-04-22 22:40:13.371630 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4075 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 22:40:13.000000 ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.500054 ehdg_pupil_detector-3.5.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4075 2024-04-23 03:55:04.498060 ehdg_pupil_detector-3.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.5.0/README.md
+-rw-rw-rw-   0        0        0     1162 2024-04-23 03:37:05.000000 ehdg_pupil_detector-3.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 03:55:04.500054 ehdg_pupil_detector-3.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.468594 ehdg_pupil_detector-3.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.476543 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    25943 2024-04-23 03:36:38.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      312 2024-04-22 23:25:41.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    24813 2024-04-23 03:52:15.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opmtrack.py
+-rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opmtrack_plot.json
+drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.497063 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4075 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.4.3/LICENSE` & `ehdg_pupil_detector-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.3/PKG-INFO` & `ehdg_pupil_detector-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.4.3
+Version: 3.5.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.4.3/README.md` & `ehdg_pupil_detector-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.4.3/pyproject.toml` & `ehdg_pupil_detector-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.4.3"
+version = "3.5.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.2", "numpy"]
 requires-python = ">=3.9"
```

### Comparing `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,16 +38,23 @@
             self.max_circular_ratio = 1.9
             self.ksize_height = 13
             self.ksize_width = 13
             self.min_binary_threshold = 20
             self.max_binary_threshold = 255
             self.reflection_fill_dilation_index = 25
             self.reflection_fill_square_dimension = 200
-            self.min_pupil_size = 50
-            self.max_pupil_size = 150
+            self.min_pupil_size = 2
+            self.max_pupil_size = 120
+        self.min_detected_pupil = 10000
+        self.max_detected_pupil = 0
+        self.rejected_by_circular_ratio = 0
+        self.rejected_by_pupil_size = 0
+        self.total_pass_count = 0
+        self.total_diameter = 0
+        self.avg_detected_pupil = 0
 
     def update_config(self, config_dict_input):
         if type(config_dict_input) is not dict:
             raise ValueError("The config input must be dictionary type.")
         else:
             for key, value in config_dict_input.items():
                 self.update_config_by_name(key, value)
@@ -140,14 +147,16 @@
         frame_height = frame_shape[0]
 
         # Checking it is rbg/bgr image or not
         # If yes, then change to grayscale image
         if len(frame_shape) == 3:
             frame_input = cv2.cvtColor(frame_input, cv2.COLOR_BGR2GRAY)
 
+        # gray_frame = np.copy(frame_input)
+
         if self.reflection_fill:
             dilation_index = self.reflection_fill_dilation_index
             square_dimension = self.reflection_fill_square_dimension
 
             _, reflection_shape = cv2.threshold(frame_input,
                                                 self.reflection_removal_lower_limit,
                                                 self.reflection_removal_upper_limit,
@@ -173,14 +182,18 @@
             cloned_black_frame[shsp:shep, swsp:swep] = cropped_dilated_reflection_shape
 
             reflection_shape_index = list(zip(*np.where(cloned_black_frame == 255)))
 
             # fill black color in pupil reflection area
             for position in reflection_shape_index:
                 frame_input[position[0], position[1]] = 0
+        else:
+            # reflection_shape = np.copy(frame_input)
+            # reflection_shape.fill(0)
+            pass
 
         if self.gaussian_blur:
             frame_input = cv2.GaussianBlur(frame_input, (self.ksize_height, self.ksize_width), 0)
 
         _, black_white_filter_frame = cv2.threshold(frame_input,
                                                     self.min_binary_threshold,
                                                     self.max_binary_threshold,
@@ -195,22 +208,22 @@
                 contours = None
         else:
             try:
                 contours, _ = cv2.findContours(black_white_filter_frame, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             except ValueError:
                 contours = None
 
+        error_string = None
         if contours is not None:
             contours = sorted(contours, key=lambda xx: cv2.contourArea(xx), reverse=True)
 
             min_circular_ratio = self.min_circular_ratio
             max_circular_ratio = self.max_circular_ratio
             largest_dia = 0.0
             largest_con_ind = 0
-            error_string = None
             center_of_pupil = (0.0, 0.0)
             reversed_center_of_pupil = (0.0, 0.0)
             axes_of_pupil = (0.0, 0.0)
             average_diameter_of_pupil = 0.0
             angle_of_pupil = 0.0
             circular_con_count = 0
             for ind, cc in enumerate(contours):
@@ -226,59 +239,94 @@
                             largest_con_ind = ind
                             center_of_pupil = (float(x), float(y))
                             reversed_center_of_pupil = (float(frame_width - x), float(frame_height - y))
                             axes_of_pupil = (float(MA / 2), float(ma / 2))
                             average_diameter_of_pupil = avg_dia
                             angle_of_pupil = float(angle)
                             circular_con_count += 1
+                    else:
+                        self.rejected_by_circular_ratio += 1
                 except Exception as e:
                     error_string = str(e)
                     pass
 
             try:
                 largest_circle = contours[largest_con_ind]
             except IndexError:
                 largest_circle = None
 
             if largest_circle is not None:
+                # print(average_diameter_of_pupil)
+                if average_diameter_of_pupil > 0:
+                    self.total_pass_count += 1
+                    if self.total_pass_count <= 1:
+                        self.avg_detected_pupil = average_diameter_of_pupil
+                        self.total_diameter = average_diameter_of_pupil
+                    else:
+                        old_total = self.total_diameter
+                        new_total = old_total + average_diameter_of_pupil
+                        self.total_diameter = new_total
+                        new_avg = new_total / self.total_pass_count
+                        self.avg_detected_pupil = new_avg
+                    if average_diameter_of_pupil >= self.max_detected_pupil:
+                        self.max_detected_pupil = average_diameter_of_pupil
+                    if average_diameter_of_pupil <= self.min_detected_pupil:
+                        self.min_detected_pupil = average_diameter_of_pupil
                 if self.min_pupil_size <= average_diameter_of_pupil <= self.max_pupil_size:
                     temp_dict = {}
                     temp_dict["detector_timestamp"] = time.time()
                     temp_dict["center_of_pupil"] = center_of_pupil
                     temp_dict["reversed_center_of_pupil"] = reversed_center_of_pupil
                     temp_dict["axes_of_pupil"] = axes_of_pupil
                     temp_dict["angle_of_pupil"] = angle_of_pupil
                     temp_dict["average_diameter_of_pupil"] = average_diameter_of_pupil
+                    temp_dict["error_string"] = error_string
+                    # temp_dict["gray_frame"] = gray_frame
+                    # temp_dict["reflection_shape"] = reflection_shape
+                    # temp_dict["black_white_filter_frame"] = black_white_filter_frame
                     return temp_dict
                 else:
+                    self.rejected_by_pupil_size += 1
                     temp_dict = {}
                     temp_dict["detector_timestamp"] = time.time()
                     temp_dict["center_of_pupil"] = (0.0, 0.0)
                     temp_dict["reversed_center_of_pupil"] = (0.0, 0.0)
                     temp_dict["axes_of_pupil"] = (0.0, 0.0)
                     temp_dict["angle_of_pupil"] = 0.0
                     temp_dict["average_diameter_of_pupil"] = 0.0
+                    temp_dict["error_string"] = error_string
+                    # temp_dict["gray_frame"] = gray_frame
+                    # temp_dict["reflection_shape"] = reflection_shape
+                    # temp_dict["black_white_filter_frame"] = black_white_filter_frame
                     return temp_dict
             else:
                 temp_dict = {}
                 temp_dict["detector_timestamp"] = time.time()
                 temp_dict["center_of_pupil"] = (0.0, 0.0)
                 temp_dict["reversed_center_of_pupil"] = (0.0, 0.0)
                 temp_dict["axes_of_pupil"] = (0.0, 0.0)
                 temp_dict["angle_of_pupil"] = 0.0
                 temp_dict["average_diameter_of_pupil"] = 0.0
+                temp_dict["error_string"] = error_string
+                # temp_dict["gray_frame"] = gray_frame
+                # temp_dict["reflection_shape"] = reflection_shape
+                # temp_dict["black_white_filter_frame"] = black_white_filter_frame
                 return temp_dict
         else:
             temp_dict = {}
             temp_dict["detector_timestamp"] = time.time()
             temp_dict["center_of_pupil"] = (0.0, 0.0)
             temp_dict["reversed_center_of_pupil"] = (0.0, 0.0)
             temp_dict["axes_of_pupil"] = (0.0, 0.0)
             temp_dict["angle_of_pupil"] = 0.0
             temp_dict["average_diameter_of_pupil"] = 0.0
+            temp_dict["error_string"] = error_string
+            # temp_dict["gray_frame"] = gray_frame
+            # temp_dict["reflection_shape"] = reflection_shape
+            # temp_dict["black_white_filter_frame"] = black_white_filter_frame
             return temp_dict
 
 
 class PimDetector:
     def __init__(self, config=None, gaussian_blur=True, binary_fill_hole=True):
         if type(gaussian_blur) is bool:
             self.gaussian_blur = gaussian_blur
@@ -422,20 +470,20 @@
         else:
             try:
                 contours, _ = cv2.findContours(black_white_filter_frame, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             except ValueError:
                 contours = None
 
         ch_circles = []
+        error_string = None
         if contours is not None:
             contours = sorted(contours, key=lambda xx: cv2.contourArea(xx), reverse=True)
 
             largest_dia = 0.0
             largest_con_ind = 0
-            error_string = None
             center_of_pupil = (0.0, 0.0)
             reversed_center_of_pupil = (0.0, 0.0)
             axes_of_pupil = (0.0, 0.0)
             average_diameter_of_pupil = 0.0
             angle_of_pupil = 0.0
             circular_con_count = 0
 
@@ -468,26 +516,29 @@
                 temp_dict = {}
                 temp_dict["detector_timestamp"] = time.time()
                 temp_dict["center_of_pupil"] = center_of_pupil
                 temp_dict["reversed_center_of_pupil"] = reversed_center_of_pupil
                 temp_dict["axes_of_pupil"] = axes_of_pupil
                 temp_dict["angle_of_pupil"] = angle_of_pupil
                 temp_dict["average_diameter_of_pupil"] = average_diameter_of_pupil
+                temp_dict["error_string"] = error_string
                 return temp_dict
             else:
                 temp_dict = {}
                 temp_dict["detector_timestamp"] = time.time()
                 temp_dict["center_of_pupil"] = (0.0, 0.0)
                 temp_dict["reversed_center_of_pupil"] = (0.0, 0.0)
                 temp_dict["axes_of_pupil"] = (0.0, 0.0)
                 temp_dict["angle_of_pupil"] = 0.0
                 temp_dict["average_diameter_of_pupil"] = 0.0
+                temp_dict["error_string"] = error_string
                 return temp_dict
         else:
             temp_dict = {}
             temp_dict["detector_timestamp"] = time.time()
             temp_dict["center_of_pupil"] = (0.0, 0.0)
             temp_dict["reversed_center_of_pupil"] = (0.0, 0.0)
             temp_dict["axes_of_pupil"] = (0.0, 0.0)
             temp_dict["angle_of_pupil"] = 0.0
             temp_dict["average_diameter_of_pupil"] = 0.0
+            temp_dict["error_string"] = error_string
             return temp_dict
```

### Comparing `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import cv2
 import commentjson
 from ehdg_pupil_detector import ehdg_pupil_detector
 from ehdg_tools.ehdg_buffers import TinyFillBuffer
 from ehdg_tools.ehdg_plotter import raw_plot
 from ehdg_tools.ehdg_functions import string_to_bgr_tuple
 import numpy as np
+from datetime import datetime
 
 
 # This function is to get built-in config location with new library (from importlib.resources import files)
 def get_config_location(module_name, config_file_name):
     config_dir = files(module_name).joinpath(config_file_name)
     return str(config_dir)
 
@@ -51,27 +52,34 @@
     temp_dict["ellipse_axis_a"] = ellipse_axis_a
     temp_dict["ellipse_axis_b"] = ellipse_axis_b
     temp_dict["ellipse_angle"] = ellipse_angle
 
     return temp_dict
 
 
+def print_and_save(file_input, string_input):
+    now = datetime.now()
+    date_time_string = now.strftime("%d-%m-%Y %H:%M:%S")
+    file = open(str(file_input), "a")
+    file.write(date_time_string + " | " + string_input + "\n")
+    print(string_input)
+
+
 # This function is to redetect with pupil detector by given detector and tiny fill buffer
 # rrt = reflection removal threshold
 def opm_detect(trial_video, out_folder, config_dict, plot_dict,
                buffer_length_input, reflection_removal=True,
                rrt_lower_limit=0, rrt_upper_limit=255,
                gaussian_blur=True, binary_fill=True,
                direction_input=None, min_max_circle=True,
                min_circle_color="green", max_circle_color="orange",
                pupil_circle_color="red"):
     out_csv_dir = os.path.join(out_folder, "result.csv")
     out_video_dir = os.path.join(out_folder, "result.mp4")
-    min_pupil_size = config_dict["min_pupil_size"]
-    max_pupil_size = config_dict["max_pupil_size"]
+    log_dir = os.path.join(out_folder, "result.txt")
     pupil_circle_color_tuple = string_to_bgr_tuple(pupil_circle_color)
     min_circle_color_tuple = string_to_bgr_tuple(min_circle_color)
     max_circle_color_tuple = string_to_bgr_tuple(max_circle_color)
 
     detector = ehdg_pupil_detector.Detector(reflection_removal=reflection_removal,
                                             reflection_removal_lower_limit=rrt_lower_limit,
                                             reflection_removal_upper_limit=rrt_upper_limit,
@@ -81,14 +89,16 @@
     buffer = TinyFillBuffer(buffer_length_input)
     detector.update_config(config_dict)
     updated_properties = detector.get_config_info()
     print("")
     print("<Detector Properties>")
     for info in updated_properties:
         print(f"{info} : {updated_properties[info]}")
+    min_pupil_size = detector.min_pupil_size
+    max_pupil_size = detector.max_pupil_size
 
     print("")
     print(f"Reflection removal : {reflection_removal}")
     print(f"Reflection removal lower threshold : {rrt_lower_limit}")
     print(f"Reflection removal upper threshold : {rrt_upper_limit}")
     print(f"Gaussian blur : {gaussian_blur}")
     print(f"Binary fill : {binary_fill}")
@@ -143,58 +153,61 @@
                 major_axis = float(axes_of_pupil[0])
                 minor_axis = float(axes_of_pupil[1])
                 angle_of_pupil = float(result["angle_of_pupil"])
                 diameter_of_pupil = float(result["average_diameter_of_pupil"])
                 confidence = 0 if x_value <= 0 and y_value <= 0 else 1
 
                 center_of_pupil = (int(center_of_pupil_x), int(center_of_pupil_y))
+                min_axis = (int(min_pupil_size / 2), int(min_pupil_size / 2))
+                max_axis = (int(max_pupil_size / 2), int(max_pupil_size / 2))
                 detected_frame = np.copy(frame)
                 if center_of_pupil != (0, 0):
+                    detected_axis = (math.ceil(major_axis), math.ceil(minor_axis))
                     cv2.ellipse(
                         detected_frame,
                         center_of_pupil,
-                        (math.ceil(major_axis), math.ceil(minor_axis)),
+                        detected_axis,
                         int(angle_of_pupil),
                         0, 360,  # start/end angle for drawing
                         pupil_circle_color_tuple
                     )
                     if min_max_circle:
                         cv2.ellipse(
                             detected_frame,
                             center_of_pupil,
-                            (int(min_pupil_size/2), int(min_pupil_size/2)),
+                            min_axis,
                             int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             min_circle_color_tuple
                         )
                         cv2.ellipse(
                             detected_frame,
                             center_of_pupil,
-                            (int(max_pupil_size/2), int(max_pupil_size/2)),
+                            max_axis,
                             int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             max_circle_color_tuple
                         )
                 else:
                     middle_of_width = int(frame_width / 2)
                     middle_of_height = int(frame_height / 2)
                     min_max_area = (middle_of_width, middle_of_height)
                     if min_max_circle:
                         cv2.ellipse(
                             detected_frame,
                             min_max_area,
-                            (int(min_pupil_size / 2), int(min_pupil_size / 2)),
+                            min_axis,
                             int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             min_circle_color_tuple
                         )
                         cv2.ellipse(
                             detected_frame,
                             min_max_area,
-                            (int(max_pupil_size / 2), int(max_pupil_size / 2)),
+                            max_axis,
                             int(angle_of_pupil),
                             0, 360,  # start/end angle for drawing
                             max_circle_color_tuple
                         )
 
                 v_writer.write(detected_frame)
 
@@ -221,14 +234,20 @@
                         temp_dict = get_data_dict(return_data, frame_rate, frame_width, frame_height, direction_input)
                         csv_writer.writerow(temp_dict)
                 destination_file.close()
                 v_writer.release()
                 print(f"Result folder dir: {out_folder}.")
                 print(f"Result csv dir: {out_csv_dir}.")
                 print(f"Result video dir: {out_video_dir}.")
+                print_and_save(log_dir, f"Min detected pupil size : {round(detector.min_detected_pupil, 2)}")
+                print_and_save(log_dir, f"Max detected pupil size : {round(detector.max_detected_pupil, 2)}")
+                print_and_save(log_dir, f"Average detected pupil size : {round(detector.avg_detected_pupil, 2)}")
+                print_and_save(log_dir, f"Number of detections rejected "
+                                        f"by circular ratio : {detector.rejected_by_circular_ratio}")
+                print_and_save(log_dir, f"Number of detections rejected by pupil size : {detector.rejected_by_pupil_size}")
                 break
 
     raw_plot_info = plot_dict["raw_plot"]
     out_image_dir = raw_plot(out_csv_dir, raw_plot_info)
     print(f"Result plot image dir: {out_image_dir}.")
```

### Comparing `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.4.3
+Version: 3.5.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.4.3/src/ehdg_pupil_detector.egg-info/SOURCES.txt` & `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

