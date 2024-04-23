# Comparing `tmp/torch_cfd-0.0.1.tar.gz` & `tmp/torch_cfd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_cfd-0.0.1.tar", last modified: Fri Apr 19 19:39:52 2024, max compression
+gzip compressed data, was "torch_cfd-0.0.2.tar", last modified: Tue Apr 23 16:11:02 2024, max compression
```

## Comparing `torch_cfd-0.0.1.tar` & `torch_cfd-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwx---   0 sch59     (1004) sch59     (1006)        0 2024-04-19 19:39:52.048585 torch_cfd-0.0.1/
--rw-rw----   0 sch59     (1004) sch59     (1006)    11357 2024-04-18 15:47:00.000000 torch_cfd-0.0.1/LICENSE
--rw-r--r--   0 sch59     (1004) sch59     (1006)      653 2024-04-19 19:39:52.048585 torch_cfd-0.0.1/PKG-INFO
--rw-rw----   0 sch59     (1004) sch59     (1006)      577 2024-04-19 19:03:35.000000 torch_cfd-0.0.1/README.md
--rw-rw----   0 sch59     (1004) sch59     (1006)       38 2024-04-19 19:39:52.048585 torch_cfd-0.0.1/setup.cfg
--rw-rw----   0 sch59     (1004) sch59     (1006)      832 2024-04-19 19:39:46.000000 torch_cfd-0.0.1/setup.py
-drwxrwx---   0 sch59     (1004) sch59     (1006)        0 2024-04-19 19:39:52.048585 torch_cfd-0.0.1/torch_cfd/
--rw-rw----   0 sch59     (1004) sch59     (1006)        0 2024-04-18 14:13:53.000000 torch_cfd-0.0.1/torch_cfd/__init__.py
--rw-rw----   0 sch59     (1004) sch59     (1006)     9214 2024-04-19 17:12:32.000000 torch_cfd-0.0.1/torch_cfd/equations.py
--rw-rw----   0 sch59     (1004) sch59     (1006)    11032 2024-04-19 17:12:32.000000 torch_cfd-0.0.1/torch_cfd/fast_diagonalization.py
--rw-rw----   0 sch59     (1004) sch59     (1006)     9103 2024-04-19 17:12:32.000000 torch_cfd-0.0.1/torch_cfd/finite_differences.py
--rw-rw----   0 sch59     (1004) sch59     (1006)     1698 2024-04-19 17:27:23.000000 torch_cfd-0.0.1/torch_cfd/forcings.py
--rw-rw----   0 sch59     (1004) sch59     (1006)    41005 2024-04-19 17:12:32.000000 torch_cfd-0.0.1/torch_cfd/grids.py
--rw-rw----   0 sch59     (1004) sch59     (1006)     7882 2024-04-19 17:12:32.000000 torch_cfd-0.0.1/torch_cfd/initial_conditions.py
--rw-rw----   0 sch59     (1004) sch59     (1006)     4072 2024-04-19 17:12:32.000000 torch_cfd-0.0.1/torch_cfd/tensor_utils.py
-drwxrwx---   0 sch59     (1004) sch59     (1006)        0 2024-04-19 19:39:52.048585 torch_cfd-0.0.1/torch_cfd.egg-info/
--rw-r--r--   0 sch59     (1004) sch59     (1006)      653 2024-04-19 19:39:52.000000 torch_cfd-0.0.1/torch_cfd.egg-info/PKG-INFO
--rw-rw----   0 sch59     (1004) sch59     (1006)      400 2024-04-19 19:39:52.000000 torch_cfd-0.0.1/torch_cfd.egg-info/SOURCES.txt
--rw-rw----   0 sch59     (1004) sch59     (1006)        1 2024-04-19 19:39:52.000000 torch_cfd-0.0.1/torch_cfd.egg-info/dependency_links.txt
--rw-rw----   0 sch59     (1004) sch59     (1006)       19 2024-04-19 19:39:52.000000 torch_cfd-0.0.1/torch_cfd.egg-info/requires.txt
--rw-rw----   0 sch59     (1004) sch59     (1006)       10 2024-04-19 19:39:52.000000 torch_cfd-0.0.1/torch_cfd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 16:03:17.000000 torch_cfd-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 16:03:17.000000 torch_cfd-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 16:10:57.000000 torch_cfd-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/torch_cfd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/fast_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/finite_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-23 16:03:18.000000 torch_cfd-0.0.2/torch_cfd/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:02.903053 torch_cfd-0.0.2/torch_cfd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:02.000000 torch_cfd-0.0.2/torch_cfd.egg-info/top_level.txt
```

### Comparing `torch_cfd-0.0.1/LICENSE` & `torch_cfd-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/PKG-INFO` & `torch_cfd-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

