# Comparing `tmp/opytimal-0.6.2.tar.gz` & `tmp/opytimal-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opytimal-0.6.2.tar", last modified: Tue Apr 23 13:18:14 2024, max compression
+gzip compressed data, was "opytimal-0.6.3.tar", last modified: Tue Apr 23 13:20:15 2024, max compression
```

## Comparing `opytimal-0.6.2.tar` & `opytimal-0.6.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:18:14.989715 opytimal-0.6.2/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     7048 2023-09-12 14:54:54.000000 opytimal-0.6.2/LICENSE
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 13:18:14.989715 opytimal-0.6.2/PKG-INFO
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      488 2023-11-17 15:48:02.000000 opytimal-0.6.2/README.md
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:18:14.989715 opytimal-0.6.2/opytimal/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2062 2024-04-23 13:18:11.000000 opytimal-0.6.2/opytimal/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      613 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/_vars.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    49923 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/analytical.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     9266 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/arrays.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    12180 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/decorator.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:18:14.989715 opytimal-0.6.2/opytimal/demos/
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      752 2023-11-17 17:30:06.000000 opytimal-0.6.2/opytimal/demos/__init__.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    29176 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optHeat1D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    26417 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optHeat2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    22362 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optPoisson1D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    24873 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optPoisson2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    23922 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optPoisson3D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    27362 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optStokes2D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    25154 2023-11-17 16:51:20.000000 opytimal-0.6.2/opytimal/demos/optStokes3D.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      841 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/dicts.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    63651 2023-11-17 13:15:29.000000 opytimal-0.6.2/opytimal/fenics.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1208 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/files.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      321 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/functions.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      105 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/mathFunctions.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    13269 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/meshes.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      798 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/modules.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      339 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/numeric.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      912 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/parallel.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    89570 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/plots.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     3695 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/profiler.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2090 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/settings.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)    21633 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/strings.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      447 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/symbols.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      344 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/tables.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1546 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/tests.py
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     2504 2023-11-17 11:54:51.000000 opytimal-0.6.2/opytimal/types.py
-drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:18:14.989715 opytimal-0.6.2/opytimal.egg-info/
--rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 13:18:14.000000 opytimal-0.6.2/opytimal.egg-info/PKG-INFO
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      862 2024-04-23 13:18:14.000000 opytimal-0.6.2/opytimal.egg-info/SOURCES.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)        1 2024-04-23 13:18:14.000000 opytimal-0.6.2/opytimal.egg-info/dependency_links.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)      276 2024-04-23 13:18:14.000000 opytimal-0.6.2/opytimal.egg-info/requires.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)        9 2024-04-23 13:18:14.000000 opytimal-0.6.2/opytimal.egg-info/top_level.txt
--rw-rw-r--   0 natanael  (1001) natanael  (1001)       38 2024-04-23 13:18:14.989715 opytimal-0.6.2/setup.cfg
--rw-rw-r--   0 natanael  (1001) natanael  (1001)     1383 2024-04-23 13:18:11.000000 opytimal-0.6.2/setup.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:20:15.218506 opytimal-0.6.3/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     7048 2023-09-12 14:54:54.000000 opytimal-0.6.3/LICENSE
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 13:20:15.218506 opytimal-0.6.3/PKG-INFO
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      488 2023-11-17 15:48:02.000000 opytimal-0.6.3/README.md
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:20:15.218506 opytimal-0.6.3/opytimal/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2062 2024-04-23 13:20:12.000000 opytimal-0.6.3/opytimal/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      613 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/_vars.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    49923 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/analytical.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     9266 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/arrays.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    12180 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/decorator.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:20:15.218506 opytimal-0.6.3/opytimal/demos/
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      752 2023-11-17 17:30:06.000000 opytimal-0.6.3/opytimal/demos/__init__.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    29176 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optHeat1D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    26417 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optHeat2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    22362 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optPoisson1D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    24873 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optPoisson2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    23922 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optPoisson3D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    27362 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optStokes2D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    25154 2023-11-17 16:51:20.000000 opytimal-0.6.3/opytimal/demos/optStokes3D.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      841 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/dicts.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    63651 2023-11-17 13:15:29.000000 opytimal-0.6.3/opytimal/fenics.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1208 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/files.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      321 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/functions.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      105 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/mathFunctions.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    13269 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/meshes.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      798 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/modules.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      339 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/numeric.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      912 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/parallel.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    89570 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/plots.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     3695 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/profiler.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2090 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/settings.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)    21633 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/strings.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      447 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/symbols.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      344 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/tables.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1546 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/tests.py
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     2504 2023-11-17 11:54:51.000000 opytimal-0.6.3/opytimal/types.py
+drwxrwxr-x   0 natanael  (1001) natanael  (1001)        0 2024-04-23 13:20:15.218506 opytimal-0.6.3/opytimal.egg-info/
+-rw-r--r--   0 natanael  (1001) natanael  (1001)     1080 2024-04-23 13:20:15.000000 opytimal-0.6.3/opytimal.egg-info/PKG-INFO
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      862 2024-04-23 13:20:15.000000 opytimal-0.6.3/opytimal.egg-info/SOURCES.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)        1 2024-04-23 13:20:15.000000 opytimal-0.6.3/opytimal.egg-info/dependency_links.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)      276 2024-04-23 13:20:15.000000 opytimal-0.6.3/opytimal.egg-info/requires.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)        9 2024-04-23 13:20:15.000000 opytimal-0.6.3/opytimal.egg-info/top_level.txt
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)       38 2024-04-23 13:20:15.218506 opytimal-0.6.3/setup.cfg
+-rw-rw-r--   0 natanael  (1001) natanael  (1001)     1383 2024-04-23 13:20:12.000000 opytimal-0.6.3/setup.py
```

### Comparing `opytimal-0.6.2/LICENSE` & `opytimal-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/PKG-INFO` & `opytimal-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opytimal
-Version: 0.6.2
+Version: 0.6.3
 Summary: Optimal control PDE-based solver
 Author: Natanael Quintino
 Author-email: natanael.quintino@ipiaget.pt
 License: CC0 1.0 Universal
 Keywords: optimalcontrol,FEniCS,FuildDynamics,NavierStokes,Stokes
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opytimal-0.6.2/opytimal/__init__.py` & `opytimal-0.6.3/opytimal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                      getDomainLabels, replaceBoundNameByMark,
                      getMeasure, evaluateErrors, Zero, getAdjointSystem,
                      getOptimalConditionsSystem, evaluateCost,
                      getLocal, setLocal, showProblemData,
                      getFunctionExpressions)
 
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 def __getattr__(attr):
     # Warn for expired attributes
     import warnings
 
     if attr == "demos":
         import opytimal.demos as demos
