# Comparing `tmp/pbc_distance_calculator-1.0.1.tar.gz` & `tmp/pbc_distance_calculator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbc_distance_calculator-1.0.1.tar", last modified: Mon Apr 22 17:06:01 2024, max compression
+gzip compressed data, was "pbc_distance_calculator-1.1.0.tar", last modified: Mon Apr 22 20:30:38 2024, max compression
```

## Comparing `pbc_distance_calculator-1.0.1.tar` & `pbc_distance_calculator-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:06:01.641719 pbc_distance_calculator-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 17:06:01.641719 pbc_distance_calculator-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-22 17:05:57.000000 pbc_distance_calculator-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:06:01.641719 pbc_distance_calculator-1.0.1/pbc_distance_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 17:05:57.000000 pbc_distance_calculator-1.0.1/pbc_distance_calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-22 17:05:57.000000 pbc_distance_calculator-1.0.1/pbc_distance_calculator/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:06:01.641719 pbc_distance_calculator-1.0.1/pbc_distance_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 17:06:01.000000 pbc_distance_calculator-1.0.1/pbc_distance_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-22 17:06:01.000000 pbc_distance_calculator-1.0.1/pbc_distance_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:06:01.000000 pbc_distance_calculator-1.0.1/pbc_distance_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 17:06:01.000000 pbc_distance_calculator-1.0.1/pbc_distance_calculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 17:06:01.641719 pbc_distance_calculator-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 17:05:57.000000 pbc_distance_calculator-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:38.553305 pbc_distance_calculator-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-22 20:30:38.553305 pbc_distance_calculator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-22 20:30:34.000000 pbc_distance_calculator-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:38.553305 pbc_distance_calculator-1.1.0/pbc_distance_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 20:30:34.000000 pbc_distance_calculator-1.1.0/pbc_distance_calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-22 20:30:34.000000 pbc_distance_calculator-1.1.0/pbc_distance_calculator/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:38.553305 pbc_distance_calculator-1.1.0/pbc_distance_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-22 20:30:38.000000 pbc_distance_calculator-1.1.0/pbc_distance_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-22 20:30:38.000000 pbc_distance_calculator-1.1.0/pbc_distance_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:30:38.000000 pbc_distance_calculator-1.1.0/pbc_distance_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 20:30:38.000000 pbc_distance_calculator-1.1.0/pbc_distance_calculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 20:30:38.553305 pbc_distance_calculator-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 20:30:34.000000 pbc_distance_calculator-1.1.0/setup.py
```

### Comparing `pbc_distance_calculator-1.0.1/PKG-INFO` & `pbc_distance_calculator-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.0.1
+Version: 1.1.0
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
 Description-Content-Type: text/markdown
 
 # pbc_distance_calculator
 
@@ -33,14 +33,31 @@
 cell_matrix: NDArray = ...
 
 # array of shape (N, N)
 # element (i, j) is minimum image distance between i and j
 pairwise_distances: NDArray = get_pairwise_distances(positions, cell_matrix)
 ```
 
-The cell matrix, is, in general:
+The above script performs the calculation in a vectorized form, computing every pairwise distance at once. To do it serially instead:
+
+```python
+from numpy.typing import NDArray
+from pbc_distance_calculator import get_pairwise_distance
+
+# arrays of shape (1, 3) or (3, 1)
+first_position: NDArray = ...
+second_position: NDArray = ...
+
+# array of shape (3, 3)
+cell_matrix: NDArray = ...
+
+# minimum image distance
+pairwise_distances: float = get_pairwise_distance(first_position - second_position, cell_matrix)
+```
+
+Note that the cell matrix, is, in general:
 
 $$
 \begin{pmatrix} \mathbf{a} & \mathbf{b} & \mathbf{c} \end{pmatrix}
 $$
 
 where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any issues, feel free to open an issue 🙂.
```