### Comparing `torch_cfd-0.0.1/setup.py` & `torch_cfd-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'torch-cfd',
   packages=find_packages(include=['torch_cfd', 'torch_cfd.*']),
-  version = '0.0.1',
+  version='0.0.2',
   license='Apache-2.0',
   description = 'PyTorch CFD',
   long_description='PyTorch Computational Fluid Dynamics Library',
   long_description_content_type="text/markdown",
   author = 'Shuhao Cao',
   author_email = 'scao.math@gmail.com',
   url = 'https://github.com/scaomath/torch-cfd',
```

### Comparing `torch_cfd-0.0.1/torch_cfd/equations.py` & `torch_cfd-0.0.2/torch_cfd/equations.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 from typing import Callable, Dict, Optional
 
 import torch
 import torch.nn as nn
 import torch.fft as fft
 from . import grids
+from tqdm.auto import tqdm
 
+TQDM_ITERS = 100
 
 Array = torch.Tensor
 Grid = grids.Grid
 
 
 class ImplicitExplicitODE(nn.Module):
     """Describes a set of ODEs with implicit & explicit terms.
@@ -55,14 +57,101 @@
         x: Array,
         step_size: float,
     ):
         """Solves `y - step_size * implicit_terms(y) = x` for y."""
         raise NotImplementedError
 
 
+def low_storage_runge_kutta_crank_nicolson(
+    u: torch.Tensor,
+    dt: float,
+    params: Dict,
+    equation: ImplicitExplicitODE,
+) -> Array:
+    """
+    ported from jax functional programming to be tensor2tensor
+    Time stepping via "low-storage" Runge-Kutta and Crank-Nicolson steps.
+
+    These scheme are second order accurate for the implicit terms, but potentially
+    higher order accurate for the explicit terms. This seems to be a favorable
+    tradeoff when the explicit terms dominate, e.g., for modeling turbulent
+    fluids.
+
+    Per Canuto: "[these methods] have been widely used for the time-discretization
+    in applications of spectral methods."
+
+    Args:
+      alphas: alpha coefficients.
+      betas: beta coefficients.
+      gammas: gamma coefficients.
+      equation.F: explicit terms (convection, rhs, drag).
+      equation.G: implicit terms (diffusion).
+      equation.implicit_solve: implicit solver, when evaluates at an input (B, n, n), outputs (B, n, n).
+      dt: time step.
+
+    Input: w^{t_i} (B, n, n)
+    Returns: w^{t_{i+1}} (B, n, n)
+
+    Reference:
+      Canuto, C., Yousuff Hussaini, M., Quarteroni, A. & Zang, T. A.
+      Spectral Methods: Evolution to Complex Geometries and Applications to
+      Fluid Dynamics. (Springer Berlin Heidelberg, 2007).
+      https://doi.org/10.1007/978-3-540-30728-0 (Appendix D.3)
+    """
+    dt = dt
+    alphas = params["alphas"]
+    betas = params["betas"]
+    gammas = params["gammas"]
+    F = equation.explicit_terms
+    G = equation.implicit_terms
+    G_inv = equation.implicit_solve
+
+    if len(alphas) - 1 != len(betas) != len(gammas):
+        raise ValueError("number of RK coefficients does not match")
+
+    h = 0
+    for k in range(len(betas)):
+        h = F(u) + betas[k] * h
+        mu = 0.5 * dt * (alphas[k + 1] - alphas[k])
+        u = G_inv(u + gammas[k] * dt * h + mu * G(u), mu)
+    return u
+
+
+def crank_nicolson_rk4(
+    u: Array,
+    dt: float,
+    equation: ImplicitExplicitODE,
+) -> Array:
+    """Time stepping via Crank-Nicolson and RK4 ("Carpenter-Kennedy")."""
+    params = dict(
+        alphas=[
+            0,
+            0.1496590219993,
+            0.3704009573644,
+            0.6222557631345,
+            0.9582821306748,
+            1,
+        ],
+        betas=[0, -0.4178904745, -1.192151694643, -1.697784692471, -1.514183444257],
+        gammas=[
+            0.1496590219993,
+            0.3792103129999,
+            0.8229550293869,
+            0.6994504559488,
+            0.1530572479681,
+        ],
+    )
+    return low_storage_runge_kutta_crank_nicolson(
+        u,
+        dt=dt,
+        params=params,
+        equation=equation,
+    )
+
+
 class NavierStokes2D(nn.Module):
     """Breaks the Navier-Stokes equation into implicit and explicit parts.
 
     Implicit parts are the linear terms and explicit parts are the non-linear
     terms.
 
     Attributes:
