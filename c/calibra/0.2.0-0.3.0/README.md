# Comparing `tmp/calibra-0.2.0.tar.gz` & `tmp/calibra-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibra-0.2.0.tar", last modified: Fri Mar  1 17:13:58 2024, max compression
+gzip compressed data, was "calibra-0.3.0.tar", last modified: Tue Apr 23 16:53:15 2024, max compression
```

## Comparing `calibra-0.2.0.tar` & `calibra-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 17:13:58.905100 calibra-0.2.0/
--rw-rw-rw-   0        0        0      173 2024-01-24 19:10:57.000000 calibra-0.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3648 2024-01-24 19:10:57.000000 calibra-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2024-01-24 19:10:57.000000 calibra-0.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1092 2024-01-24 19:10:57.000000 calibra-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      273 2024-01-24 19:10:57.000000 calibra-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1759 2024-03-01 17:13:58.905100 calibra-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      919 2024-01-24 19:10:57.000000 calibra-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-01 17:13:58.773727 calibra-0.2.0/calibra/
--rw-rw-rw-   0        0        0      134 2024-01-24 19:10:57.000000 calibra-0.2.0/calibra/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-24 19:37:39.000000 calibra-0.2.0/calibra/calibrators.py
--rw-rw-rw-   0        0        0     4647 2024-02-22 21:23:03.000000 calibra-0.2.0/calibra/errors.py
--rw-rw-rw-   0        0        0     1116 2024-02-22 21:23:26.000000 calibra-0.2.0/calibra/plotting.py
--rw-rw-rw-   0        0        0    12373 2024-02-27 09:17:55.000000 calibra-0.2.0/calibra/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-01 17:13:58.809210 calibra-0.2.0/calibra.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-03-01 17:13:58.000000 calibra-0.2.0/calibra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2024-03-01 17:13:58.000000 calibra-0.2.0/calibra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 17:13:58.000000 calibra-0.2.0/calibra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-24 19:23:17.000000 calibra-0.2.0/calibra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2024-03-01 17:13:58.000000 calibra-0.2.0/calibra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-01 17:13:58.000000 calibra-0.2.0/calibra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-01 17:13:58.892630 calibra-0.2.0/docs/
--rw-rw-rw-   0        0        0      628 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4937 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/history.rst
--rw-rw-rw-   0        0        0      324 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/index.rst
--rw-rw-rw-   0        0        0     1181 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2024-01-24 19:10:57.000000 calibra-0.2.0/docs/usage.rst
--rw-rw-rw-   0        0        0      448 2024-03-01 17:13:58.913194 calibra-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1342 2024-03-01 17:13:44.000000 calibra-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-01 17:13:58.903095 calibra-0.2.0/tests/
--rw-rw-rw-   0        0        0       38 2024-01-24 19:10:57.000000 calibra-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     9027 2024-02-22 21:21:42.000000 calibra-0.2.0/tests/test_errors.py
--rw-rw-rw-   0        0        0    22415 2024-02-21 22:30:04.000000 calibra-0.2.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.993701 calibra-0.3.0/
+-rw-rw-rw-   0        0        0      173 2024-01-24 19:10:57.000000 calibra-0.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3648 2024-01-24 19:10:57.000000 calibra-0.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-01-24 19:10:57.000000 calibra-0.3.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1092 2024-01-24 19:10:57.000000 calibra-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-01-24 19:10:57.000000 calibra-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-04-23 16:53:14.993701 calibra-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2024-01-24 19:10:57.000000 calibra-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.912011 calibra-0.3.0/calibra/
+-rw-rw-rw-   0        0        0      134 2024-01-24 19:10:57.000000 calibra-0.3.0/calibra/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 19:37:39.000000 calibra-0.3.0/calibra/calibrators.py
+-rw-rw-rw-   0        0        0     4665 2024-04-23 16:43:18.000000 calibra-0.3.0/calibra/errors.py
+-rw-rw-rw-   0        0        0    24536 2024-04-23 16:43:15.000000 calibra-0.3.0/calibra/plotting.py
+-rw-rw-rw-   0        0        0    15779 2024-04-23 16:36:15.000000 calibra-0.3.0/calibra/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.951023 calibra-0.3.0/calibra.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-24 19:23:17.000000 calibra-0.3.0/calibra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 16:53:14.000000 calibra-0.3.0/calibra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.974921 calibra-0.3.0/docs/
+-rw-rw-rw-   0        0        0      628 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4937 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1181 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2024-01-24 19:10:57.000000 calibra-0.3.0/docs/usage.rst
+-rw-rw-rw-   0        0        0      503 2024-04-23 16:53:15.001436 calibra-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-04-23 16:52:11.000000 calibra-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.987696 calibra-0.3.0/tests/
+-rw-rw-rw-   0        0        0       38 2024-01-24 19:10:57.000000 calibra-0.3.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:53:14.990698 calibra-0.3.0/tests/baseline/
+-rw-rw-rw-   0        0        0    31261 2024-04-23 16:33:55.000000 calibra-0.3.0/tests/baseline/test_plot.png
+-rw-rw-rw-   0        0        0    34731 2024-04-23 15:20:59.000000 calibra-0.3.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     5252 2024-03-22 19:03:42.000000 calibra-0.3.0/tests/test_errors.py
+-rw-rw-rw-   0        0        0    24645 2024-04-23 16:33:44.000000 calibra-0.3.0/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    17088 2024-03-22 20:26:09.000000 calibra-0.3.0/tests/test_utils.py
```

### Comparing `calibra-0.2.0/CONTRIBUTING.rst` & `calibra-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/LICENSE` & `calibra-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/PKG-INFO` & `calibra-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibra
-Version: 0.2.0
+Version: 0.3.0
 Summary: Toolkit for calibration of machine learning classifiers.
 Home-page: https://github.com/conorwalsh99/calibra
 Author: Conor Walsh
 Author-email: conorwalsh206@gmail.com
 License: MIT license
 Keywords: calibra
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `calibra-0.2.0/README.rst` & `calibra-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/calibra/errors.py` & `calibra-0.3.0/calibra/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         ) -> Union[float, tuple]:
     """ 
     Calculate the class-wise Expected Calibration Error (ECE) of a set of predictions.
 
     Args:
         y_pred (ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
-            Alternatively may be of shape (num_samples,) where i position is predicted probability of data point i belonging to class 1 (positive class).
+            Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
         y_true (ndarray):
             This 1-D array of length num_samples contains the true label for each data point.        
         num_bins (int):
             Number of bins the interval [0, 1] is divided into. Exact if method='width', approximate if method='frequency'.
         method (str):
             Method of splitting interval [0, 1] into bins. If set to 'width' divides the interval [0, 1] into num_bins bins of equal width.
             If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately num_samples/num_bins data points. 
@@ -77,15 +77,14 @@
             if bin_weight > 0:      
                 bin_deviation = _calculate_bin_deviation(bins[i][b])
                 weighted_bin_deviation = bin_weight * bin_deviation
                 errors[i] += weighted_bin_deviation 
     
     return errors
 
-      
 def _calculate_bin_deviation(bin: dict) -> float:
     """
     Calculate the deviation between the expected rate of occurrence and the actual rate of occurrence, for a given bin.
 
     Args:
         bin (dict):
             Dictionary containing the predicted probabilities for a given class and the number of occurrences of that class, for a given bin.
```

