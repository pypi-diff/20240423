# Comparing `tmp/wassncplot-2.5.1.tar.gz` & `tmp/wassncplot-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-mx_jjtzu/wassncplot-2.5.1.tar", last modified: Tue Apr 16 12:39:45 2024, max compression
+gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-caeh1pdo/wassncplot-2.5.3.tar", last modified: Tue Apr 23 07:32:30 2024, max compression
```

## Comparing `wassncplot-2.5.1.tar` & `wassncplot-2.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-16 12:39:45.723531 wassncplot-2.5.1/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.5.1/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.5.1/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-16 12:39:45.723531 wassncplot-2.5.1/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.719531 wassncplot-2.5.1/src/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/src/wassncplot/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/waveview2.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/__init.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/wassncplot.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    13861 2024-04-16 12:31:34.000000 wassncplot-2.5.1/src/wassncplot/wassncplot2.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/src/wassncplot.egg-info/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-23 07:32:30.276857 wassncplot-2.5.3/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-23 07:32:30.276857 wassncplot-2.5.3/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.5.3/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.5.3/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-23 07:32:30.276857 wassncplot-2.5.3/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-23 07:32:30.272857 wassncplot-2.5.3/src/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-23 07:32:30.272857 wassncplot-2.5.3/src/wassncplot/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-23 07:32:30.276857 wassncplot-2.5.3/src/wassncplot/WaveFieldVisualize/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.5.3/src/wassncplot/WaveFieldVisualize/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.5.3/src/wassncplot/WaveFieldVisualize/waveview2.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.5.3/src/wassncplot/__init.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.5.3/src/wassncplot/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.5.3/src/wassncplot/wassncplot.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    14215 2024-04-23 07:30:57.000000 wassncplot-2.5.3/src/wassncplot/wassncplot2.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-23 07:32:30.276857 wassncplot-2.5.3/src/wassncplot.egg-info/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-23 07:32:30.000000 wassncplot-2.5.3/src/wassncplot.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-23 07:32:30.000000 wassncplot-2.5.3/src/wassncplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-23 07:32:30.000000 wassncplot-2.5.3/src/wassncplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-23 07:32:30.000000 wassncplot-2.5.3/src/wassncplot.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-23 07:32:30.000000 wassncplot-2.5.3/src/wassncplot.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-23 07:32:30.000000 wassncplot-2.5.3/src/wassncplot.egg-info/top_level.txt
```

### Comparing `wassncplot-2.5.1/PKG-INFO` & `wassncplot-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.5.1
+Version: 2.5.3
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wassncplot-2.5.1/README.md` & `wassncplot-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5.1/pyproject.toml` & `wassncplot-2.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/waveview2.py` & `wassncplot-2.5.3/src/wassncplot/WaveFieldVisualize/waveview2.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5.1/src/wassncplot/wassncplot.py` & `wassncplot-2.5.3/src/wassncplot/wassncplot.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5.1/src/wassncplot/wassncplot2.py` & `wassncplot-2.5.3/src/wassncplot/wassncplot2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import argparse
 import glob
 import scipy.io
 from scipy.interpolate import LinearNDInterpolator, griddata
 
 
-VERSION="2.5.1"
+VERSION="2.5.3"
 
 
 
 def wassncplot_main():
 
     print(" wassncplot v.", VERSION )
     print("=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\nCopyright (C) Filippo Bergamasco 2024 \n")
@@ -185,34 +185,46 @@
 
     for image_idx in pbar:
 
         I0 = cv.imdecode( rootgrp["cam0images"][image_idx], cv.IMREAD_GRAYSCALE )
         if args.upscale2x:
             I0 = cv.pyrUp(I0)
 
-        if args.applymask:
-            I0mask = cv.imdecode( rootgrp["cam0masks"][image_idx], cv.IMREAD_GRAYSCALE )
-            I0mask = np.expand_dims(cv.resize( I0mask, (I0.shape[1],I0.shape[0]), interpolation=cv.INTER_NEAREST ), axis=-1 )
-        else:
-            I0mask = np.array([[[1]]],dtype=np.uint8)
 
         if waveview is None:
             waveview = WaveView( title="Wave field", width=I0.shape[1], height=I0.shape[0], wireframe=args.wireframe, pixel_scale=args.pxscale )
             waveview.setup_field( XX, YY, PPlane.T )
             waveview.set_zrange( -zrange/2.0, zrange/2, args.alpha )
 
         ZZ_data = np.squeeze( np.array( ZZ[data_idx,:,:] ) )/1000.0 - zmean
         if args.zeromean:
             ZZ_data -= M
         #mask = (ZZ_data == 0.0)
         #ZZ_dil = cv.dilate( ZZ_data, np.ones((3,3)))
         #ZZ_data[mask]=ZZ_dil
 
+
         img, img_xyz = waveview.render( I0, ZZ_data )
 
+
+        # OSX hack for high-dpi display
+        # This shoud be handled when creating the OpenGL window
+        # You may also want to set QT_SCALE_FACTOR=0.5 environment variable
+        if img.shape[0] != I0.shape[0] or img.shape[1] != I0.shape[1]:
+            I0 = cv.resize( I0, (img.shape[1], img.shape[0]) )
+        # end of OSX hack
+        
+
+        if args.applymask:
+            I0mask = cv.imdecode( rootgrp["cam0masks"][image_idx], cv.IMREAD_GRAYSCALE )
+            I0mask = np.expand_dims(cv.resize( I0mask, (I0.shape[1],I0.shape[0]), interpolation=cv.INTER_NEAREST ), axis=-1 )
+        else:
+            I0mask = np.array([[[1]]],dtype=np.uint8)
+
+
         #%%
         if args.createtx or args.savetx:
             interp = LinearNDInterpolator( np.reshape( img_xyz[:,:,0:2], [-1,2]), I0.flatten(), 0 )
             #interp = CloughTocher2DInterpolator( np.reshape( img_xyz[:,:,0:2], [-1,2]), I0.flatten(), 0 )
             tx = interp( XX, YY ).astype( np.uint8 )
 
             if args.createtx:
```

### Comparing `wassncplot-2.5.1/src/wassncplot.egg-info/PKG-INFO` & `wassncplot-2.5.3/src/wassncplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.5.1
+Version: 2.5.3
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