@@ -76,21 +165,23 @@
     def __init__(
         self,
         viscosity: float,
         grid: Grid,
         drag: float = 0.0,
         smooth: bool = True,
         forcing_fn: Optional[Callable] = None,
+        solver: Optional[Callable] = crank_nicolson_rk4,
     ):
         super().__init__()
         self.viscosity = viscosity
         self.grid = grid
         self.drag = drag
         self.smooth = smooth
         self.forcing_fn = forcing_fn
+        self.solver = solver
         self._initialize()
 
     def _initialize(self):
         kx, ky = self.grid.rfft_mesh()
         self.register_buffer("kx", kx)
         self.register_buffer("ky", ky)
         laplace = (torch.pi * 2j) ** 2 * (self.kx**2 + self.ky**2)
@@ -168,113 +259,67 @@
         if self.forcing_fn is not None:
             fx, fy = self.forcing_fn(self.grid, (vx, vy))
             fx_hat, fy_hat = fft.rfft2(fx.data), fft.rfft2(fy.data)
             terms += self.spectral_curl_2d((self.kx, self.ky), (fx_hat, fy_hat))
 
         return terms
 
-    def explicit_terms(self):
-        return lambda vort_hat: self._explicit_terms(vort_hat)
+    def explicit_terms(self, vort_hat):
+        return self._explicit_terms(vort_hat)
 
-    def implicit_terms(self):
-        return lambda vort_hat: self.linear_term * vort_hat
+    def implicit_terms(self, vort_hat):
+        return self.linear_term * vort_hat
 
-    def implicit_solve(self, time_step):
-        return lambda vort_hat: 1 / (1 - time_step * self.linear_term) * vort_hat
+    def implicit_solve(self, vort_hat, dt):
+        return 1 / (1 - dt * self.linear_term) * vort_hat
 
-    def step(self, time_step):
+    def get_trajectory(
+        self,
+        w0: Array,
+        dt: float,
+        time_steps: int,
+        record_every_steps=1,
+        pbar=False,
+        pbar_desc="",
+        require_grad=False,
+    ):
         """
-        this is for tests
+        vorticity stacked in the time dimension
         """
-        return lambda w: self.explicit_terms()(w) + self.implicit_solve(
-            time_step=time_step
-        )(w)
+        w_all = []
+        v_all = []
+        dwdt_all = []
+        w = w0
+        update_iters = time_steps // TQDM_ITERS
+        with tqdm(total=time_steps) as pbar:
+            for t in range(time_steps):
+                w, dwdt = self.forward(w, dt=dt)
+                w.requires_grad_(require_grad)
+                dwdt.requires_grad_(require_grad)
+
+                if t % update_iters == 0:
+                    pbar.set_description(pbar_desc)
+                    pbar.update(update_iters)
+
+                if t % record_every_steps == 0:
+                    w_ = w.detach().clone()
+                    dwdt_ = dwdt.detach().clone()
+                    v = self.vorticity_to_velocity(self.grid, w_)
+                    v = torch.stack(v, dim=0)
+                    w_all.append(w_)
+                    v_all.append(v)
+                    dwdt_all.append(dwdt_)
+        result = {
+            var_name: torch.stack(var, dim=0)
+            for var_name, var in zip(
+                ["vorticity", "velocity", "vort_t"], [w_all, v_all, dwdt_all]
+            )
+        }
+        return result
 
