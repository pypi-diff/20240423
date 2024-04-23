# Comparing `tmp/optymus-0.1.1.tar.gz` & `tmp/optymus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optymus-0.1.1.tar", max compression
+gzip compressed data, was "optymus-0.1.2.tar", max compression
```

## Comparing `optymus-0.1.1.tar` & `optymus-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,29 @@
--rw-r--r--   0        0        0     1073 2023-12-23 16:36:06.144553 optymus-0.1.1/LICENSE
--rw-r--r--   0        0        0     2677 2024-01-02 03:10:42.846666 optymus-0.1.1/README.md
--rw-r--r--   0        0        0      307 2023-12-28 19:36:37.986894 optymus-0.1.1/optymus/minimize/__init__.py
--rw-r--r--   0        0        0      528 2023-12-28 19:37:03.608646 optymus-0.1.1/optymus/minimize/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9630 2023-11-28 14:08:49.914347 optymus-0.1.1/optymus/minimize/__pycache__/_methods.cpython-311.pyc
--rw-r--r--   0        0        0     4243 2024-01-02 03:01:16.251735 optymus-0.1.1/optymus/minimize/__pycache__/_minimize.cpython-311.pyc
--rw-r--r--   0        0        0     2380 2024-01-02 03:01:10.039475 optymus-0.1.1/optymus/minimize/_minimize.py
--rw-r--r--   0        0        0       74 2023-12-28 20:22:02.188331 optymus-0.1.1/optymus/plots/__init__.py
--rw-r--r--   0        0        0      279 2023-12-28 20:22:07.092002 optymus-0.1.1/optymus/plots/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4217 2024-01-02 03:02:43.003404 optymus-0.1.1/optymus/plots/__pycache__/_plots.cpython-311.pyc
--rw-r--r--   0        0        0     1925 2024-01-02 03:02:21.846505 optymus-0.1.1/optymus/plots/_plots.py
--rw-r--r--   0        0        0      163 2023-11-06 17:53:41.316533 optymus-0.1.1/optymus/search/__init__.py
--rw-r--r--   0        0        0      362 2023-11-06 17:53:45.891480 optymus-0.1.1/optymus/search/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2823 2023-11-10 20:30:01.774511 optymus-0.1.1/optymus/search/__pycache__/_search.cpython-311.pyc
--rw-r--r--   0        0        0     4914 2023-09-19 21:46:59.508104 optymus-0.1.1/optymus/search/__pycache__/linear_search.cpython-311.pyc
--rw-r--r--   0        0        0     4079 2023-09-19 21:56:45.701981 optymus-0.1.1/optymus/search/__pycache__/plots.cpython-311.pyc
--rw-r--r--   0        0        0     1481 2023-11-10 20:29:56.850247 optymus-0.1.1/optymus/search/_search.py
--rw-r--r--   0        0        0     8611 2023-12-28 20:22:07.527973 optymus-0.1.1/optymus/utils/__pycache__/_optim_methods.cpython-311.pyc
--rw-r--r--   0        0        0      179 2023-10-24 02:12:35.552162 optymus-0.1.1/optymus/utils/__pycache__/tools.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-12-28 20:08:08.250178 optymus-0.1.1/optymus/utils/_const_methods.py
--rw-r--r--   0        0        0     5061 2023-12-28 20:06:18.489695 optymus-0.1.1/optymus/utils/_optim_methods.py
--rw-r--r--   0        0        0      741 2024-01-02 03:09:07.229066 optymus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 optymus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-18 14:49:26.833687 optymus-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2548 2024-04-22 21:42:46.814839 optymus-0.1.2/README.md
+-rw-r--r--   0        0        0       74 2024-04-22 21:42:46.902866 optymus-0.1.2/optymus/optim/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-22 21:42:46.902866 optymus-0.1.2/optymus/optim/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      252 2024-04-22 22:09:11.400491 optymus-0.1.2/optymus/optim/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      635 2024-04-22 22:09:12.924332 optymus-0.1.2/optymus/optim/__pycache__/_adaptative.cpython-312.pyc
+-rw-r--r--   0        0        0     4494 2024-04-22 23:46:52.686319 optymus-0.1.2/optymus/optim/__pycache__/_first_order.cpython-312.pyc
+-rw-r--r--   0        0        0     9630 2024-04-22 21:42:46.902866 optymus-0.1.2/optymus/optim/__pycache__/_methods.cpython-311.pyc
+-rw-r--r--   0        0        0     4243 2024-04-22 21:42:46.902866 optymus-0.1.2/optymus/optim/__pycache__/_minimize.cpython-311.pyc
+-rw-r--r--   0        0        0     3451 2024-04-22 22:18:24.983444 optymus-0.1.2/optymus/optim/__pycache__/_optimize.cpython-312.pyc
+-rw-r--r--   0        0        0     1535 2024-04-22 23:38:40.875909 optymus-0.1.2/optymus/optim/__pycache__/_second_order.cpython-312.pyc
+-rw-r--r--   0        0        0     3177 2024-04-22 23:57:03.660761 optymus-0.1.2/optymus/optim/__pycache__/_zero_order.cpython-312.pyc
+-rw-r--r--   0        0        0      204 2024-04-22 23:57:44.092110 optymus-0.1.2/optymus/optim/_adaptative.py
+-rw-r--r--   0        0        0     2834 2024-04-22 23:46:48.610445 optymus-0.1.2/optymus/optim/_first_order.py
+-rw-r--r--   0        0        0     2269 2024-04-22 22:12:05.754564 optymus-0.1.2/optymus/optim/_optimize.py
+-rw-r--r--   0        0        0      779 2024-04-22 23:38:25.872064 optymus-0.1.2/optymus/optim/_second_order.py
+-rw-r--r--   0        0        0     2238 2024-04-22 23:56:37.349196 optymus-0.1.2/optymus/optim/_zero_order.py
+-rw-r--r--   0        0        0      851 2024-04-22 22:48:47.176739 optymus-0.1.2/optymus/utils/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-22 22:48:54.040846 optymus-0.1.2/optymus/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7641 2024-04-22 23:40:42.694697 optymus-0.1.2/optymus/utils/__pycache__/_obj_functions.cpython-312.pyc
+-rw-r--r--   0        0        0     8611 2024-04-18 14:49:26.849686 optymus-0.1.2/optymus/utils/__pycache__/_optim_methods.cpython-311.pyc
+-rw-r--r--   0        0        0     5508 2024-04-22 22:09:11.732457 optymus-0.1.2/optymus/utils/__pycache__/_plots.cpython-312.pyc
+-rw-r--r--   0        0        0     2686 2024-04-22 22:40:21.075671 optymus-0.1.2/optymus/utils/__pycache__/_search.cpython-312.pyc
+-rw-r--r--   0        0        0      179 2024-04-18 14:49:26.849686 optymus-0.1.2/optymus/utils/__pycache__/tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1951 2024-04-22 23:40:38.310740 optymus-0.1.2/optymus/utils/_obj_functions.py
+-rw-r--r--   0        0        0     2953 2024-04-22 21:42:46.906868 optymus-0.1.2/optymus/utils/_plots.py
+-rw-r--r--   0        0        0     1540 2024-04-22 22:40:17.403524 optymus-0.1.2/optymus/utils/_search.py
+-rw-r--r--   0        0        0      792 2024-04-23 00:00:49.397339 optymus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 optymus-0.1.2/PKG-INFO
```

### Comparing `optymus-0.1.1/LICENSE` & `optymus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optymus-0.1.1/README.md` & `optymus-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 <h1 align="center">
-<img src="logo.png" width="400">
+<img src="logo.svg" width="400">
 </h1>
 
 [![PyPI](https://img.shields.io/pypi/v/optymus)](https://pypi.org/project/optymus/)
 [![GitHub](https://img.shields.io/github/license/kleyt0n/optymus)](https://github.com/kleyt0n/optymus/blob/master/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/optymus/badge/?version=latest)](https://optymus.readthedocs.io/en/latest/?badge=latest)
 
-Welcome to _optymus_, the Optimization Methods Library for Python! This library provides a comprehensive collection of optimization methods, both with and without constraints, implemented in the Python programming language.
+> Check the [Optimization in Deep Learning and Engineering](https://quantsci.org/odle-book) material.
 
-## Table of Contents
+> Optymus is part of [quantsci](https://quantsci.org) project.
 
-- [Introduction](#introduction)
-- [Getting Started](#getting-started)
-- [Content](#content)
-- [Contributions](#contributions)
-- [License](#license)
+This library provides a comprehensive collection of optimization methods, both with and without constraints. The main goal is provide a simple structure to improve research and development in optimization problems.
 
-## Introduction
+## Implemented Methods
+
+| Method | Description |
+| --- | --- |
+| bfgs | Broyden-Fletcher-Goldfarb-Shanno (BFGS) |
+| steepdesc | Steepest Descent |
+| newton_raphson | Newton-Raphson Method |
+| powell | Powell's Method |
+|fletcher_reeves | Fletcher-Reeves |
 
-_optymus_ is designed to empower users with a versatile set of optimization tools, facilitating the search for optimal solutions in various problem domains. This library covers a range of optimization methods, making it suitable for diverse applications in computer science and engineering.
 
 ## Getting Started
 
 To begin using _optymus_, follow these steps:
 
 1. **Install optymus:**
    ```bash
-   pip install --upgrade optymus
+   pip install optymus
    ```
 
 2. **Explore the Documentation:**
    Visit the [official documentation](https://optymus-docs.readthedocs.com) to understand the available optimization methods and how to use them effectively.
 
 3. **Get Started:**
    ```python
-   from optymus.minimize import Optimizer
+   from optymus.optim import Optimizer
+   from optymus.utils import mccormick_function
    
    import numpy as np
-   f = lambda x: x[0]**[2]-3*x[0]*x[1]+4*x[1]**2+x[0]-x[1]
-   grad = lambda x: np.array([2*x[0]-3*x[1]+1, -3*x[0]+8*x[1]-1])
-   hess = lambda x: np.array([[2, -3], [-3, 8]])
+
+   f = mccormick_function()
    initial_point = np.array([2, 2])
 
-   optimizer = Optimizer(f_obj=f,
-                        x0=initial_point,
-                        grad=grad,
-                        hess=hess,
-                        method='bfgs')
-   
-   optimizer.report()
+   opt = Optimizer(f_obj=f,
+                   x0=initial_point,
+                   method='bfgs')
 
-   optimizer.plot()
-   ```
+   opt.report()
 
-## Content
+   opt.plot()
+   ```
 
-_optymus_ includes a rich set of optimization methods, such as:
+Refer to the documentation for detailed information on each method and its application.
 
-- Unconstrained Optimization Methods
-- Constrained Optimization Methods
-- Global Optimization
-- Gradient Descent
-- Evolutionary Algorithms
+## Implement your own method an compare with the implemented ones
 
-Refer to the documentation for detailed information on each method and its application.
+We are working to implement a simple way to add your own optimization method. 
 
 ## Contributions
 
-Contributions to Optymus are highly appreciated! If you have additional optimization methods, improvements, or bug fixes, please submit a pull request following the [contribution guidelines](CONTRIBUTING.md).
+Contributions to Optymus are highly appreciated. If you have additional optimization methods, improvements, or bug fixes, please submit a pull request following the [contribution guidelines](CONTRIBUTING.md).
 
-## License
+## Cite
 
-Optymus is licensed under the [MIT License](LICENSE), allowing you to use, modify, and distribute the library for both commercial and non-commercial purposes.
+If you use Optymus in your research, please consider citing the library using the following BibTeX entry:
 
-Start optimizing with Optymus and unlock the potential for finding optimal solutions in your Python projects!
+```bibtex
+@misc{optymus2024,
+  author = {Costa, Kleyton and Menezes, Ivan},
+  title = {Optymus: Optimization Methods Library for Python},
+  year = {2024},
+  note = {GitHub Repository},
+  url = {https://github.com/quantsci/optymus}
+}
+```
```

### Comparing `optymus-0.1.1/optymus/minimize/__pycache__/__init__.cpython-311.pyc` & `optymus-0.1.2/optymus/optim/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `optymus-0.1.1/optymus/minimize/__pycache__/_methods.cpython-311.pyc` & `optymus-0.1.2/optymus/optim/__pycache__/_methods.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `optymus-0.1.1/optymus/minimize/__pycache__/_minimize.cpython-311.pyc` & `optymus-0.1.2/optymus/optim/__pycache__/_minimize.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `optymus-0.1.1/optymus/plots/_plots.py` & `optymus-0.1.2/optymus/utils/_plots.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,53 @@
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 sns.set_style('whitegrid')
 
 
+def plot_function(f, title=None, min=-10, max=10, n=100):
+    """
+    Plot the function surface.
+    
+    Parameters
+    ----------
+    f : callable
+        Function to be plotted.
+    
+    Returns
+    -------
+    Plot of the function surface.
+    """
+    x = np.linspace(min, max, n)
+    y = np.linspace(min, max, n)
+    X, Y = np.meshgrid(x, y)
+    Z = f([X, Y])
+
+    fig, ax = plt.subplots(ncols=2, nrows=1, figsize=(12, 5))
+
+    fig.delaxes(ax[0])
+    ax[0] = fig.add_subplot(121, projection='3d')
+    ax[0].view_init(40, 20)
+    ax[0].plot_surface(X, Y, Z, cmap='cividis', linewidth =0)
+    ax[0].set_xlabel('x1')
+    ax[0].set_ylabel('x2')
+    ax[0].set_zlabel("f(x_1, x2)")
+    ax[0].set_title(f'{title} surface f(x1, x2)')
+
+    countour = ax[1].contour(X, Y, Z, 200, cmap='cividis')
+    ax[1].set_xlabel('x1')
+    ax[1].set_ylabel('x2')
+    if title is not None:
+        ax[1].set_title(f'{title} contour f(x1, x2)')
+    else:
+        ax[1].set_title("Function contour f(x1, x2)")
+    plt.tight_layout()
+    plt.show()
+
 def plot_optim(f, x0, method, path=True, print_opt=True):
     """
     Plot the optimization path and the function surface.
     
     Parameters
     ----------
     f : callable
```

### Comparing `optymus-0.1.1/optymus/search/__pycache__/_search.cpython-311.pyc` & `optymus-0.1.2/optymus/utils/__pycache__/_search.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Fri Nov 10 20:29:56 2023 UTC, .py size: 1481 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,168 @@
-00000000: a70d 0d0a 0000 0000 c492 4e65 c905 0000  ..........Ne....
+00000000: cb0d 0d0a 0000 0000 51e7 2666 0406 0000  ........Q.&f....
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
-00000020: 0000 0000 00f3 3200 0000 9700 6400 6401  ......2.....d.d.
-00000030: 6c00 5a01 6407 6403 8401 5a02 6408 6405  l.Z.d.d...Z.d.d.
-00000040: 8401 5a03 6400 6401 6c04 6d05 5a06 0100  ..Z.d.d.l.m.Z...
-00000050: 6409 6406 8401 5a07 6401 5300 290a e900  d.d...Z.d.S.)...
-00000060: 0000 004e e77b 14ae 47e1 7a84 3f63 0300  ...N.{..G.z.?c..
-00000070: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-00000080: 0000 f3f0 0000 0097 007c 0102 007c 007c  .........|...|.|
-00000090: 01a6 0100 00ab 0100 0000 0000 0000 007d  ...............}
-000000a0: 047d 037c 037c 027a 0000 0002 007c 007c  .}.|.|.z.....|.|
-000000b0: 037c 027a 0000 00a6 0100 00ab 0100 0000  .|.z............
-000000c0: 0000 0000 007d 067d 057c 067c 046b 0400  .....}.}.|.|.k..
-000000d0: 0000 0072 0b7c 057c 037d 057d 037c 067c  ...r.|.|.}.}.|.|
-000000e0: 047d 067d 047c 020b 007d 0209 007c 057c  .}.}.|...}...|.|
-000000f0: 027a 0000 0002 007c 007c 057c 027a 0000  .z.....|.|.|.z..
-00000100: 00a6 0100 00ab 0100 0000 0000 0000 007d  ...............}
-00000110: 087d 077c 087c 066b 0400 0000 0072 2074  .}.|.|.k.....r t
-00000120: 0100 0000 0000 0000 0000 006a 0100 0000  ...........j....
-00000130: 0000 0000 007c 037c 076b 0000 0000 00a6  .....|.|.k......
-00000140: 0100 00ab 0100 0000 0000 0000 0072 047c  .............r.|
-00000150: 037c 0766 026e 037c 077c 0366 0253 007c  .|.f.n.|.|.f.S.|
-00000160: 057c 067c 077c 0866 045c 0400 007d 037d  .|.|.|.f.\...}.}
-00000170: 047d 057d 068c 45a9 014e 2902 da02 6e70  .}.}..E..N)...np
-00000180: da03 616c 6c29 09da 0166 da01 78da 0173  ..all)...f..x..s
-00000190: da01 61da 0279 61da 0162 da02 7962 da01  ..a..ya..b..yb..
-000001a0: 63da 0279 6373 0900 0000 2020 2020 2020  c..ycs....      
-000001b0: 2020 20fa 612f 686f 6d65 2f6b 636f 7374     .a/home/kcost
-000001c0: 612f 7265 706f 732f 7265 7365 6172 6368  a/repos/research
-000001d0: 2f6f 7074 696d 697a 6174 696f 6e2d 7079  /optimization-py
-000001e0: 7468 6f6e 2f65 7865 7263 6973 6573 2f74  thon/exercises/t
-000001f0: 7261 6261 6c68 6f31 2f2e 2e2f 2e2e 2f71  rabalho1/../../q
-00000200: 736f 7074 2f73 6561 7263 682f 5f73 6561  sopt/search/_sea
-00000210: 7263 682e 7079 da0f 6272 6163 6b65 745f  rch.py..bracket_
-00000220: 6d69 6e69 6d75 6d72 1200 0000 0300 0000  minimumr........
-00000230: 73b2 0000 0080 00d8 0c0d 8871 8871 9011  s..........q.q..
-00000240: 8974 8c74 8072 8041 d80c 0d90 0189 4590  .t.t.r.A......E.
-00000250: 3190 3190 5198 1191 5591 3894 3880 7280  1.1.Q...U.8.8.r.
-00000260: 41d8 0709 8842 8277 8077 d80f 1090 2188  A....B.w.w....!.
-00000270: 3188 01d8 1113 9052 8842 8802 d80d 0e88  1......R.B......
-00000280: 4288 01f0 0204 0524 d810 1190 4191 0590  B......$....A...
-00000290: 7190 7198 1198 5199 1591 7894 7888 3288  q.q...Q...x.x.2.
-000002a0: 01d8 0b0d 9002 8a37 8837 dd1d 1f9c 56a0  .......7.7....V.
-000002b0: 41a8 01a2 4599 5d9c 5dd0 1336 9041 9071  A...E.].]..6.A.q
-000002c0: 9036 9036 b011 b041 b006 d00c 36d8 1718  .6.6...A....6...
-000002d0: 9822 9861 a012 907c 890c 8801 8832 8871  .".a...|.....2.q
-000002e0: 9022 f009 0405 24f3 0000 0000 e7f1 68e3  ."....$.......h.
-000002f0: 88b5 f8e4 3e63 0400 0000 0000 0000 0000  ....>c..........
-00000300: 0000 0700 0000 0300 0000 f302 0200 0097  ................
-00000310: 0074 0100 0000 0000 0000 0000 006a 0100  .t...........j..
-00000320: 0000 0000 0000 0064 01a6 0100 00ab 0100  .......d........
-00000330: 0000 0000 0000 0064 027a 0a00 0064 037a  .......d.z...d.z
-00000340: 0b00 007d 0464 047d 0574 0000 0000 0000  ...}.d.}.t......
-00000350: 0000 0000 006a 0200 0000 0000 0000 00a0  .....j..........
-00000360: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 007c 027c 017a 0a00 00a6 0100  .....|.|.z......
-00000380: 00ab 0100 0000 0000 0000 007d 067c 0164  ...........}.|.d
-00000390: 027c 047a 0a00 007c 067a 0500 007a 0000  .|.z...|.z...z..
-000003a0: 007d 077c 017c 047c 067a 0500 007a 0000  .}.|.|.|.z...z..
-000003b0: 007d 0867 007d 097c 067c 036b 0400 0000  .}.g.}.|.|.k....
-000003c0: 0072 7802 007c 007c 07a6 0100 00ab 0100  .rx..|.|........
-000003d0: 0000 0000 0000 0002 007c 007c 08a6 0100  .........|.|....
-000003e0: 00ab 0100 0000 0000 0000 006b 0000 0000  ...........k....
-000003f0: 0072 037c 087d 026e 027c 077d 0174 0000  .r.|.}.n.|.}.t..
-00000400: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
-00000410: 0000 00a0 0300 0000 0000 0000 0000 0000  ................
-00000420: 0000 0000 0000 0000 007c 027c 017a 0a00  .........|.|.z..
-00000430: 00a6 0100 00ab 0100 0000 0000 0000 007d  ...............}
-00000440: 067c 0164 027c 047a 0a00 007c 067a 0500  .|.d.|.z...|.z..
-00000450: 007a 0000 007d 077c 017c 047c 067a 0500  .z...}.|.|.|.z..
-00000460: 007a 0000 007d 087c 0564 027a 0d00 007d  .z...}.|.d.z...}
-00000470: 057c 09a0 0400 0000 0000 0000 0000 0000  .|..............
-00000480: 0000 0000 0000 0000 007c 017c 027a 0000  .........|.|.z..
-00000490: 0064 037a 0b00 00a6 0100 00ab 0100 0000  .d.z............
-000004a0: 0000 0000 0001 007c 067c 036b 0400 0000  .......|.|.k....
-000004b0: 00b0 787c 027c 017a 0000 0064 037a 0b00  ..x|.|.z...d.z..
-000004c0: 007d 0a02 007c 007c 0aa6 0100 00ab 0100  .}...|.|........
-000004d0: 0000 0000 0000 007d 0b64 057c 0a7c 0b7c  .......}.d.|.|.|
-000004e0: 0574 0100 0000 0000 0000 0000 006a 0500  .t...........j..
-000004f0: 0000 0000 0000 007c 09a6 0100 00ab 0100  .......|........
-00000500: 0000 0000 0000 0064 069c 057d 0c7c 0c53  .......d...}.|.S
-00000510: 0029 074e e905 0000 00e9 0100 0000 e902  .).N............
-00000520: 0000 0072 0200 0000 7a0d 476f 6c64 656e  ...r....z.Golden
-00000530: 2053 6561 7263 6829 05da 0b6d 6574 686f   Search)...metho
-00000540: 645f 6e61 6d65 da04 786f 7074 da04 666d  d_name..xopt..fm
-00000550: 696e da08 6e75 6d5f 6974 6572 da04 7061  in..num_iter..pa
-00000560: 7468 2906 7206 0000 00da 0473 7172 74da  th).r......sqrt.
-00000570: 066c 696e 616c 67da 046e 6f72 6dda 0661  .linalg..norm..a
-00000580: 7070 656e 64da 0561 7272 6179 290d 7208  ppend..array).r.
-00000590: 0000 0072 0b00 0000 720d 0000 00da 0374  ...r....r......t
-000005a0: 6f6c da03 7068 6972 1c00 0000 da04 6265  ol..phir......be
-000005b0: 7461 da07 616c 7068 615f 65da 0761 6c70  ta..alpha_e..alp
-000005c0: 6861 5f64 721d 0000 00da 0561 6c70 6861  ha_dr......alpha
-000005d0: 721b 0000 00da 0672 6573 756c 7473 0d00  r......results..
-000005e0: 0000 2020 2020 2020 2020 2020 2020 2072  ..             r
-000005f0: 1100 0000 da0e 676f 6c64 656e 5f73 6563  ......golden_sec
-00000600: 7469 6f6e 722a 0000 0010 0000 0073 3401  tionr*.......s4.
-00000610: 0000 8000 dd0b 0d8c 3790 3189 3a8c 3a90  ........7.1.:.:.
-00000620: 6189 3c98 11d1 0a1a 8043 d80f 1080 48dd  a.<......C....H.
-00000630: 0b0d 8c39 8f3e 8a3e 9821 9841 9923 d10b  ...9.>.>.!.A.#..
-00000640: 1ed4 0b1e 8044 d80e 0f90 3190 7391 3798  .....D....1.s.7.
-00000650: 4491 2ed1 0e20 8047 d80e 0f90 3390 7491  D.... .G....3.t.
-00000660: 3889 6e80 47d8 0b0d 8044 e00a 0e90 138a  8.n.G....D......
-00000670: 2a88 2ad8 0b0c 8831 8857 893a 8c3a 9801  *.*....1.W.:.:..
-00000680: 9801 9827 990a 9c0a d20b 22d0 0b22 d810  ...'......".."..
-00000690: 1788 4188 41e0 1017 8841 e50f 118c 798f  ..A.A....A....y.
-000006a0: 7e8a 7e98 61a0 0199 63d1 0f22 d40f 2288  ~.~.a...c.."..".
-000006b0: 04d8 1213 9071 9833 9177 a004 916e d112  .....q.3.w...n..
-000006c0: 2488 07d8 1213 9073 9834 9178 912e 8807  $......s.4.x....
-000006d0: e008 1090 4189 0d88 08d8 080c 8f0b 8a0b  ....A...........
-000006e0: 9051 9071 9153 9821 9147 d108 1cd4 081c  .Q.q.S.!.G......
-000006f0: d008 1cf0 1700 0b0f 9013 8a2a 882a f01a  ...........*.*..
-00000700: 000e 0f90 1189 5590 6189 4b80 45d8 0b0c  ......U.a.K.E...
-00000710: 8831 8855 8938 8c38 8044 f006 0018 27d8  .1.U.8.8.D....'.
-00000720: 1015 d810 14d8 141c dd10 1294 0898 1491  ................
-00000730: 0e94 0ef0 0b06 0e06 f000 060e 0680 46f0  ..............F.
-00000740: 0e00 0c12 804d 7213 0000 0063 0400 0000  .....Mr....c....
-00000750: 0000 0000 0000 0000 0700 0000 0300 0000  ................
-00000760: f3a4 0000 0087 0087 0187 0297 0088 0288  ................
-00000770: 0088 0166 0364 0184 087d 0474 0100 0000  ...f.d...}.t....
-00000780: 0000 0000 0000 007c 047c 03ac 02a6 0200  .......|.|......
-00000790: 00ab 0200 0000 0000 0000 005c 0200 007d  ...........\...}
-000007a0: 057d 0674 0300 0000 0000 0000 0000 006a  .}.t...........j
-000007b0: 0200 0000 0000 0000 007c 047c 057c 0666  .........|.|.|.f
-000007c0: 0264 03ac 04a6 0300 00ab 0300 0000 0000  .d..............
-000007d0: 0000 007d 0789 017c 0789 027a 0500 007a  ...}...|...z...z
-000007e0: 0000 007d 0864 057c 077c 0802 0089 007c  ...}.d.|.|.....|
-000007f0: 08a6 0100 00ab 0100 0000 0000 0000 0064  ...............d
-00000800: 0689 0064 079c 0653 0029 084e 6301 0000  ...d...S.).Nc...
-00000810: 0000 0000 0000 0000 0005 0000 0013 0000  ................
-00000820: 00f3 2600 0000 9503 9700 0200 8902 8903  ..&.............
-00000830: 7c00 8901 7a05 0000 7a00 0000 a601 0000  |...z...z.......
-00000840: ab01 0000 0000 0000 0000 5300 7205 0000  ..........S.r...
-00000850: 00a9 0029 0472 2800 0000 da01 6472 0800  ...).r(.....dr..
-00000860: 0000 7209 0000 0073 0400 0000 2080 8080  ..r....s.... ...
-00000870: 7211 0000 00fa 083c 6c61 6d62 6461 3e7a  r......<lambda>z
-00000880: 1d6c 696e 655f 7365 6172 6368 2e3c 6c6f  .line_search.<lo
-00000890: 6361 6c73 3e2e 3c6c 616d 6264 613e 3300  cals>.<lambda>3.
-000008a0: 0000 7319 0000 00f8 8000 9861 9861 a001  ..s........a.a..
-000008b0: a045 a841 a149 a10d d11e 2ed4 1e2e 8000  .E.A.I..........
-000008c0: 7213 0000 0029 0172 0a00 0000 7214 0000  r....).r....r...
-000008d0: 0029 02da 0562 7261 636b 7223 0000 007a  .)...brackr#...z
-000008e0: 0b4c 696e 6520 5365 6172 6368 7217 0000  .Line Searchr...
-000008f0: 0029 0672 1900 0000 7228 0000 0072 1a00  .).r....r(...r..
-00000900: 0000 721b 0000 0072 1c00 0000 da08 6675  ..r....r......fu
-00000910: 6e63 7469 6f6e 2903 7212 0000 00da 036f  nction).r......o
-00000920: 7074 da06 676f 6c64 656e 2909 7208 0000  pt..golden).r...
-00000930: 0072 0900 0000 722e 0000 00da 0973 7465  .r....r......ste
-00000940: 705f 7369 7a65 da09 6f62 6a65 6374 6976  p_size..objectiv
-00000950: 6572 0b00 0000 720d 0000 0072 2800 0000  er....r....r(...
-00000960: da05 785f 6f70 7473 0900 0000 6060 6020  ..x_opts....``` 
-00000970: 2020 2020 2072 1100 0000 da0b 6c69 6e65       r......line
-00000980: 5f73 6561 7263 6872 3700 0000 3200 0000  _searchr7...2...
-00000990: 737f 0000 00f8 f8f8 8000 d810 2ed0 102e  s...............
-000009a0: d010 2ed0 102e d010 2ed0 102e 8049 dd0b  .............I..
-000009b0: 1a98 39a8 09d0 0b32 d10b 32d4 0b32 8144  ..9....2..2..2.D
-000009c0: 8041 8071 dd0c 0f8c 4a90 79a8 11a8 41a8  .A.q....J.y...A.
-000009d0: 06b0 44d0 0c39 d10c 39d4 0c39 8045 d80c  ..D..9..9..9.E..
-000009e0: 0d90 0598 0191 0989 4d80 45e0 1724 d811  ........M.E..$..
-000009f0: 16d8 1015 d810 1190 0190 2591 0894 08d8  ..........%.....
-00000a00: 1415 d814 15f0 0d07 0c06 f000 070c 06f0  ................
-00000a10: 0007 0506 7213 0000 0029 0272 0200 0000  ....r....).r....
-00000a20: 7203 0000 0029 0172 1400 0000 2901 7203  r....).r....).r.
-00000a30: 0000 0029 08da 056e 756d 7079 7206 0000  ...)...numpyr...
-00000a40: 0072 1200 0000 722a 0000 00da 0e73 6369  .r....r*.....sci
-00000a50: 7079 2e6f 7074 696d 697a 65da 086f 7074  py.optimize..opt
-00000a60: 696d 697a 6572 3200 0000 7237 0000 0072  imizer2...r7...r
-00000a70: 2d00 0000 7213 0000 0072 1100 0000 fa08  -...r....r......
-00000a80: 3c6d 6f64 756c 653e 723b 0000 0001 0000  <module>r;......
-00000a90: 0073 6c00 0000 f003 0101 01d8 0012 d000  .sl.............
-00000aa0: 12d0 0012 d000 12f0 040b 0124 f000 0b01  ...........$....
-00000ab0: 24f0 000b 0124 f000 0b01 24f0 1a1f 0112  $....$....$.....
-00000ac0: f000 1f01 12f0 001f 0112 f000 1f01 12f0  ................
-00000ad0: 4201 0001 1dd0 001c d000 1cd0 001c d000  B...............
-00000ae0: 1cd0 001c f002 0c01 06f0 000c 0106 f000  ................
-00000af0: 0c01 06f0 000c 0106 f000 0c01 06f0 000c  ................
-00000b00: 0106 7213 0000 00                        ..r....
+00000020: 0000 0000 00f3 3400 0000 9700 6400 6401  ......4.....d.d.
+00000030: 6c00 6d01 5a02 0100 6405 6402 8401 5a03  l.m.Z...d.d...Z.
+00000040: 6406 6403 8401 5a04 6400 6401 6c05 6d06  d.d...Z.d.d.l.m.
+00000050: 5a07 0100 6407 6404 8401 5a08 7901 2908  Z...d.d...Z.y.).
+00000060: e900 0000 004e 6303 0000 0000 0000 0000  .....Nc.........
+00000070: 0000 0008 0000 0003 0000 00f3 3c01 0000  ............<...
+00000080: 9700 7401 0000 0000 0000 0000 6a02 0000  ..t.........j...
+00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000a0: 7c01 ab01 0000 0000 0000 7d03 0200 7c00  |.........}...|.
+000000b0: 7c03 ab01 0000 0000 0000 7d04 7c03 7c02  |.........}.|.|.
+000000c0: 7a00 0000 7d05 0200 7c00 7c05 ab01 0000  z...}...|.|.....
+000000d0: 0000 0000 7d06 7c06 7c04 6b44 0000 720b  ....}.|.|.kD..r.
+000000e0: 7c05 7c03 7d05 7d03 7c06 7c04 7d06 7d04  |.|.}.}.|.|.}.}.
+000000f0: 7c02 0b00 7d02 0900 7c05 7c02 7a00 0000  |...}...|.|.z...
+00000100: 7d07 0200 7c00 7c07 ab01 0000 0000 0000  }...|.|.........
+00000110: 7d08 7c08 7c06 6b44 0000 7244 7401 0000  }.|.|.kD..rDt...
+00000120: 0000 0000 0000 6a04 0000 0000 0000 0000  ......j.........
+00000130: 0000 0000 0000 0000 0000 7c03 7c07 6b02  ..........|.|.k.
+00000140: 0000 7401 0000 0000 0000 0000 6a06 0000  ..t.........j...
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 7c03 7c07 6602 ab01 0000 0000 0000 7401  |.|.f.........t.
+00000170: 0000 0000 0000 0000 6a06 0000 0000 0000  ........j.......
+00000180: 0000 0000 0000 0000 0000 0000 7c07 7c03  ............|.|.
+00000190: 6602 ab01 0000 0000 0000 ab03 0000 0000  f...............
+000001a0: 0000 5300 7c05 7c06 7c07 7c08 6604 5c04  ..S.|.|.|.|.f.\.
+000001b0: 0000 7d03 7d04 7d05 7d06 8c62 a901 4e29  ..}.}.}.}..b..N)
+000001c0: 04da 036a 6e70 da05 6172 7261 79da 0577  ...jnp..array..w
+000001d0: 6865 7265 da05 7374 6163 6b29 09da 0166  here..stack)...f
+000001e0: da01 78da 0173 da01 61da 0279 61da 0162  ..x..s..a..ya..b
+000001f0: da02 7962 da01 63da 0279 6373 0900 0000  ..yb..c..ycs....
+00000200: 2020 2020 2020 2020 20fa 3e2f 686f 6d65           .>/home
+00000210: 2f6b 636f 7374 612f 7265 706f 732f 6f70  /kcosta/repos/op
+00000220: 7479 6d75 736c 6962 2f6f 7074 796d 7573  tymuslib/optymus
+00000230: 2f6f 7074 796d 7573 2f75 7469 6c73 2f5f  /optymus/utils/_
+00000240: 7365 6172 6368 2e70 79da 0f62 7261 636b  search.py..brack
+00000250: 6574 5f6d 696e 696d 756d 7213 0000 0003  et_minimumr.....
+00000260: 0000 0073 b100 0000 8000 dc06 0987 6981  ...s..........i.
+00000270: 6990 0183 6c80 21d9 0708 8811 8374 8022  i...l.!......t."
+00000280: d806 0788 2181 6580 21d9 0708 8811 8374  ....!.e.!......t
+00000290: 8022 e005 0788 2282 57d8 0b0c 8861 8071  ."....".W....a.q
+000002a0: 8041 d80d 0f90 1288 0280 42d8 090a 8802  .A........B.....
+000002b0: 8041 e008 0cd8 0809 8841 8905 8041 d909  .A.......A...A..
+000002c0: 0a88 318b 1480 42d8 0709 8842 8277 dc0d  ..1...B....B.w..
+000002d0: 108f 5989 5990 7198 3191 759c 639f 6999  ..Y.Y.q.1.u.c.i.
+000002e0: 69a8 11a8 41a8 06d3 1e2f b413 b719 b119  i...A..../......
+000002f0: b841 b871 b836 d331 42d3 0d43 d006 43d8  .A.q.6.1B..C..C.
+00000300: 1314 9062 9821 9852 903c 814c 8041 8072  ...b.!.R.<.L.A.r
+00000310: 8831 8862 f00b 0009 0df3 0000 0000 6304  .1.b..........c.
+00000320: 0000 0000 0000 0000 0000 0007 0000 0003  ................
+00000330: 0000 00f3 e801 0000 9700 7400 0000 0000  ..........t.....
+00000340: 0000 0000 6a03 0000 0000 0000 0000 0000  ....j...........
+00000350: 0000 0000 0000 0000 6401 ab01 0000 0000  ........d.......
+00000360: 0000 6402 7a0a 0000 6403 7a0b 0000 7d04  ..d.z...d.z...}.
+00000370: 6404 7d05 7400 0000 0000 0000 0000 6a04  d.}.t.........j.
+00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000390: 0000 6a07 0000 0000 0000 0000 0000 0000  ..j.............
+000003a0: 0000 0000 0000 7c02 7c01 7a0a 0000 ab01  ......|.|.z.....
+000003b0: 0000 0000 0000 7d06 7c01 6402 7c04 7a0a  ......}.|.d.|.z.
+000003c0: 0000 7c06 7a05 0000 7a00 0000 7d07 7c01  ..|.z...z...}.|.
+000003d0: 7c04 7c06 7a05 0000 7a00 0000 7d08 6700  |.|.z...z...}.g.
+000003e0: 7d09 7c06 7c03 6b44 0000 726d 0200 7c00  }.|.|.kD..rm..|.
+000003f0: 7c07 ab01 0000 0000 0000 0200 7c00 7c08  |...........|.|.
+00000400: ab01 0000 0000 0000 6b02 0000 7203 7c08  ........k...r.|.
+00000410: 7d02 6e02 7c07 7d01 7400 0000 0000 0000  }.n.|.}.t.......
+00000420: 0000 6a04 0000 0000 0000 0000 0000 0000  ..j.............
+00000430: 0000 0000 0000 6a07 0000 0000 0000 0000  ......j.........
+00000440: 0000 0000 0000 0000 0000 7c02 7c01 7a0a  ..........|.|.z.
+00000450: 0000 ab01 0000 0000 0000 7d06 7c01 6402  ..........}.|.d.
+00000460: 7c04 7a0a 0000 7c06 7a05 0000 7a00 0000  |.z...|.z...z...
+00000470: 7d07 7c01 7c04 7c06 7a05 0000 7a00 0000  }.|.|.|.z...z...
+00000480: 7d08 7c05 6402 7a0d 0000 7d05 7c09 6a09  }.|.d.z...}.|.j.
+00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0000 7c01 7c02 7a00 0000 6403 7a0b 0000  ..|.|.z...d.z...
+000004b0: ab01 0000 0000 0000 0100 7c06 7c03 6b44  ..........|.|.kD
+000004c0: 0000 7201 8c6d 7c02 7c01 7a00 0000 6403  ..r..m|.|.z...d.
+000004d0: 7a0b 0000 7d0a 0200 7c00 7c0a ab01 0000  z...}...|.|.....
+000004e0: 0000 0000 7d0b 6405 7c0a 7c0b 7c05 7400  ....}.d.|.|.|.t.
+000004f0: 0000 0000 0000 0000 6a0b 0000 0000 0000  ........j.......
+00000500: 0000 0000 0000 0000 0000 0000 7c09 ab01  ............|...
+00000510: 0000 0000 0000 6406 9c05 7d0c 7c0c 5300  ......d...}.|.S.
+00000520: 2907 4ee9 0500 0000 e901 0000 00e9 0200  ).N.............
+00000530: 0000 7202 0000 007a 0d47 6f6c 6465 6e20  ..r....z.Golden 
+00000540: 5365 6172 6368 2905 da0b 6d65 7468 6f64  Search)...method
+00000550: 5f6e 616d 65da 0478 6f70 74da 0466 6d69  _name..xopt..fmi
+00000560: 6eda 086e 756d 5f69 7465 72da 0470 6174  n..num_iter..pat
+00000570: 6829 06da 026e 70da 0473 7172 74da 066c  h)...np..sqrt..l
+00000580: 696e 616c 67da 046e 6f72 6dda 0661 7070  inalg..norm..app
+00000590: 656e 6472 0600 0000 290d 7209 0000 0072  endr....).r....r
+000005a0: 0c00 0000 720e 0000 00da 0374 6f6c da03  ....r......tol..
+000005b0: 7068 6972 1c00 0000 da04 6265 7461 da07  phir......beta..
+000005c0: 616c 7068 615f 65da 0761 6c70 6861 5f64  alpha_e..alpha_d
+000005d0: 721d 0000 00da 0561 6c70 6861 721b 0000  r......alphar...
+000005e0: 00da 0672 6573 756c 7473 0d00 0000 2020  ...results....  
+000005f0: 2020 2020 2020 2020 2020 2072 1200 0000             r....
+00000600: da0e 676f 6c64 656e 5f73 6563 7469 6f6e  ..golden_section
+00000610: 722a 0000 0015 0000 0073 1201 0000 8000  r*.......s......
+00000620: dc0b 0d8f 3789 3790 318b 3a90 6189 3c98  ....7.7.1.:.a.<.
+00000630: 11d1 0a1a 8043 d80f 1080 48dc 0b0d 8f39  .....C....H....9
+00000640: 8939 8f3e 893e 9821 9841 9923 d30b 1e80  .9.>.>.!.A.#....
+00000650: 44d8 0e0f 9031 9073 9137 9844 912e d10e  D....1.s.7.D....
+00000660: 2080 47d8 0e0f 9033 9074 9138 896e 8047   .G....3.t.8.n.G
+00000670: d80b 0d80 44e0 0a0e 9013 8a2a d90b 0c88  ....D......*....
+00000680: 578b 3a99 0198 279b 0ad2 0b22 d810 1789  W.:...'...."....
+00000690: 41e0 1017 8841 e40f 118f 7989 798f 7e89  A....A....y.y.~.
+000006a0: 7e98 61a0 0199 63d3 0f22 8804 d812 1390  ~.a...c.."......
+000006b0: 7198 3391 77a0 0491 6ed1 1224 8807 d812  q.3.w...n..$....
+000006c0: 1390 7398 3491 7891 2e88 07e0 0810 9041  ..s.4.x........A
+000006d0: 890d 8808 d808 0c8f 0b89 0b90 5190 7191  ............Q.q.
+000006e0: 5398 2191 47d4 081c f017 000b 0f90 138b  S.!.G...........
+000006f0: 2af0 1a00 0e0f 9011 8955 9061 894b 8045  *........U.a.K.E
+00000700: d90b 0c88 558b 3880 44f0 0600 1827 d810  ....U.8.D....'..
+00000710: 15d8 1014 d814 1cdc 1012 9708 9108 9814  ................
+00000720: 930e f10b 060e 0680 46f0 0e00 0c12 804d  ........F......M
+00000730: 7214 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00000740: 0000 0700 0000 0300 0000 f398 0000 0087  ................
+00000750: 0087 0187 0297 0088 0288 0088 0166 0364  .............f.d
+00000760: 0184 087d 0474 0100 0000 0000 0000 007c  ...}.t.........|
+00000770: 047c 03ac 02ab 0200 0000 0000 005c 0200  .|...........\..
+00000780: 007d 057d 0674 0300 0000 0000 0000 006a  .}.}.t.........j
+00000790: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+000007a0: 0000 007c 047c 057c 0666 0264 03ac 04ab  ...|.|.|.f.d....
+000007b0: 0300 0000 0000 007d 0789 017c 0789 027a  .......}...|...z
+000007c0: 0500 007a 0000 007d 0864 057c 077c 0802  ...z...}.d.|.|..
+000007d0: 0089 007c 08ab 0100 0000 0000 0064 0689  ...|.........d..
+000007e0: 0064 079c 0653 0029 084e 6301 0000 0000  .d...S.).Nc.....
+000007f0: 0000 0000 0000 0005 0000 0013 0000 00f3  ................
+00000800: 2000 0000 9503 9700 0200 8902 8903 7c00   .............|.
+00000810: 8901 7a05 0000 7a00 0000 ab01 0000 0000  ..z...z.........
+00000820: 0000 5300 7204 0000 00a9 0029 0472 2800  ..S.r......).r(.
+00000830: 0000 da01 6472 0900 0000 720a 0000 0073  ....dr....r....s
+00000840: 0400 0000 2080 8080 7212 0000 00fa 083c  .... ...r......<
+00000850: 6c61 6d62 6461 3e7a 1d6c 696e 655f 7365  lambda>z.line_se
+00000860: 6172 6368 2e3c 6c6f 6361 6c73 3e2e 3c6c  arch.<locals>.<l
+00000870: 616d 6264 613e 3800 0000 7314 0000 00f8  ambda>8...s.....
+00000880: 8000 9961 a001 a045 a841 a149 a10d d31e  ...a...E.A.I....
+00000890: 2e80 0072 1400 0000 2901 720b 0000 00e7  ...r....).r.....
+000008a0: f168 e388 b5f8 e43e 2902 da05 6272 6163  .h.....>)...brac
+000008b0: 6b72 2300 0000 7a0b 4c69 6e65 2053 6561  kr#...z.Line Sea
+000008c0: 7263 6872 1700 0000 2906 7219 0000 0072  rchr....).r....r
+000008d0: 2800 0000 721a 0000 0072 1b00 0000 721c  (...r....r....r.
+000008e0: 0000 00da 0866 756e 6374 696f 6e29 0372  .....function).r
+000008f0: 1300 0000 da03 6f70 74da 0667 6f6c 6465  ......opt..golde
+00000900: 6e29 0972 0900 0000 720a 0000 0072 2e00  n).r....r....r..
+00000910: 0000 da09 7374 6570 5f73 697a 65da 096f  ....step_size..o
+00000920: 626a 6563 7469 7665 720c 0000 0072 0e00  bjectiver....r..
+00000930: 0000 7228 0000 00da 0578 5f6f 7074 7309  ..r(.....x_opts.
+00000940: 0000 0060 6060 2020 2020 2020 7212 0000  ...```      r...
+00000950: 00da 0b6c 696e 655f 7365 6172 6368 7238  ...line_searchr8
+00000960: 0000 0037 0000 0073 5b00 0000 fa80 00dd  ...7...s[.......
+00000970: 102e 8049 dc0b 1a98 39a8 09d4 0b32 8144  ...I....9....2.D
+00000980: 8041 8071 dc0c 0f8f 4a89 4a90 79a8 11a8  .A.q....J.J.y...
+00000990: 41a8 06b0 44d4 0c39 8045 d80c 0d90 0598  A...D..9.E......
+000009a0: 0191 0989 4d80 45e0 1724 d811 16d8 1015  ....M.E..$......
+000009b0: d910 1190 2593 08d8 1415 d814 15f1 0d07  ....%...........
+000009c0: 0c06 f000 0705 0672 1400 0000 2902 6700  .......r....).g.
+000009d0: 0000 0000 0000 00e7 7b14 ae47 e17a 843f  ........{..G.z.?
+000009e0: 2901 7230 0000 0029 0172 3900 0000 2909  ).r0...).r9...).
+000009f0: da09 6a61 782e 6e75 6d70 79da 056e 756d  ..jax.numpy..num
+00000a00: 7079 7205 0000 0072 1300 0000 722a 0000  pyr....r....r*..
+00000a10: 00da 0e73 6369 7079 2e6f 7074 696d 697a  ...scipy.optimiz
+00000a20: 65da 086f 7074 696d 697a 6572 3300 0000  e..optimizer3...
+00000a30: 7238 0000 0072 2d00 0000 7214 0000 0072  r8...r-...r....r
+00000a40: 1200 0000 fa08 3c6d 6f64 756c 653e 723e  ......<module>r>
+00000a50: 0000 0001 0000 0073 1d00 0000 f003 0101  .......s........
+00000a60: 01dd 0017 f304 1001 20f3 241f 0112 f542  ........ .$....B
+00000a70: 0100 011d f402 0c01 0672 1400 0000       .........r....
```

### Comparing `optymus-0.1.1/optymus/search/_search.py` & `optymus-0.1.2/optymus/utils/_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-import numpy as np
+import jax.numpy as jnp
 
-def bracket_minimum(f, x=0, s=0.01):
-    a, ya = x, f(x)
-    b, yb = a + s, f(a + s)
-    if yb > ya:
-        a, b = b, a
-        ya, yb = yb, ya
-        s = -s
-    while True:
-        c, yc = b + s, f(b + s)
-        if yc > yb:
-            return (a, c) if np.all(a < c) else (c, a)
-        a, ya, b, yb = b, yb, c, yc
+def bracket_minimum(f, x=0.0, s=0.01):
+  a = jnp.array(x)  # Ensure x is a JAX array
+  ya = f(a)
+  b = a + s
+  yb = f(b)
+
+  if yb > ya:
+    a, b = b, a
+    ya, yb = yb, ya
+    s = -s
+
+  while True:
+    c = b + s
+    yc = f(c)
+    if yc > yb:
+      return jnp.where(a < c, jnp.stack((a, c)), jnp.stack((c, a)))  # Use jnp.where for condition
+    a, ya, b, yb = b, yb, c, yc
 
 def golden_section(f, a, b, tol=1e-5):
     phi = (np.sqrt(5)-1)/2
     num_iter = 0
     beta = np.linalg.norm(b-a)
     alpha_e = a + (1 - phi)*beta
     alpha_d = a + (phi*beta)
```

### Comparing `optymus-0.1.1/optymus/utils/__pycache__/_optim_methods.cpython-311.pyc` & `optymus-0.1.2/optymus/utils/__pycache__/_optim_methods.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `optymus-0.1.1/PKG-INFO` & `optymus-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optymus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Optimization Methods Library
 Author: Kleyton da Costa
 Maintainer: Kleyton da Costa
 Maintainer-email: kleyton.vsc@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,82 +14,85 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autograd (>=1.6.2)
 Requires-Dist: seaborn (>=0.11.2)
 Requires-Dist: tqdm (>=4.64.1)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
-<img src="logo.png" width="400">
+<img src="logo.svg" width="400">
 </h1>
 
 [![PyPI](https://img.shields.io/pypi/v/optymus)](https://pypi.org/project/optymus/)
 [![GitHub](https://img.shields.io/github/license/kleyt0n/optymus)](https://github.com/kleyt0n/optymus/blob/master/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/optymus/badge/?version=latest)](https://optymus.readthedocs.io/en/latest/?badge=latest)
 
-Welcome to _optymus_, the Optimization Methods Library for Python! This library provides a comprehensive collection of optimization methods, both with and without constraints, implemented in the Python programming language.
+> Check the [Optimization in Deep Learning and Engineering](https://quantsci.org/odle-book) material.
 
-## Table of Contents
+> Optymus is part of [quantsci](https://quantsci.org) project.
 
-- [Introduction](#introduction)
-- [Getting Started](#getting-started)
-- [Content](#content)
-- [Contributions](#contributions)
-- [License](#license)
+This library provides a comprehensive collection of optimization methods, both with and without constraints. The main goal is provide a simple structure to improve research and development in optimization problems.
 
-## Introduction
+## Implemented Methods
+
+| Method | Description |
+| --- | --- |
+| bfgs | Broyden-Fletcher-Goldfarb-Shanno (BFGS) |
+| steepdesc | Steepest Descent |
+| newton_raphson | Newton-Raphson Method |
+| powell | Powell's Method |
+|fletcher_reeves | Fletcher-Reeves |
 
-_optymus_ is designed to empower users with a versatile set of optimization tools, facilitating the search for optimal solutions in various problem domains. This library covers a range of optimization methods, making it suitable for diverse applications in computer science and engineering.
 
 ## Getting Started
 
 To begin using _optymus_, follow these steps:
 
 1. **Install optymus:**
    ```bash
-   pip install --upgrade optymus
+   pip install optymus
    ```
 
 2. **Explore the Documentation:**
    Visit the [official documentation](https://optymus-docs.readthedocs.com) to understand the available optimization methods and how to use them effectively.
 
 3. **Get Started:**
    ```python
-   from optymus.minimize import Optimizer
+   from optymus.optim import Optimizer
+   from optymus.utils import mccormick_function
    
    import numpy as np
-   f = lambda x: x[0]**[2]-3*x[0]*x[1]+4*x[1]**2+x[0]-x[1]
-   grad = lambda x: np.array([2*x[0]-3*x[1]+1, -3*x[0]+8*x[1]-1])
-   hess = lambda x: np.array([[2, -3], [-3, 8]])
+
+   f = mccormick_function()
    initial_point = np.array([2, 2])
 
-   optimizer = Optimizer(f_obj=f,
-                        x0=initial_point,
-                        grad=grad,
-                        hess=hess,
-                        method='bfgs')
-   
-   optimizer.report()
+   opt = Optimizer(f_obj=f,
+                   x0=initial_point,
+                   method='bfgs')
 
-   optimizer.plot()
-   ```
+   opt.report()
 
-## Content
+   opt.plot()
+   ```
 
-_optymus_ includes a rich set of optimization methods, such as:
+Refer to the documentation for detailed information on each method and its application.
 
-- Unconstrained Optimization Methods
-- Constrained Optimization Methods
-- Global Optimization
-- Gradient Descent
-- Evolutionary Algorithms
+## Implement your own method an compare with the implemented ones
 
-Refer to the documentation for detailed information on each method and its application.
+We are working to implement a simple way to add your own optimization method. 
 
 ## Contributions
 
-Contributions to Optymus are highly appreciated! If you have additional optimization methods, improvements, or bug fixes, please submit a pull request following the [contribution guidelines](CONTRIBUTING.md).
-
-## License
+Contributions to Optymus are highly appreciated. If you have additional optimization methods, improvements, or bug fixes, please submit a pull request following the [contribution guidelines](CONTRIBUTING.md).
 
-Optymus is licensed under the [MIT License](LICENSE), allowing you to use, modify, and distribute the library for both commercial and non-commercial purposes.
+## Cite
 
-Start optimizing with Optymus and unlock the potential for finding optimal solutions in your Python projects!
+If you use Optymus in your research, please consider citing the library using the following BibTeX entry:
 
+```bibtex
+@misc{optymus2024,
+  author = {Costa, Kleyton and Menezes, Ivan},
+  title = {Optymus: Optimization Methods Library for Python},
+  year = {2024},
+  note = {GitHub Repository},
+  url = {https://github.com/quantsci/optymus}
+}
+```
```

