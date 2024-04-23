# Comparing `tmp/intervalpylib-0.1.1.tar.gz` & `tmp/intervalpylib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intervalpylib-0.1.1.tar", last modified: Mon Apr 22 11:15:02 2024, max compression
+gzip compressed data, was "intervalpylib-0.1.2.tar", last modified: Tue Apr 23 07:25:33 2024, max compression
```

## Comparing `intervalpylib-0.1.1.tar` & `intervalpylib-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-22 11:15:02.229106 intervalpylib-0.1.1/
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)    11356 2024-04-20 09:02:52.000000 intervalpylib-0.1.1/LICENSE
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     2156 2024-04-22 11:15:02.229106 intervalpylib-0.1.1/PKG-INFO
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     1491 2024-04-20 11:37:19.000000 intervalpylib-0.1.1/README.md
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)      710 2024-04-22 11:14:09.000000 intervalpylib-0.1.1/pyproject.toml
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       65 2024-04-20 11:23:13.000000 intervalpylib-0.1.1/requirements.txt
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       38 2024-04-22 11:15:02.229106 intervalpylib-0.1.1/setup.cfg
-drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-22 11:15:02.229106 intervalpylib-0.1.1/src/
-drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-22 11:15:02.229106 intervalpylib-0.1.1/src/intervalpylib/
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)    14758 2024-04-22 11:13:50.000000 intervalpylib-0.1.1/src/intervalpylib/AreaCalculator.py
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     7446 2024-04-22 10:56:07.000000 intervalpylib-0.1.1/src/intervalpylib/Solvers.py
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     4064 2024-04-20 10:15:21.000000 intervalpylib-0.1.1/src/intervalpylib/SymbolicEquationSolver.py
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       90 2024-04-22 11:01:27.000000 intervalpylib-0.1.1/src/intervalpylib/__init__.py
-drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-22 11:15:02.229106 intervalpylib-0.1.1/src/intervalpylib.egg-info/
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     2156 2024-04-22 11:15:02.000000 intervalpylib-0.1.1/src/intervalpylib.egg-info/PKG-INFO
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)      392 2024-04-22 11:15:02.000000 intervalpylib-0.1.1/src/intervalpylib.egg-info/SOURCES.txt
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)        1 2024-04-22 11:15:02.000000 intervalpylib-0.1.1/src/intervalpylib.egg-info/dependency_links.txt
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       65 2024-04-22 11:15:02.000000 intervalpylib-0.1.1/src/intervalpylib.egg-info/requires.txt
--rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       14 2024-04-22 11:15:02.000000 intervalpylib-0.1.1/src/intervalpylib.egg-info/top_level.txt
+drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-23 07:25:33.046565 intervalpylib-0.1.2/
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)    11356 2024-04-20 09:02:52.000000 intervalpylib-0.1.2/LICENSE
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     2156 2024-04-23 07:25:33.046565 intervalpylib-0.1.2/PKG-INFO
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     1491 2024-04-20 11:37:19.000000 intervalpylib-0.1.2/README.md
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)      710 2024-04-23 07:25:27.000000 intervalpylib-0.1.2/pyproject.toml
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       65 2024-04-20 11:23:13.000000 intervalpylib-0.1.2/requirements.txt
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       38 2024-04-23 07:25:33.046565 intervalpylib-0.1.2/setup.cfg
+drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-23 07:25:33.046565 intervalpylib-0.1.2/src/
+drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-23 07:25:33.046565 intervalpylib-0.1.2/src/intervalpylib/
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)    14656 2024-04-23 07:24:31.000000 intervalpylib-0.1.2/src/intervalpylib/AreaCalculator.py
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     7446 2024-04-22 10:56:07.000000 intervalpylib-0.1.2/src/intervalpylib/Solvers.py
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     4064 2024-04-20 10:15:21.000000 intervalpylib-0.1.2/src/intervalpylib/SymbolicEquationSolver.py
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       90 2024-04-22 11:01:27.000000 intervalpylib-0.1.2/src/intervalpylib/__init__.py
+drwxr-xr-x   0 schuakrk  (1000) schuakrk  (1000)        0 2024-04-23 07:25:33.046565 intervalpylib-0.1.2/src/intervalpylib.egg-info/
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)     2156 2024-04-23 07:25:33.000000 intervalpylib-0.1.2/src/intervalpylib.egg-info/PKG-INFO
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)      392 2024-04-23 07:25:33.000000 intervalpylib-0.1.2/src/intervalpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)        1 2024-04-23 07:25:33.000000 intervalpylib-0.1.2/src/intervalpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       65 2024-04-23 07:25:33.000000 intervalpylib-0.1.2/src/intervalpylib.egg-info/requires.txt
+-rw-r--r--   0 schuakrk  (1000) schuakrk  (1000)       14 2024-04-23 07:25:33.000000 intervalpylib-0.1.2/src/intervalpylib.egg-info/top_level.txt
```

### Comparing `intervalpylib-0.1.1/LICENSE` & `intervalpylib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intervalpylib-0.1.1/PKG-INFO` & `intervalpylib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intervalpylib
-Version: 0.1.1
+Version: 0.1.2
 Summary: An interval solver for robots' workspace area
 Author-email: Schukark <schukark2004@gmail.com>
 Project-URL: Homepage, https://github.com/schukark/intervalpylib
 Project-URL: Issues, https://github.com/schukark/intervalpylib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `intervalpylib-0.1.1/README.md` & `intervalpylib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `intervalpylib-0.1.1/pyproject.toml` & `intervalpylib-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "intervalpylib"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Schukark", email = "schukark2004@gmail.com" }]
 description = "An interval solver for robots' workspace area"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `intervalpylib-0.1.1/src/intervalpylib/AreaCalculator.py` & `intervalpylib-0.1.2/src/intervalpylib/AreaCalculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import matplotlib.lines as mlines
 from matplotlib.patches import Rectangle
 from typing import Dict, List
 
 class AreaCalculator:   
     """
     Class that allows to visualize the solution if the dimensionality is less than 3
+    
     Precalculated areas for 2-RPR and 3-RPR robots are also included in the class
     """ 
     def __init__(self, name, pa_params=None):
         """Constructor
 
         Args:
             name (string): The name of the robot configuration
@@ -23,20 +24,14 @@
             NotImplementedError: if the configuration is not supported
         """
         if name is not None and name not in ["2-RPR", "3-RPR"]:
             raise NotImplementedError
         self.name = name
         self.pa_params = pa_params
     
-    """
-            Make list of boxes in dim dimension from vector grid
-            :param grid: vector on which grid is constructed
-            :param dim:  the dimensional of grid
-            :return: the list of boxes in dim
-            """
     def make_boxes_list(grid: List[float], dim: int, uniform=True) -> List[tuple]:
         """Makes the grid boxes for the solver and the drawer
 
         Args:
             grid (np.array or list): the 1d-grid that will be used for each axis
             dim (int): the number of dimensions of the grid
             uniform (bool, optional): Defines the grid to be uniform on each axis. Defaults to True.
@@ -62,25 +57,27 @@
                 grid_size = len(one_grid) - 1
                 for j in range(grid_size):
                     grid_intervals.append(ival.Interval([one_grid[j], one_grid[j + 1]]))
                 grid_variants.append(grid_intervals)
             grid_n_size = list(it.product(*grid_variants))
         return grid_n_size
     
-    def __plot_area_3RPR(self, ax: plt.axes, x_c: List[float], y_c: List[float]):
+    def __plot_area_3RPR(self, ax: plt.axes, x_c: List[float], y_c: List[float], r_0: float, r_1: float):
         """private function to plot the workspace area of the 3-RPR robot
 
         Args:
             ax (plt.ax): the axes where to plot the area
             x_c (List): the x-coordinates of the 3 circles' centers
             y_c (List): the y-coordinates of the 3 circles' centers
+            r_0 (float): the radius of the inner circle
+            r_1 (float): the radius of the outer circle
         """
         for i in range(3):
-            circle = plt.Circle((x_c[i], y_c[i]), radius=12, fc='y', fill=False)
-            circle1 = plt.Circle((x_c[i], y_c[i]), radius=27, fc='y', fill=False)
+            circle = plt.Circle((x_c[i], y_c[i]), radius=r_0, fc='y', fill=False)
+            circle1 = plt.Circle((x_c[i], y_c[i]), radius=r_1, fc='y', fill=False)
             ax.add_patch(circle)
             ax.add_patch(circle1)
         ax.grid()
 
     def __plot_area_2RPR(self, ax: plt.axes, r1: float=3, r2: float =15, d: float=8):
         """private function to plot the workspace are of the 2-RPR robot
```

### Comparing `intervalpylib-0.1.1/src/intervalpylib/Solvers.py` & `intervalpylib-0.1.2/src/intervalpylib/Solvers.py`

 * *Files identical despite different names*

### Comparing `intervalpylib-0.1.1/src/intervalpylib/SymbolicEquationSolver.py` & `intervalpylib-0.1.2/src/intervalpylib/SymbolicEquationSolver.py`

 * *Files identical despite different names*

### Comparing `intervalpylib-0.1.1/src/intervalpylib.egg-info/PKG-INFO` & `intervalpylib-0.1.2/src/intervalpylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intervalpylib
-Version: 0.1.1
+Version: 0.1.2
 Summary: An interval solver for robots' workspace area
 Author-email: Schukark <schukark2004@gmail.com>
 Project-URL: Homepage, https://github.com/schukark/intervalpylib
 Project-URL: Issues, https://github.com/schukark/intervalpylib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

