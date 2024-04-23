# Comparing `tmp/ctkdlib-4.2.tar.gz` & `tmp/ctkdlib-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkdlib-4.2.tar", last modified: Sun Apr  7 11:53:48 2024, max compression
+gzip compressed data, was "ctkdlib-5.0.tar", last modified: Tue Apr 23 10:44:15 2024, max compression
```

## Comparing `ctkdlib-4.2.tar` & `ctkdlib-5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 11:53:48.690549 ctkdlib-4.2/
--rw-rw-rw-   0        0        0     1086 2024-01-18 07:56:50.000000 ctkdlib-4.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1086 2024-04-07 11:53:48.690549 ctkdlib-4.2/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-03-13 10:43:59.000000 ctkdlib-4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 11:53:48.629261 ctkdlib-4.2/ctkdlib/
--rw-rw-rw-   0        0        0      685 2024-03-13 10:48:58.000000 ctkdlib-4.2/ctkdlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:53:48.685548 ctkdlib-4.2/ctkdlib/custom_widgets/
--rw-rw-rw-   0        0        0      477 2024-03-12 10:56:48.000000 ctkdlib-4.2/ctkdlib/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 ctkdlib-4.2/ctkdlib/custom_widgets/color_wheel.png
--rw-rw-rw-   0        0        0    12066 2024-02-22 07:44:24.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_calendar.py
--rw-rw-rw-   0        0        0     8619 2024-02-22 07:43:03.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_chart.py
--rw-rw-rw-   0        0        0     7504 2024-02-12 11:58:17.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_colorpicker.py
--rw-rw-rw-   0        0        0     7885 2024-04-07 11:50:38.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_draw.py
--rw-rw-rw-   0        0        0     4391 2024-03-10 14:04:27.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_gif.py
--rw-rw-rw-   0        0        0     6822 2024-02-09 06:29:39.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_graph.py
--rw-rw-rw-   0        0        0     2282 2024-02-09 06:50:34.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_hyperlink.py
--rw-rw-rw-   0        0        0     8508 2024-03-12 13:28:00.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_meter.py
--rw-rw-rw-   0        0        0     5287 2024-03-12 14:02:06.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_popupmenu.py
--rw-rw-rw-   0        0        0    59314 2024-02-08 18:29:38.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_rangeslider.py
--rw-rw-rw-   0        0        0    11004 2024-03-12 12:30:12.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_spinbox.py
--rw-rw-rw-   0        0        0     3404 2024-03-13 09:04:59.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_tooltip.py
--rw-rw-rw-   0        0        0    18678 2024-03-13 10:52:17.000000 ctkdlib-4.2/ctkdlib/custom_widgets/ctk_video.py
--rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 ctkdlib-4.2/ctkdlib/custom_widgets/target.png
-drwxrwxrwx   0        0        0        0 2024-04-07 11:53:48.688552 ctkdlib-4.2/ctkdlib.egg-info/
--rw-rw-rw-   0        0        0     1086 2024-04-07 11:53:48.000000 ctkdlib-4.2/ctkdlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2024-04-07 11:53:48.000000 ctkdlib-4.2/ctkdlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2024-04-07 11:53:48.000000 ctkdlib-4.2/ctkdlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-07 11:53:48.000000 ctkdlib-4.2/ctkdlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 11:53:48.000000 ctkdlib-4.2/ctkdlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      563 2024-04-07 11:53:48.693066 ctkdlib-4.2/setup.cfg
--rw-rw-rw-   0        0        0     1134 2024-04-07 11:52:51.000000 ctkdlib-4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:44:15.462387 ctkdlib-5.0/
+-rw-rw-rw-   0        0        0     1086 2024-01-18 07:56:50.000000 ctkdlib-5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1191 2024-04-23 10:44:15.461384 ctkdlib-5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-23 10:43:20.000000 ctkdlib-5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 10:44:15.260789 ctkdlib-5.0/ctkdlib/
+-rw-rw-rw-   0        0        0      725 2024-04-20 14:30:37.000000 ctkdlib-5.0/ctkdlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:44:15.457249 ctkdlib-5.0/ctkdlib/custom_widgets/
+-rw-rw-rw-   0        0        0      514 2024-04-20 14:00:40.000000 ctkdlib-5.0/ctkdlib/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 ctkdlib-5.0/ctkdlib/custom_widgets/color_wheel.png
+-rw-rw-rw-   0        0        0    12066 2024-02-22 07:44:24.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_calendar.py
+-rw-rw-rw-   0        0        0     8619 2024-02-22 07:43:03.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_chart.py
+-rw-rw-rw-   0        0        0     7504 2024-02-12 11:58:17.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_colorpicker.py
+-rw-rw-rw-   0        0        0     7885 2024-04-07 11:50:38.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_draw.py
+-rw-rw-rw-   0        0        0     4468 2024-04-21 15:13:18.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_gif.py
+-rw-rw-rw-   0        0        0     6822 2024-02-09 06:29:39.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_graph.py
+-rw-rw-rw-   0        0        0     2282 2024-02-09 06:50:34.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_hyperlink.py
+-rw-rw-rw-   0        0        0     8543 2024-04-22 07:17:28.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_meter.py
+-rw-rw-rw-   0        0        0     5287 2024-03-12 14:02:06.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_popupmenu.py
+-rw-rw-rw-   0        0        0    59314 2024-02-08 18:29:38.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_rangeslider.py
+-rw-rw-rw-   0        0        0    11004 2024-03-12 12:30:12.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_spinbox.py
+-rw-rw-rw-   0        0        0     3404 2024-03-13 09:04:59.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_tooltip.py
+-rw-rw-rw-   0        0        0    18680 2024-03-13 13:20:47.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_video.py
+-rw-rw-rw-   0        0        0     5691 2024-04-21 07:20:47.000000 ctkdlib-5.0/ctkdlib/custom_widgets/ctk_xyframe.py
+-rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 ctkdlib-5.0/ctkdlib/custom_widgets/target.png
+drwxrwxrwx   0        0        0        0 2024-04-23 10:44:15.459388 ctkdlib-5.0/ctkdlib.egg-info/
+-rw-rw-rw-   0        0        0     1191 2024-04-23 10:44:15.000000 ctkdlib-5.0/ctkdlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-04-23 10:44:15.000000 ctkdlib-5.0/ctkdlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2024-04-23 10:44:15.000000 ctkdlib-5.0/ctkdlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-23 10:44:15.000000 ctkdlib-5.0/ctkdlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 10:44:15.000000 ctkdlib-5.0/ctkdlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      563 2024-04-23 10:44:15.468914 ctkdlib-5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2024-04-23 10:14:40.000000 ctkdlib-5.0/setup.py
```

### Comparing `ctkdlib-4.2/LICENSE.txt` & `ctkdlib-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/PKG-INFO` & `ctkdlib-5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctkdlib
-Version: 4.2
+Version: 5.0
 Summary: A special widget library for CTkDesigner
 Home-page: https://github.com/Akascape/CTkDesigner
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,ctkdesigner,gui-builder,ui-designer,python-gui-builder
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -39,8 +39,11 @@
 
 ## Usage
 
 ```python
 from ctkdlib.custom_widgets import *
 ```
 
