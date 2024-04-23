# Comparing `tmp/RIIGID-1.0.3.tar.gz` & `tmp/RIIGID-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RIIGID-1.0.3.tar", last modified: Thu Feb  8 13:22:17 2024, max compression
+gzip compressed data, was "RIIGID-1.0.4.tar", last modified: Tue Apr 23 08:06:01 2024, max compression
```

## Comparing `RIIGID-1.0.3.tar` & `RIIGID-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-02-08 13:22:17.759677 RIIGID-1.0.3/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1065 2024-01-11 12:46:47.000000 RIIGID-1.0.3/LICENSE.md
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2023-12-21 09:34:18.000000 RIIGID-1.0.3/MANIFEST.in
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-02-08 13:22:17.759677 RIIGID-1.0.3/PKG-INFO
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3521 2024-02-08 12:37:57.000000 RIIGID-1.0.3/README.rst
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-02-08 13:22:17.755677 RIIGID-1.0.3/RIIGID.egg-info/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-02-08 13:22:17.000000 RIIGID-1.0.3/RIIGID.egg-info/PKG-INFO
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      610 2024-02-08 13:22:17.000000 RIIGID-1.0.3/RIIGID.egg-info/SOURCES.txt
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        1 2024-02-08 13:22:17.000000 RIIGID-1.0.3/RIIGID.egg-info/dependency_links.txt
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       29 2024-02-08 13:22:17.000000 RIIGID-1.0.3/RIIGID.egg-info/requires.txt
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        7 2024-02-08 13:22:17.000000 RIIGID-1.0.3/RIIGID.egg-info/top_level.txt
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-02-08 13:22:17.755677 RIIGID-1.0.3/riigid/
--rw-r--r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      504 2024-01-17 09:04:14.000000 RIIGID-1.0.3/riigid/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      182 2024-02-08 12:37:57.000000 RIIGID-1.0.3/riigid/config.json
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-02-08 13:22:17.755677 RIIGID-1.0.3/riigid/convergence/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      118 2024-01-16 15:58:55.000000 RIIGID-1.0.3/riigid/convergence/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3775 2024-01-16 16:14:49.000000 RIIGID-1.0.3/riigid/convergence/criterion.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2401 2024-01-16 16:14:49.000000 RIIGID-1.0.3/riigid/convergence/displacement.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    18463 2024-01-24 15:31:45.000000 RIIGID-1.0.3/riigid/fragment.py
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-02-08 13:22:17.755677 RIIGID-1.0.3/riigid/library/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-01-11 08:41:35.000000 RIIGID-1.0.3/riigid/library/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     5818 2024-02-08 12:37:57.000000 RIIGID-1.0.3/riigid/library/misc.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     6801 2024-01-16 16:14:49.000000 RIIGID-1.0.3/riigid/library/rotation.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1869 2024-01-16 16:14:49.000000 RIIGID-1.0.3/riigid/optimization_step.py
-drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-02-08 13:22:17.759677 RIIGID-1.0.3/riigid/optimizer/
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13952 2024-02-08 12:37:57.000000 RIIGID-1.0.3/riigid/optimizer/Deprecated_GDWAS.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    15695 2024-02-08 12:37:57.000000 RIIGID-1.0.3/riigid/optimizer/GDWAS.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      153 2024-01-25 08:48:31.000000 RIIGID-1.0.3/riigid/optimizer/__init__.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2457 2024-02-08 12:37:57.000000 RIIGID-1.0.3/riigid/optimizer/optimizer.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13104 2024-02-08 12:37:57.000000 RIIGID-1.0.3/riigid/riigid.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    18395 2024-01-25 08:32:41.000000 RIIGID-1.0.3/riigid/structure.py
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       38 2024-02-08 13:22:17.759677 RIIGID-1.0.3/setup.cfg
--rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      544 2024-02-08 12:39:57.000000 RIIGID-1.0.3/setup.py
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1065 2024-01-11 12:46:47.000000 RIIGID-1.0.4/LICENSE.md
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2023-12-21 09:34:18.000000 RIIGID-1.0.4/MANIFEST.in
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-04-23 08:06:01.324062 RIIGID-1.0.4/PKG-INFO
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3521 2024-02-08 12:37:57.000000 RIIGID-1.0.4/README.rst
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.320062 RIIGID-1.0.4/RIIGID.egg-info/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      345 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/PKG-INFO
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      610 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/SOURCES.txt
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        1 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/dependency_links.txt
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       29 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/requires.txt
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        7 2024-04-23 08:06:01.000000 RIIGID-1.0.4/RIIGID.egg-info/top_level.txt
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/
+-rw-r--r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      504 2024-01-17 09:04:14.000000 RIIGID-1.0.4/riigid/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      242 2024-04-19 13:07:04.000000 RIIGID-1.0.4/riigid/config.json
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/convergence/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      118 2024-01-16 15:58:55.000000 RIIGID-1.0.4/riigid/convergence/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     3775 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/convergence/criterion.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2401 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/convergence/displacement.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    18860 2024-04-19 11:27:53.000000 RIIGID-1.0.4/riigid/fragment.py
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/library/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-01-11 08:41:35.000000 RIIGID-1.0.4/riigid/library/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     5818 2024-02-08 12:37:57.000000 RIIGID-1.0.4/riigid/library/misc.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     6801 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/library/rotation.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     1869 2024-01-16 16:14:49.000000 RIIGID-1.0.4/riigid/optimization_step.py
+drwxrwxr-x   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)        0 2024-04-23 08:06:01.324062 RIIGID-1.0.4/riigid/optimizer/
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13952 2024-02-08 12:37:57.000000 RIIGID-1.0.4/riigid/optimizer/Deprecated_GDWAS.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    15707 2024-04-19 11:05:43.000000 RIIGID-1.0.4/riigid/optimizer/GDWAS.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      153 2024-01-25 08:48:31.000000 RIIGID-1.0.4/riigid/optimizer/__init__.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)     2457 2024-02-08 12:37:57.000000 RIIGID-1.0.4/riigid/optimizer/optimizer.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    13522 2024-04-19 13:12:28.000000 RIIGID-1.0.4/riigid/riigid.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)    19025 2024-04-19 13:27:18.000000 RIIGID-1.0.4/riigid/structure.py
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)       38 2024-04-23 08:06:01.324062 RIIGID-1.0.4/setup.cfg
+-rw-rw-r--   0 siegfried_kaidisch  (1000) siegfried_kaidisch  (1000)      544 2024-04-23 08:02:07.000000 RIIGID-1.0.4/setup.py
```

### Comparing `RIIGID-1.0.3/LICENSE.md` & `RIIGID-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/README.rst` & `RIIGID-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/RIIGID.egg-info/SOURCES.txt` & `RIIGID-1.0.4/RIIGID.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/convergence/criterion.py` & `RIIGID-1.0.4/riigid/convergence/criterion.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/convergence/displacement.py` & `RIIGID-1.0.4/riigid/convergence/displacement.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/fragment.py` & `RIIGID-1.0.4/riigid/fragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     The orientation of a fragment can be defined using Euler angles and its position can be defined
     by its center of mass.
 
     Attributes
     ----------
     atoms: ase.atoms.Atoms
         The atoms forming the fragment.
