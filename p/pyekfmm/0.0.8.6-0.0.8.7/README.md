# Comparing `tmp/pyekfmm-0.0.8.6.tar.gz` & `tmp/pyekfmm-0.0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyekfmm-0.0.8.6.tar", last modified: Wed Oct 11 17:48:05 2023, max compression
+gzip compressed data, was "pyekfmm-0.0.8.7.tar", last modified: Tue Apr 23 03:20:14 2024, max compression
```

## Comparing `pyekfmm-0.0.8.6.tar` & `pyekfmm-0.0.8.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-10-11 17:48:05.715173 pyekfmm-0.0.8.6/
--rw-r--r--   0 chenyk     (501) staff       (20)    35149 2023-08-01 16:20:53.000000 pyekfmm-0.0.8.6/LICENSE
--rw-r--r--   0 chenyk     (501) staff       (20)     1145 2023-10-11 17:48:05.714632 pyekfmm-0.0.8.6/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     5399 2023-08-01 16:20:53.000000 pyekfmm-0.0.8.6/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-10-11 17:48:05.706252 pyekfmm-0.0.8.6/pyekfmm/
--rw-r--r--   0 chenyk     (501) staff       (20)      628 2023-10-11 17:10:42.000000 pyekfmm-0.0.8.6/pyekfmm/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     3844 2023-08-01 16:20:53.000000 pyekfmm-0.0.8.6/pyekfmm/fmm.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4068 2023-08-01 16:20:53.000000 pyekfmm-0.0.8.6/pyekfmm/fmmvti.py
--rw-r--r--   0 chenyk     (501) staff       (20)     3941 2023-10-11 17:38:47.000000 pyekfmm-0.0.8.6/pyekfmm/plot.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-10-11 17:48:05.712570 pyekfmm-0.0.8.6/pyekfmm/src/
--rw-r--r--   0 chenyk     (501) staff       (20)    43292 2023-08-05 13:07:21.000000 pyekfmm-0.0.8.6/pyekfmm/src/eikonal.c
--rw-r--r--   0 chenyk     (501) staff       (20)    52781 2023-08-01 16:20:53.000000 pyekfmm-0.0.8.6/pyekfmm/src/eikonalvti.c
--rw-r--r--   0 chenyk     (501) staff       (20)     9787 2023-10-11 17:41:29.000000 pyekfmm-0.0.8.6/pyekfmm/stream.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-10-11 17:48:05.709855 pyekfmm-0.0.8.6/pyekfmm.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1145 2023-10-11 17:48:05.000000 pyekfmm-0.0.8.6/pyekfmm.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      344 2023-10-11 17:48:05.000000 pyekfmm-0.0.8.6/pyekfmm.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-10-11 17:48:05.000000 pyekfmm-0.0.8.6/pyekfmm.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-08-05 12:48:53.000000 pyekfmm-0.0.8.6/pyekfmm.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-10-11 17:48:05.000000 pyekfmm-0.0.8.6/pyekfmm.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       29 2023-10-11 17:48:05.000000 pyekfmm-0.0.8.6/pyekfmm.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-10-11 17:48:05.715260 pyekfmm-0.0.8.6/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     1924 2023-10-11 17:10:54.000000 pyekfmm-0.0.8.6/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2024-04-23 03:20:14.193646 pyekfmm-0.0.8.7/
+-rw-r--r--   0 chenyk     (501) staff       (20)    35149 2024-04-18 01:08:48.000000 pyekfmm-0.0.8.7/LICENSE
+-rw-r--r--   0 chenyk     (501) staff       (20)     1145 2024-04-23 03:20:14.193235 pyekfmm-0.0.8.7/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     6034 2024-04-18 01:44:29.000000 pyekfmm-0.0.8.7/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2024-04-23 03:20:14.187217 pyekfmm-0.0.8.7/pyekfmm/
+-rw-r--r--   0 chenyk     (501) staff       (20)      628 2024-04-18 01:08:48.000000 pyekfmm-0.0.8.7/pyekfmm/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     3844 2024-04-18 01:47:03.000000 pyekfmm-0.0.8.7/pyekfmm/fmm.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4068 2024-04-18 01:08:48.000000 pyekfmm-0.0.8.7/pyekfmm/fmmvti.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4116 2024-04-23 02:47:10.000000 pyekfmm-0.0.8.7/pyekfmm/plot.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2024-04-23 03:20:14.191918 pyekfmm-0.0.8.7/pyekfmm/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)    43328 2024-04-18 01:47:10.000000 pyekfmm-0.0.8.7/pyekfmm/src/eikonal.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    52817 2024-04-18 01:08:48.000000 pyekfmm-0.0.8.7/pyekfmm/src/eikonalvti.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     9787 2024-04-18 01:08:48.000000 pyekfmm-0.0.8.7/pyekfmm/stream.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2024-04-23 03:20:14.190212 pyekfmm-0.0.8.7/pyekfmm.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1145 2024-04-23 03:20:14.000000 pyekfmm-0.0.8.7/pyekfmm.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      344 2024-04-23 03:20:14.000000 pyekfmm-0.0.8.7/pyekfmm.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2024-04-23 03:20:14.000000 pyekfmm-0.0.8.7/pyekfmm.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2024-04-18 01:09:29.000000 pyekfmm-0.0.8.7/pyekfmm.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2024-04-23 03:20:14.000000 pyekfmm-0.0.8.7/pyekfmm.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       29 2024-04-23 03:20:14.000000 pyekfmm-0.0.8.7/pyekfmm.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2024-04-23 03:20:14.193754 pyekfmm-0.0.8.7/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     1924 2024-04-23 03:18:33.000000 pyekfmm-0.0.8.7/setup.py
```

### Comparing `pyekfmm-0.0.8.6/LICENSE` & `pyekfmm-0.0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.6/PKG-INFO` & `pyekfmm-0.0.8.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyekfmm
-Version: 0.0.8.6
+Version: 0.0.8.7
 Summary: Fast Marching Method for Traveltime Calculation
 Home-page: https://github.com/aaspip/pyekfmm
 Author: pyekfmm developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,exploration seismology,array seismology,traveltime,ray tracing,earthquake location,earthquake relocation,surface wave tomography,body wave tomography
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyekfmm-0.0.8.6/README.md` & `pyekfmm-0.0.8.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,20 @@
     pip install pyekfmm
 
 -----------
 ## Examples
     The "demo" directory contains all runable scripts to demonstrate different applications of pyekfmm. 
 
 -----------
