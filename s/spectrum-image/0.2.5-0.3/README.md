# Comparing `tmp/spectrum_image-0.2.5.tar.gz` & `tmp/spectrum_image-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.2.5.tar", last modified: Wed Apr 10 01:20:33 2024, max compression
+gzip compressed data, was "spectrum_image-0.3.tar", last modified: Mon Apr 22 04:10:59 2024, max compression
```

## Comparing `spectrum_image-0.2.5.tar` & `spectrum_image-0.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.590579 spectrum_image-0.2.5/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.5/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1726 2024-04-10 01:20:33.590388 spectrum_image-0.2.5/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.2.5/README.md
--rw-r--r--   0 sung       (501) staff       (20)      863 2024-04-10 01:20:19.000000 spectrum_image-0.2.5/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-10 01:20:33.590622 spectrum_image-0.2.5/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.587623 spectrum_image-0.2.5/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.589444 spectrum_image-0.2.5/src/spectrum_image/
--rw-r--r--   0 sung       (501) staff       (20)    51688 2024-04-10 01:11:02.000000 spectrum_image-0.2.5/src/spectrum_image/EELS.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.5/src/spectrum_image/EELS_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)    12298 2024-04-10 01:08:18.000000 spectrum_image-0.2.5/src/spectrum_image/EELS_util.py
--rw-r--r--   0 sung       (501) staff       (20)    28413 2024-04-04 21:13:52.000000 spectrum_image-0.2.5/src/spectrum_image/RIXS.py
--rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.5/src/spectrum_image/SI_bckup.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.5/src/spectrum_image/__init__.py
--rw-r--r--   0 sung       (501) staff       (20)    13294 2024-04-07 21:36:17.000000 spectrum_image-0.2.5/src/spectrum_image/eels_bgsub.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-10 01:20:33.590197 spectrum_image-0.2.5/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1726 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      460 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-10 01:20:33.000000 spectrum_image-0.2.5/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 04:10:59.773310 spectrum_image-0.3/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.3/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1798 2024-04-22 04:10:59.773122 spectrum_image-0.3/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.3/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      979 2024-04-22 04:09:14.000000 spectrum_image-0.3/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-22 04:10:59.773347 spectrum_image-0.3/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 04:10:59.768499 spectrum_image-0.3/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 04:10:59.769616 spectrum_image-0.3/src/spectrum_image/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 04:10:59.772639 spectrum_image-0.3/src/spectrum_image/EELS/
+-rw-r--r--   0 sung       (501) staff       (20)    24186 2024-04-22 03:59:53.000000 spectrum_image-0.3/src/spectrum_image/EELS/EELS_LP.py
+-rw-r--r--   0 sung       (501) staff       (20)    23464 2024-04-22 04:04:52.000000 spectrum_image-0.3/src/spectrum_image/EELS/EELS_SI.py
+-rw-r--r--   0 sung       (501) staff       (20)    13359 2024-04-22 03:35:02.000000 spectrum_image-0.3/src/spectrum_image/EELS/EELS_bgsub.py
+-rw-r--r--   0 sung       (501) staff       (20)      764 2024-04-22 02:26:56.000000 spectrum_image-0.3/src/spectrum_image/EELS/EELS_edge.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.3/src/spectrum_image/EELS/EELS_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)    12303 2024-04-22 02:15:06.000000 spectrum_image-0.3/src/spectrum_image/EELS/EELS_util.py
+-rw-r--r--   0 sung       (501) staff       (20)      582 2024-04-22 04:00:49.000000 spectrum_image-0.3/src/spectrum_image/EELS/__init__.py
+-rw-r--r--   0 sung       (501) staff       (20)    28413 2024-04-04 21:13:52.000000 spectrum_image-0.3/src/spectrum_image/RIXS.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.3/src/spectrum_image/__init__.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-22 04:10:59.772897 spectrum_image-0.3/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1798 2024-04-22 04:10:59.000000 spectrum_image-0.3/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      560 2024-04-22 04:10:59.000000 spectrum_image-0.3/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-22 04:10:59.000000 spectrum_image-0.3/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-22 04:10:59.000000 spectrum_image-0.3/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-22 04:10:59.000000 spectrum_image-0.3/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.2.5/LICENSE` & `spectrum_image-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.5/PKG-INFO` & `spectrum_image-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.5
+Version: 0.3
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
-Author-email: Suk Hyun Sung <sukhsung@umich.edu>
+Author-email: Suk Hyun Sung <sukhsung@umich.edu>, Michale Colletta <mrc297@cornell.edu>, Alex Stangle <astangel@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
 Project-URL: Repository, https://github.com/sukhsung/spectrum-image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