+    indices_in_structure: list of int
+        Indices of the Fragment's atoms, relative to the Structure, that the Fragment is
+        a part of.
     allowed_translation: str
         How shall the fragment be allowed to translate?
         See docstring of __init__ for more details.
     allowed_rotation: str
         Allows the user to set constraints on the rotation axis of a fragment.
         See docstring of __init__ for more details.
     body_fixed_axis_x/y/z: numpy.ndarray of shape (3,)
@@ -36,21 +39,26 @@
     euler_angles: list of length 3
         The Euler angles of the fragment (alpha, beta, gamma); [°]
     inertia_matrix/_inv: numpy.ndarray of shape (3,3)
             The (inverse) inertia matrix of the fragment; [(Da*Å**2)]; (inverse:[1/(Da*Å**2)])
 
     """
 
-    def __init__(self, atoms: Atoms, allowed_translation, allowed_rotation):
+    def __init__(
+        self, atoms: Atoms, indices_in_structure, allowed_translation, allowed_rotation
+    ):
         """Define a new fragment using an ASE Atoms object
 
         Parameters
         ----------
         atoms: ase.atoms.Atoms
             The atoms forming the fragment.
+        indices_in_structure: list of int
+            Indices of the Fragment's atoms, relative to the Structure, that the Fragment is
+            a part of.
         allowed_translation: str
             How shall the fragment be allowed to translate?
             If the string contains an "x", translation in x-direction is allowed, etc.
             E.g., to allow only translation in x- and y-direction, set allowed_translation="xy"
             To completely forbid any translation, use an empty string.
         allowed_rotation: str
             Allows the user to set constraints on the rotation axis of a fragment.