+[Read the docs](https://github.com/Akascape/CTkDesigner-Support/blob/main/ctkdlib_documentation.md)
+
+
 Author: Akash Bora (Akascape)
```

### Comparing `ctkdlib-4.2/ctkdlib/__init__.py` & `ctkdlib-5.0/ctkdlib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 from .custom_widgets import CTkChart
 from .custom_widgets import CTkCalendar
 from .custom_widgets import CTkGif
 from .custom_widgets import CTkTooltip
 from .custom_widgets import CTkDraw
 from .custom_widgets import CTkVideo
 from .custom_widgets import CTkPopupMenu
+from .custom_widgets import CTkXYFrame
```

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/color_wheel.png` & `ctkdlib-5.0/ctkdlib/custom_widgets/color_wheel.png`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_calendar.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_calendar.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_chart.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_chart.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_colorpicker.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_colorpicker.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_draw.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_draw.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_gif.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_gif.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,18 @@
             super().configure(fg_color="transparent")
             self.n_frame = self.gif.n_frames  
             self.frame_duration = self.gif.info['duration'] * 1/self.speed
         if "speed" in kwargs:
             self.speed = kwargs.pop("speed")
             if self.speed>50:
                 self.speed = 50
+            if self.speed<=0:
+                self.speed = 1
             self.frame_duration = self.gif.info['duration'] * 1/self.speed
+            
             if self.speed==0:
                 self.speed = 1
         
         super().configure(**kwargs)
 
     def cget(self, param):
         if param=="repeat":
```

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_graph.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_graph.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_hyperlink.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_hyperlink.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_meter.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_meter.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,21 @@
         width = self.width *10
         angle = int(float(self.arcvariable.get())) + 90
         self.im = Image.new('RGBA', (1000, 1000))
         draw = ImageDraw.Draw(self.im)
         draw.arc((0,0, 990, 990), 0, 360, self.widget._apply_appearance_mode(self.border_color), self.border_width)
         draw.arc((self.border_width, self.border_width, 990-self.border_width, 990-self.border_width), 0, 360, self.widget._apply_appearance_mode(self.foreground), width)
         draw.arc((self.border_width, self.border_width, 990-self.border_width, 990-self.border_width), 90, angle, self.widget._apply_appearance_mode(self.progresscolor), width)
-        draw.arc((width+self.border_width, width+self.border_width, 990-width-self.border_width, 990-width-self.border_width), 0, 360,
+        
+        x0 = width+self.border_width
+        x1 = 990-width-self.border_width
+        if x0>x1:
+            x1=x0
+
+        draw.arc((x0,x0,x1,x1), 0, 360,
                  self.widget._apply_appearance_mode(self.border_color), self.border_width)
         self.arc = ctk.CTkImage(self.im.resize((self.size, self.size), Image.LANCZOS), size=(self.size, self.size))
         super().configure(image=self.arc)
         
     def set(self, value):
         """Set the value of arcvariable and call loading_hover_effect if refresh_value is True"""
         angle = float(-(360/(self.min_value - self.max_value))*(value - self.max_value))
```

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_popupmenu.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_popupmenu.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_rangeslider.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_rangeslider.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_spinbox.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_spinbox.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_tooltip.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/ctk_video.py` & `ctkdlib-5.0/ctkdlib/custom_widgets/ctk_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         self.set_scaled(scaled)
         self._keep_aspect_ratio = keep_aspect
         self._resampling_method: int = Image.NEAREST
 
         self.bind("<<Destroy>>", self.stop)
         self.bind("<<FrameGenerated>>", self._display_frame)
 
-        if missing:
-            warnings.warn("You are using CTkVideo without installing pyav and pyaudio, please install them!")
+        #if missing:
+            #warnings.warn("You are using CTkVideo without installing pyav and pyaudio, please install them!")
             
     def keep_aspect(self, keep_aspect: bool):
         """ keeps the aspect ratio when resizing the image """
         self._keep_aspect_ratio = keep_aspect
 
     def set_resampling_method(self, method: int):
         """ sets the resampling method when resizing """
```

### Comparing `ctkdlib-4.2/ctkdlib/custom_widgets/target.png` & `ctkdlib-5.0/ctkdlib/custom_widgets/target.png`

 * *Files identical despite different names*

### Comparing `ctkdlib-4.2/ctkdlib.egg-info/PKG-INFO` & `ctkdlib-5.0/ctkdlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctkdlib
-Version: 4.2
+Version: 5.0
 Summary: A special widget library for CTkDesigner
 Home-page: https://github.com/Akascape/CTkDesigner
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,ctkdesigner,gui-builder,ui-designer,python-gui-builder
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -39,8 +39,11 @@
 
 ## Usage
 
 ```python
 from ctkdlib.custom_widgets import *
 ```
 
+[Read the docs](https://github.com/Akascape/CTkDesigner-Support/blob/main/ctkdlib_documentation.md)
+
+
 Author: Akash Bora (Akascape)
```

### Comparing `ctkdlib-4.2/ctkdlib.egg-info/SOURCES.txt` & `ctkdlib-5.0/ctkdlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 ctkdlib/custom_widgets/ctk_hyperlink.py
 ctkdlib/custom_widgets/ctk_meter.py
 ctkdlib/custom_widgets/ctk_popupmenu.py
 ctkdlib/custom_widgets/ctk_rangeslider.py
 ctkdlib/custom_widgets/ctk_spinbox.py
 ctkdlib/custom_widgets/ctk_tooltip.py
 ctkdlib/custom_widgets/ctk_video.py
+ctkdlib/custom_widgets/ctk_xyframe.py
 ctkdlib/custom_widgets/target.png
```

### Comparing `ctkdlib-4.2/setup.cfg` & `ctkdlib-5.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 746b 646c 6962 0d0a 7665 7273   = ctkdlib..vers
-00000020: 696f 6e20 3d20 342e 320d 0a64 6573 6372  ion = 4.2..descr
+00000020: 696f 6e20 3d20 352e 300d 0a64 6573 6372  ion = 5.0..descr
 00000030: 6970 7469 6f6e 203d 2041 2073 7065 6369  iption = A speci
 00000040: 616c 2077 6964 6765 7420 6c69 6272 6172  al widget librar
 00000050: 7920 666f 7220 4354 6b44 6573 6967 6e65  y for CTkDesigne
 00000060: 720d 0a6c 6f6e 675f 6465 7363 7269 7074  r..long_descript
 00000070: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
 00000080: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 00000090: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
```

### Comparing `ctkdlib-4.2/setup.py` & `ctkdlib-5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'ctkdlib',
-    version = '4.2',
+    version = '5.0',
     description = "A special widget library for CTkDesigner",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkDesigner",
```