```

### Comparing `spectrum_image-0.2.5/README.md` & `spectrum_image-0.3/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.5/pyproject.toml` & `spectrum_image-0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.2.5"
+version = "0.3"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
   "lmfit"
 ]
 requires-python = ">=3.10"
 authors = [
-  {name = "Suk Hyun Sung", email = "sukhsung@umich.edu"}
+  {name = "Suk Hyun Sung", email = "sukhsung@umich.edu"},
+  {name = "Michale Colletta", email = "mrc297@cornell.edu"},
+  {name = "Alex Stangle", email = "astangel@umich.edu"}
 ]
 description = "Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 keywords = ["Electron Microscopy", "EELS", "TEM", "STEM", "Electron Energy Loss Spectroscopy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `spectrum_image-0.2.5/src/spectrum_image/EELS_lineshapes.py` & `spectrum_image-0.3/src/spectrum_image/EELS/EELS_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.5/src/spectrum_image/EELS_util.py` & `spectrum_image-0.3/src/spectrum_image/EELS/EELS_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.optimize import curve_fit
 from scipy.ndimage import affine_transform
 from tqdm import tqdm, tqdm_notebook
-import spectrum_image.EELS_lineshapes as ls
+import spectrum_image.EELS.EELS_lineshapes as ls
 
 from sklearn.decomposition import PCA
 from tqdm import tqdm, tqdm_notebook
 import hyperspy.api as hs
 
 
 def remove_outlier( si, threshold_multiplier=5, remove_nn=True):
```

### Comparing `spectrum_image-0.2.5/src/spectrum_image/RIXS.py` & `spectrum_image-0.3/src/spectrum_image/RIXS.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.5/src/spectrum_image/eels_bgsub.py` & `spectrum_image-0.3/src/spectrum_image/EELS/EELS_bgsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import copy
 from tqdm import tqdm, tqdm_notebook
 import numpy.linalg as LA
 from scipy.ndimage import gaussian_filter
 from scipy.stats import norm
-import spectrum_image.SI_lineshapes as ls
+import spectrum_image.EELS.EELS_lineshapes as ls
 from scipy.optimize import curve_fit
 
 
 class options_bgsub:
 
     def __init__(self, fit='pl', log='False', lc=False, perc=(5,95), lba=False, gfwhm=None,
                        maxfev=50000, method='trf', ftol=0.0005, gtol=0.00005, xtol=None):
@@ -127,14 +127,15 @@
     if mask is None and threshold is not None:
         mean_back = np.mean(si[:,:,fit_start_ch:fit_end_ch],axis=2)
         mask = mean_back > threshold
     elif mask is None and threshold is None:
         mask = np.ones((xdim,ydim), dtype='bool')
     
     maskline = np.reshape( mask,(xdim*ydim))
+    fit_params = np.reshape( fit_params, (2, xdim, ydim))
     rline_long = -1*np.reshape( fit_params[1,:,:], (xdim*ydim) )
     rline = rline_long[maskline]
 
     ## Given r values of SI, refit background using a linear combination of power laws, 
     ## using either 5/95 percentile or 20/80 percentile r values.
     if fit_options.lc:
         bg_lcpl_SI = bgsub_SI_LC(fit_data, energy, edge, rline, fit_options)
```

### Comparing `spectrum_image-0.2.5/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.3/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.5
+Version: 0.3
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
-Author-email: Suk Hyun Sung <sukhsung@umich.edu>
+Author-email: Suk Hyun Sung <sukhsung@umich.edu>, Michale Colletta <mrc297@cornell.edu>, Alex Stangle <astangel@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
 Project-URL: Repository, https://github.com/sukhsung/spectrum-image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
```