@@ -64,14 +72,15 @@
             'z' allows only rotation of the fragment around the (space-fixed) z-axis
             'xyz' allows for unrestricted rotation of the fragment
 
         """
 
         # Initialize using an already existing Atoms object
         self.atoms = deepcopy(atoms)
+        self.indices_in_structure = indices_in_structure
 
         # Tranlation and rotation, which the fragment is allowed to do
         self.allowed_translation = allowed_translation
         self.allowed_rotation = allowed_rotation
 
         # Create body-fixed axis system, euler angles and inertia matrix
         self.body_fixed_axis_x = np.array([1.0, 0.0, 0.0])
```

### Comparing `RIIGID-1.0.3/riigid/library/misc.py` & `RIIGID-1.0.4/riigid/library/misc.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/library/rotation.py` & `RIIGID-1.0.4/riigid/library/rotation.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/optimization_step.py` & `RIIGID-1.0.4/riigid/optimization_step.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/optimizer/Deprecated_GDWAS.py` & `RIIGID-1.0.4/riigid/optimizer/Deprecated_GDWAS.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/optimizer/GDWAS.py` & `RIIGID-1.0.4/riigid/optimizer/GDWAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
             # Check for convergence
             self.convergence_criterion.check(
                 optimization_history=self.optimization_history
             )
 
             # If a callback function was provided, execute it. Useful to save data after every step
-            if callback:
+            if callback is not None:
                 callback()
 
         self.print_reason_for_end_of_optimization()
 
     def adapt_stepsize_to_energy_change(self):
         """Adapt the stepsize according to the last update step.
```

### Comparing `RIIGID-1.0.3/riigid/optimizer/optimizer.py` & `RIIGID-1.0.4/riigid/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `RIIGID-1.0.3/riigid/riigid.py` & `RIIGID-1.0.4/riigid/riigid.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 import time
 import warnings
 import json
 from importlib import resources
 
 from ase.calculators.vasp.vasp import Vasp
 from ase.io.trajectory import Trajectory
+from ase.io import write as ase_write
 
 from riigid.structure import Structure
 from riigid.convergence.displacement import Criterion_Displacement
 from riigid.library.misc import copy_docstring, redirect_stdout_to_file
 from riigid.optimizer.GDWAS import GDWAS
 from riigid.optimizer.Deprecated_GDWAS import Deprecated_GDWAS
 
 # Load the configuration file
 with resources.open_text("riigid", "config.json") as config_file:
     config = json.load(config_file)
 # Accessing file names from the configuration
 out_file = config["output_files"]["out_file"]
 opt_file = config["output_files"]["opt_file"]
 traj_file = config["output_files"]["traj_file"]
+final_geometry_file = config["output_files"]["final_geometry_file"]
 opt_hist_file = config["output_files"]["opt_hist_file"]
 
 
 class RIIGID:
     """RIgid Interface Geometry IDentification
 
     The structure under investigation is separated into so-called fragments, which are a
@@ -290,14 +292,15 @@
         print()
 
     @redirect_stdout_to_file(out_file)
     def save_optimization_progress(self):
         """Saves the progress of the optimization."""
         self.save_optimization_history()
         self.create_trajectory_file_from_optimization_history()
+        self.save_final_geometry()
         self.save_optimization_summary()
 
     @redirect_stdout_to_file(out_file)
     def save_optimization_history(self):
         """Save the optimization history (list of optimization steps) as a pickle file."""
         optimization_history = self.optimizer.optimization_history
         fn = opt_hist_file
@@ -314,14 +317,22 @@
         for optimization_step in optimization_history:
             traj.write(
                 atoms=optimization_step.structure.atoms, energy=optimization_step.energy
             )
         traj.close()
 
     @redirect_stdout_to_file(out_file)
+    def save_final_geometry(self):
+        """Saves the final geometry as an xyz file."""
+        ase_write(
+            filename=final_geometry_file,
+            images=self.optimizer.optimization_history[-1].structure.atoms,
+        )
+
+    @redirect_stdout_to_file(out_file)
     def save_optimization_summary(self):
         """Save Information about the optimization to a separate file."""
         fn = opt_file
         with open(fn, "w") as file:
             file.write("Summary of Optimization:\n")
             optimization_history = self.optimizer.optimization_history
             for iteration, step in enumerate(optimization_history):
```

