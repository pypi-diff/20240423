# Comparing `tmp/attosecondraytracing_core-0.9.tar.gz` & `tmp/attosecondraytracing_core-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attosecondraytracing_core-0.9.tar", last modified: Mon Apr 22 08:28:35 2024, max compression
+gzip compressed data, was "attosecondraytracing_core-0.92.tar", last modified: Tue Apr 23 13:42:13 2024, max compression
```

## Comparing `attosecondraytracing_core-0.9.tar` & `attosecondraytracing_core-0.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:35.321594 attosecondraytracing_core-0.9/
--rw-r--r--   0 andre     (1000) andre     (1000)    26526 2024-04-15 11:23:52.000000 attosecondraytracing_core-0.9/LICENSE
--rw-r--r--   0 andre     (1000) andre     (1000)     4569 2024-04-22 08:28:35.321594 attosecondraytracing_core-0.9/PKG-INFO
--rw-r--r--   0 andre     (1000) andre     (1000)     3971 2024-04-22 08:24:48.000000 attosecondraytracing_core-0.9/README.md
--rw-r--r--   0 andre     (1000) andre     (1000)      802 2024-04-22 08:04:10.000000 attosecondraytracing_core-0.9/pyproject.toml
--rw-r--r--   0 andre     (1000) andre     (1000)       38 2024-04-22 08:28:35.321594 attosecondraytracing_core-0.9/setup.cfg
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:35.321594 attosecondraytracing_core-0.9/src/
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:35.321594 attosecondraytracing_core-0.9/src/ART_core/
--rw-r--r--   0 andre     (1000) andre     (1000)     6186 2024-04-22 08:09:01.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleDefects.py
--rw-r--r--   0 andre     (1000) andre     (1000)    10159 2024-04-22 08:09:03.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleDetector.py
--rw-r--r--   0 andre     (1000) andre     (1000)    10257 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleGeometry.py
--rw-r--r--   0 andre     (1000) andre     (1000)     3862 2024-04-22 08:09:04.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleMask.py
--rw-r--r--   0 andre     (1000) andre     (1000)    31860 2024-04-22 08:09:05.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleMirror.py
--rw-r--r--   0 andre     (1000) andre     (1000)    27737 2024-04-22 08:09:05.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleOpticalChain.py
--rw-r--r--   0 andre     (1000) andre     (1000)    10018 2024-04-22 08:09:06.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleOpticalElement.py
--rw-r--r--   0 andre     (1000) andre     (1000)     4995 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleOpticalRay.py
--rw-r--r--   0 andre     (1000) andre     (1000)    24386 2024-04-22 08:09:07.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleProcessing.py
--rw-r--r--   0 andre     (1000) andre     (1000)     8702 2024-04-22 08:09:07.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleSource.py
--rw-r--r--   0 andre     (1000) andre     (1000)    18090 2024-04-22 08:09:08.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleSupport.py
--rw-r--r--   0 andre     (1000) andre     (1000)    10647 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.9/src/ART_core/ModuleZernike.py
--rw-r--r--   0 andre     (1000) andre     (1000)      142 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.9/src/ART_core/__init__.py
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-22 08:28:35.321594 attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/
--rw-r--r--   0 andre     (1000) andre     (1000)     4569 2024-04-22 08:28:35.000000 attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/PKG-INFO
--rw-r--r--   0 andre     (1000) andre     (1000)      696 2024-04-22 08:28:35.000000 attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/SOURCES.txt
--rw-r--r--   0 andre     (1000) andre     (1000)        1 2024-04-22 08:28:35.000000 attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/dependency_links.txt
--rw-r--r--   0 andre     (1000) andre     (1000)       29 2024-04-22 08:28:35.000000 attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/requires.txt
--rw-r--r--   0 andre     (1000) andre     (1000)        9 2024-04-22 08:28:35.000000 attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/top_level.txt
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:13.556851 attosecondraytracing_core-0.92/
+-rw-r--r--   0 andre     (1000) andre     (1000)    26526 2024-04-15 11:23:52.000000 attosecondraytracing_core-0.92/LICENSE
+-rw-r--r--   0 andre     (1000) andre     (1000)     2833 2024-04-23 13:42:13.556851 attosecondraytracing_core-0.92/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)     2234 2024-04-23 13:40:40.000000 attosecondraytracing_core-0.92/README.md
+-rw-r--r--   0 andre     (1000) andre     (1000)      803 2024-04-23 13:41:45.000000 attosecondraytracing_core-0.92/pyproject.toml
+-rw-r--r--   0 andre     (1000) andre     (1000)       38 2024-04-23 13:42:13.556851 attosecondraytracing_core-0.92/setup.cfg
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:13.553517 attosecondraytracing_core-0.92/src/
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:13.556851 attosecondraytracing_core-0.92/src/ARTcore/
+-rw-r--r--   0 andre     (1000) andre     (1000)     6185 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleDefects.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    10157 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleDetector.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    10257 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleGeometry.py
+-rw-r--r--   0 andre     (1000) andre     (1000)     3861 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleMask.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    31859 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleMirror.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    27732 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleOpticalChain.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    10017 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleOpticalElement.py
+-rw-r--r--   0 andre     (1000) andre     (1000)     4995 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleOpticalRay.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    24378 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleProcessing.py
+-rw-r--r--   0 andre     (1000) andre     (1000)     8699 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleSource.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    18089 2024-04-23 13:36:34.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleSupport.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    10647 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.92/src/ARTcore/ModuleZernike.py
+-rw-r--r--   0 andre     (1000) andre     (1000)      142 2024-04-15 08:05:22.000000 attosecondraytracing_core-0.92/src/ARTcore/__init__.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2024-04-23 13:42:13.556851 attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/
+-rw-r--r--   0 andre     (1000) andre     (1000)     2833 2024-04-23 13:42:13.000000 attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)      683 2024-04-23 13:42:13.000000 attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/SOURCES.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        1 2024-04-23 13:42:13.000000 attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/dependency_links.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)       29 2024-04-23 13:42:13.000000 attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/requires.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        8 2024-04-23 13:42:13.000000 attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/top_level.txt
```

### Comparing `attosecondraytracing_core-0.9/LICENSE` & `attosecondraytracing_core-0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `attosecondraytracing_core-0.9/pyproject.toml` & `attosecondraytracing_core-0.92/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "package_name.__version__"}
 
 [project]
 name = "AttosecondRayTracing_core"
-version = "0.9"
+version = "0.92"
 authors = [
   { name="Stefan Haessler", email="stefan.haessler@ensta-paris.fr" },
   { name="André Kalouguine", email="andre.kalouguine@ensta-paris.fr" },
   { name="Anthony Guillaume"}
 ]
 description = "Attosecond Ray Tracing core calculation package"
 readme = "README.md"
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleDefects.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleDefects.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # %% Modules
 
 import numpy as np
 #import cupy as cp
 from abc import ABC, abstractmethod
 import scipy
 import math
-from ART_core.ModuleZernike import zernike_gradient
+from ARTcore.ModuleZernike import zernike_gradient
 
 # %% Abstract class
 
 
 class Defect(ABC):
     """
     Abstract class representing a defect on the optical surface.
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleDetector.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleDetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 Created in Sept 2020
 
 @author: Stefan Haessler
 """
 # %% Modules
 
 import numpy as np
-import ART_core.ModuleProcessing as mp
-import ART_core.ModuleGeometry as mgeo
+import ARTcore.ModuleProcessing as mp
+import ARTcore.ModuleGeometry as mgeo
 
 LightSpeed = 299792458000
 
 
 # %%
 class Detector:
     """
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleGeometry.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleGeometry.py`

 * *Files identical despite different names*

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleMask.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleMask.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Created in 2021
 
 @author: Stefan Haessler
 """
 # %% Modules
 
 import numpy as np
-import ART_core.ModuleGeometry as mgeo
+import ARTcore.ModuleGeometry as mgeo
 
 
 # %%############################################################################
 class Mask:
     """
     A mask: a plane surface of the shape of its [Support](ModuleSupport.html), which stops all rays that hit it,
     while all other rays continue their path unchanged.
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleMirror.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleMirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Created in 2019
 
 @author: Anthony Guillaume and Stefan Haessler and Semptum and Charles Bourassin-Bouchet
 """
 # %% Modules
 
 import numpy as np
-import ART_core.ModuleGeometry as mgeo
+import ARTcore.ModuleGeometry as mgeo
 import math
 
 
 # %%
 
 
 def _IntersectionRayMirror(PointMirror, ListPointIntersectionMirror):
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleOpticalChain.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleOpticalChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 Created in Jan 2022
 
 @author: Stefan Haessler
 """
 # %% Modules
 import copy
 import numpy as np
