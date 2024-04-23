# Comparing `tmp/delicatessen-2.1.tar.gz` & `tmp/delicatessen-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delicatessen-2.1.tar", last modified: Sat Mar 16 15:47:55 2024, max compression
+gzip compressed data, was "delicatessen-2.2.tar", last modified: Tue Apr 23 15:00:25 2024, max compression
```

## Comparing `delicatessen-2.1.tar` & `delicatessen-2.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 15:47:55.472825 delicatessen-2.1/
--rw-rw-rw-   0        0        0     1087 2021-10-29 16:28:15.000000 delicatessen-2.1/LICENSE
--rw-rw-rw-   0        0        0     5572 2024-03-16 15:47:55.472825 delicatessen-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4227 2024-03-16 15:44:37.000000 delicatessen-2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 15:47:55.422432 delicatessen-2.1/delicatessen/
--rw-rw-rw-   0        0        0      547 2022-01-18 20:28:36.000000 delicatessen-2.1/delicatessen/__init__.py
--rw-rw-rw-   0        0        0     3169 2023-01-12 21:09:35.000000 delicatessen-2.1/delicatessen/data.py
--rw-rw-rw-   0        0        0    28779 2023-10-16 18:41:28.000000 delicatessen-2.1/delicatessen/derivative.py
-drwxrwxrwx   0        0        0        0 2024-03-16 15:47:55.462434 delicatessen-2.1/delicatessen/estimating_equations/
--rw-rw-rw-   0        0        0      949 2024-03-16 15:44:37.000000 delicatessen-2.1/delicatessen/estimating_equations/__init__.py
--rw-rw-rw-   0        0        0    15736 2023-12-04 19:08:33.000000 delicatessen-2.1/delicatessen/estimating_equations/basic.py
--rw-rw-rw-   0        0        0    60546 2024-03-16 15:44:37.000000 delicatessen-2.1/delicatessen/estimating_equations/causal.py
--rw-rw-rw-   0        0        0    19850 2023-12-04 19:08:33.000000 delicatessen-2.1/delicatessen/estimating_equations/dose_response.py
--rw-rw-rw-   0        0        0     6575 2024-03-16 15:44:37.000000 delicatessen-2.1/delicatessen/estimating_equations/measurement.py
--rw-rw-rw-   0        0        0      824 2023-01-02 18:05:53.000000 delicatessen-2.1/delicatessen/estimating_equations/processing.py
--rw-rw-rw-   0        0        0    84752 2024-03-16 15:44:37.000000 delicatessen-2.1/delicatessen/estimating_equations/regression.py
--rw-rw-rw-   0        0        0    39523 2023-12-04 19:08:33.000000 delicatessen-2.1/delicatessen/estimating_equations/survival.py
--rw-rw-rw-   0        0        0    37594 2023-10-16 18:41:28.000000 delicatessen-2.1/delicatessen/mestimation.py
--rw-rw-rw-   0        0        0    32470 2024-03-16 15:44:37.000000 delicatessen-2.1/delicatessen/utilities.py
--rw-rw-rw-   0        0        0       21 2024-03-16 15:44:37.000000 delicatessen-2.1/delicatessen/version.py
-drwxrwxrwx   0        0        0        0 2024-03-16 15:47:55.443545 delicatessen-2.1/delicatessen.egg-info/
--rw-rw-rw-   0        0        0     5572 2024-03-16 15:47:55.000000 delicatessen-2.1/delicatessen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2024-03-16 15:47:55.000000 delicatessen-2.1/delicatessen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 15:47:55.000000 delicatessen-2.1/delicatessen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-03-16 15:47:55.000000 delicatessen-2.1/delicatessen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-16 15:47:55.000000 delicatessen-2.1/delicatessen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2024-03-16 15:47:55.472825 delicatessen-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1732 2024-03-16 15:44:38.000000 delicatessen-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:00:25.564225 delicatessen-2.2/
+-rw-rw-rw-   0        0        0     1087 2021-10-29 16:28:15.000000 delicatessen-2.2/LICENSE
+-rw-rw-rw-   0        0        0     5611 2024-04-23 15:00:25.564225 delicatessen-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4266 2024-04-23 14:58:46.000000 delicatessen-2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 15:00:25.502736 delicatessen-2.2/delicatessen/
+-rw-rw-rw-   0        0        0      587 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/__init__.py
+-rw-rw-rw-   0        0        0     4007 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/data.py
+-rw-rw-rw-   0        0        0    35079 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/derivative.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:00:25.564225 delicatessen-2.2/delicatessen/estimating_equations/
+-rw-rw-rw-   0        0        0      974 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/__init__.py
+-rw-rw-rw-   0        0        0    15039 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/basic.py
+-rw-rw-rw-   0        0        0    58960 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/causal.py
+-rw-rw-rw-   0        0        0    19303 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/dose_response.py
+-rw-rw-rw-   0        0        0    14192 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/measurement.py
+-rw-rw-rw-   0        0        0      824 2023-01-02 18:05:53.000000 delicatessen-2.2/delicatessen/estimating_equations/processing.py
+-rw-rw-rw-   0        0        0    85061 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/regression.py
+-rw-rw-rw-   0        0        0    38968 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/estimating_equations/survival.py
+-rw-rw-rw-   0        0        0    35395 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/mestimation.py
+-rw-rw-rw-   0        0        0    16050 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/sandwich.py
+-rw-rw-rw-   0        0        0    32593 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/utilities.py
+-rw-rw-rw-   0        0        0       21 2024-04-23 14:58:46.000000 delicatessen-2.2/delicatessen/version.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:00:25.535492 delicatessen-2.2/delicatessen.egg-info/
+-rw-rw-rw-   0        0        0     5611 2024-04-23 15:00:25.000000 delicatessen-2.2/delicatessen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2024-04-23 15:00:25.000000 delicatessen-2.2/delicatessen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 15:00:25.000000 delicatessen-2.2/delicatessen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-23 15:00:25.000000 delicatessen-2.2/delicatessen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-23 15:00:25.000000 delicatessen-2.2/delicatessen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2024-04-23 15:00:25.564225 delicatessen-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1732 2024-03-16 15:44:38.000000 delicatessen-2.2/setup.py
```

### Comparing `delicatessen-2.1/LICENSE` & `delicatessen-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `delicatessen-2.1/PKG-INFO` & `delicatessen-2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delicatessen
-Version: 2.1
+Version: 2.2
 Summary: Generalized M-Estimation
 Home-page: https://github.com/pzivich/Deli
 Author: Paul Zivich
 Author-email: zivich.5@gmail.com
 License: MIT
 Description: ![delicatessen](docs/images/delicatessen_header.png)
         
@@ -22,18 +22,18 @@
         **Citation**: Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-Estimation in Python.
         *arXiv:2203.11300* [stat.ME]
         
         
         ## M-Estimation and Estimating Equations
         
         Here, we provide a brief overview of M-estimation theory. For more detailed introductions to M-estimation, see Ross
-        et al. (2024) or Chapter 7 of Boos & Stefanski (2013). M-estimation is a generalization of likelihood-based methods.
-        *M-estimators* are solutions to estimating equations. To apply the M-estimator, we solve the estimating equations using
-        observed data. This is similar to other approaches, but the key advantage of M-Estimators is estimation of the variance
-        via the sandwich variance.
+        et al. (2024), Stefanski & Boos (2002), or Chapter 7 of Boos & Stefanski (2013). M-estimation is a generalization of
+        likelihood-based methods. *M-estimators* are solutions to estimating equations. To apply the M-estimator, we solve the
+        estimating equations using observed data. This is similar to other approaches, but the key advantage of M-Estimators is
+        variance estimation via the empirical sandwich variance estimator.
         
         While M-Estimation is a powerful tool, the derivatives and matrix algebra can quickly become unwieldy. This is where 
         `delicatessen` comes in. `delicatessen` takes estimating functions and data, and solves for the parameter estimates,
         computes the derivatives, and performs the matrix algebra calculations. Therefore, M-estimators can be more easily
         adopted without having to perform by-hand calculations. In other words, we can let the computer do the math for us.
         
         To further ease use, `delicatessen` also comes with a variety of built-in estimating equations. See
@@ -88,19 +88,19 @@
         at [delicatessen website](https://deli.readthedocs.io/en/latest/).
         
         ## References
         
         Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
         (pp. 297-337). Springer, New York, NY.
         
+        Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
+        
         Ross RK, Zivich PN, Stringer JS, & Cole SR. (2024). M-estimation for common epidemiological measures: introduction and
         applied examples. *International Journal of Epidemiology*, 53(2).
         
-        Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
-        
         Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-Estimation in Python.
         *arXiv preprint arXiv:2203.11300*.
         
 Keywords: m-estimation sandwich-variance estimating-equations
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `delicatessen-2.1/README.md` & `delicatessen-2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 **Citation**: Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-Estimation in Python.
 *arXiv:2203.11300* [stat.ME]
 
 
 ## M-Estimation and Estimating Equations
 
 Here, we provide a brief overview of M-estimation theory. For more detailed introductions to M-estimation, see Ross
-et al. (2024) or Chapter 7 of Boos & Stefanski (2013). M-estimation is a generalization of likelihood-based methods.
-*M-estimators* are solutions to estimating equations. To apply the M-estimator, we solve the estimating equations using
-observed data. This is similar to other approaches, but the key advantage of M-Estimators is estimation of the variance
-via the sandwich variance.
+et al. (2024), Stefanski & Boos (2002), or Chapter 7 of Boos & Stefanski (2013). M-estimation is a generalization of
+likelihood-based methods. *M-estimators* are solutions to estimating equations. To apply the M-estimator, we solve the
+estimating equations using observed data. This is similar to other approaches, but the key advantage of M-Estimators is
+variance estimation via the empirical sandwich variance estimator.
 
 While M-Estimation is a powerful tool, the derivatives and matrix algebra can quickly become unwieldy. This is where 
 `delicatessen` comes in. `delicatessen` takes estimating functions and data, and solves for the parameter estimates,
 computes the derivatives, and performs the matrix algebra calculations. Therefore, M-estimators can be more easily
 adopted without having to perform by-hand calculations. In other words, we can let the computer do the math for us.
 
 To further ease use, `delicatessen` also comes with a variety of built-in estimating equations. See
