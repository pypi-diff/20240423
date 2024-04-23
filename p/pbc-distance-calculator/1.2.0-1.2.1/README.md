# Comparing `tmp/pbc_distance_calculator-1.2.0.tar.gz` & `tmp/pbc_distance_calculator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbc_distance_calculator-1.2.0.tar", last modified: Tue Apr 23 01:52:09 2024, max compression
+gzip compressed data, was "pbc_distance_calculator-1.2.1.tar", last modified: Tue Apr 23 15:51:57 2024, max compression
```

## Comparing `pbc_distance_calculator-1.2.0.tar` & `pbc_distance_calculator-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:52:09.934917 pbc_distance_calculator-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-23 01:52:09.934917 pbc_distance_calculator-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-23 01:52:02.000000 pbc_distance_calculator-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:52:09.930917 pbc_distance_calculator-1.2.0/pbc_distance_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 01:52:02.000000 pbc_distance_calculator-1.2.0/pbc_distance_calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-23 01:52:02.000000 pbc_distance_calculator-1.2.0/pbc_distance_calculator/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:52:09.934917 pbc_distance_calculator-1.2.0/pbc_distance_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-23 01:52:09.000000 pbc_distance_calculator-1.2.0/pbc_distance_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 01:52:09.000000 pbc_distance_calculator-1.2.0/pbc_distance_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:52:09.000000 pbc_distance_calculator-1.2.0/pbc_distance_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 01:52:09.000000 pbc_distance_calculator-1.2.0/pbc_distance_calculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 01:52:09.934917 pbc_distance_calculator-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 01:52:02.000000 pbc_distance_calculator-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:51:57.077690 pbc_distance_calculator-1.2.1/pbc_distance_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/setup.py
```

### Comparing `pbc_distance_calculator-1.2.0/PKG-INFO` & `pbc_distance_calculator-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.2.0
+Version: 1.2.1
+Summary: A package for computing distances accounting for periodic boundary conditions
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
+License: MIT
+Keywords: periodic-boundary-conditions,distance-computation,simulation,molecular-dynamics,lattice-systems,neighbor-lists,periodic-images
+Requires-Python: <=3.12,>=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
 
 # pbc_distance_calculator
 
 ![](https://img.shields.io/badge/python-3.9--3.12-blue?logo=python&logoColor=white&labelColor=blue&color=grey)
 
 This Python package computes pairwise distances in a simulation box accounting for [periodic boundary conditions](https://en.wikipedia.org/wiki/Periodic_boundary_conditions).
 
@@ -47,31 +53,38 @@
 first_position: NDArray = ...
 second_position: NDArray = ...
 
 # array of shape (3, 3)
 cell_matrix: NDArray = ...
 
 # minimum image distance
-pairwise_distances: float = get_pairwise_distance(first_position - second_position, cell_matrix)
+pairwise_distance: float = get_pairwise_distance(
+    first_position - second_position,
+    cell_matrix
+)
 ```
 
-In both functions, you can also specify different engines to compute the distances. This is especially advantageous for large systems, where you can specify ``jax`` or ``torch`` as an engine. For example:
+In both functions, you can also specify different engines to compute the distances. This is especially advantageous for large systems, where you can specify ``jax.numpy`` or ``torch`` as an engine. For example:
 
 ```python
 import torch
 from pbc_distance_calculator import get_pairwise_distances
 
 ...
 
 torch.set_default_device("cuda")
-pairwise_distances = get_pairwise_distances(positions, cell_matrix, engine=torch)
+pairwise_distances = get_pairwise_distances(
+    positions,
+    cell_matrix,
+    engine=torch
+)
 ```
 
 which will calculate the pairwise distances using the CUDA-backend of PyTorch. Note that the only engine installed by default is ``numpy``, so make sure to separately install ``jax`` or ``torch`` if you want to use these modules.
 
 Note that the cell matrix, is, in general:
 
 $$
 \begin{pmatrix} \mathbf{a} & \mathbf{b} & \mathbf{c} \end{pmatrix}
 $$
 
-where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any issues, feel free to open an issue 🙂.
+where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any problems, feel free to [open an issue](https://github.com/MUEXLY/pbc_distance_calculator/issues) 🙂.
```

### Comparing `pbc_distance_calculator-1.2.0/README.md` & `pbc_distance_calculator-1.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -39,31 +39,38 @@
 first_position: NDArray = ...
 second_position: NDArray = ...
 
 # array of shape (3, 3)
 cell_matrix: NDArray = ...
 
 # minimum image distance
-pairwise_distances: float = get_pairwise_distance(first_position - second_position, cell_matrix)
+pairwise_distance: float = get_pairwise_distance(
+    first_position - second_position,
+    cell_matrix
+)
 ```
 
-In both functions, you can also specify different engines to compute the distances. This is especially advantageous for large systems, where you can specify ``jax`` or ``torch`` as an engine. For example:
+In both functions, you can also specify different engines to compute the distances. This is especially advantageous for large systems, where you can specify ``jax.numpy`` or ``torch`` as an engine. For example:
 
 ```python
 import torch
 from pbc_distance_calculator import get_pairwise_distances
 
 ...
 
 torch.set_default_device("cuda")
-pairwise_distances = get_pairwise_distances(positions, cell_matrix, engine=torch)
+pairwise_distances = get_pairwise_distances(
+    positions,
+    cell_matrix,
+    engine=torch
+)
 ```
 
 which will calculate the pairwise distances using the CUDA-backend of PyTorch. Note that the only engine installed by default is ``numpy``, so make sure to separately install ``jax`` or ``torch`` if you want to use these modules.
 
 Note that the cell matrix, is, in general:
 
 $$
 \begin{pmatrix} \mathbf{a} & \mathbf{b} & \mathbf{c} \end{pmatrix}
 $$
 
-where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any issues, feel free to open an issue 🙂.
+where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any problems, feel free to [open an issue](https://github.com/MUEXLY/pbc_distance_calculator/issues) 🙂.
```

### Comparing `pbc_distance_calculator-1.2.0/pbc_distance_calculator/calculator.py` & `pbc_distance_calculator-1.2.1/pbc_distance_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `pbc_distance_calculator-1.2.0/pbc_distance_calculator.egg-info/PKG-INFO` & `pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.2.0
+Version: 1.2.1
+Summary: A package for computing distances accounting for periodic boundary conditions
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
+License: MIT
+Keywords: periodic-boundary-conditions,distance-computation,simulation,molecular-dynamics,lattice-systems,neighbor-lists,periodic-images
+Requires-Python: <=3.12,>=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
 
 # pbc_distance_calculator
 
 ![](https://img.shields.io/badge/python-3.9--3.12-blue?logo=python&logoColor=white&labelColor=blue&color=grey)
 
 This Python package computes pairwise distances in a simulation box accounting for [periodic boundary conditions](https://en.wikipedia.org/wiki/Periodic_boundary_conditions).
 
@@ -47,31 +53,38 @@
 first_position: NDArray = ...
 second_position: NDArray = ...
 
 # array of shape (3, 3)
 cell_matrix: NDArray = ...
 
 # minimum image distance
-pairwise_distances: float = get_pairwise_distance(first_position - second_position, cell_matrix)
+pairwise_distance: float = get_pairwise_distance(
+    first_position - second_position,
+    cell_matrix
+)
 ```
 
-In both functions, you can also specify different engines to compute the distances. This is especially advantageous for large systems, where you can specify ``jax`` or ``torch`` as an engine. For example:
+In both functions, you can also specify different engines to compute the distances. This is especially advantageous for large systems, where you can specify ``jax.numpy`` or ``torch`` as an engine. For example:
 
 ```python
 import torch
 from pbc_distance_calculator import get_pairwise_distances
 
 ...
 
 torch.set_default_device("cuda")
-pairwise_distances = get_pairwise_distances(positions, cell_matrix, engine=torch)
+pairwise_distances = get_pairwise_distances(
+    positions,
+    cell_matrix,
+    engine=torch
+)
 ```
 
 which will calculate the pairwise distances using the CUDA-backend of PyTorch. Note that the only engine installed by default is ``numpy``, so make sure to separately install ``jax`` or ``torch`` if you want to use these modules.
 
 Note that the cell matrix, is, in general:
 
 $$
 \begin{pmatrix} \mathbf{a} & \mathbf{b} & \mathbf{c} \end{pmatrix}
 $$
 
-where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any issues, feel free to open an issue 🙂.
+where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any problems, feel free to [open an issue](https://github.com/MUEXLY/pbc_distance_calculator/issues) 🙂.
```

