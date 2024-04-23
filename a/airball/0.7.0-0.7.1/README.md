# Comparing `tmp/airball-0.7.0.tar.gz` & `tmp/airball-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airball-0.7.0.tar", last modified: Wed Apr 17 19:46:05 2024, max compression
+gzip compressed data, was "airball-0.7.1.tar", last modified: Tue Apr 23 17:50:23 2024, max compression
```

## Comparing `airball-0.7.0.tar` & `airball-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.216738 airball-0.7.0/
--rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.7.0/LICENSE
--rw-r--r--   0 zyrxvo     (501) staff       (20)     3261 2024-04-17 19:46:05.216559 airball-0.7.0/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)     2592 2023-10-11 05:11:21.000000 airball-0.7.0/README.md
--rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2023-12-11 15:38:51.000000 airball-0.7.0/pyproject.toml
--rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2024-04-17 19:46:05.216774 airball-0.7.0/setup.cfg
--rw-r--r--   0 zyrxvo     (501) staff       (20)      930 2024-04-17 19:44:38.000000 airball-0.7.0/setup.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.213464 airball-0.7.0/src/
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.215619 airball-0.7.0/src/airball/
--rw-r--r--   0 zyrxvo     (501) staff       (20)      639 2024-04-17 19:44:56.000000 airball-0.7.0/src/airball/__init__.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    31576 2024-04-11 20:48:41.000000 airball-0.7.0/src/airball/analytic.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    43194 2024-04-17 18:42:00.000000 airball-0.7.0/src/airball/core.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    29017 2024-03-07 15:29:46.000000 airball-0.7.0/src/airball/environments.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    16366 2024-04-12 21:11:30.000000 airball-0.7.0/src/airball/imf.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    42685 2024-02-02 19:59:31.000000 airball-0.7.0/src/airball/stars.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    32730 2024-04-17 18:41:31.000000 airball-0.7.0/src/airball/tools.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     7407 2023-12-17 07:19:28.000000 airball-0.7.0/src/airball/units.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.216366 airball-0.7.0/src/airball.egg-info/
--rw-r--r--   0 zyrxvo     (501) staff       (20)     3261 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      393 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/SOURCES.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/dependency_links.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)       42 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/requires.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:50:23.646426 airball-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 17:50:00.000000 airball-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-23 17:50:23.646426 airball-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-23 17:50:00.000000 airball-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 17:50:00.000000 airball-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:50:23.646426 airball-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-23 17:50:00.000000 airball-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:50:23.642426 airball-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:50:23.646426 airball-0.7.1/src/airball/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31576 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43194 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29017 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16366 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/imf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42700 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/stars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32641 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-23 17:50:00.000000 airball-0.7.1/src/airball/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:50:23.646426 airball-0.7.1/src/airball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-23 17:50:23.000000 airball-0.7.1/src/airball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 17:50:23.000000 airball-0.7.1/src/airball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:50:23.000000 airball-0.7.1/src/airball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 17:50:23.000000 airball-0.7.1/src/airball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 17:50:23.000000 airball-0.7.1/src/airball.egg-info/top_level.txt
```

### Comparing `airball-0.7.0/LICENSE` & `airball-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/PKG-INFO` & `airball-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package for running and managing flybys using REBOUND
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `airball-0.7.0/README.md` & `airball-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/setup.py` & `airball-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airball",
-    version="0.7.0",
+    version="0.7.1",
     author="Garett Brown",
     author_email="garett.brown@mail.utoronto.ca",
     description="A package for running and managing flybys using REBOUND",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zyrxvo/airball/",
     project_urls={
```

### Comparing `airball-0.7.0/src/airball/__init__.py` & `airball-0.7.1/src/airball/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from .core import (add_star_to_sim, flyby, flybys, hybrid_flyby, hybrid_flybys, successive_flybys, concurrent_flybys)
 from .environments import (StellarEnvironment, LocalNeighborhood, OpenCluster, GlobularCluster, GalacticBulge, GalacticCore)
 from .analytic import (relative_energy_change, energy_change_adiabatic_estimate, eccentricity_change_adiabatic_estimate, inclination_change_adiabatic_estimate)
 from .imf import (IMF)
 from .stars import (Star, Stars)
 from .units import (UnitSet)
 
-__version__ = 'v0.7.0'
+__version__ = 'v0.7.1'
```

### Comparing `airball-0.7.0/src/airball/analytic.py` & `airball-0.7.1/src/airball/analytic.py`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/src/airball/core.py` & `airball-0.7.1/src/airball/core.py`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/src/airball/environments.py` & `airball-0.7.1/src/airball/environments.py`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/src/airball/imf.py` & `airball-0.7.1/src/airball/imf.py`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/src/airball/stars.py` & `airball-0.7.1/src/airball/stars.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,15 @@
       ```
     """
     if not isinstance(filename, str): raise ValueError('Filename must be a string.')
     with open(filename, 'wb') as pfile:
       _pickle.dump(self, pfile, protocol=_pickle.HIGHEST_PROTOCOL)
 
   @classmethod
-  def _load(cls, filename, init=False):
+  def _load(cls, filename):
     """
     Load an instance of the Stars class from a file using pickle.
 
     Args:
       filename (str): The name of the file to load the instance from. The file should be in binary format, pickled.
 
     Returns:
@@ -862,15 +862,16 @@
     Example:
       ```python
       import airball
       stars = airball.Stars('open_cluster.stars')
       ```
     """
     if not isinstance(filename, str): raise ValueError('Filename must be a string.')
-    return _pickle.load(open(filename, 'rb'))
+    with open(filename, 'rb') as pfile:
+      return _pickle.load(pfile)
 
   def stats(self, returned=False):
     '''
     Prints a summary of the current stats of the Stars object.
     The stats are returned as a string if `returned=True`.
     '''
     s = f"<{self.__module__}.{type(self).__name__} object at {hex(id(self))}, "
```

### Comparing `airball-0.7.0/src/airball/tools.py` & `airball-0.7.1/src/airball/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import numpy as _np
 import rebound as _rebound
 import joblib as _joblib
 import warnings as _warnings
 from .units import UnitSet as _UnitSet
 from . import units as _u
-from mpmath import mp as _mp
-
-# Set the precision
-_mp.dps = 50  # 50 digits of precision
 
 twopi = 2.*_np.pi
 
 ############################################################
 ################### Helper Functions #######################
 ############################################################
```

### Comparing `airball-0.7.0/src/airball/units.py` & `airball-0.7.1/src/airball/units.py`

 * *Files identical despite different names*

### Comparing `airball-0.7.0/src/airball.egg-info/PKG-INFO` & `airball-0.7.1/src/airball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package for running and managing flybys using REBOUND
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