-    def forward(self, vort_hat, dt):
-        return crank_nicolson_rk4(self, vort_hat, dt)
-
-
-def low_storage_runge_kutta_crank_nicolson(
-    u: torch.Tensor,
-    params: Dict,
-    equation: ImplicitExplicitODE,
-    time_step: float,
-) -> Array:
-    """
-    ported from jax functional programming to be tensor2tensor
-    Time stepping via "low-storage" Runge-Kutta and Crank-Nicolson steps.
-
-    These scheme are second order accurate for the implicit terms, but potentially
-    higher order accurate for the explicit terms. This seems to be a favorable
-    tradeoff when the explicit terms dominate, e.g., for modeling turbulent
-    fluids.
-
-    Per Canuto: "[these methods] have been widely used for the time-discretization
-    in applications of spectral methods."
-
-    Args:
-      alphas: alpha coefficients.
-      betas: beta coefficients.
-      gammas: gamma coefficients.
-      equation.F: explicit terms (convection, rhs, drag).
-      equation.G: implicit terms (diffusion).
-      equation.implicit_solve: implicit solver, when evaluates at an input (B, n, n), outputs (B, n, n).
-      time_step: time step.
-
-    Input: w^{t_i} (B, n, n)
-    Returns: w^{t_{i+1}} (B, n, n)
-
-    Reference:
-      Canuto, C., Yousuff Hussaini, M., Quarteroni, A. & Zang, T. A.
-      Spectral Methods: Evolution to Complex Geometries and Applications to
-      Fluid Dynamics. (Springer Berlin Heidelberg, 2007).
-      https://doi.org/10.1007/978-3-540-30728-0 (Appendix D.3)
-    """
-    dt = time_step
-    alphas = params["alphas"]
-    betas = params["betas"]
-    gammas = params["gammas"]
-    F = equation.explicit_terms()
-    G = equation.implicit_terms()
-    G_inv = equation.implicit_solve
-
-    if len(alphas) - 1 != len(betas) != len(gammas):
-        raise ValueError("number of RK coefficients does not match")
-
-    h = 0
-    for k in range(len(betas)):
-        h = F(u) + betas[k] * h
-        mu = 0.5 * dt * (alphas[k + 1] - alphas[k])
-        u = G_inv(mu)(u + gammas[k] * dt * h + mu * G(u))
-    return u
+    def step(self, *args, **kwargs):
+        return self.forward(*args, **kwargs)
 
-
-def crank_nicolson_rk4(
-    equation: ImplicitExplicitODE,
-    u: Array,
-    time_step: float,
-) -> Array:
-    """Time stepping via Crank-Nicolson and RK4 ("Carpenter-Kennedy")."""
-    params = dict(
-        alphas=[
-            0,
-            0.1496590219993,
-            0.3704009573644,
-            0.6222557631345,
-            0.9582821306748,
-            1,
-        ],
-        betas=[0, -0.4178904745, -1.192151694643, -1.697784692471, -1.514183444257],
-        gammas=[
-            0.1496590219993,
-            0.3792103129999,
-            0.8229550293869,
-            0.6994504559488,
-            0.1530572479681,
-        ],
-    )
-    return low_storage_runge_kutta_crank_nicolson(
-        u,
-        params=params,
-        equation=equation,
-        time_step=time_step,
-    )
+    def forward(self, vort_hat, dt):
+        vort_hat_new = self.solver(vort_hat, dt, self)
+        dvortdt_hat = 1 / dt * (vort_hat_new - vort_hat)
+        return vort_hat_new, dvortdt_hat
```

### Comparing `torch_cfd-0.0.1/torch_cfd/fast_diagonalization.py` & `torch_cfd-0.0.2/torch_cfd/fast_diagonalization.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/torch_cfd/finite_differences.py` & `torch_cfd-0.0.2/torch_cfd/finite_differences.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/torch_cfd/forcings.py` & `torch_cfd-0.0.2/torch_cfd/forcings.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/torch_cfd/grids.py` & `torch_cfd-0.0.2/torch_cfd/grids.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/torch_cfd/initial_conditions.py` & `torch_cfd-0.0.2/torch_cfd/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/torch_cfd/tensor_utils.py` & `torch_cfd-0.0.2/torch_cfd/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.1/torch_cfd.egg-info/PKG-INFO` & `torch_cfd-0.0.2/torch_cfd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