```

### Comparing `opytimal-0.6.2/opytimal/_vars.py` & `opytimal-0.6.3/opytimal/_vars.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/analytical.py` & `opytimal-0.6.3/opytimal/analytical.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/arrays.py` & `opytimal-0.6.3/opytimal/arrays.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/decorator.py` & `opytimal-0.6.3/opytimal/decorator.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/__init__.py` & `opytimal-0.6.3/opytimal/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optHeat1D.py` & `opytimal-0.6.3/opytimal/demos/optHeat1D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optHeat2D.py` & `opytimal-0.6.3/opytimal/demos/optHeat2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optPoisson1D.py` & `opytimal-0.6.3/opytimal/demos/optPoisson1D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optPoisson2D.py` & `opytimal-0.6.3/opytimal/demos/optPoisson2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optPoisson3D.py` & `opytimal-0.6.3/opytimal/demos/optPoisson3D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optStokes2D.py` & `opytimal-0.6.3/opytimal/demos/optStokes2D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/demos/optStokes3D.py` & `opytimal-0.6.3/opytimal/demos/optStokes3D.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/dicts.py` & `opytimal-0.6.3/opytimal/dicts.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/fenics.py` & `opytimal-0.6.3/opytimal/fenics.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/files.py` & `opytimal-0.6.3/opytimal/files.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/meshes.py` & `opytimal-0.6.3/opytimal/meshes.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/modules.py` & `opytimal-0.6.3/opytimal/modules.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/parallel.py` & `opytimal-0.6.3/opytimal/parallel.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/plots.py` & `opytimal-0.6.3/opytimal/plots.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/profiler.py` & `opytimal-0.6.3/opytimal/profiler.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/settings.py` & `opytimal-0.6.3/opytimal/settings.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/strings.py` & `opytimal-0.6.3/opytimal/strings.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/tests.py` & `opytimal-0.6.3/opytimal/tests.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal/types.py` & `opytimal-0.6.3/opytimal/types.py`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/opytimal.egg-info/PKG-INFO` & `opytimal-0.6.3/opytimal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opytimal
-Version: 0.6.2
+Version: 0.6.3
 Summary: Optimal control PDE-based solver
 Author: Natanael Quintino
 Author-email: natanael.quintino@ipiaget.pt
 License: CC0 1.0 Universal
 Keywords: optimalcontrol,FEniCS,FuildDynamics,NavierStokes,Stokes
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opytimal-0.6.2/opytimal.egg-info/SOURCES.txt` & `opytimal-0.6.3/opytimal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opytimal-0.6.2/setup.py` & `opytimal-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.6.2"
+VERSION = "0.6.3"
 DESCRIPTION = 'Optimal control PDE-based solver'
 LONG_DESCRIPTION = 'Opytimal is a Python/FEniCS framework that have the main goal solve Optimal Control problems considering multiple and mixed controls based to linear and nonlinear PDEs, in addition to can also solve PDEs simply and clearly'
 
 setup(
     name="opytimal",
     version=VERSION,
     description=DESCRIPTION,
```