+## Notebook tutorials
+Some notebook tutorials are stored separately to ensure the minimal size of the pyekfmm package. They can be found at 
+
+	https://github.com/aaspip/notebook/blob/main/pyekfmm
+
+-----------
 ## Dependence Packages
 * scipy 
 * numpy 
 * matplotlib
 
 -----------
 ## Development
@@ -102,10 +108,15 @@
 The following figure shows a surface-wave tomography test. (a) Ray path between a pair of virtual source (red star) and station (blue triangle). The background is the 5 sec group velocities of the Australian continent from ambient noise imaging. (b) Travel time field. (c) Ray paths of all 25,899 pairs. (d)-(f) The same as (a)-(c) but for the initial model with a constant velocity.
 <img src='https://github.com/aaspip/gallery/blob/main/pyekfmm/test_pyekfmm_fig8.png' alt='DEMO8' width=960/>
 
 DEMO9
 The following figure shows the traveltime misfit in the surface-wave tomography test. (a) Group velocities inverted from the travel time residuals using the kernel constructed from the initial model. (b) Travel time misfits estimated from the initial and final models.
 <img src='https://github.com/aaspip/gallery/blob/main/pyekfmm/test_pyekfmm_fig9.png' alt='DEMO9' width=960/>
 
+# Below are new examples in addition to the results in the original paper
+DEM10
+The following figure shows an example of traveltime calculation of two shots for 3D isotropic media
+ Generated by [demos/test_pyekfmm_fig2-multishots.py](https://github.com/aaspip/pyekfmm/blob/main/demos/test_pyekfmm_fig2.py)
+<img src='https://github.com/aaspip/gallery/blob/main/pyekfmm/test_pyekfmm_fig2-multishots.png' alt='DEMO2' width=960/>
```

### Comparing `pyekfmm-0.0.8.6/pyekfmm/__init__.py` & `pyekfmm-0.0.8.7/pyekfmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.6/pyekfmm/fmm.py` & `pyekfmm-0.0.8.7/pyekfmm/fmm.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.6/pyekfmm/fmmvti.py` & `pyekfmm-0.0.8.7/pyekfmm/fmmvti.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.6/pyekfmm/plot.py` & `pyekfmm-0.0.8.7/pyekfmm/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 (np.concatenate((0.5*np.ones([1,40]),np.expand_dims(np.linspace(0.5,1,88),axis=1).transpose(),np.expand_dims(np.linspace(1,0,88),axis=1).transpose(),np.zeros([1,40])),axis=1).transpose(),
 np.concatenate((0.25*np.ones([1,40]),np.expand_dims(np.linspace(0.25,1,88),axis=1).transpose(),np.expand_dims(np.linspace(1,0,88),axis=1).transpose(),np.zeros([1,40])),axis=1).transpose(),
 np.concatenate((np.zeros([1,40]),np.expand_dims(np.linspace(0,1,88),axis=1).transpose(),np.expand_dims(np.linspace(1,0,88),axis=1).transpose(),np.zeros([1,40])),axis=1).transpose()),axis=1)
 
 	return ListedColormap(seis)
 	
 