@@ -80,14 +80,14 @@
 at [delicatessen website](https://deli.readthedocs.io/en/latest/).
 
 ## References
 
 Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
 (pp. 297-337). Springer, New York, NY.
 
+Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
+
 Ross RK, Zivich PN, Stringer JS, & Cole SR. (2024). M-estimation for common epidemiological measures: introduction and
 applied examples. *International Journal of Epidemiology*, 53(2).
 
-Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
-
 Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-Estimation in Python.
 *arXiv preprint arXiv:2203.11300*.
```

### Comparing `delicatessen-2.1/delicatessen/__init__.py` & `delicatessen-2.2/delicatessen/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 $ python -m pip install delicatessen
 
 """
 
 from .version import __version__
 
 from .mestimation import MEstimator
+from .sandwich import compute_sandwich
```

### Comparing `delicatessen-2.1/delicatessen/data.py` & `delicatessen-2.2/delicatessen/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,21 @@
     From left to right, the columns in the array correspond to:
         * game - game number
         * ft_success - free throws made during game
         * ft_attempt - free throws attempted during game
 
     Returns
     -------
-    ndarray
+    array :
+        Returns a 24-by-2 NumPy array.
+
+    References
+    ----------
+    Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
+    (pp. 297-337). Springer, New York, NY.
     """
     d = np.array([[ 1,  4,  5],
                   [ 2,  5, 11],
                   [ 3,  5, 14],
                   [ 4,  5, 12],
                   [ 5,  2,  7],
                   [ 6,  7, 10],
@@ -39,25 +45,31 @@
                   [21, 10, 17],
                   [22,  1,  6],
                   [23,  3, 12], ])
     return d
 
 
 def load_inderjit():
-    """Load example data from Inderjit et al. (2002) on the dose-response of herbicide on perennial ryegrass growth
+    """Load example data from Inderjit et al. (2002) on the dose-response of herbicide on perennial ryegrass growth.
 
     Notes
     -----
     From left to right, the columns in the array correspond to:
         * response - ryegrass root length
         * dose - herbicide dose
 
     Returns
     -------
-    ndarray
+    array :
+        Returns a 24-by-2 NumPy array.
+
+    References
+    ----------
+    Inderjit, Streibig JC, & Olofsdotter M. (2002). Joint action of phenolic acid mixtures and its significance in
+    allelopathy research. *Physiologia Plantarum*, 114(3), 422-428.
     """
     d = np.array([[7.5800000,  0.00],
                   [8.0000000,  0.00],
                   [8.3285714,  0.00],
                   [7.2500000,  0.00],
                   [7.3750000,  0.00],
                   [7.9625000,  0.00],
@@ -79,22 +91,30 @@
                   [0.2500000, 30.00],
                   [0.2200000, 30.00],
                   [0.4400000, 30.00], ])
     return d
 
 
 def load_robust_regress(outlier=True):
-    """Load illustrative example for robust linear regression.
+    """Load illustrative example of robust linear regression published in Zivich et al. (2022).
 
     Parameters
     ----------
+    outlier : bool, optional
+        Whether to induce the outlier (``True``) or not (``False``).
 
     Returns
     -------
+    array :
+        Returns a 15-by-2 NumPy array.
 
+    References
+    ----------
+    Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-estimation in Python.
+    *arXiv:2203.11300*.
     """
     height = [168.519, 166.944, 164.327, 164.058, 166.212, 167.358,
               165.244, 169.352, 159.386, 166.953, 163.876,
               164.245, 165.061, 162.876, 164.185]
     weight = [67.634, 67.418, 63.394, 66.18, 65.573, 67.66, 64.592,
               68.4, 62.043, 67.093, 65.202, 64.328, 64.754,
               62.179, 64.716]
```

### Comparing `delicatessen-2.1/delicatessen/derivative.py` & `delicatessen-2.2/delicatessen/derivative.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,144 @@
 import numpy
 import numpy as np
 import scipy as sp
 from scipy.stats import norm
 
 
+def approx_differentiation(xk, f, epsilon=1e-9, method='capprox'):
+    r"""Numerical approximation to compute the gradient. This function implements numerical approximation methods for
+    derivatives generally (i.e., it provides the first-order forward, backward, and central difference approximations).
+
+    Note
+    ----
+    This functionality is only intended for use behind the scenes in ``delicatessen``. Numerical approximation is
+    implemented from scratch to offer backward and central difference approximations (SciPy's ``approx_fprime`` only
+    offers the forward difference).
+
+
+    The forward difference approximation is
+
+    .. math::
+
+        \frac{f(x + \epsilon) - f(x)}{\epsilon}
+
+    the backward difference approximation is
+
+    .. math::
+
+        \frac{f(x) - f(x - \epsilon)}{\epsilon}
+
+    and the central difference approximation is
+
+    .. math::
+
+        \frac{f(x + \epsilon) - f(x - \epsilon)}{2\epsilon}
+
+    Here, the numerical approximation is implemented by generating matrices for output from a function evaluated under
+    minor perturbations (determined by ``epsilon``) of each input argument. These matrices are then subtracted from
+    each other and then scaled by ``epsilon``.
+
+    Parameters
+    ----------
+    xk : ndarray, list, shape (n, )
+        Point(s) or coordinate vector to evaluate the gradient at.
+    f : callable
+        Function of which to estimate the gradient of.
+    epsilon : float, optional
+        Increment to perturb the points by to compute the gradient. This should be a small value
+    method : str, optional
+        Approximation to use to compute the gradient. Default is `capprox` which uses the central difference method.
+        One can also specify the forward difference (`fapprox`) or backward difference (`bapprox`) methods.
+
+    Returns
+    -------
+    numpy.array :
+        Corresponding array of the pairwise derivatives for all different input x values.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from delicatessen.derivative import approx_differentiation
+
+    To illustrate use, we will compute the derivative of the following function
+
+    .. math::
+
+        f(x) = x^2 - x^1 + sin(x + \sqrt{x})
+
+    >>> def f(x):
+    >>>     return x**2 - x + np.sin(x + np.sqrt(x))
+
+    If you work out the deriative by-hand, you will end up with the following
+
+    .. math::
+
+        2x - 1 + \left( \frac{1}{2 \sqrt{x}} + 1 \right) \cos(x + \sqrt{x})
+
+    Instead, we can use the central difference approximation to evaluate the derivative at a specific point. Here, we
+    will evaluate the derivative at :math:`x=1`
+
+    >>> dy = approx_differentiation(xk=[1, ], f=f)
+
+    which returns ``0.37578``, which is close to plugging in :math:`x=1` into the previous equation.
+
+    The derivative of a function with multiple inputs and multiple outputs can also be evaluated. Consider the following
+    example with three inputs and two outputs
+
+    >>> def f(x):
+    >>>     return [x[0]**2 - x[1], np.sin(np.sqrt(x[1]) + x[2]) + x[2]*(x[1]**2)]
+
+    >>> approx_differentiation(xk=[0.7, 1.2, -0.9], f=f, method='fapprox')
+    >>> approx_differentiation(xk=[0.7, 1.2, -0.9], f=f, method='bapprox')
+    >>> approx_differentiation(xk=[0.7, 1.2, -0.9], f=f, method='capprox')
+
+    which will return a 2-by-3 array of all the x-y pair derivatives at the given values. Here, the rows correspond to
+    the output and the columns correspond to the inputs. The approximation methods are forward, backward, and central.
+    """
+    # Setup parameters for call
+    xk = np.asarray(xk)                               # Convert inputs into NumPy array if not already
+    xp = xk.shape[0]                                  # Get the number of parameters in the input
+    shift = np.identity(n=xk.shape[0]) * epsilon      # Define the shift matrix for the partials
+
+    def generate_matrix(x_shift, f):
+        """Internal function to generate a matrix of the outputs under the parameter shifts, defined by x_shift"""
+        shift_matrix = []                             # Storage for matrices
+        for j in range(xp):                           # Looping over shift combinations
+            shift_matrix.append(f(x_shift[j, :]))     # ... compute output at shifted values
+        return np.asarray(shift_matrix)               # Return matrix under all shifts
+
+    # Computing the gradient using the corresponding method
+    if method == 'capprox':                           # Central difference
+        lower = (xk - shift)                          # ... defining lower shift
+        f0 = generate_matrix(x_shift=lower, f=f)      # ... output for lower shift
+        upper = (xk + shift)                          # ... defining upper shift
+        f1 = generate_matrix(x_shift=upper, f=f)      # ... output for upper shift
+        deriv = (f1 - f0).T / (2*epsilon)             # ... central difference approximation
+    elif method == 'bapprox':                         # Backward difference
+        lower = (xk - shift)                          # ... defining lower shift
+        f0 = generate_matrix(x_shift=lower, f=f)      # ... output for lower shift
+        f_eval = f(xk)                                # ... upper is held fixed
+        f1 = np.asarray([f_eval for i in range(xp)])  # ... stack upper into a matrix
+        deriv = (f1 - f0).T / epsilon                 # ... backward difference approximation
+    elif method == 'fapprox':                         # Forward difference
+        f_eval = f(xk)                                # ... lower is held fixed
+        f0 = np.asarray([f_eval for i in range(xp)])  # ... stack lower into a matrix
+        upper = (xk + shift)                          # ... defining upper shift
+        f1 = generate_matrix(x_shift=upper, f=f)      # ... output for upper shift
+        deriv = (f1 - f0).T / epsilon                 # ... forward difference approximation
+    else:                                             # Otherwise error
+        raise ValueError("Method chosen is not supported")
+
+    # Processing the final return based on parameter shape
+    if xp == 1:
+        return np.asarray([deriv, ])
+    else:
+        return deriv
+
+
 def auto_differentiation(xk, f):
     r"""Forward-mode automatic differentiation. Automatic differentiation offers a way to compute the exact derivative,
     rather than numerically approximated (i.e., the central difference method). Automatic differentiation iteratively
     applies the chain rule through recursive calls to evaluate the derivative.
 
     Note
     ----
@@ -18,17 +149,17 @@
     This is accomplished by the ``PrimalTangentPairs`` class, which is a special data type in ``delicatessen`` that
     stores pairs of the original evaluation and the corresponding derivative for a variety of different mathematical
     operations. This is what allows for the exact derivative calculation. The ``auto_differentiation`` function is
     a wrapper to access and use this class object as it is intended for derivative computations.
 
     Parameters
     ----------
-    xk: ndarray, list, shape (n, )
+    xk : ndarray, list, shape (n, )
         Point(s) or coordinate vector to evaluate the gradient at.
-    f: callable
+    f : callable
         Function of which to estimate the gradient of.
 
     Returns
     -------
     numpy.array :
         Corresponding array of the pairwise derivatives for all different input x values.
```

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/__init__.py` & `delicatessen-2.2/delicatessen/estimating_equations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .causal import (ee_ipw, ee_ipw_msm, ee_gformula, ee_aipw, ee_gestimation_snmm,
                      ee_mean_sensitivity_analysis)
 
 from .dose_response import (ee_4p_logistic, ee_3p_logistic, ee_2p_logistic,
                             ee_effective_dose_delta)
 
-from .measurement import (ee_rogan_gladen,
+from .measurement import (ee_rogan_gladen, ee_rogan_gladen_extended
                           )
 
 from .regression import (ee_regression, ee_glm, ee_mlogit,
                          ee_robust_regression,
                          ee_ridge_regression, ee_lasso_regression, ee_elasticnet_regression, ee_bridge_regression,
                          ee_additive_regression)
```

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/basic.py` & `delicatessen-2.2/delicatessen/estimating_equations/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,31 +16,26 @@
 def ee_mean(theta, y):
     r"""Estimating equation for the mean. The estimating equation for the mean is
 
     .. math::
 
         \sum_{i=1}^n (Y_i - \theta) = 0
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
         Theta in the case of the mean consists of a single value. Therefore, an initial value like the form of
         ``[0, ]`` should be provided.
     y : ndarray, list, vector
         1-dimensional vector of n observed values.
 
     Returns
     -------
     array :
-        Returns a 1-by-n NumPy array evaluated for the input ``theta`` and ``y``
+        Returns a 1-by-`n` NumPy array evaluated for the input ``theta`` and ``y``
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_mean`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.estimating_equations import ee_mean
@@ -85,42 +80,37 @@
 
         \sum_{i=1}^n f_k(Y_i - \theta) = 0
 
     where :math:`f_k(x)` is the corresponding robust loss function. Options for the loss function include: Huber,
     Tukey's biweight, Andrew's Sine, and Hampel. See ``robust_loss_function`` for further details on the loss
     functions for the robust mean.
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
         Theta in the case of the robust mean consists of a single value. Therefore, an initial value like the form of
         ``[0, ]`` is should be provided.
     y : ndarray, vector, list
         1-dimensional vector of n observed values.
     k : int, float
         Tuning or hyperparameter for the chosen loss function. Notice that the choice of hyperparameter depends on the
         loss function.
     loss : str, optional
-        Robust loss function to use. Default is 'huber'. Options include 'andrew', 'hampel', 'huber', 'tukey'.
+        Robust loss function to use. Default is ``'huber'``. Options include ``'andrew'``, ``'hampel'``, ``'tukey'``.
     lower : int, float, None, optional
-        Lower parameter for the 'hampel' loss function. This parameter does not impact the other loss functions.
+        Lower parameter for the Hampel loss function. This parameter does not impact the other loss functions.
         Default is ``None``.
     upper : int, float, None, optional
-        Upper parameter for the 'hampel' loss function. This parameter does not impact the other loss functions.
+        Upper parameter for the Hampel loss function. This parameter does not impact the other loss functions.
         Default is ``None``.
 
     Returns
     -------
     array :
-        Returns a 1-by-n NumPy array evaluated for the input theta and y
+        Returns a 1-by-`n` NumPy array evaluated for the input ``theta`` and ``y``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_mean_robust`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.estimating_equations import ee_mean_robust
@@ -182,33 +172,27 @@
             (Y_i - \theta_1)^2 - \theta_2
         \end{bmatrix}
         = 0
 
     Unlike ``ee_mean``, ``theta`` consists of 2 parameters. The output covariance matrix will also provide estimates
     for each of the ``theta`` values.
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
-
     Parameters
     ----------
     theta : ndarray, list, vector
         Theta in this case consists of two values. Therefore, initial values like the form of ``[0, 0]`` should be
         provided.
     y : ndarray, list, vector
         1-dimensional vector of n observed values. No missing data should be included (missing data may cause unexpected
         behavior when attempting to calculate the mean).
 
     Returns
     -------
     array :
-        Returns a 2-by-n NumPy array evaluated for the input theta and y
+        Returns a 2-by-`n` NumPy array evaluated for the input ``theta`` and ``y``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_mean_variance`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.estimating_equations import ee_mean_variance
@@ -269,20 +253,20 @@
     theta : ndarray, list, vector
         Theta in this case consists of one value. Therefore, initial values like the form of ``[0, ]`` should be
         provided.
     y : ndarray, list, vector
         1-dimensional vector of n observed values. No missing data should be included (missing data may cause unexpected
         behavior when attempting to calculate the mean).
     q : float
-        Percentile to calculate. Must be (0, 1)
+        Percentile to calculate. Must be :math:`(0, 1)`
 
     Returns
     -------
     array :
-        Returns a 1-by-n NumPy array evaluated for the input theta and y
+        Returns a 1-by-`n` NumPy array evaluated for the input ``theta`` and ``y``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_percentile`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.estimating_equations import ee_percentile
@@ -305,15 +289,15 @@
     Notice that we use a different solver, tolerance values, and parameters for numerically approximating the derivative
     here. These changes generally work better for the percentile since the estimating equation is non-smooth.
     Furthermore, optimization is hard when only a few observations (<100) are available.
 
     >>> estr.theta
 
     Then displays the estimated percentile / median. In this example, there is a difference between the closed form
-    solution (-0.07978) and M-Estimation (-0.06022).
+    solution (``-0.07978``) and M-Estimation (``-0.06022``).
 
     References
     ----------
     Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
     (pp. 297-337). Springer, New York, NY.
     """
     # Warning about the bread
@@ -348,32 +332,27 @@
 
     Note
     ----
     As the derivative of the estimating equation for the median is not defined at :math:`\hat{\theta}`, the bread (and
     sandwich) cannot be used to estimate the variance. This estimating equation is offered for completeness, but is not
     generally recommended for applications.
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
         Theta in this case consists of two values. Therefore, initial values like the form of ``[0, 0]`` are
         recommended.
     y : ndarray, list, vector
         1-dimensional vector of n observed values. No missing data should be included (missing data may cause unexpected
         behavior when attempting to calculate the positive mean deviation).
 
     Returns
     -------
     array :
-        Returns a 2-by-n NumPy array evaluated for the input theta and y
+        Returns a 2-by-`n` NumPy array evaluated for the input ``theta`` and ``y``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_positive_mean_deviation`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.estimating_equations import ee_positive_mean_deviation
```

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/causal.py` & `delicatessen-2.2/delicatessen/estimating_equations/causal.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,93 +9,84 @@
 
 
 #################################################################
 # Causal Inference (ATE) Estimating Equations
 
 
 def ee_gformula(theta, y, X, X1, X0=None, force_continuous=False):
-    r"""Estimating equations for the g-computation. The parameter of interest can either be the mean under a single
-    policy or plan of action, or the mean difference between two policies. This is accomplished by providing the
-    estimating equation the observed data (``X``, ``y``), and the same data under the actions (``X1`` and optionally
-    ``X0``).
+    r"""Estimating equations for the g-formula (or g-computation). The parameter of interest can either be the mean
+    under a single policy or plan of action, or the mean difference between two policies. This is accomplished by
+    providing the estimating equation the observed data (``X``, ``y``), and the same data under the actions (``X1``
+    and optionally ``X0``).
 
-    The outcome regression estimating equation is
+    The stack of estimating equations are
 
     .. math::
 
-        \sum_{i=1}^n \left\{ Y_i - g(X_i^T \beta) \right\} X_i = 0
+        \sum_{i=1}^n
+        \begin{bmatrix}
+            \left\{ g({X_i^*}^T \beta) - \theta_1 \right\} \\
+            \left\{ Y_i - g(X_i^T \beta) \right\} X_i
+        \end{bmatrix}
+        = 0
 
-    where :math:`g` indicates a transformation function. For linear regression, :math:`g` is the identity function.
-    Logistic regression uses the inverse-logit function. By default, `ee_gformula` detects whether `y` is all binary
+    where the first is the mean under the specified plan, with the plan setting the values of action :math:`A` (e.g.,
+    exposure, treatment, vaccination, etc.), and the second equation is the outcome regression model.
+    Here, :math:`g` indicates a transformation function. For linear regression, :math:`g` is the identity function.
+    Logistic regression uses the inverse-logit function. By default, ``ee_gformula`` detects whether `y` is all binary
     (zero or one), and applies logistic regression if that is evaluated to be true.
 
-    There are two variations on the parameter of interest. The first could be the mean under a plan, where the plan sets
-    the values of action :math:`A` (e.g., exposure, treatment, vaccination, etc.). The estimating equation for this
-    causal mean is
-
-    .. math::
-
-        \sum_{i=1}^n \left\{ g({X_i^*}^T \beta) - \theta_1 \right\} = 0
-
     Note
     ----
-    This variation includes :math:`1+b` parameters, where the first parameter is the causal mean, and the remainder are
+    This variation includes 1+`b` parameters, where the first parameter is the causal mean, and the remainder are
     the parameters for the regression model.
 
 
-    The alternative parameter of interest could be the mean difference between two plans. A common example of this would
-    be the average causal effect, where the plans are all-action-one versus all-action-zero. Therefore, the estimating
+    Alternatively, a causal mean difference is estimated when ``X0`` is specified. A common example of this would be
+    the average causal effect, where the plans are all-action-one versus all-action-zero. Therefore, the estimating
     equations consist of the following three equations
 
     .. math::
 
         \sum_{i=1}^n
         \begin{bmatrix}
             (\theta_1 - \theta_2) - \theta_0 \\
             g({X_i^1}^T \beta) - \theta_1 \\
-            g({X_i^0}^T \beta) - \theta_2
+            g({X_i^0}^T \beta) - \theta_2 \\
+            \left\{ Y_i - g(X_i^T \beta) \right\} X_i
         \end{bmatrix}
         = 0
 
     Note
     ----
-    This variation includes :math:`3+b` parameters, where the first parameter is the causal mean difference, the second
+    This variation includes 3+`b` parameters, where the first parameter is the causal mean difference, the second
     is the causal mean under plan 1, the third is the causal mean under plan 0, and the remainder are the parameters
     for the regression model.
 
-
-    The parameter of interest is designated by the user via whether the optional argument ``X0`` is left as ``None``
-    (which estimates the causal mean) or is given an array (which estimates the causal mean difference and the
-    corresponding causal means).
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta consists of 1+b values if ``X0`` is ``None``, and 3+b values if ``X0`` is not ``None``.
+        Theta consists of 1+`b` values if ``X0`` is ``None``, and 3+`b` values if ``X0`` is not ``None``.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     X1 : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables under the action plan.
+        2-dimensional vector of `n` observed values for `b` variables under the action plan.
     X0 : ndarray, list, vector, None, optional
-        2-dimensional vector of n observed values for b variables under the separate action plan. This second argument
-        is optional and should be specified if the causal mean difference between two action plans is of interest.
+        2-dimensional vector of `n` observed values for `b` variables under the separate action plan. This second
+        argument is optional and should be specified if the causal mean difference between two action plans is of
+        interest.
     force_continuous : bool, optional
         Option to force the use of linear regression despite detection of a binary variable.
 
     Returns
     -------
     array :
-        Returns a (1+b)-by-n NumPy array if ``X0=None``, or returns a (3+b)-by-n NumPy array if ``X0!=None``
+        Returns a (1+`b`)-by-`n` NumPy array if ``X0=None``, or returns a (3+`b`)-by-`n` NumPy array if ``X0!=None``
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_gformula`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -244,79 +235,60 @@
         return np.vstack((ace,            # theta[0] is the mean difference between X1 and X0
                           ya1[None, :],   # theta[1] is the mean under X1
                           ya0[None, :],   # theta[2] is the mean under X0
                           preds_reg))     # theta[3:] is for the regression coefficients
 
 
 def ee_ipw(theta, y, A, W, truncate=None, weights=None):
-    r"""Estimating equation for inverse probability weighting estimator. For estimation of the weights (or propensity
-    scores), a logistic model is used. The first estimating equations for the logistic regression model are
+    r"""Estimating equation for inverse probability weighting (IPW) estimator. The average causal effect is estimated by
+    this implementation of the IPW estimator. For estimation of the propensity scores, a logistic model is used.
 
-    .. math::
-
-        \sum_{i=1}^n \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i = 0
-
-    where A is the action and W is the set of confounders.
-
-    For the implementation of the inverse probability weighting estimator, stacked estimating equations are used
-    for the mean had everyone been set to ``A=1``, the mean had everyone been set to ``A=0``, and the mean difference
-    between the two causal means. The estimating equations are
+    The stacked estimating equations are
 
     .. math::
 
         \sum_{i=1}^n
         \begin{bmatrix}
             (\theta_1 - \theta_2) - \theta_0 \\
             \frac{A_i Y_i}{\pi_i} - \theta_1 - \theta_1 \\
-            \frac{(1-A_i) Y_i}{1-\pi_i} - \theta_2
+            \frac{(1-A_i) Y_i}{1-\pi_i} - \theta_2 \\
+            \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i
         \end{bmatrix}
         = 0
 
-    where :math:`\pi_i = expit(W_i^T \alpha)`. Due to these 3 extra values, the length of the theta vector is 3+b,
-    where b is the number of parameters in the regression model.
-
-    Note
-    ----
-    Unlike ``ee_gformula``, ``ee_ipw`` always provides the average causal effect, and causal means for ``A=1`` and
-    ``A=0``.
-
-
-    Here, theta corresponds to a variety of different quantities. The *first* value in theta vector is the causal mean
-    difference, the *second* is the mean had everyone been set to ``A=1``, the *third* is the mean had everyone been
-    set to ``A=0``. The remainder of the parameters correspond to the logistic regression model coefficients.
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
+    where :math:`A` is the action, math:`W` is the set of confounders, and :math:`\pi_i = expit(W_i^T \alpha)`. The
+    first estimating equation is for the average causal effect, the second is for the mean under :math:`A:=1`,
+    the third is for the mean under :math:`A:=0`, and the last is the logistic regression model for the propensity
+    scores. Here, the length of the theta vector is 3+`b`, where `b` is the number of parameters in the regression
+    model.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta consists of 3+b values.
+        Theta consists of 3+`b` values.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     A : ndarray, list, vector
-        1-dimensional vector of n observed values. The A values should all be 0 or 1.
+        1-dimensional vector of `n` observed values. The A values should all be 0 or 1.
     W : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables to model the probability of ``A`` with.
+        2-dimensional vector of `n` observed values for `b` variables to model the probability of ``A`` with.
     truncate : None, list, set, ndarray, optional
         Bounds to truncate the estimated probabilities of ``A`` at. For example, estimated probabilities above 0.99 or
         below 0.01 can be set to 0.99 or 0.01, respectively. This is done by specifying ``truncate=(0.01, 0.99)``. Note
         this step is done via ``numpy.clip(.., a_min, a_max)``, so order is important. Default
         is ``None``, which applies no truncation.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations. This
+        1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations. This
         argument is intended to support the use of missingness weights. The propensity score model is *not* fit using
         these weights.
 
     Returns
     -------
     array :
-        Returns a (3+b)-by-n NumPy array evaluated for the input ``theta``
+        Returns a (3+`b`)-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_ipw`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -330,15 +302,15 @@
     >>> d['W'] = np.random.binomial(1, p=0.5, size=n)
     >>> d['A'] = np.random.binomial(1, p=(0.25 + 0.5*d['W']), size=n)
     >>> d['Ya0'] = np.random.binomial(1, p=(0.75 - 0.5*d['W']), size=n)
     >>> d['Ya1'] = np.random.binomial(1, p=(0.75 - 0.5*d['W'] - 0.1*1), size=n)
     >>> d['Y'] = (1-d['A'])*d['Ya0'] + d['A']*d['Ya1']
     >>> d['C'] = 1
 
-    Defining psi, or the stacked estimating equations. Note that 'A' is the action.
+    Defining psi, or the stacked estimating equations. Note that ``'A'`` is the action.
 
     >>> def psi(theta):
     >>>     return ee_ipw(theta, y=d['Y'], A=d['A'],
     >>>                   W=d[['C', 'W']])
 
     Calling the M-estimation procedure. Since ``W`` is 2-by-n here and IPW has 3 additional parameters, the initial
     values should be of length 3+2=5. In general, it will be best to start with [0., 0.5, 0.5, ...] as the initials when
@@ -405,47 +377,50 @@
     return np.vstack((ate,             # theta[0] is for the ATE
                       ya1[None, :],    # theta[1] is for R1
                       ya0[None, :],    # theta[2] is for R0
                       preds_reg))      # theta[3:] is for the regression coefficients
 
 
 def ee_ipw_msm(theta, y, A, W, V, distribution, link, hyperparameter=None, truncate=None, weights=None):
-    r"""Estimating equation for inverse probability weighting estimator of the parameters of a marginal structural
-    model. For estimation of the weights (or propensity scores), a logistic model is used. The first estimating
-    equations for the logistic regression model are
+    r"""Estimating equation for parameters of a marginal structural model estimated using inverse probability weighting.
+    For estimation of the propensity scores, a logistic model is used.
+
+    The stacked estimating equations are
 
     .. math::
 
-        \sum_{i=1}^n \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i = 0
+        \sum_{i=1}^n
+        \begin{bmatrix}
+            \frac{1}{\pi_i} \left\{ Y_i - g^{-1}(X_i^T \beta) \right\} \times \frac{D(\beta)}{v(\beta)} X_i \\
+            \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i
+        \end{bmatrix}
+        = 0
 
-    where A is the action and W is the set of confounders. For the implementation of the inverse probability weighting
-    estimator of the marginal structural model, a weighted generalized linear model is used. See ``ee_glm`` for details
-    on this estimating equation.
+    where :math:`A` is the action, math:`W` is the set of confounders, and :math:`\pi_i = \text{expit}(W_i^T \alpha)`.
+    Here, :math:`X` is the design matrix for the marginal structural model (it includes :math:`A`, and possibly some
+    covariates from :math:`W`). The first estimating equation is a weighted generalized linear model is used. See
+    ``ee_glm`` for details on this estimating equation. The second estimating equation is the logistic model for the
+    propensity scores.
 
     Here, ``theta`` corresponds to multiple quantities. The *first* set of values correspond to the parameters of the
     marginal structural model, and the *second* set correspond to the logistic regression model coefficients for the
     propensity scores.
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta consists of 3+b values.
+        Theta consists of `c`+`b` values.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     A : ndarray, list, vector
-        1-dimensional vector of n observed values. The A values should all be 0 or 1.
+        1-dimensional vector of `n` observed values. The A values should all be 0 or 1.
     W : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables to model the probability of ``A`` with.
+        2-dimensional vector of `n` observed values for `b` variables to model the probability of ``A`` with.
     V : ndarray, list, vector
-        2-dimensional vector of n observed values for c variables in the marginal structural model.
+        2-dimensional vector of `n` observed values for `c` variables in the marginal structural model.
     distribution : str
         Distribution for the generalized linear model. See ``ee_glm`` for options.
     link : str
         Link function for the generalized linear model. See ``ee_glm`` for options.
     truncate : None, list, set, ndarray, optional
         Bounds to truncate the estimated probabilities of ``A`` at. For example, estimated probabilities above 0.99 or
         below 0.01 can be set to 0.99 or 0.01, respectively. This is done by specifying ``truncate=(0.01, 0.99)``. Note
@@ -455,15 +430,15 @@
         1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations. This
         argument is intended to support the use of missingness weights. The propensity score model is *not* fit using
         these weights.
 
     Returns
     -------
     array :
-        Returns a (3+b)-by-n NumPy array evaluated for the input ``theta``
+        Returns a (`c`+`b`)-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_ipw_msm`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -554,93 +529,69 @@
     # Output (c+b)-by-n stacked array
     return np.vstack((ee_msm,          # theta[:c] is the marginal structural model parameters
                       preds_reg))      # theta[c:] is for the regression coefficients
 
 
 def ee_aipw(theta, y, A, W, X, X1, X0, truncate=None, force_continuous=False):
     r"""Estimating equation for augmented inverse probability weighting (AIPW) estimator. AIPW consists of two nuisance
-    models (the propensity score model and the outcome model). For estimation of the propensity scores, the estimating
-    equations are
+    models (the propensity score model and the outcome model).
 
-    .. math::
-
-        \sum_{i=1}^n \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i = 0
-
-    where ``A`` is the treatment and ``W`` is the set of confounders. The estimating equations for the outcome model
-    are
-
-    .. math::
-
-        \sum_{i=1}^n \left\{ Y_i - g(X_i^T \beta) \right\} X_i = 0
-
-    By default, `ee_aipw` detects whether `y` is all binary (zero or one), and applies logistic regression. Notice that
-    ``X`` here should consists of both ``A`` and ``W`` (with possible interaction terms or other differences in
-    functional forms from the propensity score model).
-
-    The AIPW estimating equations include the causal mean difference, mean had everyone been set to ``A=1``, and the
-    mean had everyone been set to ``A=0``
+    The stacked estimating equations are
 
     .. math::
 
         \sum_{i=1}^n
         \begin{bmatrix}
             (\theta_1 - \theta_2) - \theta_0 \\
             \frac{A_i Y_i}{\pi_i} - \frac{\hat{Y^1}(A_i-\pi_i}{\pi_i} - \theta_1 \\
-            \frac{(1-A_i) Y_i}{1-\pi_i} + \frac{\hat{Y^0}(A_i-\pi_i}{1-\pi_i} - \theta_2
+            \frac{(1-A_i) Y_i}{1-\pi_i} + \frac{\hat{Y^0}(A_i-\pi_i}{1-\pi_i} - \theta_2 \\
+            \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i \\
+            \left\{ Y_i - g(X_i^T \beta) \right\} X_i
         \end{bmatrix}
         = 0
 
-    where :math:`\hat{Y}^a = g({X_i^*}^T \beta)`.
-
-    Note
-    ----
-    Unlike ``ee_gformula``, ``ee_aipw`` always provides the average causal effect, and causal means for ``A=1`` and
-    ``A=0``.
-
+    where :math:`A` is the action and :math:`W` is the set of confounders, :math:`Y` is the outcome, and
+    :math:`\pi_i = \text{expit}(W_i^T \alpha)`. The first estimating equation is for the average causal effect, the
+    second is for the mean under :math:`A:=1`, the third is for the mean under :math:`A:=0`, the fourth is the logistic
+    regression model for the propensity scores, and the last is for the outcome model. Here, the length of the theta
+    vector is 3+`b`+`c`, where `b` is the number of parameters in the propensity score model and `c` is the number
+    of parameters in the outcome model.
 
-    Due to these 3 extra values and two nuisance models, the length of the parameter vector is 3+b+c, where b is the
-    number of columns in ``W``, and c is the number of columns in ``X``. The *first* value in theta vector is the
-    causal mean difference (or average causal effect), the *second* is the mean had everyone been given ``A=1``, the
-    *third* is the mean had everyone been given ``A=0``. The remainder of the parameters correspond to the regression
-    model coefficients, in the order input. The first 'chunk' of  coefficients correspond to the propensity score model
-    and the last 'chunk' correspond to the outcome model.
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
+    By default, `ee_aipw` detects whether `y` is all binary (zero or one), and applies logistic regression. Notice that
+    ``X`` here should consists of both ``A`` and ``W`` (with possible interaction terms or other differences in
+    functional forms from the propensity score model).
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta consists of 3+b+c values.
+        Theta consists of 3+`b`+`c` values.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     A : ndarray, list, vector
-        1-dimensional vector of n observed values. The A values should all be 0 or 1.
+        1-dimensional vector of `n` observed values. The A values should all be 0 or 1.
     W : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables to model the probability of ``A`` with.
+        2-dimensional vector of `n` observed values for `b` variables to model the probability of ``A`` with.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for c variables to model the outcome ``y``.
+        2-dimensional vector of `n` observed values for `c` variables to model the outcome ``y``.
     X1 : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables under the action plan where ``A=1`` for all units.
+        2-dimensional vector of `n` observed values for `c` variables under the action plan where ``A=1`` for all units.
     X0 : ndarray, list, vector, None, optional
-        2-dimensional vector of n observed values for b variables under the action plan where ``A=0`` for all units.
+        2-dimensional vector of `n` observed values for `c` variables under the action plan where ``A=0`` for all units.
     truncate : None, list, set, ndarray, optional
         Bounds to truncate the estimated probabilities of ``A`` at. For example, estimated probabilities above 0.99 or
         below 0.01 can be set to 0.99 or 0.01, respectively. This is done by specifying ``truncate=(0.01, 0.99)``. Note
         this step is done via ``numpy.clip(.., a_min, a_max)``, so order is important. Default
         is ``None``, which applies to no truncation.
     force_continuous : bool, optional
         Option to force the use of linear regression despite detection of a binary variable.
 
     Returns
     -------
     array :
-        Returns a (3+b+c)-by-n NumPy array evaluated for the input ``theta``
+        Returns a (3+`b`+`c`)-by-`n` NumPy array evaluated for the input ``theta``
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_aipw`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -783,81 +734,92 @@
     estimates the average causal effect in the acted on within strata of a set of covariates, :math:`V`. Options for
     SMM include the linear SMM and the log-linear SMM. The linear SMM is defined as
 
     .. math::
 
         E[Y^a - Y^{0} | A=a, V] = \beta_1 a + \beta_2 a V
 
-    This model corresponds to the average causal effect among those with :math:`A=a` within strata of :math:`V`. The
+    This model corresponds to the average causal effect among those with :math:`A=a` by :math:`V`. The
     log-linear SMM is defined as
 
     .. math::
 
         \frac{E[Y^a | A=a, V]}{E[Y^{0} | A=a, V]} = \exp(\beta_1 a + \beta_2 a V)
 
-    This model corresponds to the causal mean ratio among those with :math:`A=a` within strata of :math:`V`. Note that
-    the log-linear SMM is only defined when :math:`Y > 0`. The parameters of either SMM can be identified under the
+    This model corresponds to the causal mean ratio among those with :math:`A=a` by :math:`V`. Note that
+    the log-linear SMM is only defined when :math:`Y > 0`. The parameters of either SMM are identified under the
     assumptions of  causal consistency, and exchangeability with positivity.
 
     Two different estimating equations are available for g-estimation. The first set is referred to at the 'inefficient'
     g-estimator. For the inefficient g-estimator we solve for :math:`\beta` in the following estimating equation
 
     .. math::
 
-        \sum_{i=1}^n \left\{ H(\beta) \times (A - E[A | W]) \right\}  \times \mathbb{V}_i = 0
+        \sum_{i=1}^n
+        \begin{bmatrix}
+            \left\{ H(\beta) \times (A - \pi_i) \right\}  \times V_i \\
+            \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i
+        \end{bmatrix}
+        = 0
 
-    where :math:`H(\beta) = Y - \beta A \mathbb{V}` for a linear SMM and
-    :math:`H(\beta) = Y \times \exp(-A \beta \mathbb{V})` for a log-linear SMM, where :math:`\mathbb{V}` is a design
-    matrix. Note that :math:`V \subseteq W`, where :math:`W` is the set of confounding variables. This estimating
-    equation requires :math:`E[A|W]`, which must be estimated. This is done via the following estimating equation for
-    binary actions
+    where :math:`\pi_i = \text{expit}(W_i^T \alpha)`, and
+    :math:`H(\beta) = Y - \beta A \mathbb{V}` for a linear SMM and
+    :math:`H(\beta) = Y \times \exp(-A \beta \mathbb{V})` for a log-linear SMM, where .
+    Note that :math:`V \subseteq W`, where :math:`W` is the set of confounding variables.
+    The length of the parameter vector is `b`+`c`, where `b` is the number of columns in ``V``, and
+    `c` is the number of columns in ``W``.
 
-    .. math::
+    The second implementation for g-estimation is the 'efficient' g-estimator. For the efficient g-estimator we replace
+    :math:`H(\beta)` with :math:`\{H(\beta) - E[H(\beta) | W]\}` in the prior estimating equation and specify a model
+    for :math:`E[H(\beta) | W]`. The corresponding stacked estimating equations are
 
-        \sum_{i=1}^n \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i = 0
+    .. math::
 
-    These estimating equations are stacked together. Therefore, the length of the parameter vector is b+c, where b is
-    the number of columns in ``V``, and c is the number of columns in ``W``. The *first* b values in theta
-    vector are the SMM parameters. The *second* set are the parameters corresponding to the :math:`E[A|W]` model.
+        \sum_{i=1}^n
+        \begin{bmatrix}
+            \left\{ (H(\beta) - g^{-1}(W_i^T \gamma)) \times (A - \pi_i) \right\}  \times V_i \\
+            \left\{ A_i - \text{expit}(W_i^T \alpha) \right\} W_i \\
+            \left\{ H(\beta) - g^{-1}(W_i^T \gamma) \right\} W_i \\
+        \end{bmatrix}
+        = 0
 
-    The second implementation for g-estimation is the 'efficient' g-estimator. For the efficient g-estimator we replace
-    :math:`H(\beta)` with :math:`\{H(\beta) - E[H(\beta) | W]\}` in the prior estimating equation. Here, we also need to
-    specify a model for :math:`E[H(\beta) | W]`. Therefore, an additional estimating equation for
-    :math:`E[H(\beta) | W]` is stacked with the others. Therefore, there are b+c+d parameters for the efficient
-    g-estimator, where d is the number of parameters in the model for :math:`E[H(\beta) | W]`.
+    where :math:`g^{-1}` is the inverse transformation for the specified SMM. Therefore, there are b+c+d parameters
+    for the efficient g-estimator, where `d` is the number of parameters in the model for :math:`E[H(\beta) | W]`.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta consists of 1+b values if ``X0`` is ``None``, and 3+b values if ``X0`` is not ``None``.
+        Theta consists of 1+`b` values if ``X0`` is ``None``, and 3+b values if ``X0`` is not ``None``.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values of the outcome.
+        1-dimensional vector of `n` observed values of the outcome.
     A : ndarray, list, vector
-        1-dimensional vector of n observed values of the action. The A values should all be 0 or 1.
+        1-dimensional vector of `n` observed values of the action. The A values should all be 0 or 1.
     W : ndarray, list, vector
-        2-dimensional vector of n observed values for b columns of a design matrix to model the expected value of ``A``.
+        2-dimensional vector of `n` observed values for b columns of a design matrix to model the expected value of
+        ``A``.
     V : ndarray, list, vector
-        2-dimensional vector of n observed values for b columns of a design matrix for the structural mean model. Note
-        that the design matrix here is expected to not include the observed values of ``A``
+        2-dimensional vector of `n` observed values for `b` columns of a design matrix for the structural mean model.
+        Note that the design matrix here is expected to not include the observed values of ``A``
     X : ndarray, list, vector, None, optional
         Default of this argument is ``None``, which implements the estimating equation for the inefficient g-estimator.
-        To use the efficient g-estimator, a 2-dimensional vector of n observed values for b columns of a design matrix
+        To use the efficient g-estimator, a 2-dimensional vector of n observed values for `b` columns of a design matrix
         for the :math:`E[H(\beta) | W]` model should be provided here.
     model : str, optional
         Type of structural mean model to fit. Options are currently: ``linear``, ``poisson``. Default is ``linear``.
         The Poisson model specification can be used for positive continuous data, or with binary data in order to
         estimate causal risk ratios.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations. This
+        1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations. This
         argument is intended to support the use of sampling or missingness weights.
 
     Returns
     -------
     array :
-        Returns a (b+c)-by-n (inefficient) or (b+c+d)-by-n (efficient) NumPy array evaluated for the input ``theta``
+        Returns a (`b`+`c`)-by-`n` (inefficient) or (`b`+`c`+`d`)-by-`n` (efficient) NumPy array evaluated for the
+        input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_gestimation_snmm`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -1036,42 +998,43 @@
     Note
     ----
     This estimator looks like the inverse probability weighting estimator, but the estimating equation for the mean
     is slightly different. When :math:`q(Y, \alpha) = 0`, the estimates between this estimator and the inverse
     probability weighting estimator will result in different (but similar) estimates.
 
 
-    The length of the parameter vector, :math:`\theta`, is 1+b, where b is the number of columns in ``X``. The *first*
-    value in the theta vector is the corrected mean of :math:`Y`. The remainder of the parameters correspond to the
-    regression model coefficients.
+    The length of the parameter vector, :math:`\theta`, is 1+`b`, where `b` is the number of columns in ``X``.
+    The *first* value in the theta vector is the corrected mean of :math:`Y`. The remainder of the parameters
+    correspond to the regression model coefficients.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of 1+b values. Therefore, initial values should consist of one plus the number of
+        Theta in this case consists of 1+`b` values. Therefore, initial values should consist of one plus the number of
         columns present in ``X``. This can easily be accomplished generally by ``[0, ] + [0, ] * X.shape[1]``.
     y : ndarray, list, vector
-        1-dimensional vector of n values. Any values of ``y`` that are missing should be indicated by the ``delta``
+        1-dimensional vector of `n` values. Any values of ``y`` that are missing should be indicated by the ``delta``
         parameter.
     delta : ndarray, list, vector
-        1-dimensional vector of n observed values indicating whether the observation has a value for ``y`` observed,
+        1-dimensional vector of `n` observed values indicating whether the observation has a value for ``y`` observed,
         where 1 indicates yes and 0 indicated no. This vector should not include any ``nan`` values.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables consider as predictors. At a minimum, a vector of ones
-        (intercept) should be included. This matrix should not include any ``nan`` values.
+        2-dimensional vector of `n` observed values for `b` variables consider as predictors. At a minimum, a vector
+        of ones (intercept) should be included. This matrix cannot include any ``nan`` values.
     q_eval : ndarray, list, vector
-        1-dimensional vector of n values evaluated using the :math:`q(Y; \alpha)` function.
+        1-dimensional vector of `n` values evaluated using the :math:`q(Y; \alpha)` function.
     H_function : callable
-        Function use to bound the observations between 0,1. The function must be monotonic increasing and be bounded by
-        :math:`[0,1]`. For example, the expit (``delicatessen.utilities.inverse_logit``) function meets this criteria.
+        Function use to bound the observations between :math:`[0,1]`. The function must be monotonic increasing and be
+        bounded by :math:`[0,1]`. For example, the expit (``delicatessen.utilities.inverse_logit``) function meets
+        this criteria.
 
     Returns
     -------
     array :
-        Returns a (1+b)-by-n NumPy array evaluated for the input ``theta``
+        Returns a (1+`b`)-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_mean_sensitivity_analysis`` should be done similar to the
     following
 
     >>> import numpy as np
```

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/dose_response.py` & `delicatessen-2.2/delicatessen/estimating_equations/dose_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,36 +22,32 @@
         \end{bmatrix}
         = 0
 
     where :math:`R_i` is the response of individual :math:`i`, :math:`D_i` is the dose,
     :math:`\rho = \frac{D_i}{\theta_1}^{\theta_2}`, and
     :math:`\hat{Y_i} = \theta_0 + \frac{\theta_3 - \theta_0}{1+\rho}`.
 
-    Here, theta is a 1-by-4 array, where 4 are the 4 parameters of the 4PL. The first theta corresponds to lower limit
+    Here, theta is a 1-by-4 array. The first theta corresponds to lower limit
     (:math:`\theta_0`), the second corresponds to the effective dose (ED50) (:math:`\theta_1`), the third corresponds
     to the steepness of the curve (:math:`\theta_2`), and the fourth corresponds to the upper limit (:math:`\theta_3`).
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of 4 values. In general, starting values ``>0`` are better choices for the 4PL model
+        Theta in this case consists of 4 values. In general, starting values :math:`>0` are better choices for the
+        4PL model
     X : ndarray, list, vector
-        1-dimensional vector of n dose values.
+        1-dimensional vector of `n` dose values.
     y : ndarray, list, vector
-        1-dimensional vector of n response values.
+        1-dimensional vector of `n` response values.
 
     Returns
     -------
     array :
-        Returns a 4-by-n NumPy array evaluated for the input ``theta``
+        Returns a 4-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_4p_logistic`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.data import load_inderjit
@@ -158,34 +154,30 @@
     :math:`\hat{Y_i} = \theta_0 + \frac{\theta_3 - \theta_0}{1+\rho}`.
 
     Here, theta is a 1-by-3 array for the 3PL. The first theta corresponds to the effective dose (ED50)
     (:math:`\theta_1`), the second corresponds to the steepness of the curve (:math:`\theta_2`), and the third
     corresponds to the upper limit (:math:`\theta_3`). The lower limit (:math:`\theta_0`, ``lower``) is pre-specified
     by the user (and is no longer estimated)
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of 3 values. In general, starting values ``>0`` are better choices for the 3PL model
+        Theta in this case consists of 3 values. In general, starting values :math:`>0` are better choices for the
+        3PL model
     X : ndarray, list, vector
-        1-dimensional vector of n dose values.
+        1-dimensional vector of `n` dose values.
     y : ndarray, list, vector
-        1-dimensional vector of n response values.
+        1-dimensional vector of `n` response values.
     lower : int, float
         Set value for the lower limit.
 
     Returns
     -------
     array :
-        Returns a 3-by-n NumPy array evaluated for the input theta, y, X
+        Returns a 3-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_3p_logistic`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.data import load_inderjit
@@ -256,36 +248,32 @@
     :math:`\hat{Y_i} = \theta_0 + \frac{\theta_3 - \theta_0}{1+\rho}`.
 
     Here, theta is a 1-by-2 array for the 2PL. The first theta corresponds to the effective dose (ED50)
     (:math:`\theta_1`), and the second corresponds to the steepness of the curve (:math:`\theta_2`). The lower limit
     (:math:`\theta_0`, ``lower``) and upper limit (:math:`\theta_3`, ``upper``) are pre-specified by the user (and are
     no longer estimated)
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of 2 values. In general, starting values >0 are better choices for the 3PL model
+        Theta in this case consists of 2 values. In general, starting values :math:`>0` are better choices for the
+        2PL model
     X : ndarray, list, vector
-        1-dimensional vector of n dose values.
+        1-dimensional vector of `n` dose values.
     y : ndarray, list, vector
-        1-dimensional vector of n response values.
+        1-dimensional vector of `n` response values.
     lower : int, float
         Set value for the lower limit.
     upper : int, float
         Set value for the upper limit.
 
     Returns
     -------
     array :
-        Returns a 2-by-n NumPy array evaluated for the input theta, y, X
+        Returns a 2-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_2p_logistic`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.data import load_inderjit
@@ -352,15 +340,15 @@
     stacked with the correspond PL model.
 
     Parameters
     ----------
     theta : int, float
         Theta value corresponding to the ED(alpha).
     y : ndarray, list, vector
-        1-dimensional vector of n response values, used to construct correct shape for output.
+        1-dimensional vector of `n` response values, used to construct correct shape for output.
     delta : float
         The effective dose level of interest, ED(alpha).
     steepness : float
         Estimated parameter for the steepness from the PL.
     ed50 : float
         Estimated parameter for the ED50, or ED(alpha=50), from the PL.
     lower : int, float
@@ -369,15 +357,15 @@
     upper : int, float
         Estimated parameter or pre-specified constant for the lower limit. This should be a pre-specified constant for
         the 2PL.
 
     Returns
     -------
     array :
-        Returns a 1-by-n NumPy array evaluated for the input theta
+        Returns a 1-by-`n` NumPy array evaluated for the input theta
 
     Examples
     --------
     Construction of a estimating equations for ED25 with ``ee_3p_logistic`` should be done similar to the following
 
     >>> from delicatessen import MEstimator
     >>> from delicatessen.data import load_inderjit
```

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/processing.py` & `delicatessen-2.2/delicatessen/estimating_equations/processing.py`

 * *Files identical despite different names*

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/regression.py` & `delicatessen-2.2/delicatessen/estimating_equations/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,47 +23,39 @@
 
         \sum_{i=1}^n \left\{ Y_i - g(X_i^T \theta) \right\} X_i = 0
 
     where :math:`g` indicates a transformation function. For linear regression, :math:`g` is the identity function.
     Logistic regression uses the inverse-logit function, :math:`\text{expit}(u) = 1 / (1 + \exp(u))`. Finally, Poisson
     regression is :math:`\exp(u)`.
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughout, these
-    user-defined functions are defined as ``psi``.
-
-
-    Here, :math:`\theta` corresponds to the coefficients in the corresponding regression model
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented by ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_regression`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -141,47 +133,39 @@
 def ee_glm(theta, X, y, distribution, link, hyperparameter=None, weights=None, offset=None):
     r"""Estimating equation for regression with a generalized linear model. Unlike ``ee_regression``, this functionality
     supports generic distribution and link specifications. The general estimating equation for the outcome :math:`Y_i`
     with the design matrix :math:`X_i`
 
     .. math::
 
-        \sum_{i=1}^n W_i \left\{ Y_i - g^{-1}(X_i^T \theta) \times \frac{D(\theta)}{v(\theta)} \right\} X_i = 0
+        \sum_{i=1}^n \left\{ Y_i - g^{-1}(X_i^T \theta) \right\} \times \frac{D(\theta)}{v(\theta)} X_i = 0
 
     where :math:`g` is the link function, :math:`g^{-1}` is the inverse link function, :math:`D(\theta)` is the
     derivative of the inverse link function by :math:`\theta`, and :math:`v(\theta)` is the variance function for the
     specified distribution.
 
     Note
     ----
     Some distributions (i.e., negative-binomial, gamma) involve additional parameters. These are estimated using
     additional parameter-specific estimating equations.
 
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughout, these
-    user-defined functions are defined as ``psi``.
-
-
-    Here, :math:`\theta` corresponds to the coefficients in the corresponding regression model
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented by ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     distribution : str
         Distribution for the generalized linear model. Options are:
         ``'normal'`` (alias: ``gaussian``),
         ``'binomial'`` (aliases: ``bernoulli``, ``bin``),
         ``'poisson'``,
         ``'gamma'``,
         ``'inverse_normal'`` (alias: ``inverse_gaussian``),
@@ -195,30 +179,30 @@
         ``probit``,
         ``cauchit`` (alias: ``cauchy``),
         ``loglog``,
         ``cloglog``,
         ``inverse``,
         and ``square_root`` (alias: ``sqrt``).
     hyperparameter : None, int, float
-        Hyperparameter specification. Default is None. This option is only used by the tweedie distribution. It is
+        Hyperparameter specification. Default is ``None``. This option is only used by the tweedie distribution. It is
         ignored by all other distributions.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Note
     ----
     Link and distribution combinations are not checked for their validity. Some pairings may not converge or may
-    produce nonsensical results. Please check the combination you are using is valid.
+    produce nonsensical results. Please check the distribution-link combination you are using is valid.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_regression`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -281,27 +265,27 @@
 
     Calling the M-estimator (note that ``init`` requires 4 values, since ``X.shape[1]`` is 3 and the gamma distribution
     has an additional parameter).
 
     >>> estr = MEstimator(stacked_equations=psi, init=[0., 0., 0., 0.])
     >>> estr.estimate()
 
-    Note that ``delicatessen`` appropriately incorporates the estimation of the additional parameter for the
+    Note that delicatessen appropriately incorporates the estimation of the additional parameter for the
     negative-binomial and gamma distributions. This is unlike some statistical software that estimates this parameter
     but does *not* incorporate the uncertainty in estimation of that parameter. This may explain differences you
-    encounter across software (and the ``delicatessen`` implementation is preferred, as it is a more honest expression
-    of the uncertainty).
+    encounter across software (and the delicatessen implementation is to be preferred, as it is a more honest
+    expression of the uncertainty).
 
     Finally, the tweedie distribution for GLM is a generalization of the Poisson and gamma distributions. Unlike the
-    negative-binomial and gamma distributions, there is a fixed (i.e., not estimated) hyperparameter bounded to be >0.
-    When the tweedie distribution hyperparameter is set to 1, it is equivalent to the Poisson distribution. When the
-    tweedie distribution hyperparameter is set to 2, it is equivalent to the gamma distribution. When the tweedie
-    distribution hyperparameter is set to 3, it is equivalent to the inverse-normal distribution. However, the tweedie
-    distribution hyperparameter can be specified for any values. Here, we illustrate the tweedie distribution that is
-    between a Poisson and gamma distribution.
+    negative-binomial and gamma distributions, there is a fixed (i.e., not estimated) hyperparameter bounded to be
+    :math:`>0`. When the tweedie distribution hyperparameter is set to 1, it is equivalent to the Poisson distribution.
+    When the tweedie distribution hyperparameter is set to 2, it is equivalent to the gamma distribution. When the
+    tweedie distribution hyperparameter is set to 3, it is equivalent to the inverse-normal distribution. However, the
+    tweedie distribution hyperparameter can be specified for any values. Here, we illustrate the tweedie distribution
+    that is between a Poisson and gamma distribution.
 
     >>> def psi(theta):
     >>>     return ee_glm(theta, X=X, y=d['Y1'],
     >>>                   distribution='tweedie', link='log',
     >>>                   hyperparameter=1.5)
 
     Calling the M-estimator (note that ``init`` requires 3 values, since ``X.shape[1]`` is 3).
@@ -360,59 +344,50 @@
         return ee_beta                                                                   # ... only beta EE
 
 
 def ee_mlogit(theta, X, y, weights=None, offset=None):
     r"""Estimating equation for multinomial logistic regression. This estimating equation functionality supports
     unranked categorical outcome data, unlike ``ee_regression`` and ``ee_glm``.
 
-    Note
-    ----
     Unlike the other regression estimating equations, ``ee_mlogit`` expects a matrix of indicators for each possible
     value of ``y``, with the first column being used as the referent category. In other words, the outcome variable is
     a matrix of dummy variables that includes the reference.
-
-
-    The estimating equation for column :math:`r` of the indicator variable :math:`Y_{r}`
-    of a :math:`Y` with :math:`k` unique categories is
+    The estimating equation for column :math:`r` of the indicator variable :math:`Y_{r}` of a :math:`Y` with :math:`k`
+    unique categories is
 
     .. math::
 
         \sum_{i=1}^n \left\{ Y_{r,i} - \frac{\exp(X_i^T \theta_r)}{1 + \sum_{j=2}^{k} \exp(X_i^T \theta_j)}  \right\}
         X_i = 0
 
     where :math:`\theta_r` are the coefficients correspond to the log odds ratio comparing :math:`Y_r` to all other
-    categories of :math:`Y`. Here, :math:`\theta` is a 1-by-(b :math`\times` (k-1)) array, where b is the distinct
-    covariates included as part of X. So, the stack of estimating equations consists of :math:`(k-1)` estimating
-    equations of the dimension :math:`X_i`. For example, if X is a 3-by-n matrix and :math:`Y` has three unique
+    categories of :math:`Y`. Here, :math:`\theta` is a 1-by-(`b` :math`\times` (`k`-1)) array, where `b` is the distinct
+    covariates included as part of ``X``. So, the stack of estimating equations consists of (`k`-1) estimating
+    equations of the dimension :math:`X_i`. For example, if X is a 3-by-`n` matrix and :math:`Y` has three unique
     categories, then :math:`\theta` will be a 1-by-6 array.
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughout, these
-    user-defined functions are defined as ``psi``.
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b :math:`\times` (k-1) values. Therefore, initial values should consist of the
-        same number as the number of columns present in the design matrix for each category of the outcome matrix
+        Theta in this case consists of `b` :math:`\times` (`k`-1) values. Therefore, initial values should consist of
+        the same number as the number of columns present in the design matrix for each category of the outcome matrix
         besides the reference.
     X : ndarray, list, vector
-        2-dimensional design matrix of n observed covariates for b variables.
+        2-dimensional design matrix of `n` observed covariates for `b` variables.
     y : ndarray, list, vector
-        2-dimensional indicator matrix of n observed outcomes.
+        2-dimensional indicator matrix of `n` observed outcomes.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a (b*(k-1))-by-n NumPy array evaluated for the input ``theta``
+        Returns a (`b` :math:`\times` (`k`-1))-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_regression`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -528,54 +503,49 @@
     Note
     ----
     The estimating-equation is not non-differentiable everywhere for some loss functions. Therefore, it is assumed that
     no points occur exactly at the non-differentiable points. For truly continuous :math:`Y`, the probability of that
     occurring is zero.
 
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented via ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     model : str
         Type of regression model to estimate. Options include: ``'linear'`` (linear regression).
     k : int, float
         Tuning or hyperparameter for the chosen loss function. Notice that the choice of hyperparameter should depend
         on the chosen loss function.
     loss : str, optional
-        Robust loss function to use. Default is 'huber'. Options include 'andrew', 'hampel', 'huber', 'tukey'.
+        Robust loss function to use. Default is ``'huber'``. Options include ``'andrew'``, ``'hampel'``, ``'tukey'``.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     lower : int, float, None, optional
-        Lower parameter for the 'hampel' loss function. This parameter does not impact the other loss functions.
+        Lower parameter for the Hampel loss function. This parameter does not impact the other loss functions.
         Default is ``None``.
     upper : int, float, None, optional
-        Upper parameter for the 'hampel' loss function. This parameter does not impact the other loss functions.
+        Upper parameter for the Hampel loss function. This parameter does not impact the other loss functions.
         Default is ``None``.
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_robust_regression`` should be done similar to the
     following
 
     >>> import numpy as np
@@ -664,58 +634,57 @@
 
     .. math::
 
         \sum_{i=1}^n \left\{(Y_i - X_i^T \theta) X_i - \lambda \theta \right\} = 0
 
     where :math:`\lambda` is the penalty term.
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Note
     ----
     The 'strength' of the penalty term is indicated by :math:`\lambda`, which is the ``penalty`` argument scaled (or
     divided by) the number of observations.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented via ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     penalty : int, float, ndarray, list, vector
         Penalty term to apply to all coefficients (if only a integer or float is provided) or the corresponding
         coefficient (if a list or vector of integers or floats is provided). Note that the penalty term should either
-        consists of a single value or b values (to match the length of ``theta``). The penalty is scaled by n.
+        consists of a single value or `b` values (to match the length of ``theta``). The penalty is scaled by `n`.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
-    Construction of a estimating equation(s) with ``ee_ridge_regression`` should be done similar to the
-    following
+    Construction of a estimating equation(s) with ``ee_ridge_regression`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
     >>> from scipy.stats import logistic
     >>> from delicatessen import MEstimator
     >>> from delicatessen.estimating_equations import ee_ridge_regression
 
@@ -792,76 +761,76 @@
                                 offset=offset)
 
 
 def ee_lasso_regression(theta, X, y, model, penalty, epsilon=3.e-3, weights=None, center=0., offset=None):
     r"""Estimating equation for an approximate LASSO (least absolute shrinkage and selection operator) regressor. LASSO
     regression applies an L1-regularization through a magnitude penalty.
 
-    Note
-    ----
-    As the derivative of the estimating equation for LASSO is not defined at :math:`\theta=0`, the bread (and sandwich)
-    cannot be used to estimate the variance in all settings.
-
-
     The estimating equation for the approximate LASSO linear regression is
 
     .. math::
 
         \sum_{i=1}^n \left\{(Y_i - X_i^T \theta) X_i - \lambda (1 + \epsilon) | \theta |^{\epsilon} sign(\theta)
         \right\} = 0
 
     where :math:`\lambda` is the penalty term.
 
+    Note
+    ----
+    As the derivative of the estimating equation for LASSO is not defined at :math:`\theta=0`, the bread (and sandwich)
+    cannot be used to estimate the variance in all settings.
+
+
     Here, an approximation based on the bridge penalty for the LASSO is used. For the bridge penalty, LASSO is the
     special case where :math:`\epsilon = 0`. By making :math:`\epsilon > 0`, we can approximate the LASSO. The true
     LASSO may not be possible to implement due to the existence of multiple solutions
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Note
     ----
     The 'strength' of the penalty term is indicated by :math:`\lambda`, which is the ``penalty`` argument scaled (or
     divided by) the number of observations.
 
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented via ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     penalty : int, float, ndarray, list, vector
         Penalty term to apply to all coefficients (if only a integer or float is provided) or the corresponding
         coefficient (if a list or vector of integers or floats is provided). Note that the penalty term should either
-        consists of a single value or b values (to match the length of ``theta``).  The penalty is scaled by n.
+        consists of a single value or `b` values (to match the length of ``theta``).  The penalty is scaled by `n`.
     epsilon : float, optional
         Approximation error to use for the LASSO approximation. Default argument is ``0.003``, which results in a
-        bridge penalty of 1.0003.
+        bridge penalty of ``1.0003``.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_lasso_regression`` should be done similar to the
     following
 
     >>> import numpy as np
@@ -945,74 +914,74 @@
 
 
 def ee_elasticnet_regression(theta, X, y, model, penalty, ratio, epsilon=3.e-3, weights=None, center=0., offset=None):
     r"""Estimating equations for Elastic-Net regression. Elastic-Net applies both L1- and L2-regularization at a
     pre-specified ratio. Notice that the L1 penalty is based on an approximation. See ``ee_lasso_regression`` for
     further details on the approximation for the L1 penalty.
 
-    Note
-    ----
-    As the derivative of the estimating equation for LASSO is not defined at :math:`\theta=0`, the bread (and sandwich)
-    cannot be used to estimate the variance in all settings.
-
-
     The estimating equation for Elastic-Net linear regression with the approximate L1 penalty is
 
     .. math::
 
         \sum_{i=1}^n \left\{ (Y_i - X_i^T \theta) X_i - \lambda r (1 + \epsilon)
         | \theta |^{\epsilon} sign(\theta) - \lambda (1-r) \theta \right\} = 0
 
     where :math:`\lambda` is the penalty term and :math:`r` is the ratio for the L1 vs L2 penalty.
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
+    Note
+    ----
+    As the derivative of the estimating equation for LASSO is not defined at :math:`\theta=0`, the bread (and sandwich)
+    cannot be used to estimate the variance in all settings.
+
+
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Note
     ----
     The 'strength' of the penalty term is indicated by :math:`\lambda`, which is the ``penalty`` argument scaled (or
     divided by) the number of observations.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented via ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     penalty : int, float, ndarray, list, vector
         Penalty term to apply to all coefficients (if only a integer or float is provided) or the corresponding
         coefficient (if a list or vector of integers or floats is provided). Note that the penalty term should either
-        consists of a single value or b values (to match the length of ``theta``). The penalty is scaled by n.
+        consists of a single value or `b` values (to match the length of ``theta``). The penalty is scaled by `n`.
     ratio : float
         Ratio for the L1 vs L2 penalty in Elastic-net. The ratio must be be :math:`0 \le r \le 1`. Setting ``ratio=1``
         results in LASSO and ``ratio=0`` results in ridge regression.
     epsilon : float, optional
         Approximation error to use for the LASSO approximation. Default argument is ``0.003``, which results in a
-        bridge penalty of 1.0003.
+        bridge penalty of ``1.0003``.
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ```None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input theta and y
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_elasticnet_regression`` should be done similar to the
     following
 
     >>> import numpy as np
@@ -1124,56 +1093,56 @@
 
     .. math::
 
         \sum_{i=1}^n \left\{ (Y_i - X_i^T \theta) X_i - \lambda \gamma | \theta |^{\gamma - 1} sign(\theta) \right\} = 0
 
     where :math:`\lambda` is the penalty term and :math:`\gamma` is a tuning parameter.
 
-    Here, :math:`\theta` is a 1-by-b array, where b is the distinct covariates included as part of X. For example, if
-    X is a 3-by-n matrix, then :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary
-    number of X's (as long as there is enough support in the data).
+    Here, :math:`\theta` is a 1-by-`b` array, which corresponds to the coefficients in the corresponding regression
+    model and `b` is the distinct covariates included as part of ``X``. For example, if ``X`` is a 3-by-`n` matrix, then
+    :math:`\theta` will be a 1-by-3 array. The code is general to allow for an arbitrary number of elements in ``X``.
 
     Note
     ----
     The 'strength' of the penalty term is indicated by :math:`\lambda`, which is the ``penalty`` argument scaled (or
     divided by) the number of observations.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in this case consists of b values. Therefore, initial values should consist of the same number as the
+        Theta in this case consists of `b` values. Therefore, initial values should consist of the same number as the
         number of columns present. This can easily be implemented via ``[0, ] * X.shape[1]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     penalty : int, float, ndarray, list, vector
         Penalty term to apply to all coefficients (if only a integer or float is provided) or the corresponding
         coefficient (if a list or vector of integers or floats is provided). Note that the penalty term should either
-        consists of a single value or b values (to match the length of ``theta``). The penalty is scaled by n.
+        consists of a single value or `b` values (to match the length of ``theta``). The penalty is scaled by `n`.
     gamma : float
         Hyperparameter for the bridge penalty, defined for :math:`\gamma > 0`. However, only :math:`\gamma \ge 1` are
         supported.
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``
+        Returns a `b`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_bridge_regression`` should be done similar to the
     following
 
     >>> import numpy as np
@@ -1300,52 +1269,52 @@
     Note
     ----
     Originally, GAMs were implemented via splines with a knot at each unique values of :math:`X`. More recently, GAMs
     use a more moderate amount of knots to improve computationally efficiency. Both versions can be implemented by
     ``ee_additive_regression`` through setting the knot locations.
 
 
-    Here, :math:`\theta` is a 1-by-(b+k) array, where b is the distinct covariates included as part of X and the k
-    distinct spline basis functions. For example, if X is a 2-by-n matrix with a 10-knot natural spline for the second
-    column in X, then :math:`\theta` will be a 1-by-(2+9) array. The code is general to allow for an arbitrary
-    number of X variables and spline knots.
+    Here, :math:`\theta` is a 1-by-(`b`+`k`) array, where `b` is the distinct covariates included as part of ``X`` and
+    the `k` distinct spline basis functions. For example, if ``X`` is a 2-by-`n` matrix with a 10-knot natural spline
+    for the second column in X, then :math:`\theta` will be a 1-by-(2+9) array. The code is general to allow for an
+    arbitrary number of X variables and spline knots.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        Parameter values. Number of values should match the number of columns in the additive design matrix.
+        Theta in this case consists of `b`+`k` values. Number of values should match the number of columns in the
+        additive design matrix.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     y : ndarray, list, vector
-        1-dimensional vector of n observed values.
+        1-dimensional vector of `n` observed values.
     specifications : list, dict, None
         A list of dictionaries that define the hyperparameters for the spline (e.g., number of knots, strength of
         penalty). For terms that should not have splines, ``None`` should be specified instead (see examples below).
-        Each dictionary supports the following parameters:
-        "knots", "natural", "power", "penalty"
-        * knots (list): controls the position of the knots, with knots are placed at given locations. There is no
-            default, so must be specified by the user.
-        * natural (bool): controls whether to generate natural (restricted) or unrestricted splines.
-            Default is ``True``, which corresponds to natural splines.
-        * power (float): controls the power to raise the spline terms to. Default is 3, which corresponds to cubic
-            splines.
-        * penalty (float): penalty term (:math:`\lambda`) applied to each corresponding spline basis term. Default is 0,
-            which applies no penalty to the spline basis terms.
+        Each dictionary supports the following parameters: "knots", "natural", "power", "penalty"
+        knots (list): controls the position of the knots, with knots are placed at given locations. There is no
+        default, so must be specified by the user.
+        natural (bool): controls whether to generate natural (restricted) or unrestricted splines.
+        Default is ``True``, which corresponds to natural splines.
+        power (float): controls the power to raise the spline terms to. Default is 3, which corresponds to cubic
+        splines.
+        penalty (float): penalty term (:math:`\lambda`) applied to each corresponding spline basis term. Default is 0,
+        which applies no penalty to the spline basis terms.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
     offset : ndarray, list, vector, None, optional
-        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
+        A 1-dimensional offset to be included in the model. Default is ``None``, which applies no offset term.
 
     Returns
     -------
     array :
-        Returns a (b+k)-by-n NumPy array evaluated for the input ``theta``
+        Returns a (`b`+`k`)-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_additive_regression`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -1568,14 +1537,23 @@
     else:                                   # Else results in error
         raise ValueError("Invalid input:", model,
                          ". Please select: 'linear', 'logistic', or 'poisson'.")
     return transform
 
 
 def _inverse_link_(betax, link):
+    """Internal function to return the evaluated inverse link and derivative of the inverse link.
+
+    Parameters
+    ----------
+    betax : ndarray, list, array
+        Parameter values
+    link : str
+        Specified link function
+    """
     # Distributions not implemented: power, inverse power
     if link == 'identity':
         py = identity(betax)                    # Inverse link
         dpy = 1                                 # Derivative of inverse link
     elif link == 'log':
         py = np.exp(betax)                      # Inverse link
         dpy = py                                # Derivative of inverse link
@@ -1608,14 +1586,27 @@
         dpy = 2 * betax                         # Derivative of inverse link
     else:
         raise ValueError("invalid link")
     return py, dpy
 
 
 def _distribution_variance_(dist, mu, hyperparameter=None, alpha=None):
+    """Internal function to return the distribution variance for GLM specifications.
+
+    Parameters
+    ----------
+    dist : str
+        Distribution
+    mu :
+        Prediction
+    hyperparameter : int, float, None, optional
+        Hyperparameter for the Tweedie distribution
+    alpha : int, float, None, optional
+        Hyperparameter for gamma or negative-binomial
+    """
     if dist in ['normal', 'gaussian']:
         v = 1
     elif dist == 'poisson':
         v = mu
     elif dist in ['binomial', 'bin', 'bernoulli']:
         v = mu - mu**2
     elif dist == 'gamma':
```

### Comparing `delicatessen-2.1/delicatessen/estimating_equations/survival.py` & `delicatessen-2.2/delicatessen/estimating_equations/survival.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,34 +23,28 @@
     Here, :math:`\theta` is a single parameter that corresponds to the scale parameter for the exponential distribution.
     The hazard from the exponential model is parameterized as the following
 
     .. math::
 
         h(t) = \lambda
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
-
     Parameters
     ----------
     theta : ndarray, list, vector
         Theta in the case of the exponential model consists of a single value. Furthermore, the parameter will be
         non-negative. Therefore, an initial value like the ``[1, ]`` should be provided.
     t : ndarray, list, vector
-        1-dimensional vector of n observed times.
+        1-dimensional vector of `n` observed times.
     delta : ndarray, list, vector
-        1-dimensional vector of n event indicators, where 1 indicates an event and 0 indicates right censoring.
+        1-dimensional vector of `n` event indicators, where 1 indicates an event and 0 indicates right censoring.
 
     Returns
     -------
     array :
-        Returns a 1-by-n NumPy array evaluated for the input ``theta``
+        Returns a 1-by-`n` NumPy array evaluated for the input ``theta``
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_exponential_model`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -117,36 +111,30 @@
     Here, :math:`\theta` consists of two parameters for the Weibull model: the scale (:math:`\lambda`) and the shape
     (:math:`\gamma`). The hazard from the Weibull model is parameterized as the following
 
     .. math::
 
         h(t) = \lambda \gamma t^{\gamma - 1}
 
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
-
-
     Parameters
     ----------
     theta : ndarray, list, vector
-        Theta in the case of the exponential model consists of a single value. Furthermore, the parameter will be
+        Theta in the case of the Weibull model consists of two values. Furthermore, the parameter will be
         non-negative. Therefore, an initial value like the ``[1, ]`` is recommended.
     t : ndarray, list, vector
-        1-dimensional vector of n observed times. No missing data should be included (missing data may cause
+        1-dimensional vector of `n` observed times. No missing data should be included (missing data may cause
         unexpected behavior).
     delta : ndarray, list, vector
-        1-dimensional vector of n event indicators, where 1 indicates an event and 0 indicates right censoring. No
+        1-dimensional vector of `n` event indicators, where 1 indicates an event and 0 indicates right censoring. No
         missing data should be included (missing data may cause unexpected behavior).
 
     Returns
     -------
     array :
-        Returns a 2-by-n NumPy array evaluated for the input theta.
+        Returns a 2-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_weibull_model`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -250,15 +238,15 @@
         density (``'risk'``), hazard (``'hazard'``), or cumulative hazard (``'cumulative_hazard'``).
     scale : float, int
         The estimated scale parameter from the Weibull model. From ``ee_weibull_model``, will be the first element.
 
     Returns
     -------
     array :
-        Returns a t-by-n NumPy array evaluated for the input ``theta``
+        Returns a `t`-by-`n` NumPy array evaluated for the input ``theta``
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_exponential_model`` and ``ee_exponential_measure`` should be done
     similar to the following. First, we will estimate the survival at time 5.
 
     >>> import numpy as np
@@ -372,16 +360,16 @@
     Note
     ----
     For proper uncertainty estimation, this estimating equation is meant to be stacked with ``ee_weibull_model``.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        theta consists of t values. The initial values should consist of the same number of elements as provided in the
-        ``times`` argument.
+        theta consists of `t` values. The initial values should consist of the same number of elements as provided in
+        the ``times`` argument.
     times : int, float, ndarray, list, vector
         A single time or 1-dimensional collection of times to calculate the measure at. The number of provided times
         should consist of the same number of elements as provided in the ``theta`` argument.
     n : int
         Number of observations in the input data. This argument ensures that the dimensions of the estimating equation
         are correct given the number of observations in the data.
     measure : str
@@ -392,15 +380,15 @@
     shape :
         The estimated shape parameter from the Weibull model. From ``ee_weibull_model``, will be the second (last)
         element.
 
     Returns
     -------
     array :
-        Returns a t-by-n NumPy array evaluated for the input ``theta``
+        Returns a `t`-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_weibull_model`` and ``ee_weibull_measure`` should be done
     similar to the following. First, we will estimate the survival at time 5.
 
     >>> import numpy as np
@@ -542,42 +530,37 @@
         = 0
 
     The AFT consists of the following parameters: :math:`\mu, \beta, \sigma`. The above
     estimating equations use the proportional hazards form of the Weibull model. For the Weibull AFT, notice the
     following relation between the coefficients: :math:`\lambda = - \mu \gamma`,
     :math:`\beta_{PH} = - \beta_{AFT} \gamma`, and :math:`\gamma = \exp(\sigma)`.
 
-    Here, :math:`\theta` is a 1-by-(2+b) array, where b is the distinct covariates included as part of X. For example,
-    if X is a 3-by-n matrix, then theta will be a 1-by-5 array. The code is general to allow for an arbitrary number of
-    X's (as long as there is enough support in the data).
-
-    Note
-    ----
-    All provided estimating equations are meant to be wrapped inside a user-specified function. Throughtout, these
-    user-defined functions are defined as ``psi``.
+    Here, :math:`\theta` is a 1-by-(2+`b`) array, where `b` is the distinct covariates included as part of ``X``. For
+    example, if ``X`` is a 3-by-`n` matrix, then theta will be a 1-by-5 array. The code is general to allow for an
+    arbitrary dimension of ``X``.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        theta consists of 1+b+1 values. Therefore, initial values should consist of the same number as the number of
+        theta consists of 1+`b`+1 values. Therefore, initial values should consist of the same number as the number of
         columns present in ``X`` plus 2. This can easily be implemented via
         ``[0, ] + [0, ] * X.shape[1] + [0, ]``.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     t : ndarray, list, vector
-        1-dimensional vector of n observed times.
+        1-dimensional vector of `n` observed times.
     delta : ndarray, list, vector
-        1-dimensional vector of n values indicating whether the time was an event or censoring.
+        1-dimensional vector of `n` values indicating whether the time was an event or censoring.
     weights : ndarray, list, vector, None, optional
-        1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
+        1-dimensional vector of `n` weights. Default is ``None``, which assigns a weight of 1 to all observations.
 
     Returns
     -------
     array :
-        Returns a b-by-n NumPy array evaluated for the input ``theta``.
+        Returns a 1+`b`+1-by-`n` NumPy array evaluated for the input ``theta``.
 
     Examples
     --------
     Construction of a estimating equation(s) with ``ee_aft_weibull`` should be done similar to the following
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -707,35 +690,35 @@
     ----
     For proper uncertainty estimation, this estimating equation is meant to be stacked together with the corresponding
     Weibull AFT model.
 
     Parameters
     ----------
     theta : ndarray, list, vector
-        theta consists of t values. The initial values should consist of the same number of elements as provided in the
+        theta consists of `t` values. The initial values should consist of the same number of elements as provided in the
         ``times`` argument.
     times : int, float, ndarray, list, vector
         A single time or 1-dimensional collection of times to calculate the measure at. The number of provided times
         should consist of the same number of elements as provided in the ``theta`` argument.
     X : ndarray, list, vector
-        2-dimensional vector of n observed values for b variables.
+        2-dimensional vector of `n` observed values for `b` variables.
     measure : str
         Measure to calculate. Options include survival (``'survival'``), density (``'density'``), risk or the cumulative
         density (``'risk'``), hazard (``'hazard'``), or cumulative hazard (``'cumulative_hazard'``).
     mu : float, int
         The estimated scale parameter from the Weibull AFT. From ``ee_aft_weibull``, will be the first element.
     beta :
         The estimated scale coefficients from the Weibull AFT. From ``ee_aft_weibull``, will be the middle element(s).
     sigma :
         The estimated shape parameter from the Weibull AFT. From ``ee_aft_weibull``, will be the last element.
 
     Returns
     -------
     array :
-        Returns a t-by-n NumPy array evaluated for the input theta
+        Returns a `t`-by-`n` NumPy array evaluated for the input theta
 
     Examples
     --------
     Construction of a estimating equations for :math:`S(t=5)` with ``ee_aft_weibull_measure`` should be done similar to
     the following
 
     >>> import numpy as np
```

### Comparing `delicatessen-2.1/delicatessen/mestimation.py` & `delicatessen-2.2/delicatessen/mestimation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,94 +1,99 @@
-import warnings
+#####################################################################################################################
+# Implementation of the M-estimator
+#####################################################################################################################
 
 import numpy as np
 from scipy.optimize import newton, root
-from scipy.misc import derivative
-from scipy.optimize import approx_fprime
 from scipy.stats import norm
 
-from delicatessen.derivative import auto_differentiation
+from delicatessen.sandwich import compute_bread, compute_meat, build_sandwich
 
 
 class MEstimator:
     r"""M-Estimator for stacked estimating equations.
 
-    M-Estimation, or loosely referred to as estimating equations, is a general approach to point and variance
-    estimation that consists of defining an estimator as the solution to an estimating equation. M-estimators
-    satisify the following
+    Estimating equations are a general approach to point and variance estimation that consists of defining an estimator
+    as the solution to a vector of equations that are equal to zero. The corresponding estimators, often called
+    M-estimators or Z-estimators, satisify the following equation
 
     .. math::
 
         \sum_{i=1}^n \psi(O_i, \hat{\theta}) = 0
 
     where :math:`\psi` is the :math:`v`-dimensional vector of estimating equation(s), :math:`\hat{\theta}` is the
     :math:`v`-dimensional parameter vector, and :math:`O_i` is the observed data (where units are independent but not
     necessarily identically distributed).
 
     Note
     ----
-    M-Estimation is advantageous in both theoretical and applied research. M-estimation simplifies proofs of
+    Estimating equations are advantageous in both theoretical and applied research. They simplifies proofs of
     consistency and asymptotic normality of estimators under a large-sample approximation framework. In application,
-    M-estimators simplify estimation of the variance of parameters and automate the delta-method.
+    this approach simplifies variance estimation and automates the delta-method.
 
 
-    M-Estimation consists of two broad step: point estimation and variance estimation. Point estimation is carried out
-    by determining the values of :math:`\theta` where the sum of the estimating equations are zero. For variance
-    estimation, the asymptotic sandwich variance estimator is used, which consists of
+    M-Estimators consists of two broad step: point estimation and variance estimation. Point estimation is carried out
+    by determining the values of :math:`\theta` where the sum of the estimating equations are zero. This is done via
+    standard root-finding algorithms.
+
+    For variance estimation, sandwich variance estimator is used. The asymptotic sandwich variance estimator consists of
 
     .. math::
 
-        B_n(O, \hat{\theta})^{-1} F_n(O, \hat{\theta}) \left\{B_n(O, \hat{\theta}^{-1})\right\}^T
+        V_n(O, \hat{\theta}) = B_n(O, \hat{\theta})^{-1} F_n(O, \hat{\theta}) \left\{B_n(O, \hat{\theta}^{-1})\right\}^T
 
-    where :math:`B` is the 'bread' and :math:`F` is the 'filling'
+    where :math:`B` is the 'bread' and :math:`F` is the 'filling' matrix. These matrices are defined as
 
     .. math::
 
-        B_n(O, \hat{\theta}) = n^{-1} \sum_{i=1}^{n} - \psi'(O_i, \hat{\theta})
+        B_n(O, \hat{\theta}) = n^{-1} \sum_{i=1}^{n} - \frac{\partial}{\partial \theta} \psi(O_i, \hat{\theta})
 
     .. math::
 
         F_n(O, \hat{\theta}) = n^{-1} \sum_{i=1}^{n} \psi(O_i, \hat{\theta}) \psi(O_i, \hat{\theta})^T
 
-    The partial derivatives for the bread are calculated using either numerical approximation (i.e., central difference
-    method) or forward-mode automatic differentiation. Inverting the bread is done via NumPy's ``linalg.pinv``. For
-    the filling, the dot product is taken at :math:`\hat{\theta}`.
+    respectively. The partial derivatives for the bread are calculated using either numerical approximation (e.g.,
+    forward difference method) or forward-mode automatic differentiation. Inverting the bread is done via NumPy's
+    ``linalg.pinv``. For the filling, the dot product is taken at :math:`\hat{\theta}`.
 
     Note
     ----
-    A hard part, that must be done by the user, is to specify the estimating equations. Be sure to check the provided
-    examples for the expected format. Pre-built estimating equations for common problems are also made available.
+    The difficult part (that must be done by the user) is to specify the estimating equations. Be sure to check the
+    provided examples for the expected format. Pre-built estimating equations for common problems are also made
+    available.
 
 
     After completion of these steps, point and variance estimates are stored. These can be extracted from
-    ``MEstimator``.
+    ``MEstimator``. Further, confidence intervals, Z-scores, P-values, or S-values can all be generated.
 
     Note
     ----
     For complex regression problems, the root-finding algorithms are not as robust relative to maximization approaches.
-    A solution for difficult problems is to 'pre-wash' the initial values.
+    A simple solution for difficult problems is to 'pre-wash' or find the solution to the equations and provide those
+    as the initial starting values.
 
     Parameters
     ----------
     stacked_equations : function, callable
-        Function that returns a b-by-n NumPy array of the estimating equations. See provided examples in the
+        Function that returns a `v`-by-`n` NumPy array of the estimating equations. See provided examples in the
         documentation for how to construct a set of estimating equations.
     init : list, set, array
-        Initial values for the root-finding algorithm.
+        Initial values for the root-finding algorithm. A total of `v` values should be provided.
     subset : list, set, array, None, optional
         Optional argument to conduct the root-finding procedure on a subset of parameters in the estimating equations.
         The input list is used to location index the parameter array via ``np.take()``. The subset list will
         only affect the root-finding procedure (i.e., the sandwich variance estimator ignores the subset argument).
         Default is ``None``, which runs the root-finding procedure for all parameters in the estimating equations.
 
     Note
     ----
-    Because the root-finding procedure is NOT ran for parameters outside of the subset, those coefficients must be
-    solved outside of ``MEstimator``. In general, I do NOT recommend using the ``subset`` argument unless a series of
-    complex estimating equations need to be solved.
+    Because the root-finding procedure is NOT ran for parameters outside of the subset, those coefficients *must* be
+    solved outside of ``MEstimator``. In general, I do *NOT* recommend using the ``subset`` argument unless a series of
+    complex estimating equations need to be solved. In general, this argument does not massively improve speed until
+    the estimating equations consist of hundreds of parameters.
 
     Examples
     --------
     Loading necessary functions and building a generic data set for estimation of the mean
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -111,34 +116,38 @@
 
     Inspecting the output results
 
     >>> estr.theta                                  # Point estimates
     >>> estr.variance                               # Covariance
     >>> estr.asymptotic_variance                    # Asymptotic covariance
     >>> np.sqrt(np.diag(estr.asymptotic_variance))  # Standard deviation
+    >>> estr.variance                               # Covariance
     >>> np.sqrt(np.diag(estr.variance))             # Standard error
     >>> estr.confidence_intervals()                 # Confidence intervals
+    >>> estr.z_scores()                             # Z-scores
+    >>> estr.p_values()                             # P-values
+    >>> estr.s_values()                             # S-values
 
     Alternatively, a custom estimating equation can be specified. This is done by constructing a valid estimating
-    equation for the ``MEstimator``. The ``MEstimator`` expects the ``psi`` function to return a b-by-n array, where b
-    is the number of parameters (length of ``theta``) and n is the total number of observations. Below is an example
-    of the mean and variance estimating equation from before
+    equation for the ``MEstimator``. The ``MEstimator`` expects the ``psi`` function to return a `v`-by-`n` array,
+    where `v` is the number of parameters (length of ``theta``) and n is the total number of observations. Below is an
+    example of the mean and variance estimating equation from before, but implemented by-hand
 
     >>> def psi(theta):
     >>>     y = np.array(y_dat)
     >>>     mean = y - theta[0]
     >>>     variance = (y - theta[0]) ** 2 - theta[1]
     >>>     return mean, variance
 
     The M-estimation procedure is called using the same approach as before
 
     >>> estr = MEstimator(stacked_equations=psi, init=[0, 0, ])
     >>> estr.estimate()
 
-    Note that ``len(init)`` should be equal to b. So in this case, two initial values are provided.
+    Note that ``len(init)`` should be equal to `v`. So in this case, two initial values are provided.
 
     ``MEstimator`` can also be run with a user-provided root-finding algorithm. To specify a custom root-finder, a
     function must be created by the user that consists of two keyword arguments (``stacked_equations``, ``init``) and
     must return only the optimized values. The following is an example with SciPy's Levenberg-Marquardt algorithm
     implemented in ``root``.
 
     >>> def custom_solver(stacked_equations, init):
@@ -150,20 +159,25 @@
 
     The provided custom root-finder can then be implemented like the following (continuing with the estimating equation
     from the previous example):
 
     >>> estr = MEstimator(stacked_equations=psi, init=[0, 0, ])
     >>> estr.estimate(solver=custom_solver)
 
+    For more examples on how to apply ``MEstimator``, see https://deli.readthedocs.io/en/latest/
+
     References
     ----------
     Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
     (pp. 297-337). Springer, New York, NY.
 
-    Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. The American Statistician, 56(1), 29-38.
+    Ross RK, Zivich PN, Stringer JSA, & Cole SR. (2024). M-estimation for common epidemiological measures: introduction
+    and applied examples. *International Journal of Epidemiology*, 53(2), dyae030.
+
+    Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
     """
     def __init__(self, stacked_equations, init=None, subset=None):
         self.stacked_equations = stacked_equations     # User-input stacked estimating equations
         self.init = init                               # User-input initial starting values for solving estimating eqs
         if subset is None:                             # Handling subset of parameters
             self._subset_ = subset                     # ... when None, set as None
         else:                                          # Otherwise
@@ -174,42 +188,46 @@
         self.theta = None                 # Optimized theta values (calculated later)
         self.bread = None                 # Bread from theta values (calculated later)
         self.meat = None                  # Meat from theta values (calculated later)
         self.variance = None              # Covariance matrix for theta values (calculated later)
         self.asymptotic_variance = None   # Asymptotic covariance matrix for theta values (calculated later)
 
     def estimate(self, solver='lm', maxiter=5000, tolerance=1e-9, deriv_method='approx', dx=1e-9, allow_pinv=True):
-        """Function to carry out the point and variance estimation of theta. After this procedure, the point estimates
-        (in ``theta``) and the covariance matrix (in ``variance``) can be extracted.
+        """Run the point and variance estimation procedures for given estimating equation and starting values. This
+        function carries out the point and variance estimation of ``theta``. After this procedure, the point estimates
+        (in ``theta``) and the covariance matrix (in ``variance``) can be extracted from the ``MEstimator`` object.
 
         Parameters
         ----------
         solver : str, function, callable, optional
             Method to use for the root-finding procedure. Default is the Levenberg-Marquardt algorithm
-            (``scipy.optimize.root(method='lm')``). Other built-in option is the secant method
-            (``scipy.optimize.newton``), and a modification of the Powell hybrid method
-            (``scipy.optimize.root(method='hybr')``). Finally, any generic root-finding algorithm can be used via a
-            user-provided callable object. The function must consist of two keyword arguments: ``stacked_equations``,
-            and ``init``. Additionally, the function should return only the optimized values. Please review the
-            provided example in the documentation for how to implement a custom root-finding algorithm.
+            (``scipy.optimize.root(method='lm')``, specified by ``solver='lm'``). Other built-in option is the secant
+            method (``scipy.optimize.newton``, specified by ``solver='newton'``), and a modification of the Powell
+            hybrid method (``scipy.optimize.root(method='hybr')``, specified by ``solver='hybr'``). Finally, any generic
+            root-finding algorithm can be used via a user-provided callable object. The function must consist of two
+            keyword arguments: ``stacked_equations``, and ``init``. Additionally, the function should return only the
+            optimized values. Please review the provided example in the documentation for how to implement a custom
+            root-finding algorithm.
         maxiter : int, optional
             Maximum iterations to consider for the root finding procedure. Default is 5000 iterations. For complex
-            estimating equations (without preceding optimization), this value may need to be increased. This argument
-            is not used for user-specified solvers.
+            estimating equations, this value may need to be increased. This argument is not used when a custom
+            root-finding method (e.g., ``solver``) is provided.
         tolerance : float, optional
-            Maximum tolerance for errors in the root finding. This argument is passed ``scipy.optimize`` via the
-            ``tol`` parameter. This argument is not used for user-specified solvers. Default is 1e-9.
+            Maximum tolerance for errors in the root finding in ``scipy.optimize``. Default is 1e-9. This argument is
+            not used when a custom root-finding method (e.g., ``solver``) is provided.
         deriv_method : str, optional
-            Method to compute the derivative of the estimating equations for the bread matrix. Options include numerical
-            approximation via the central difference method (``'approx'``) and forward-mode automatic differentiation
-            (``'exact'``). Default is ``'approx'``.
+            Method to compute the derivative of the estimating equations for the bread matrix. Default is ``'approx'``.
+            Options include numerical approximation via the forward difference method via SciPy (``'approx'``), forward
+            difference as implemented in delicatessen (`'fapprox'`), backward difference as implemented in delicatessen
+            (`'bapprox'`), central difference implemented as in delicatessen (`'capprox'`), or forward-mode automatic
+            differentiation as implemented in delicatessen(``'exact'``).
         dx : float, optional
-            Spacing to use to numerically approximate the partial derivatives of the bread matrix. Here, a small value
-            for ``dx`` should be used, since some large values can result in poor approximations. This argument is only
-            used when ``deriv_method='approx'``. Default is 1e-9.
+            Spacing to use to numerically approximate the partial derivatives of the bread matrix. Default is 1e-9.
+            Here, a small value for ``dx`` should be used, since some large values can result in poor approximations.
+            This argument is only used with numerical approximation methods.
         allow_pinv : bool, optional
             Whether to allow for the pseudo-inverse (via ``numpy.linalg.pinv``) if the bread matrix is determined to be
             non-invertible. If you want to disallow the pseudo-inverse (i.e., use ``numpy.linalg.inv``), set this
             argument to ``False``. Default is ``True``, which  is more robust to the possible bread matrices.
 
         Returns
         -------
@@ -261,18 +279,17 @@
         # To allow for optimization of only a subset of parameters in the estimating equation (in theory meant to
         #   simplify the process of complex stacked estimating equations where pre-washing can be done effectively),
         #   we do some internal processing. Essentially, we 'freeze' the parameters outside of self._subset_ as their
         #   inits, and let the root-finding procedure update the self._subset_ parameters. We do this by subsetting out
         #   the init values then passing them along to root(). Behind the scenes, self._mestimation_answer_() expands
         #   the parameters (to include everything), calculates the estimating equation at those values, and then
         #   extracts the corresponding subset.
-        #   This process only takes place within Step 1 (the sandwich variance did not require any corresponding
-        #   updates). There is an inherent danger with this process in that if non-subset parameters are not pre-washed,
-        #   then the returned parameters will not be correct. I am considering adding a warning for self_subset_, but I
-        #   may just have to trust the user...
+        #   This process only takes place within Step 1. There is an inherent danger with this process in that if
+        #   non-subset parameters are not pre-washed, then the returned parameters will not be correct. I am
+        #   considering adding a warning for self_subset_, but I currently just trust the user...
 
         # Processing initial values based on whether subset option was specified
         if self._subset_ is None:                        # If NOT subset,
             inits = self.init                            # ... give all initial values
         else:                                            # If subset,
             inits = np.take(self.init, self._subset_)    # ... then extract initial values for the subset
 
@@ -288,44 +305,40 @@
         if self._subset_ is None:                        # If NOT subset,
             self.theta = slv_theta                       # ... then use the full output/solved theta
         else:                                            # If subset,
             self.theta = np.asarray(self.init)           # ... copy the initial values
             for s, n in zip(self._subset_, slv_theta):   # ... then look over the subset and input theta
                 self.theta[s] = n                        # ... and update the subset to the output/solved theta
 
-        # STEP 2: calculating Variance
+        # STEP 2: calculating the sandwich variance
+        # After solving for the parameters, we now can compute the empirical sandwich variance estimator. This is
+        #   done by compute the bread and meat matrices and then combining them. This is now done by a separate
+        #   functionalities within the `sandwich.py` file as of v2.2.
         # STEP 2.1: baking the Bread
-        self.bread = self._bread_matrix_(theta=self.theta,                           # Provide theta-hat
-                                         method=deriv_method,                        # Method to use
-                                         dx=dx) / self.n_obs                         # Derivative approximation value
+        self.bread = compute_bread(stacked_equations=self.stacked_equations,
+                                   theta=self.theta,
+                                   deriv_method=deriv_method,
+                                   dx=dx) / self.n_obs
 
         # STEP 2.2: slicing the meat
-        evald_theta = np.asarray(self.stacked_equations(theta=self.theta))           # Evaluating EE at theta-hat
-        self.meat = np.dot(evald_theta, evald_theta.T) / self.n_obs                  # Meat is dot product of arrays
+        self.meat = compute_meat(stacked_equations=self.stacked_equations,
+                                 theta=self.theta) / self.n_obs
 
         # STEP 2.3: assembling the sandwich (variance)
-        if np.isnan(self.bread).any():
-            warnings.warn("The bread matrix contains at least one np.nan, so it cannot be inverted. The variance will "
-                          "not be calculated. This may be an issue with the provided estimating equations or the "
-                          "evaluated theta.",
-                          UserWarning)
+        self.asymptotic_variance = build_sandwich(bread=self.bread,
+                                                  meat=self.meat,
+                                                  allow_pinv=allow_pinv)
+        if self.asymptotic_variance is None:
+            self.variance = self.asymptotic_variance
         else:
-            if allow_pinv:                                                               # Support 1D theta-hat
-                bread_invert = np.linalg.pinv(self.bread)                                # ... find pseudo-inverse
-            else:                                                                        # Support 1D theta-hat
-                bread_invert = np.linalg.inv(self.bread)                                 # ... find inverse
-            sandwich = np.dot(np.dot(bread_invert, self.meat), bread_invert.T)           # Compute sandwich
-
-            # STEP 3: updating storage for results
-            self.asymptotic_variance = sandwich       # Asymptotic variance requires division by n (done above)
-            self.variance = sandwich / self.n_obs     # Variance estimate requires division by n^2 (second done here)
+            self.variance = self.asymptotic_variance / self.n_obs
 
     def confidence_intervals(self, alpha=0.05):
-        r"""Calculate Wald-type :math:`(1 - \alpha) \times` 100% confidence intervals using the point estimates and
-        the sandwich variance. The formula for the confidence intervals are
+        r"""Calculate two-sided Wald-type :math:`(1 - \alpha) \times` 100% confidence intervals using the point
+        and sandwich variance estimates. The formula for the confidence intervals is
 
         .. math::
 
             \hat{\theta} \pm z_{\alpha / 2} \times \widehat{SE}(\hat{\theta})
 
         Note
         ----
@@ -366,28 +379,28 @@
         r"""Calculate the Z-score using the point estimates and the sandwich variance. The formula for the Z score is
 
         .. math::
 
             \frac{\hat{\theta} - \theta}{\widehat{SE}(\hat{\theta})}
 
         where :math:`\theta` is the null. The ``.estimate()`` function must be called before the Z-scores can be
-        calculated.
+        calculated. Note that the default value for the null is zero.
 
         Parameters
         ----------
         null: int, float, ndarray, optional
             Null or reference for the the corresponding P-values. Default is 0.
 
         Returns
         -------
         array :
             Array of Z-scores for :math:`\theta_1, ..., \theta_b`, respectively
         """
         # Check that self.estimate() has been called
-        if self.theta is None:
+        if self.variance is None:
             raise ValueError("Either theta has not been estimated yet, or there is a np.nan in the bread matrix. "
                              "Therefore, z_scores() cannot be called.")
 
         # Calculating Z-scores
         se = np.sqrt(np.diag(self.variance))       # Extract the standard error estimates from the sandwich
         z_score = (self.theta - null) / se         # Compute the Z-score
         return z_score                             # Return the Z-score to the user
@@ -412,29 +425,29 @@
         z_score = self.z_scores(null=null)         # Calculating the Z-scores
         p_value = norm.sf(np.abs(z_score)) * 2     # Compute the corresponding P-values
         return p_value                             # Return P-values to the user
 
     def s_values(self, null=0):
         r"""Calculate two-sided Wald-type S-values using the point estimates and the sandwich variance. The S-value,
         or Shannon Information value, is a transformation of the P-values that has been argued to be more easily
-        interpretable as it can be related back to simple coin-flipping scenarios.
-
-        Suppose the S-value is :math:`s`. Then :math:`s` corresponds to the number of heads in a row with a fair coin
-        (equal chances heads or tails). As :math:`s` increases, one would be more 'surprised' by the result (e.g., it
-        might not be surprising to have two heads in a row, but it would be surprising for 10 in a row).
-
-        The transformation from a P-value into a S-value is.
+        interpretable as it can be related back to simple coin-flipping scenarios. The transformation from a P-value
+        into a S-value is.
 
         .. math::
 
             S = - \log_2(P)
 
         where :math:`P` is the corresponding P-value. The ``.estimate()`` function must be called before the S-values
         can be calculated.
 
+        The S-value can be contextualized in terms of coin-flips. Suppose the S-value is :math:`s`. Then :math:`s`
+        corresponds to the number of heads in a row with a fair coin (equal chances heads or tails). As :math:`s`
+        increases, one would be more 'surprised' by the result (e.g., it might not be surprising to have 2 heads in a
+        row, but it would be surprising for 20 in a row).
+
         Parameters
         ----------
         null: int, float, ndarray, optional
             Null or reference for the the corresponding S-values. Default is 0.
 
         Returns
         -------
@@ -476,33 +489,14 @@
                    ind=self._subset_,                  # ... go to the subset indices
                    v=theta)                            # ... then input current iteration values
 
         stacked_equations = np.asarray(self.stacked_equations(full_theta))  # Returning stacked equation
         return self._mestimator_sum_(stacked_equations=stacked_equations,   # Passing to evaluating function
                                      subset=self._subset_)                  # ... with specified subset
 
-    def _mestimation_answer_no_subset_(self, theta):
-        """Internal function to evaluate the sum of the estimating equations. The summation is internally evaluated
-        since access to the estimating functions is needed for the sandwich variance computations. This function is
-        used by the bread matrix computation procedure (since subset is ignored for the bread).
-
-        Parameters
-        ----------
-        theta : array
-            b-by-n matrix to sum over the values of n.
-
-        Returns
-        -------
-        array :
-            b-by-1 array, which is the sum over n for each b.
-        """
-        stacked_equations = np.asarray(self.stacked_equations(theta))       # Returning stacked equation
-        return self._mestimator_sum_(stacked_equations=stacked_equations,   # Passing to evaluating function
-                                     subset=None)                           # ... with always /no/ subset
-
     @staticmethod
     def _mestimator_sum_(stacked_equations, subset):
         """Function to evaluate the sum of the M-estimator over the :math:`n` units.
 
         Note
         ----
         Added in v1.0 to replace the inner functionality of ``_mestimation_answer_`` for the new ``approx_fprime`` but
@@ -539,16 +533,16 @@
             vals = np.asarray(vals)                    # ... converting to a NumPy array for ease
 
         # Return the calculated values of theta
         return vals
 
     @staticmethod
     def _solve_coefficients_(stacked_equations, init, method, maxiter, tolerance):
-        """Quasi-Newton solver for the values of theta, such that the estimating equations are equal to zero. Default
-        uses the secant method from SciPy's `newton` optimizer.
+        """Calls the root-finding procedure for the values of theta, such that the estimating equations are equal to
+        zero. Default uses the Levenberg-Marquardt algorithm from SciPy.
 
         Parameters
         ----------
         stacked_equations : function
             Function that contains the estimating equations
         init : array
             Initial values for the optimizer
@@ -602,55 +596,13 @@
             except TypeError:
                 raise TypeError("The user-specified root-finding `solver` must be a function (or callable object) with "
                                 "the following keyword arguments: `stacked_equations`, `init`.")
             if psi is None:
                 raise ValueError("The user-specified root-finding `solver` must return the solution to the "
                                  "optimization")
         else:
-            raise ValueError("The solver '" +  # ... otherwise throw ValueError
-                             str(method) +
-                             "' is not available. Please see the "
-                             "documentation for valid"
-                             "options for the optimizer.")
+            # ... otherwise throw ValueError if no other root-finding steps are triggered.
+            raise ValueError("The solver '" +  str(method) + "' is not available. Please see the "
+                             "documentation for valid options for the optimizer.")
 
         # Return optimized theta array
         return psi
-
-    def _bread_matrix_(self, theta, method, dx):
-        """Evaluate the bread matrix by taking all partial derivatives of the thetas in the estimating equation.
-
-        Parameters
-        ----------
-        theta : ndarray, float
-            Solved values of theta to evaluate at
-        dx : float
-            Spacing to use to numerically approximate the partial derivatives of the bread matrix.
-
-        Returns
-        -------
-        numpy.array
-        """
-        val_range = len(theta)                                       # Check how many values of theta there is
-        est_eq = self._mestimation_answer_no_subset_                 # Estimating equations to compute derivative of
-
-        # Compute the derivative
-        if method.lower() == "approx":                               # Numerical approximation method
-            if val_range == 1:                                       # When only a single theta is present
-                d = derivative(est_eq,                               # ... approximate the derivative
-                               theta, dx=dx)                         # ... at the solved theta (input)
-                bread_matrix = np.array([[d, ], ])                   # ... return as 1-by-1 array object for inversion
-            else:                                                    # Otherwise approximate the partial derivatives
-                bread_matrix = approx_fprime(xk=theta,               # ... use built-in jacobian functionality of SciPy
-                                             f=est_eq,               # ... with not-subset estimating equations
-                                             epsilon=dx)             # ... order option removed in v1.0
-
-        elif method.lower() == "exact":                              # Automatic Differentiation
-            bread_matrix = auto_differentiation(xk=theta,            # Compute the exact derivative at theta
-                                                f=est_eq)            # ... for the given estimating equations
-
-        else:                                                        # Error for unsupported option
-            raise ValueError("The input for deriv_method was "
-                             + str(method)
-                             + ", but only 'approx' and 'exact' are available.")
-
-        # Return bread (multiplied by negative 1 as in Stefanski & Boos)
-        return -1 * bread_matrix
```

### Comparing `delicatessen-2.1/delicatessen/utilities.py` & `delicatessen-2.2/delicatessen/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,55 @@
 import numpy as np
 import scipy as sp
 from scipy.stats import norm
 from delicatessen.derivative import PrimalTangentPairs as PTPair
 
 
 def logit(prob):
-    """Logistic transformation of probabilities. Returns log-odds
+    r"""Logistic transformation. Used to transform probabilities into log-odds.
+
+    .. math::
+
+        \log \left( \frac{p}{1-p} \right)
 
     Parameters
     ----------
     prob : float, ndarray
         A single probability or an array of probabilities
 
     Returns
     -------
-    logit-transformed probabilities
+    array :
+        logit-transformed values
     """
     return np.log(prob / (1 - prob))
 
 
 def inverse_logit(logodds):
-    """Inverse logistic transformation. Returns probabilities
+    r"""Inverse logistic transformation. Used to transform log-odds into probabilities.
+
+    .. math::
+
+        \frac{1}{1 + \exp(o)}
 
     Parameters
     ----------
     logodds : float, ndarray
         A single log-odd or an array of log-odds
 
     Returns
     -------
-    inverse-logit transformed results (i.e. probabilities for log-odds)
+    array :
+        inverse-logit transformed values
     """
     return 1 / (1 + np.exp(-logodds))
 
 
 def identity(value):
-    """Identity transformation. Returns itself
+    """Identity transformation. Used to transform input into itself (i.e., no transformation in applied).
 
     Note
     ----
     This function doesn't actually apply any transformation. It is used for arbitrary function calls that apply
     transformations, and this is called when no transformation is to be applied
 
     Parameters
@@ -52,15 +62,15 @@
     -------
     value
     """
     return value
 
 
 def polygamma(n, x):
-    """Polygamma functions. This is a wrapper function of ``scipy.special.polygamma`` meant to enable automatic
+    """Polygamma function. This is a wrapper function of ``scipy.special.polygamma`` meant to enable automatic
     differentation with ``delicatessen``. When the input is a ``PrimalTangentPairs`` object, then an internal function
     that implements the polygamma function is called. Otherwise, ``scipy.special.polygamma`` is called for the input
     object.
 
     Parameters
     ----------
     n : int
@@ -158,52 +168,52 @@
         return x.normal_pdf()
     else:
         return norm.pdf(x=x)
 
 
 def robust_loss_functions(residual, loss, k, a=None, b=None):
     r"""Loss functions for robust mean and robust regression estimating equations. This function is called internally
-    for ``ee_mean_robust`` and ``ee_robust_regression``. This function can also be loaded, so user's can easily adapt
+    for ``ee_mean_robust`` and ``ee_robust_regression``. This function can also be accessed, so user's can easily adapt
     their own regression models into robust regression models using the pre-defined loss functions.
 
     Note
     ----
-    The loss functions here are technically the first-order derivatives of the loss functions
+    The loss functions here are technically the first-order derivatives of the loss functions you see in the literature.
 
 
     The following score of the loss functions, :math:`f_k()`, are available.
 
     Andrew's Sine
 
     .. math::
 
-        f_k(x) = I(k \pi <= x <= k \pi) \times \sin(x/k)
+        f_k(x) = I(k \pi \le x \le k \pi) \times \sin(x/k)
 
     Huber
 
     .. math::
 
-        f_k(x) = x \times I(-k < x < k) + k \times (1 - I(-k < x < k)) \times \text{sign}(x)
+        f_k(x) = x I(-k < x < k) + \text{sign}(x) k (1 - I(-k < x < k))
 
     Tukey's biweight
 
     .. math::
 
-        f_k(x) = x \times I(-k < x < k) + x \left( 1 - (x/k)^2 \right)^2
+        f_k(x) = x I(-k < x < k) + x \left( 1 - (x/k)^2 \right)^2
 
     Hampel (Hampel's add two additional parameters, :math:`a` and :math:`b`)
 
     .. math::
 
-        f_k(x) =
+        f_{k,a,b}(x) =
         \begin{bmatrix}
             I(-a < x < a) \times x \\
-            + I(a \ge |x| < b) \times a \times \text{sign}(x) \\
-            + I(b \ge x < k) \times a \frac{k - x}{k - b} \\
-            + I(-b \le x > -k) \times -a \frac{-k + x}{-k + b} \\
+            + I(a \le |x| < b) \times a \times \text{sign}(x) \\
+            + I(b \le x < k) \times a \frac{k - x}{k - b} \\
+            + I(-k \ge x > -b) \times -a \frac{-k + x}{-k + b} \\
             + I(|x| \ge k) \times 0
         \end{bmatrix}
 
     Parameters
     ----------
     residual : ndarray, vector, list
         1-dimensional vector of n observed values. Input should consists of the residuals (the difference between the
@@ -311,31 +321,32 @@
     :math:`(1 - \alpha) \times` 100% confidence intervals from estimated coefficients and covariance of a regression
     model given a set of specific covariate values.
 
     This function is a helper function to compute the predictions from a regression model for a set of given :math:`X`
     values. Importantly, this method allows for the variance of :math:`\hat{Y}` to be estimated without having to expand
     the estimating equations. As such, this functionality is meant to be used after ``MEstimator`` has been used to
     estimate the coefficients (i.e., this function is for use after the M-estimator has computed the results for the
-    chosen regression model). Therefore, this function should be viewed as a post-processing functionality.
+    chosen regression model). Therefore, this function should be viewed as a post-processing functionality for
+    generating plots or tables.
 
     Note
     ----
     No tranformations are applied by this function. So, input from a logistic model will generate the *log-odds* of the
     outcome (not probability).
 
 
     Parameters
     ----------
     X : ndarray, list, vector
         2-dimensional vector of values to generate predicted variances for. The number of columns must match the number
         of coefficients / parameters in ``theta``.
     theta : ndarray
-        Estimated coefficients from ``delicatessen.MEstimator.theta``.
+        Estimated coefficients from ``MEstimator.theta``.
     covariance : ndarray
-        Estimated covariance matrix from ``delicatessen.MEstimator.variance``.
+        Estimated covariance matrix from ``MEstimator.variance``.
     offset : ndarray, None, optional
         A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
     alpha : float, optional
         The :math:`\alpha` level for the corresponding confidence intervals. Default is 0.05, which calculate the
         95% confidence intervals. Notice that :math:`0<\alpha<1`.
 
     Returns
@@ -444,17 +455,18 @@
 
     Restricted splines are generated via
 
     .. math::
 
         r_k(X) = I(X > k) \left\{ X - k \right\}^a - s_K(X)
 
-    where :math:`K` is largest knot value. Splines are normalized by the upper knot minus the lower knot to the
-    corresponding power. Normalizing the splines can be helpful for the root-finding procedure, but does change the
-    interpretation of the corresponding coefficients.
+    where :math:`K` is largest knot value.
+
+    Splines are normalized by the upper knot minus the lower knot to the corresponding power. Normalizing the splines
+    can be helpful for the root-finding procedure.
 
     Parameters
     ----------
     variable : ndarray, vector, list
         1-dimensional vector of observed values. Input should consists of the variable to generate spline terms for
     knots : ndarray, vector, list
         1-dimensional vector of pre-specified knot locations. All knots should be between the minimum and maximum
@@ -542,24 +554,24 @@
     X : ndarray, vector, list
         Input independent variable data.
     specifications : ndarray, vector, list
         A list of dictionaries that define the hyperparameters for the spline (e.g., number of knots, strength of
         penalty). For terms that should not have splines, ``None`` should be specified instead (see examples below).
         Each dictionary supports the following parameters:
         "knots", "natural", "power", "penalty"
-        * knots (list): controls the position of the knots, with knots are placed at given locations. There is no
-            default, so must be specified by the user.
-        * natural (bool): controls whether to generate natural (restricted) or unrestricted splines.
-            Default is ``True``, which corresponds to natural splines.
-        * power (float): controls the power to raise the spline terms to. Default is 3, which corresponds to cubic
-            splines.
-        * penalty (float): penalty term (:math:`\lambda`) applied to each corresponding spline basis term. Default is 0,
-            which applies no penalty to the spline basis terms.
-        * normalized (bool): whether to normalize the spline terms. Default is ``False``, with a default change coming
-            with v3.0 release.
+        knots (list): controls the position of the knots, with knots are placed at given locations. There is no
+        default, so must be specified by the user.
+        natural (bool): controls whether to generate natural (restricted) or unrestricted splines.
+        Default is ``True``, which corresponds to natural splines.
+        power (float): controls the power to raise the spline terms to. Default is 3, which corresponds to cubic
+        splines.
+        penalty (float): penalty term (:math:`\lambda`) applied to each corresponding spline basis term. Default is 0,
+        which applies no penalty to the spline basis terms.
+        normalized (bool): whether to normalize the spline terms. Default is ``False``, with a default change coming
+        with v3.0 release.
     return_penalty : bool, optional
         Whether the list of the corresponding penalty terms should also be returned. This functionality is used
         internally to create the list of penalty terms to provide the Ridge regression model, where only the spline
         terms are penalized. Default is False.
 
     Returns
     -------
```

### Comparing `delicatessen-2.1/delicatessen.egg-info/PKG-INFO` & `delicatessen-2.2/delicatessen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delicatessen
-Version: 2.1
+Version: 2.2
 Summary: Generalized M-Estimation
 Home-page: https://github.com/pzivich/Deli
 Author: Paul Zivich
 Author-email: zivich.5@gmail.com
 License: MIT
 Description: ![delicatessen](docs/images/delicatessen_header.png)
         
@@ -22,18 +22,18 @@
         **Citation**: Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-Estimation in Python.
         *arXiv:2203.11300* [stat.ME]
         
         
         ## M-Estimation and Estimating Equations
         
         Here, we provide a brief overview of M-estimation theory. For more detailed introductions to M-estimation, see Ross
-        et al. (2024) or Chapter 7 of Boos & Stefanski (2013). M-estimation is a generalization of likelihood-based methods.
-        *M-estimators* are solutions to estimating equations. To apply the M-estimator, we solve the estimating equations using
-        observed data. This is similar to other approaches, but the key advantage of M-Estimators is estimation of the variance
-        via the sandwich variance.
+        et al. (2024), Stefanski & Boos (2002), or Chapter 7 of Boos & Stefanski (2013). M-estimation is a generalization of
+        likelihood-based methods. *M-estimators* are solutions to estimating equations. To apply the M-estimator, we solve the
+        estimating equations using observed data. This is similar to other approaches, but the key advantage of M-Estimators is
+        variance estimation via the empirical sandwich variance estimator.
         
         While M-Estimation is a powerful tool, the derivatives and matrix algebra can quickly become unwieldy. This is where 
         `delicatessen` comes in. `delicatessen` takes estimating functions and data, and solves for the parameter estimates,
         computes the derivatives, and performs the matrix algebra calculations. Therefore, M-estimators can be more easily
         adopted without having to perform by-hand calculations. In other words, we can let the computer do the math for us.
         
         To further ease use, `delicatessen` also comes with a variety of built-in estimating equations. See
@@ -88,19 +88,19 @@
         at [delicatessen website](https://deli.readthedocs.io/en/latest/).
         
         ## References
         
         Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
         (pp. 297-337). Springer, New York, NY.
         
+        Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
+        
         Ross RK, Zivich PN, Stringer JS, & Cole SR. (2024). M-estimation for common epidemiological measures: introduction and
         applied examples. *International Journal of Epidemiology*, 53(2).
         
-        Stefanski LA, & Boos DD. (2002). The calculus of M-estimation. *The American Statistician*, 56(1), 29-38.
-        
         Zivich PN, Klose M, Cole SR, Edwards JK, & Shook-Sa BE. (2022). Delicatessen: M-Estimation in Python.
         *arXiv preprint arXiv:2203.11300*.
         
 Keywords: m-estimation sandwich-variance estimating-equations
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `delicatessen-2.1/delicatessen.egg-info/SOURCES.txt` & `delicatessen-2.2/delicatessen.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 delicatessen/__init__.py
 delicatessen/data.py
 delicatessen/derivative.py
 delicatessen/mestimation.py
+delicatessen/sandwich.py
 delicatessen/utilities.py
 delicatessen/version.py
 delicatessen.egg-info/PKG-INFO
 delicatessen.egg-info/SOURCES.txt
 delicatessen.egg-info/dependency_links.txt
 delicatessen.egg-info/requires.txt
 delicatessen.egg-info/top_level.txt
```

### Comparing `delicatessen-2.1/setup.py` & `delicatessen-2.2/setup.py`

 * *Files identical despite different names*