### Comparing `RIIGID-1.0.3/riigid/structure.py` & `RIIGID-1.0.4/riigid/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,22 @@
             To initialize a structure, an atoms object must be given, which can later be separated
             into fragments. It will also be possible to define a fragment by adding additional atoms later
             on (not yet implemented).
 
         """
         self.atoms = atoms
         self.fragments = []
+        rest_fragment_indices, _ = get_indices_of_atoms1_in_atoms2(
+            atoms1=self.atoms, atoms2=self.atoms
+        )
         self.rest_fragment = Fragment(
-            atoms=self.atoms, allowed_translation="", allowed_rotation=""
+            atoms=self.atoms,
+            indices_in_structure=rest_fragment_indices,
+            allowed_translation="",
+            allowed_rotation="",
         )
 
     def define_fragment_by_indices(
         self, indices, allowed_translation, allowed_rotation
     ):
         """Define a RIIGID fragment by its indices.
 
@@ -86,14 +92,15 @@
 
         """
         fragment_atoms = deepcopy(self.atoms[indices])
         rest_fragment_atoms = deepcopy(self.rest_fragment.atoms)
 
         new_fragment = Fragment(
             atoms=fragment_atoms,
+            indices_in_structure=indices,
             allowed_translation=allowed_translation,
             allowed_rotation=allowed_rotation,
         )
 
         # Remove atoms of this new fragment from the rest-fragment
         (
             indices_of_new_fragment_in_rest_fragment,
@@ -104,16 +111,22 @@
         if not found:
             raise RuntimeError(
                 "Atoms not found in rest-fragment. Did you already include some of the atoms in another fragment? Every atom has to belong to exactly one fragment. (All atoms not assigned to any fragment form the rest-fragment.)"
             )
         del rest_fragment_atoms[indices_of_new_fragment_in_rest_fragment]
 
         # Update rest-fragment and append new fragment to list of fragments
+        rest_fragment_indices, _ = get_indices_of_atoms1_in_atoms2(
+            atoms1=rest_fragment_atoms, atoms2=self.atoms
+        )
         self.rest_fragment = Fragment(
-            atoms=rest_fragment_atoms, allowed_translation="", allowed_rotation=""
+            atoms=rest_fragment_atoms,
+            indices_in_structure=rest_fragment_indices,
+            allowed_translation="",
+            allowed_rotation="",
         )
         self.fragments.append(new_fragment)
 
     def define_fragment_by_adding_atoms(
         self, atoms, position, orientation, allowed_translation="", allowed_rotation=""
     ):
         """Define fragments by adding additional atoms to Structure.atoms.
@@ -251,19 +264,22 @@
 
     def update_atoms_attribute_from_fragments(self):
         """Update Structure.atoms after movement of fragments.
 
         When individual fragments are moved, the atoms object of the structure must also be updated
         accordingly.
 
-        """
-        self.atoms = deepcopy(self.rest_fragment.atoms)
+        The function also makes sure that the order of the atoms in Structure.atoms
+        is not changed!
 
-        for fragment in self.fragments:
-            self.atoms += deepcopy(fragment.atoms)
+        """
+        for fragment in self.fragments + [self.rest_fragment]:
+            self.atoms.positions[list(fragment.indices_in_structure),:] = deepcopy(
+                fragment.atoms.positions
+            )
 
     def move(self, forces, stepsize):
         """Move the fragments according to the forces.
 
         Given the forces on all individual atoms and a stepsize, move the fragments.
 
         The functions first calculates the net force and the torque acting on each fragment.
```

### Comparing `RIIGID-1.0.3/setup.py` & `RIIGID-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RIIGID",
-    version="1.0.3",
+    version="1.0.4",
     description="RIIGID - RIgid Interface Geometry IDentification",
     packages=find_packages(),
     license="MIT",
     python_requires=">3.8.0",
     url="https://github.com/siegfriedkaidisch/RIIGID",
     author="Siegfried Kaidisch",
     author_email="siegfried.kaidisch@uni-graz.at",
```