### Comparing `calibra-0.2.0/calibra/utils.py` & `calibra-0.3.0/calibra/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,75 @@
 import math
 import pandas as pd
 import numpy as np
+from typing import Callable, Any, List
+from functools import wraps
 
 
+def validate_input(func: Callable[..., Any]) -> Callable[..., Any]:
+    """
+    Validate the input parameters to ensure they are in the correct format. Convert to correct format where possible, otherwise, raise error.
+
+    Args:
+        func: The method for which we validate the input.
+
+    The decorator performs the following validations:
+    1. y_pred must be a 1D or 2D array with values between 0 and 1. It is converted to a NumPy array.
+    2. y_true must be a list or 1D array of non-negative whole numbers. It is converted to a NumPy array.
+    3. y_true and y_pred must have the same length.
+    4. num_bins must be a positive whole number.
+    5. method must be one of two specific string values ('width' or 'frequency').
+
+    Raises:
+      ValueError: If any of the inputs do not meet the validation criteria.
+
+    Returns:
+      The original function's return value, if all inputs are valid.
+    """    
+    @wraps(func)
+    def wrapper(y_pred, y_true, num_bins, method, *args, **kwargs):
+        
+        y_pred = np.asarray(y_pred)
+        if y_pred.ndim > 2 or np.any(y_pred < 0) or np.any(y_pred > 1):
+            raise ValueError("y_pred must be a 1D or 2D array with values between 0 and 1.")
+        
+        if isinstance(y_true, list):
+            if not all(label % 1 == 0 and label >= 0 for label in y_true):
+                raise ValueError("y_true must only contain non-negative whole numbers.")
+            y_true = np.array(y_true)
+
+        elif isinstance(y_true, np.ndarray):
+            if y_true.ndim != 1 or np.any(y_true % 1 != 0) or np.any(y_true < 0):
+                raise ValueError("y_true must be a list or 1D array of non-negative whole numbers.")
+        else:
+            raise TypeError("y_true must be either a list or a 1D numpy array.")
+
+        if y_true.size != y_pred.shape[0]:
+            raise ValueError("y_true and y_pred must have the same length.")
+        
+        if num_bins % 1 != 0 or num_bins <= 0:
+            raise ValueError("num_bins must be a positive whole number.")
+        num_bins = int(num_bins)
+        
+        if method not in ['width', 'frequency']:
+            raise ValueError("Method must be either 'width' or 'frequency'")
+
+        return func(y_pred, y_true, num_bins, method, *args, **kwargs)
+    return wrapper
+
+
+@validate_input
 def bin_probabilities(y_pred: np.ndarray, y_true: np.ndarray, num_bins: int, method: str = 'width') -> dict:
     """
     Group predictions into bins, along with corresponding true labels.
     
     Args:
         y_pred (ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
-            Alternatively may be of shape (num_samples,) where i position is predicted probability of data point i belonging to class 1 (positive class).
+            Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
         y_true (ndarray):
             This 1-D array of length num_samples contains the true label for each data point.        
         num_bins (int):
             Number of bins the interval [0, 1] is divided into. Exact if method='width', approximate if method='frequency'.
         method (str):
             Method of splitting interval [0, 1] into bins. If set to 'width' divides the interval [0, 1] into num_bins bins of equal width.
             If set to 'frequency' divides the interval [0, 1] into approximately num_bins bins, each containing approximately num_samples/num_bins data points. 
@@ -36,45 +91,41 @@
                 }
                 for j in range(num_bins)
             } 
             for i in range(num_classes)
         }
 
     if method == 'width':
-        bins = get_equal_width_bins(y_pred, y_true, num_classes, num_samples, num_bins, bins)
+        bins = _get_equal_width_bins(y_pred, y_true, num_classes, num_samples, num_bins, bins)
     elif method == 'frequency':
-        bins = get_equal_frequency_bins(y_pred, y_true, num_classes, num_samples, num_bins, bins)
-    else:
-        raise ValueError("Method must be 'width' or 'frequency'")
+        bins = _get_equal_frequency_bins(y_pred, y_true, num_classes, num_samples, num_bins, bins)
 
     return bins
 
-
 def _reshape_y_pred(y_pred: np.ndarray) -> np.ndarray:
     """
     If y_pred is a 1D array, reshape to (num_samples, num_classes)
 
     Args:
         y_pred (ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
-            Alternatively may be of shape (num_samples,) where i position is predicted probability of data point i belonging to class 1 (positive class).
+            Alternatively may be of shape (num_samples,) for binary classification where i position is predicted probability of data point i belonging to class 1 (positive class).
 
     Returns:
         ndarray
     """
     if np.asarray(y_pred).ndim == 1:
         y_pred = np.asarray(
             [
             [1 - prob, prob] for prob in y_pred
             ]
         )
 
     return y_pred
 
-
 def _get_bin_weight(bin: dict, num_samples: int) -> float:
     """
     Calculate the proportion of the overall dataset whose predictions lie in the given bin.
 
     Args:
         bin (dict):
             Dictionary containing the predicted probabilities for a given class and the number of occurrences of that class, for a given bin.
@@ -86,15 +137,15 @@
     """
     probs = bin['probs']
     num_trials = len(probs)
     weight = num_trials / num_samples
     return weight
 
 
-def get_equal_width_bins(y_pred: np.ndarray, y_true: np.ndarray, num_classes: int, num_samples: int, num_bins: int, bins: dict) -> dict:
+def _get_equal_width_bins(y_pred: np.ndarray, y_true: np.ndarray, num_classes: int, num_samples: int, num_bins: int, bins: dict) -> dict:
     """
     Group predictions into bins of equal width.
 
     Args:
         y_pred (ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
         y_true (ndarray):
@@ -116,22 +167,22 @@
         y_true_class_i = list(y_true == i) 
         bin_index = list(
             map(
                 lambda x: (num_bins-1) if x==1 else math.floor(num_bins * x), 
                     y_pred_class_i
                 )
             ) 
-        # returns num_bins-1 if p==1, else returns m for p in [(m-1)/num_bins, m/num_bins] 
+        # returns num_bins-1 if p==1, else returns m for p in [m/num_bins, (m+1)/num_bins) 
         for j in range(num_samples): 
             bins[i][bin_index[j]]['probs'].append(y_pred_class_i[j]) # group predicted probabilities into the bins
             bins[i][bin_index[j]]['num_occurrences'] += y_true_class_i[j] # keep track of the number of occurrences of class i in each bin
             
     return bins
 
-def get_equal_frequency_bins(y_pred: np.ndarray, y_true: np.ndarray, num_classes: int, num_samples: int, num_bins: int, bins: dict) -> dict:
+def _get_equal_frequency_bins(y_pred: np.ndarray, y_true: np.ndarray, num_classes: int, num_samples: int, num_bins: int, bins: dict) -> dict:
     """
     Group predictions into bins containing equal numbers of data points.
 
     Args:
         y_pred (ndarray):
             Array-like object of shape (num_samples, num_classes) where ij position is predicted probability of data point i belonging to class j.
         y_true (ndarray):
@@ -150,34 +201,34 @@
     """    
     lower_bound_freq = math.floor(num_samples / num_bins)
     upper_bound_freq = math.ceil(num_samples / num_bins)
 
     for i in range(num_classes):
         y_pred_class_i = y_pred[i].to_list()
         y_true_class_i = list(y_true == i)
-        y_pred_class_i_sorted, y_true_class_i_sorted = sort_predictions(y_pred_class_i, y_true_class_i)
+        y_pred_class_i_sorted, y_true_class_i_sorted = _sort_predictions(y_pred_class_i, y_true_class_i)
         # forward-fill bins up to upper bound 
-        bins = forward_fill_equal_frequency_bins(class_label=i, 
+        bins = _forward_fill_equal_frequency_bins(class_label=i, 
                                                 num_bins=num_bins, 
                                                 bins=bins, 
                                                 upper_bound_freq=upper_bound_freq, 
                                                 y_pred_class_i_sorted=y_pred_class_i_sorted, 
                                                 y_true_class_i_sorted=y_true_class_i_sorted)     
         # back-fill bins above lower bound
-        bins = back_fill_equal_frequency_bins(class_label=i,
+        bins = _back_fill_equal_frequency_bins(class_label=i,
                                             num_bins=num_bins,
                                             bins=bins,
                                             lower_bound_freq=lower_bound_freq)
         # calculate num_occurrences once bins filled satisfactorily
-        bins = sum_occurrences(class_label=i, num_bins=num_bins, bins=bins)
+        bins = _sum_occurrences(class_label=i, num_bins=num_bins, bins=bins)
     
     return bins
 
 
-def forward_fill_equal_frequency_bins(class_label: str, num_bins: int, bins: dict, upper_bound_freq: int, y_pred_class_i_sorted: list, y_true_class_i_sorted: list) -> dict:
+def _forward_fill_equal_frequency_bins(class_label: str, num_bins: int, bins: dict, upper_bound_freq: int, y_pred_class_i_sorted: list, y_true_class_i_sorted: list) -> dict:
     """
     For each bin in the given class, assign predictions until the upper limit of points per bin is reached.    
 
     Args:
         class_label (str):
             The class under consideration.
         num_bins (int):
@@ -198,15 +249,15 @@
     for b in range(num_bins):
         bins[i][b]['occurrences'] = [] # need to track the occurrence associated with each prediction because these may be redistributed to different bins later
         while len(bins[i][b]['probs']) < upper_bound_freq and len(y_pred_class_i_sorted) > 0:
             bins[i][b]['probs'].append(y_pred_class_i_sorted.pop(0))
             bins[i][b]['occurrences'].append(y_true_class_i_sorted.pop(0))
     return bins
 
-def back_fill_equal_frequency_bins(class_label: str, num_bins: int, bins: dict, lower_bound_freq: int) -> dict:
+def _back_fill_equal_frequency_bins(class_label: str, num_bins: int, bins: dict, lower_bound_freq: int) -> dict:
     """
     Redistribute predictions between bins so that each bin contains at least a specified minimum number of samples.
 
     For a given class, iterate backwards through the bins, continuously reassigning the final sample in the preceding bin to the given bin, 
     until the given bin contains at least a specified minimum number of points. If a bin already has at least this number of minimum points upon first inspection, 
     exit the loop.
 
@@ -232,15 +283,15 @@
         if len(bins[i][b]['probs']) >= lower_bound_freq:
             return bins
         while len(bins[i][b]['probs']) < lower_bound_freq:
             bins[i][b]['probs'].insert(0, bins[i][b-1]['probs'].pop(-1))
             bins[i][b]['occurrences'].insert(0, bins[i][b-1]['occurrences'].pop(-1))
     return bins
 
-def sum_occurrences(class_label: str, num_bins: int, bins: dict) -> dict:
+def _sum_occurrences(class_label: str, num_bins: int, bins: dict) -> dict:
     """
     For a given class, loop through the bins and find the number of occurrences of the given class in each bin.
 
     Once this sum of occurrences is found, delete the (now irrelevant) list tracking these occurrences.
 
     Args:
         class_label (str):
@@ -253,15 +304,15 @@
     i = class_label
     for b in range(num_bins):
         bins[i][b]['num_occurrences'] = sum(bins[i][b]['occurrences'])
         del bins[i][b]['occurrences']    
     return bins
 
 
-def sort_predictions(y_pred_class_i: list, y_true_class_i: list) -> tuple:
+def _sort_predictions(y_pred_class_i: list, y_true_class_i: list) -> tuple:
     """
     Sort the predicted probabilities in ascending order. Sort the true labels so they correspond to the sorted predictions.
 
     Args:
         y_pred_class_i (ndarray):
             Array-like object of shape (num_samples,) where i position is predicted probability of data point i belonging to given class.
         y_true_class_i (ndarray):
@@ -271,7 +322,35 @@
         tuple
     """
     zipped_list = list(zip(y_pred_class_i, y_true_class_i))
     sorted_zipped_list = sorted(zipped_list)
     y_pred_sorted, y_true_sorted = zip(*sorted_zipped_list)
 
     return list(y_pred_sorted), list(y_true_sorted)
+
+
+def get_classwise_bin_weights(bins: dict, num_bins: int, num_samples: int, num_classes: int) -> np.ndarray:
+    """
+    Calculate the 
+    Args:
+        bins (dict):
+            Dictionary containing, for each class, each bin, itself containing the predicted probabilities and occurences of the given class.                    
+        num_bins (int):
+            Number of equal-width bins the interval [0, 1] is divided into.
+        num_samples (int):
+            Number of data points.
+        num_classes (int):
+            Number of classes.
+
+    Returns:
+        np.ndarray:
+            Numpy array of shape (num_classes, num_bins) whose ijth element represents the proportion of the overall dataset whose predictions for class i lie in bin j.    
+    """    
+    weights = [
+        [
+            _get_bin_weight(bins[i][b], num_samples) for b in range(num_bins)
+        ]
+        for i in range(num_classes)
+    ]
+    
+    return np.asarray(weights)
+
```

### Comparing `calibra-0.2.0/calibra.egg-info/PKG-INFO` & `calibra-0.3.0/calibra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibra
-Version: 0.2.0
+Version: 0.3.0
 Summary: Toolkit for calibration of machine learning classifiers.
 Home-page: https://github.com/conorwalsh99/calibra
 Author: Conor Walsh
 Author-email: conorwalsh206@gmail.com
 License: MIT license
 Keywords: calibra
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `calibra-0.2.0/calibra.egg-info/SOURCES.txt` & `calibra-0.3.0/calibra.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
+tests/conftest.py
 tests/test_errors.py
-tests/test_utils.py
+tests/test_plotting.py
+tests/test_utils.py
+tests/baseline/test_plot.png
```

### Comparing `calibra-0.2.0/docs/Makefile` & `calibra-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/docs/conf.py` & `calibra-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/docs/installation.rst` & `calibra-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/docs/make.bat` & `calibra-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calibra-0.2.0/setup.py` & `calibra-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='calibra',
     name='calibra',
     packages=find_packages(include=['calibra', 'calibra.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/conorwalsh99/calibra',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