-import ART_core.ModuleProcessing as mp
-import ART_core.ModuleGeometry as mgeo
-import ART_core.ModuleOpticalRay as mray
-import ART_core.ModuleOpticalElement as moe
-import ART_core.ModuleSource as msource
+import ARTcore.ModuleProcessing as mp
+import ARTcore.ModuleGeometry as mgeo
+import ARTcore.ModuleOpticalRay as mray
+import ARTcore.ModuleOpticalElement as moe
+import ARTcore.ModuleSource as msource
 
 
 # %%
 class OpticalChain:
     """
     The OpticalChain represents the whole optical setup to be simulated:
     Its main attributes are a list source-[Rays](ModuleOpticalRay.html) and
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleOpticalElement.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleOpticalElement.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Created in Apr 2020
 
 @author: Anthony Guillaume + Stefan Haessler
 """
 # %%
 import numpy as np
-import ART_core.ModuleGeometry as mgeo
+import ARTcore.ModuleGeometry as mgeo
 
 
 # %%
 class OpticalElement:
     """
     An optical element, to define the position and orientation of different optics in the 'lab-frame'.
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleOpticalRay.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleOpticalRay.py`

 * *Files identical despite different names*

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleProcessing.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleProcessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 # import gzip
 import lzma
 from time import perf_counter
 from datetime import datetime
 import copy
 import numpy as np
-import ART_core.ModuleGeometry as mgeo
-import ART_core.ModuleMirror as mmirror
-import ART_core.ModuleMask as mmask
-import ART_core.ModuleSource as msource
-import ART_core.ModuleOpticalElement as moe
-import ART_core.ModuleOpticalRay as mray
-import ART_core.ModuleSupport as msupp
-import ART_core.ModuleOpticalChain as moc
+import ARTcore.ModuleGeometry as mgeo
+import ARTcore.ModuleMirror as mmirror
+import ARTcore.ModuleMask as mmask
+import ARTcore.ModuleSource as msource
+import ARTcore.ModuleOpticalElement as moe
+import ARTcore.ModuleOpticalRay as mray
+import ARTcore.ModuleSupport as msupp
+import ARTcore.ModuleOpticalChain as moc
 
 
 # %%
 def _singleOEPlacement(
     SourceProperties: dict,
     OpticsList: list,
     DistanceList: list[(int, float)],
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleSource.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleSource.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 @author: Anthony Guillaume and Stefan Haessler
 """
 
 # %% Modules
 
 import numpy as np
