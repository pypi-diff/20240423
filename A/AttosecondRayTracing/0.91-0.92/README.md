# Comparing `tmp/attosecondraytracing-0.91.tar.gz` & `tmp/attosecondraytracing-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attosecondraytracing-0.91.tar", last modified: Mon Apr 22 08:28:16 2024, max compression
+gzip compressed data, was "attosecondraytracing-0.92.tar", last modified: Tue Apr 23 13:42:04 2024, max compression
```

## Comparing `attosecondraytracing-0.91.tar` & `attosecondraytracing-0.92.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:16.534780 attosecondraytracing-0.91/
--rw-r--r--   0 andre     (1000) andre     (1000)    26527 2024-04-15 11:24:05.000000 attosecondraytracing-0.91/LICENSE
--rw-r--r--   0 andre     (1000) andre     (1000)      615 2024-04-22 08:28:16.531447 attosecondraytracing-0.91/PKG-INFO
--rw-r--r--   0 andre     (1000) andre     (1000)     3971 2024-04-22 08:27:39.000000 attosecondraytracing-0.91/README.md
--rw-r--r--   0 andre     (1000) andre     (1000)      815 2024-04-22 08:28:00.000000 attosecondraytracing-0.91/pyproject.toml
--rw-r--r--   0 andre     (1000) andre     (1000)       38 2024-04-22 08:28:16.534780 attosecondraytracing-0.91/setup.cfg
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:16.531447 attosecondraytracing-0.91/src/
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:16.531447 attosecondraytracing-0.91/src/ART/
--rw-r--r--   0 andre     (1000) andre     (1000)    16034 2024-04-22 08:11:47.000000 attosecondraytracing-0.91/src/ART/ARTmain.py
--rw-r--r--   0 andre     (1000) andre     (1000)     2823 2024-04-15 08:05:22.000000 attosecondraytracing-0.91/src/ART/DefaultOptions.py
--rw-r--r--   0 andre     (1000) andre     (1000)    25514 2024-04-22 08:07:07.000000 attosecondraytracing-0.91/src/ART/ModuleAnalysisAndPlots.py
--rw-r--r--   0 andre     (1000) andre     (1000)      142 2024-04-15 08:05:22.000000 attosecondraytracing-0.91/src/ART/__init__.py
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:16.531447 attosecondraytracing-0.91/src/AttosecondRayTracing.egg-info/
--rw-r--r--   0 andre     (1000) andre     (1000)      615 2024-04-22 08:28:16.000000 attosecondraytracing-0.91/src/AttosecondRayTracing.egg-info/PKG-INFO
--rw-r--r--   0 andre     (1000) andre     (1000)      370 2024-04-22 08:28:16.000000 attosecondraytracing-0.91/src/AttosecondRayTracing.egg-info/SOURCES.txt
--rw-r--r--   0 andre     (1000) andre     (1000)        1 2024-04-22 08:28:16.000000 attosecondraytracing-0.91/src/AttosecondRayTracing.egg-info/dependency_links.txt
--rw-r--r--   0 andre     (1000) andre     (1000)       64 2024-04-22 08:28:16.000000 attosecondraytracing-0.91/src/AttosecondRayTracing.egg-info/requires.txt
--rw-r--r--   0 andre     (1000) andre     (1000)        4 2024-04-22 08:28:16.000000 attosecondraytracing-0.91/src/AttosecondRayTracing.egg-info/top_level.txt
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:04.230173 attosecondraytracing-0.92/
+-rw-r--r--   0 andre     (1000) andre     (1000)    26527 2024-04-15 11:24:05.000000 attosecondraytracing-0.92/LICENSE
+-rw-r--r--   0 andre     (1000) andre     (1000)     2547 2024-04-23 13:42:04.230173 attosecondraytracing-0.92/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)     1891 2024-04-23 13:41:15.000000 attosecondraytracing-0.92/README.md
+-rw-r--r--   0 andre     (1000) andre     (1000)      836 2024-04-23 13:41:38.000000 attosecondraytracing-0.92/pyproject.toml
+-rw-r--r--   0 andre     (1000) andre     (1000)       38 2024-04-23 13:42:04.230173 attosecondraytracing-0.92/setup.cfg
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:04.226840 attosecondraytracing-0.92/src/
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:04.226840 attosecondraytracing-0.92/src/ART/
+-rw-r--r--   0 andre     (1000) andre     (1000)    16031 2024-04-23 13:36:32.000000 attosecondraytracing-0.92/src/ART/ARTmain.py
+-rw-r--r--   0 andre     (1000) andre     (1000)     2823 2024-04-15 08:05:22.000000 attosecondraytracing-0.92/src/ART/DefaultOptions.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    25512 2024-04-23 13:36:34.000000 attosecondraytracing-0.92/src/ART/ModuleAnalysisAndPlots.py
+-rw-r--r--   0 andre     (1000) andre     (1000)      142 2024-04-15 08:05:22.000000 attosecondraytracing-0.92/src/ART/__init__.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:04.230173 attosecondraytracing-0.92/src/AttosecondRayTracing.egg-info/
+-rw-r--r--   0 andre     (1000) andre     (1000)     2547 2024-04-23 13:42:04.000000 attosecondraytracing-0.92/src/AttosecondRayTracing.egg-info/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)      370 2024-04-23 13:42:04.000000 attosecondraytracing-0.92/src/AttosecondRayTracing.egg-info/SOURCES.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        1 2024-04-23 13:42:04.000000 attosecondraytracing-0.92/src/AttosecondRayTracing.egg-info/dependency_links.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)       64 2024-04-23 13:42:04.000000 attosecondraytracing-0.92/src/AttosecondRayTracing.egg-info/requires.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        4 2024-04-23 13:42:04.000000 attosecondraytracing-0.92/src/AttosecondRayTracing.egg-info/top_level.txt
```

### Comparing `attosecondraytracing-0.91/LICENSE` & `attosecondraytracing-0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `attosecondraytracing-0.91/pyproject.toml` & `attosecondraytracing-0.92/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "package_name.__version__"}
 
 [project]
 name = "AttosecondRayTracing"
-version = "0.91"
+version = "0.92"
 authors = [
   { name="Stefan Haessler", email="stefan.haessler@ensta-paris.fr" },
   { name="André Kalouguine", email="andre.kalouguine@ensta-paris.fr" },
   { name="Anthony Guillaume"}
 ]
 description = "Attosecond Ray Tracing visualisation package"
+readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies= ["AttosecondRayTracing_core", "pyvista", "matplotlib", "pyvistaqt", "colorcet"]
```