### Comparing `pbc_distance_calculator-1.0.1/README.md` & `pbc_distance_calculator-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,31 @@
 cell_matrix: NDArray = ...
 
 # array of shape (N, N)
 # element (i, j) is minimum image distance between i and j
 pairwise_distances: NDArray = get_pairwise_distances(positions, cell_matrix)
 ```
 
-The cell matrix, is, in general:
+The above script performs the calculation in a vectorized form, computing every pairwise distance at once. To do it serially instead:
+
+```python
+from numpy.typing import NDArray
+from pbc_distance_calculator import get_pairwise_distance
+
+# arrays of shape (1, 3) or (3, 1)
+first_position: NDArray = ...
+second_position: NDArray = ...
+
+# array of shape (3, 3)
+cell_matrix: NDArray = ...
+
+# minimum image distance
+pairwise_distances: float = get_pairwise_distance(first_position - second_position, cell_matrix)
+```
+
+Note that the cell matrix, is, in general:
 
 $$
 \begin{pmatrix} \mathbf{a} & \mathbf{b} & \mathbf{c} \end{pmatrix}
 $$
 
 where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any issues, feel free to open an issue 🙂.
```

### Comparing `pbc_distance_calculator-1.0.1/pbc_distance_calculator/calculator.py` & `pbc_distance_calculator-1.1.0/pbc_distance_calculator/calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 def get_pairwise_distances(positions: NDArray, cell_matrix: NDArray) -> NDArray:
 
     """
     function for computing pairwise distances
     """
 
+    assert positions.shape[1] == 3
+    assert cell_matrix.shape == (3, 3)
+
     # first, invert cell matrix
     inverted_cell_matrix = np.linalg.inv(cell_matrix)
 
     # calculate physical difference tensor
     differences = positions[:, None] - positions
 
     # get fractional differences, changing from distance units to supercell lattice units
@@ -31,7 +34,24 @@
     images = np.einsum("km,ijm->ijk", cell_matrix, np.round(fractional_differences))
 
     # subtract off the images to get the minimum image differences
     differences = differences - images
     minimum_image_distances = np.linalg.norm(differences, axis=2)
 
     return minimum_image_distances
+
+
+def get_pairwise_distance(difference: NDArray, cell_matrix: NDArray) -> float:
+
+    """
+    function for computing pairwise distance
+    """
+
+    assert difference.shape in {(1, 3), (3, )}
+    assert cell_matrix.shape == (3, 3)
+
+    inverted_cell_matrix = np.linalg.inv(cell_matrix)
+    fractional_difference = inverted_cell_matrix @ difference
+    image = cell_matrix @ np.round(fractional_difference)
+    difference = difference - image
+
+    return float(np.linalg.norm(difference))
```

### Comparing `pbc_distance_calculator-1.0.1/pbc_distance_calculator.egg-info/PKG-INFO` & `pbc_distance_calculator-1.1.0/pbc_distance_calculator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.0.1
+Version: 1.1.0
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
 Description-Content-Type: text/markdown
 
 # pbc_distance_calculator
 
@@ -33,14 +33,31 @@
 cell_matrix: NDArray = ...
 
 # array of shape (N, N)
 # element (i, j) is minimum image distance between i and j
 pairwise_distances: NDArray = get_pairwise_distances(positions, cell_matrix)
 ```
 
-The cell matrix, is, in general:
+The above script performs the calculation in a vectorized form, computing every pairwise distance at once. To do it serially instead:
+
+```python
+from numpy.typing import NDArray
+from pbc_distance_calculator import get_pairwise_distance
+
+# arrays of shape (1, 3) or (3, 1)
+first_position: NDArray = ...
+second_position: NDArray = ...
+
+# array of shape (3, 3)
+cell_matrix: NDArray = ...
+
+# minimum image distance
+pairwise_distances: float = get_pairwise_distance(first_position - second_position, cell_matrix)
+```
+
+Note that the cell matrix, is, in general:
 
 $$
 \begin{pmatrix} \mathbf{a} & \mathbf{b} & \mathbf{c} \end{pmatrix}
 $$
 
 where $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$ are the lattice vectors of the supercell. Note that this definition works for any set of lattice parameters! So, no matter how weird your crystal, this package should work. If there are any issues, feel free to open an issue 🙂.
```