-import ART_core.ModuleOpticalRay as mray
-import ART_core.ModuleGeometry as mgeo
-import ART_core.ModuleProcessing as mp
+import ARTcore.ModuleOpticalRay as mray
+import ARTcore.ModuleGeometry as mgeo
+import ARTcore.ModuleProcessing as mp
 
 # %%
 
 
 def _Cone(Angle: float, NbRays: int, Wavelength=None):
     """
     Return a list of rays filling a cone according to Vogel's spiral.
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleSupport.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleSupport.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @author: Anthony Guillaume and Stefan Haessler
 """
 
 # %%
 
 import numpy as np
 import math
-import ART_core.ModuleGeometry as mgeo
+import ARTcore.ModuleGeometry as mgeo
 from abc import ABC, abstractmethod
 
 
 # %%
 
 
 class Support(ABC):
```

### Comparing `attosecondraytracing_core-0.9/src/ART_core/ModuleZernike.py` & `attosecondraytracing_core-0.92/src/ARTcore/ModuleZernike.py`

 * *Files identical despite different names*

### Comparing `attosecondraytracing_core-0.9/src/AttosecondRayTracing_core.egg-info/SOURCES.txt` & `attosecondraytracing_core-0.92/src/AttosecondRayTracing_core.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
-src/ART_core/ModuleDefects.py
-src/ART_core/ModuleDetector.py
-src/ART_core/ModuleGeometry.py
-src/ART_core/ModuleMask.py
-src/ART_core/ModuleMirror.py
-src/ART_core/ModuleOpticalChain.py
-src/ART_core/ModuleOpticalElement.py
-src/ART_core/ModuleOpticalRay.py
-src/ART_core/ModuleProcessing.py
-src/ART_core/ModuleSource.py
-src/ART_core/ModuleSupport.py
-src/ART_core/ModuleZernike.py
-src/ART_core/__init__.py
+src/ARTcore/ModuleDefects.py
+src/ARTcore/ModuleDetector.py
+src/ARTcore/ModuleGeometry.py
+src/ARTcore/ModuleMask.py
+src/ARTcore/ModuleMirror.py
+src/ARTcore/ModuleOpticalChain.py
+src/ARTcore/ModuleOpticalElement.py
+src/ARTcore/ModuleOpticalRay.py
+src/ARTcore/ModuleProcessing.py
+src/ARTcore/ModuleSource.py
+src/ARTcore/ModuleSupport.py
+src/ARTcore/ModuleZernike.py
+src/ARTcore/__init__.py
 src/AttosecondRayTracing_core.egg-info/PKG-INFO
 src/AttosecondRayTracing_core.egg-info/SOURCES.txt
 src/AttosecondRayTracing_core.egg-info/dependency_links.txt
 src/AttosecondRayTracing_core.egg-info/requires.txt
 src/AttosecondRayTracing_core.egg-info/top_level.txt
```