### Comparing `attosecondraytracing-0.91/src/ART/ARTmain.py` & `attosecondraytracing-0.92/src/ART/ARTmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 @author: Stefan Haessler
 """
 import os
 import sys
 from datetime import datetime
 import numpy as np
 import importlib.util
-import ART_core.ModuleProcessing as mp
-import ART_core.ModuleDetector as mdet
+import ARTcore.ModuleProcessing as mp
+import ARTcore.ModuleDetector as mdet
 import ART.ModuleAnalysisAndPlots as mplots
 #import matplotlib.pyplot as plt
-import ART_core.ModuleOpticalChain as moc
+import ARTcore.ModuleOpticalChain as moc
 
 
 def print_banner(i):
     """Show the important name banner and the version-number and date."""
 
     banner = [
         r"""
```

### Comparing `attosecondraytracing-0.91/src/ART/DefaultOptions.py` & `attosecondraytracing-0.92/src/ART/DefaultOptions.py`

 * *Files identical despite different names*

### Comparing `attosecondraytracing-0.91/src/ART/ModuleAnalysisAndPlots.py` & `attosecondraytracing-0.92/src/ART/ModuleAnalysisAndPlots.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
 import pyvista as pv
 import pyvistaqt as pvqt
 import colorcet as cc
 import colorsys
 
-import ART_core.ModuleProcessing as mp
-import ART_core.ModuleGeometry as mgeo
+import ARTcore.ModuleProcessing as mp
+import ARTcore.ModuleGeometry as mgeo
 import itertools
 
 
 # %%
 def _getDetectorPoints(RayListAnalysed, Detector) -> tuple[np.ndarray, np.ndarray, float, float]:
     """
     Prepare the ray impact points on the detector in a format used for the plotting,
```