-def plot3d(d3d,frames=None,z=None,x=None,y=None,nlevel=100,figname=None,showf=True,close=True,**kwargs):
+def plot3d(d3d,frames=None,dz=0.01,dx=0.01,dy=0.01,z=None,x=None,y=None,nlevel=100,figname=None,showf=True,close=True,**kwargs):
 	'''
 	plot3d: plot beautiful 3D slices
 	
 	By Yangkang Chen
 	June, 18, 2023
 	
 	EXAMPLE 1
@@ -45,16 +45,27 @@
 	'''
 
 	[nz,nx,ny] = d3d.shape;
 	
 	if frames is None:
 		frames=[int(nz/2),int(nx/2),int(ny/2)]
 		
-	X, Y, Z = np.meshgrid(np.arange(nx)*0.01, np.arange(ny)*0.01, np.arange(nz)*0.01)
+	# X, Y, Z = np.meshgrid(np.arange(nx)*0.01, np.arange(ny)*0.01, np.arange(nz)*0.01)
 
+	if z is None:
+		z=np.arange(nz)*dz
+	
+	if x is None:
+		x=np.arange(nx)*dx
+		
+	if y is None:
+		y=np.arange(ny)*dy
+	
+	X, Y, Z = np.meshgrid(x, y, z)
+	
 	d3d=d3d.transpose([1,2,0])
 	
 	kw = {
     'vmin': d3d.min(),
     'vmax': d3d.max(),
     'levels': np.linspace(d3d.min(), d3d.max(), nlevel),
     'cmap':cseis()
```

### Comparing `pyekfmm-0.0.8.6/pyekfmm/src/eikonal.c` & `pyekfmm-0.0.8.7/pyekfmm/src/eikonal.c`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include <math.h>
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <numpy/arrayobject.h>
 
 #define FMM_HUGE 9999999999999999
+#define M_PI 3.14159265358979323846
 
 /*****pqueue for neighbor***/
 enum {FMM_IN, FMM_FRONT, FMM_OUT};
 
 static float **x, **xn, **x1;
 
 void pqueue_init (int n)
```

### Comparing `pyekfmm-0.0.8.6/pyekfmm/src/eikonalvti.c` & `pyekfmm-0.0.8.7/pyekfmm/src/eikonalvti.c`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include <math.h>
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <numpy/arrayobject.h>
 
 #define FMM_HUGE 9999999999999999
+#define M_PI 3.14159265358979323846
 
 /*****pqueue for neighbor***/
 enum {FMM_IN, FMM_FRONT, FMM_OUT};
 
 static float **xx, **xn, **x1;
 
 static float approx(float cos2, float sx, float sz, float q)
```

### Comparing `pyekfmm-0.0.8.6/pyekfmm/stream.py` & `pyekfmm-0.0.8.7/pyekfmm/stream.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.6/pyekfmm.egg-info/PKG-INFO` & `pyekfmm-0.0.8.7/pyekfmm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyekfmm
-Version: 0.0.8.6
+Version: 0.0.8.7
 Summary: Fast Marching Method for Traveltime Calculation
 Home-page: https://github.com/aaspip/pyekfmm
 Author: pyekfmm developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,exploration seismology,array seismology,traveltime,ray tracing,earthquake location,earthquake relocation,surface wave tomography,body wave tomography
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyekfmm-0.0.8.6/setup.py` & `pyekfmm-0.0.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 										include_dirs=[numpy.get_include()])
 
 eikonalvtic_module = Extension('eikonalvtic', sources=['pyekfmm/src/eikonalvti.c'], 
 										include_dirs=[numpy.get_include()])
 
 setup(
     name="pyekfmm",
-    version="0.0.8.6",
+    version="0.0.8.7",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="Fast Marching Method for Traveltime Calculation",
     long_description=long_description,
     author="pyekfmm developing team",
     author_email="chenyk2016@gmail.com",
     url="https://github.com/aaspip/pyekfmm",
     ext_modules=[eikonalc_module,eikonalvtic_module],
```

