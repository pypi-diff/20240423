# Comparing `tmp/fisspy-1.0.4.tar.gz` & `tmp/fisspy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.4.tar", last modified: Mon Apr 22 08:35:24 2024, max compression
+gzip compressed data, was "fisspy-1.0.5.tar", last modified: Tue Apr 23 12:49:07 2024, max compression
```

## Comparing `fisspy-1.0.4.tar` & `fisspy-1.0.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.790470 fisspy-1.0.4/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.4/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      572 2024-04-22 08:35:24.790281 fisspy-1.0.4/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     2007 2024-04-22 06:20:20.000000 fisspy-1.0.4/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.778836 fisspy-1.0.4/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-22 08:34:31.000000 fisspy-1.0.4/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.780025 fisspy-1.0.4/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    14687 2024-04-22 08:27:59.000000 fisspy-1.0.4/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.782236 fisspy-1.0.4/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-21 06:20:03.000000 fisspy-1.0.4/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35503 2024-04-22 08:27:41.000000 fisspy-1.0.4/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.4/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.4/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.783671 fisspy-1.0.4/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.784653 fisspy-1.0.4/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.4/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.4/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.4/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.4/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.785337 fisspy-1.0.4/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/image/base.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.785732 fisspy-1.0.4/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.786185 fisspy-1.0.4/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.4/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.4/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.788344 fisspy-1.0.4/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.789892 fisspy-1.0.4/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    47723 2024-04-22 03:30:24.000000 fisspy-1.0.4/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.4/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 08:35:24.779667 fisspy-1.0.4/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      572 2024-04-22 08:35:24.000000 fisspy-1.0.4/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-22 08:35:24.000000 fisspy-1.0.4/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-22 08:35:24.000000 fisspy-1.0.4/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-22 08:35:24.000000 fisspy-1.0.4/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      135 2024-04-22 08:35:24.000000 fisspy-1.0.4/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-22 08:35:24.000000 fisspy-1.0.4/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-22 08:35:24.790512 fisspy-1.0.4/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      580 2024-04-22 08:34:30.000000 fisspy-1.0.4/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.569193 fisspy-1.0.5/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.5/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-23 12:49:07.569070 fisspy-1.0.5/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.5/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.557470 fisspy-1.0.5/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-23 12:45:48.000000 fisspy-1.0.5/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.559018 fisspy-1.0.5/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    14687 2024-04-22 08:27:59.000000 fisspy-1.0.5/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.561262 fisspy-1.0.5/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-21 06:20:03.000000 fisspy-1.0.5/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35503 2024-04-22 08:27:41.000000 fisspy-1.0.5/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.5/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.562753 fisspy-1.0.5/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.563762 fisspy-1.0.5/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.5/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.5/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.5/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.564868 fisspy-1.0.5/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.565299 fisspy-1.0.5/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.565782 fisspy-1.0.5/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.567543 fisspy-1.0.5/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.568734 fisspy-1.0.5/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    49070 2024-04-23 12:44:46.000000 fisspy-1.0.5/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.558377 fisspy-1.0.5/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      135 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-23 12:49:07.569234 fisspy-1.0.5/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      580 2024-04-23 12:45:46.000000 fisspy-1.0.5/setup.py
```

### Comparing `fisspy-1.0.4/LICENSE.txt` & `fisspy-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/README.md` & `fisspy-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,22 +20,19 @@
 Recommend to install the Python from the [Anaconda](https://www.continuum.io/why-anaconda).
 
 To install these packages, first set the conda-forge server:
 
     conda config --append channels conda-forge
     
 ### <span style="color: red">Option 1)</span> Using Mamba
-We recommend you use the mamba to install the FISSpy:
+We highly recommend you use the mamba to install the FISSpy:
 
     mamba install fisspy
 
-If you don't have mamba you can download the mamba using the conda:
-
-    conda install -n base conda-libmamba-solver
-    conda install mamba --solver=libmamba
+If you don't have mamba please see [mamba installation](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html)
 
 After installing the mamba you can download the FISSpy using the previous command.
 
 ### <span style="color: red">Option 2)</span> Using Conda
 Sometimes an old version of the conda has some errors and takes lots of time to download the FISSpy. If then we recommend you use the mamba instead See [Option 1](#option-1-using-mamba).
 
     conda install fisspy
```

### Comparing `fisspy-1.0.4/fisspy/align/alignment.py` & `fisspy-1.0.5/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/align/base.py` & `fisspy-1.0.5/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/analysis/doppler.py` & `fisspy-1.0.5/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/analysis/filter.py` & `fisspy-1.0.5/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/analysis/forecast.py` & `fisspy-1.0.5/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/analysis/ofe.py` & `fisspy-1.0.5/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/analysis/tdmap.py` & `fisspy-1.0.5/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/analysis/wavelet.py` & `fisspy-1.0.5/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/cm.py` & `fisspy-1.0.5/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/correction/correction.py` & `fisspy-1.0.5/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/correction/get_inform.py` & `fisspy-1.0.5/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/data/_sample.py` & `fisspy-1.0.5/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/data/download.py` & `fisspy-1.0.5/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/image/base.py` & `fisspy-1.0.5/fisspy/image/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/image/interactive_image.py` & `fisspy-1.0.5/fisspy/image/interactive_image.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/image/raster_set.py` & `fisspy-1.0.5/fisspy/image/raster_set.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/io/read.py` & `fisspy-1.0.5/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/makevideo.py` & `fisspy-1.0.5/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/preprocess/proc_base.py` & `fisspy-1.0.5/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/preprocess/proc_gui.py` & `fisspy-1.0.5/fisspy/preprocess/proc_gui.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/preprocess/t_y_sh.py` & `fisspy-1.0.5/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy/read/read_factory.py` & `fisspy-1.0.5/fisspy/read/read_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 from matplotlib import ticker
 from .. import cm
 from .readbase import getRaster, getHeader, readFrame
 from ..analysis import lambdameter
 from ..image import interactive_image as II
-from ..correction import LineName, wvCalib, smoothingProf
+from ..correction import LineName, wvCalib, smoothingProf, CorSLA
 from ..analysis import FourierFilter, Wavelet, makeTDmap
 
 __author__= "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
 __all__ = ["rawData", "FISS", "FD", "calibData", "AlignCube"]
 
 class rawData:
@@ -328,37 +328,14 @@
                               0, self.ny*self.yDelt]
         
         if smoothingMethod is None:
             self.smoothing = True
         if self.smoothing:
             self.smoothingProf(method=smoothingMethod, **kwargs)
 
-    def getRaster(self, wv, hw=0.05):
-        """
-        Make a raster image for a given wavelength with in width 2*hw
-
-        Parameters
-        ----------
-        wv : float
-            Referenced wavelength.
-        hw : float
-            A half-width of wavelength to be integrated
-            Default is 0.05
-
-        Example
-        -------
-        >>> from fisspy.read import FISS
-        >>> fiss = FISS(file)
-        >>> raster = fiss.getRaster(0.5)
-        """
-
-        self.wv = wv
-        return getRaster(self.data, self.wave, wv, self.wvDelt, hw=hw)
-
-
     def wvCalib(self, profile=None, method='photo'):
         """
         Wavelength calibration
 
         Parameters
         ---------
         profile: `~numpy.ndarray`
@@ -377,14 +354,50 @@
         """
         if profile is None:
             pf = self.refProfile
         else:
             pf = profile
         return wvCalib(pf, self.header, method=method)
 
+    def CorSLA(self, refProf=None, pure=None, eps=0.027, zeta=0.055):
+        """
+        Correction of spectral line(s) profile for stray linght and far wing red-blue asymmetry.
+
+        Parameters
+        ----------
+        refProf: `numpy.ndarray`, shape (N,), (optional)
+            (Spatially averaged) Reference line profile.
+            If None, make refProfile by spatially averaging the Data.
+            Default is None.
+        pure: `~numpy.ndarry`, (optional)
+            True if not blended.
+            Please see `~fisspy.correction.get_inform.Pure`
+        eps: `float`, (optional)
+            Fraction of spatial stray light.
+            The default is 0.027
+        zeta: `float`, (optional)
+            Fration of spectral stray light.
+            The default is 0.055
+
+        See Also
+        --------
+        Chae et al. (2013), https://ui.adsabs.harvard.edu/abs/2013SoPh..288....1C/abstract
+        CorStrayLight: correction for stray light.
+        CorAsymmetry: correction for far wing red-blue asymmetry.
+        """
+        if refProf is None:
+            ndim = self.data.ndim
+            axes = tuple([i for i in range(ndim-1)])
+            rp = self.data.mean(axes)
+        else:
+            rp = refProf
+
+        self.data = CorSLA(self.wave, self.data, rp, self.line, pure=pure, eps=eps, zeta=zeta)
+
+
     def smoothingProf(self, method='savgol', **kwargs):
         """
         Parameters
         ----------
         method: `str`, optional
             If 'savgol', apply the Savitzky-Golay noise filter in the wavelength axis.
             If 'gauss', apply the Gaussian noise filter in the wavelength axis.
@@ -392,14 +405,38 @@
 
         Other Parameters
         ----------------
         **kwargs : `~scipy.signal.savgol_filter` properties or `~scipy.ndimage.gaussian_filter1d` properties.
         """
         self.data = smoothingProf(self.data, method=method, **kwargs)
         self.smoothing = True
+    
+    def getRaster(self, wv, hw=0.05):
+        """
+        Make a raster image for a given wavelength with in width 2*hw
+
+        Parameters
+        ----------
+        wv : float
+            Referenced wavelength.
+        hw : float
+            A half-width of wavelength to be integrated
+            Default is 0.05
+
+        Example
+        -------
+        >>> from fisspy.read import FISS
+        >>> fiss = FISS(file)
+        >>> raster = fiss.getRaster(0.5)
+        """
+
+        self.wv = wv
+        return getRaster(self.data, self.wave, wv, self.wvDelt, hw=hw)
+
+
 
     def lambdameter(self, **kw):
         """
         Calculate the doppler shift by using lambda-meter (bisector) method.
 
         Parameters
         ----------
```

### Comparing `fisspy-1.0.4/fisspy/read/readbase.py` & `fisspy-1.0.5/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/fisspy.egg-info/SOURCES.txt` & `fisspy-1.0.5/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.4/setup.py` & `fisspy-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.4',
+    version='1.0.5',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

