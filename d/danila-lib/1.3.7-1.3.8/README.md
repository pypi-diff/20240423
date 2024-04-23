# Comparing `tmp/danila-lib-1.3.7.tar.gz` & `tmp/danila-lib-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.3.7.tar", last modified: Mon Apr 22 21:02:14 2024, max compression
+gzip compressed data, was "danila-lib-1.3.8.tar", last modified: Mon Apr 22 21:09:32 2024, max compression
```

## Comparing `danila-lib-1.3.7.tar` & `danila-lib-1.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 21:02:14.728900 danila-lib-1.3.7/
--rw-rw-rw-   0        0        0     9615 2024-04-22 21:02:14.727905 danila-lib-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 21:02:14.704012 danila-lib-1.3.7/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.3.7/danila/__init__.py
--rw-rw-rw-   0        0        0     9738 2024-04-22 21:01:41.000000 danila-lib-1.3.7/danila/danila.py
-drwxrwxrwx   0        0        0        0 2024-04-22 21:02:14.718945 danila-lib-1.3.7/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-04-22 21:02:14.000000 danila-lib-1.3.7/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2024-04-22 21:02:14.000000 danila-lib-1.3.7/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 21:02:14.000000 danila-lib-1.3.7/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-04-22 21:02:14.000000 danila-lib-1.3.7/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 21:02:14.000000 danila-lib-1.3.7/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 21:02:14.719941 danila-lib-1.3.7/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.3.7/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 21:02:14.722927 danila-lib-1.3.7/data/neuro/
--rw-rw-rw-   0        0        0     5749 2024-04-22 21:01:41.000000 danila-lib-1.3.7/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.3.7/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.3.7/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.3.7/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.3.7/data/neuro/__init__.py
--rw-rw-rw-   0        0        0      675 2024-04-22 21:01:41.000000 danila-lib-1.3.7/data/neuro/models.py
-drwxrwxrwx   0        0        0        0 2024-04-22 21:02:14.727905 danila-lib-1.3.7/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.3.7/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.3.7/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.3.7/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.3.7/data/result/Label_area.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.3.7/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.3.7/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.3.7/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.3.7/data/result/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-22 21:02:14.729896 danila-lib-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-22 21:02:12.000000 danila-lib-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:09:32.148320 danila-lib-1.3.8/
+-rw-rw-rw-   0        0        0     9615 2024-04-22 21:09:32.148320 danila-lib-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 21:09:32.127413 danila-lib-1.3.8/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.3.8/danila/__init__.py
+-rw-rw-rw-   0        0        0     9738 2024-04-22 21:01:41.000000 danila-lib-1.3.8/danila/danila.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:09:32.138365 danila-lib-1.3.8/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-04-22 21:09:32.000000 danila-lib-1.3.8/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2024-04-22 21:09:32.000000 danila-lib-1.3.8/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 21:09:32.000000 danila-lib-1.3.8/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-04-22 21:09:32.000000 danila-lib-1.3.8/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 21:09:32.000000 danila-lib-1.3.8/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 21:09:32.139361 danila-lib-1.3.8/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.3.8/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:09:32.142347 danila-lib-1.3.8/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.3.8/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.3.8/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.3.8/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.3.8/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.3.8/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0      675 2024-04-22 21:01:41.000000 danila-lib-1.3.8/data/neuro/models.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:09:32.147325 danila-lib-1.3.8/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.3.8/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.3.8/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.3.8/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.3.8/data/result/Label_area.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.3.8/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.3.8/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.3.8/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.3.8/data/result/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-22 21:09:32.150311 danila-lib-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-22 21:09:27.000000 danila-lib-1.3.8/setup.py
```

### Comparing `danila-lib-1.3.7/PKG-INFO` & `danila-lib-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.3.7
+Version: 1.3.8
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.3.7/README.md` & `danila-lib-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/danila/danila.py` & `danila-lib-1.3.8/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.3.8/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.3.7
+Version: 1.3.8
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.3.7/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.3.8/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/danila_lib.egg-info/requires.txt` & `danila-lib-1.3.8/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/neuro/Letters_recognize.py` & `danila-lib-1.3.8/data/neuro/Letters_recognize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import zipfile
+import requests
 from urllib.parse import urlencode
 
 import cv2
 import keras
 import numpy as np
-from google.auth.transport import requests
 
 from data.neuro.models import *
 from data.result.Class_text import Class_text
 from data.result.Label_area import Label_area
 """class for recognizing letters in text_area"""
 
 class Letters_recognize:
```

### Comparing `danila-lib-1.3.7/data/neuro/Rama_classify_class.py` & `danila-lib-1.3.8/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/neuro/Rama_detect_class.py` & `danila-lib-1.3.8/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/neuro/Text_detect_class.py` & `danila-lib-1.3.8/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/neuro/models.py` & `danila-lib-1.3.8/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/result/Image_text_areas.py` & `danila-lib-1.3.8/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/result/Rect.py` & `danila-lib-1.3.8/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/result/Text_area.py` & `danila-lib-1.3.8/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/data/result/Yolo_label_rect.py` & `danila-lib-1.3.8/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.3.7/setup.py` & `danila-lib-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.3.7',
+  version='1.3.8',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

