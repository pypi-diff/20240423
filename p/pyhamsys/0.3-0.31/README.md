# Comparing `tmp/pyhamsys-0.3.tar.gz` & `tmp/pyhamsys-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhamsys-0.3.tar", last modified: Mon Apr 15 09:30:24 2024, max compression
+gzip compressed data, was "pyhamsys-0.31.tar", last modified: Tue Apr 23 07:44:00 2024, max compression
```

## Comparing `pyhamsys-0.3.tar` & `pyhamsys-0.31.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.474318 pyhamsys-0.3/
--rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.3/LICENSE
--rw-r--r--   0 cchandre   (501) staff       (20)    12226 2024-04-15 09:30:24.473925 pyhamsys-0.3/PKG-INFO
--rw-r--r--   0 cchandre   (501) staff       (20)    11413 2023-10-20 15:20:51.000000 pyhamsys-0.3/README.md
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.470272 pyhamsys-0.3/pyhamsys/
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.471831 pyhamsys-0.3/pyhamsys/src/
-drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-15 09:30:24.473439 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/
--rw-r--r--   0 cchandre   (501) staff       (20)    12226 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
--rw-r--r--   0 cchandre   (501) staff       (20)      275 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
--rw-r--r--   0 cchandre   (501) staff       (20)        1 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
--rw-r--r--   0 cchandre   (501) staff       (20)       12 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/requires.txt
--rw-r--r--   0 cchandre   (501) staff       (20)        9 2024-04-15 09:30:24.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/top_level.txt
--rw-r--r--   0 cchandre   (501) staff       (20)    22136 2023-10-24 14:15:51.000000 pyhamsys-0.3/pyhamsys/src/pyhamsys.py
--rw-r--r--   0 cchandre   (501) staff       (20)       38 2024-04-15 09:30:24.474421 pyhamsys-0.3/setup.cfg
--rw-r--r--   0 cchandre   (501) staff       (20)     1127 2024-04-15 09:29:02.000000 pyhamsys-0.3/setup.py
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-23 07:44:00.492952 pyhamsys-0.31/
+-rw-r--r--   0 cchandre   (501) staff       (20)     1304 2023-04-05 14:49:59.000000 pyhamsys-0.31/LICENSE
+-rw-r--r--   0 cchandre   (501) staff       (20)    12269 2024-04-23 07:44:00.492330 pyhamsys-0.31/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)    11413 2023-10-20 15:20:51.000000 pyhamsys-0.31/README.md
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-23 07:44:00.488335 pyhamsys-0.31/pyhamsys/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-23 07:44:00.489853 pyhamsys-0.31/pyhamsys/src/
+drwxr-xr-x   0 cchandre   (501) staff       (20)        0 2024-04-23 07:44:00.491862 pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/
+-rw-r--r--   0 cchandre   (501) staff       (20)    12269 2024-04-23 07:44:00.000000 pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/PKG-INFO
+-rw-r--r--   0 cchandre   (501) staff       (20)      275 2024-04-23 07:44:00.000000 pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/SOURCES.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        1 2024-04-23 07:44:00.000000 pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/dependency_links.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)       12 2024-04-23 07:44:00.000000 pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/requires.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)        9 2024-04-23 07:44:00.000000 pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/top_level.txt
+-rw-r--r--   0 cchandre   (501) staff       (20)    22148 2024-04-23 07:35:50.000000 pyhamsys-0.31/pyhamsys/src/pyhamsys.py
+-rw-r--r--   0 cchandre   (501) staff       (20)       38 2024-04-23 07:44:00.493046 pyhamsys-0.31/setup.cfg
+-rw-r--r--   0 cchandre   (501) staff       (20)     1128 2024-04-23 07:39:38.000000 pyhamsys-0.31/setup.py
```

### Comparing `pyhamsys-0.3/LICENSE` & `pyhamsys-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.3/PKG-INFO` & `pyhamsys-0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.3
+Version: 0.31
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
@@ -15,14 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # pyHamSys
 pyHamSys is a Python package for scientific computing involving Hamiltonian systems
 
 ![PyPI](https://img.shields.io/pypi/v/pyhamsys)
 ![License](https://img.shields.io/badge/license-BSD-lightgray)
```

### Comparing `pyhamsys-0.3/README.md` & `pyhamsys-0.31/README.md`

 * *Files identical despite different names*

### Comparing `pyhamsys-0.3/pyhamsys/src/pyhamsys.egg-info/PKG-INFO` & `pyhamsys-0.31/pyhamsys/src/pyhamsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhamsys
-Version: 0.3
+Version: 0.31
 Summary: Some tools for Hamiltonian systems
 Home-page: http://github.com/cchandre/pyhamsys
 Author: Cristel Chandre
 Author-email: cristel.chandre@cnrs.fr
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
@@ -15,14 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # pyHamSys
 pyHamSys is a Python package for scientific computing involving Hamiltonian systems
 
 ![PyPI](https://img.shields.io/pypi/v/pyhamsys)
 ![License](https://img.shields.io/badge/license-BSD-lightgray)
```

### Comparing `pyhamsys-0.3/pyhamsys/src/pyhamsys.py` & `pyhamsys-0.31/pyhamsys/src/pyhamsys.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 			t += h
 		return t, y
 
 	count = 0
 	t, y_ = t0, y0.copy()
 	while t < tf:
 		t, y_ = _integrate(t, y_)
-		if t_eval is not None and t > t_eval.max():
+		if t_eval is not None and t >= t_eval.max() + step / 2:
 			break
 		if t_eval is not None:
 			count += 1
 			if count % spacing == 0:
 				count = 0
 				t_vec.append(t)
 				y_vec = xp.concatenate((y_vec, y_[..., xp.newaxis]), axis=-1)
```

### Comparing `pyhamsys-0.3/setup.py` & `pyhamsys-0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhamsys',
-    version='0.3',
+    version='0.31',
     description='Some tools for Hamiltonian systems',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url='http://github.com/cchandre/pyhamsys',
     classifiers=[
       'Programming Language :: Python :: 3',
```

