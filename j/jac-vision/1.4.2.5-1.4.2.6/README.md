# Comparing `tmp/jac_vision-1.4.2.5.tar.gz` & `tmp/jac_vision-1.4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_vision-1.4.2.5.tar", last modified: Tue Jan  9 16:44:24 2024, max compression
+gzip compressed data, was "jac_vision-1.4.2.6.tar", last modified: Tue Apr 23 19:42:50 2024, max compression
```

## Comparing `jac_vision-1.4.2.5.tar` & `jac_vision-1.4.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.635903 jac_vision-1.4.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-01-09 16:44:24.635903 jac_vision-1.4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.631904 jac_vision-1.4.2.5/jac_vision/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.631904 jac_vision-1.4.2.5/jac_vision/detr/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/detr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/detr/detr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/detr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/detr/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.631904 jac_vision-1.4.2.5/jac_vision/dpt/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/dpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/dpt/dpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/dpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/dpt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.635903 jac_vision-1.4.2.5/jac_vision/rftm/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/rftm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/rftm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/rftm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/rftm/rftm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.635903 jac_vision-1.4.2.5/jac_vision/yolos/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/yolos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/yolos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/yolos/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/jac_vision/yolos/yolos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:24.635903 jac_vision-1.4.2.5/jac_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-01-09 16:44:24.000000 jac_vision-1.4.2.5/jac_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-09 16:44:24.000000 jac_vision-1.4.2.5/jac_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:44:24.000000 jac_vision-1.4.2.5/jac_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-09 16:44:24.000000 jac_vision-1.4.2.5/jac_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-09 16:44:24.000000 jac_vision-1.4.2.5/jac_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 16:44:24.635903 jac_vision-1.4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-09 16:44:08.000000 jac_vision-1.4.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.576603 jac_vision-1.4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-23 19:42:50.576603 jac_vision-1.4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.568603 jac_vision-1.4.2.6/jac_vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.572603 jac_vision-1.4.2.6/jac_vision/detr/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/detr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/detr/detr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/detr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/detr/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.572603 jac_vision-1.4.2.6/jac_vision/dpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/dpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/dpt/dpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/dpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/dpt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.572603 jac_vision-1.4.2.6/jac_vision/rftm/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/rftm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/rftm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/rftm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/rftm/rftm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.572603 jac_vision-1.4.2.6/jac_vision/yolos/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/yolos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/yolos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/yolos/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/jac_vision/yolos/yolos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:50.572603 jac_vision-1.4.2.6/jac_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-23 19:42:50.000000 jac_vision-1.4.2.6/jac_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 19:42:50.000000 jac_vision-1.4.2.6/jac_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:42:50.000000 jac_vision-1.4.2.6/jac_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 19:42:50.000000 jac_vision-1.4.2.6/jac_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 19:42:50.000000 jac_vision-1.4.2.6/jac_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:42:50.576603 jac_vision-1.4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 19:42:34.000000 jac_vision-1.4.2.6/setup.py
```

### Comparing `jac_vision-1.4.2.5/PKG-INFO` & `jac_vision-1.4.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jac_vision
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
-Requires-Dist: jaseci==1.4.2.5
+Requires-Dist: jaseci==1.4.2.6
 Requires-Dist: pytest<7.1,>=7.0.1
 Requires-Dist: pytest-order<1.1,>=1.0.1
 Provides-Extra: all
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
 Requires-Dist: numpy>=1.23.0; extra == "all"
 Requires-Dist: transformers>=4.25.1; extra == "all"
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
```

### Comparing `jac_vision-1.4.2.5/jac_vision/detr/detr.py` & `jac_vision-1.4.2.6/jac_vision/detr/detr.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision/detr/model.py` & `jac_vision-1.4.2.6/jac_vision/detr/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision/dpt/dpt.py` & `jac_vision-1.4.2.6/jac_vision/dpt/dpt.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision/dpt/model.py` & `jac_vision-1.4.2.6/jac_vision/dpt/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision/rftm/model.py` & `jac_vision-1.4.2.6/jac_vision/rftm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,14 @@
 def resnet152(**kwargs):
     """Constructs a ResNet-101 model."""
     model = ResNeXt(ResNeXtBottleneck, [3, 8, 36, 3], **kwargs)
     return model
 
 
 class ToTensor(object):
-
     """Convert a ``PIL.Image`` or ``numpy.ndarray`` to tensor.
     Converts a PIL.Image or numpy.ndarray (H x W x C) in the range
     [0, 255] to a torch.FloatTensor of shape (C x H x W) in the range [0.0, 1.0].
     """
 
     def __init__(self, norm_value=255):
         self.norm_value = norm_value
```

### Comparing `jac_vision-1.4.2.5/jac_vision/rftm/rftm.py` & `jac_vision-1.4.2.6/jac_vision/rftm/rftm.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision/yolos/model.py` & `jac_vision-1.4.2.6/jac_vision/yolos/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision/yolos/yolos.py` & `jac_vision-1.4.2.6/jac_vision/yolos/yolos.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/jac_vision.egg-info/PKG-INFO` & `jac_vision-1.4.2.6/jac_vision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jac_vision
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
-Requires-Dist: jaseci==1.4.2.5
+Requires-Dist: jaseci==1.4.2.6
 Requires-Dist: pytest<7.1,>=7.0.1
 Requires-Dist: pytest-order<1.1,>=1.0.1
 Provides-Extra: all
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
 Requires-Dist: numpy>=1.23.0; extra == "all"
 Requires-Dist: transformers>=4.25.1; extra == "all"
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
```

### Comparing `jac_vision-1.4.2.5/jac_vision.egg-info/SOURCES.txt` & `jac_vision-1.4.2.6/jac_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.2.5/setup.py` & `jac_vision-1.4.2.6/setup.py`

 * *Files identical despite different names*

