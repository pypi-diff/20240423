# Comparing `tmp/pudu-0.3.2.tar.gz` & `tmp/pudu-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pudu-0.3.2.tar", last modified: Sun Sep 17 14:55:03 2023, max compression
+gzip compressed data, was "pudu-0.3.4.tar", last modified: Tue Apr 23 13:03:43 2024, max compression
```

## Comparing `pudu-0.3.2.tar` & `pudu-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 14:55:03.736528 pudu-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-09-17 14:54:54.000000 pudu-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-09-17 14:54:54.000000 pudu-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2023-09-17 14:55:03.736528 pudu-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2023-09-17 14:54:54.000000 pudu-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-09-17 14:54:54.000000 pudu-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 14:55:03.736528 pudu-0.3.2/pudu/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11912 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/perturbation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13521 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/pudu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-09-17 14:54:54.000000 pudu-0.3.2/pudu/standards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 14:55:03.736528 pudu-0.3.2/pudu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2023-09-17 14:55:03.000000 pudu-0.3.2/pudu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-09-17 14:55:03.000000 pudu-0.3.2/pudu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-17 14:55:03.000000 pudu-0.3.2/pudu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 14:55:03.000000 pudu-0.3.2/pudu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-17 14:55:03.000000 pudu-0.3.2/pudu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-17 14:55:03.000000 pudu-0.3.2/pudu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-17 14:54:54.000000 pudu-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-17 14:54:54.000000 pudu-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-09-17 14:55:03.736528 pudu-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-09-17 14:54:54.000000 pudu-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:43.439830 pudu-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-23 13:03:31.000000 pudu-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 13:03:31.000000 pudu-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-23 13:03:43.439830 pudu-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-23 13:03:31.000000 pudu-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-23 13:03:31.000000 pudu-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:43.435830 pudu-0.3.4/pudu/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/perturbation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27931 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/pudu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-23 13:03:31.000000 pudu-0.3.4/pudu/standards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:43.439830 pudu-0.3.4/pudu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-23 13:03:43.000000 pudu-0.3.4/pudu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-23 13:03:43.000000 pudu-0.3.4/pudu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 13:03:43.000000 pudu-0.3.4/pudu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:03:43.000000 pudu-0.3.4/pudu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 13:03:43.000000 pudu-0.3.4/pudu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 13:03:43.000000 pudu-0.3.4/pudu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 13:03:31.000000 pudu-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 13:03:31.000000 pudu-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-23 13:03:43.439830 pudu-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-23 13:03:31.000000 pudu-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:43.439830 pudu-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-23 13:03:31.000000 pudu-0.3.4/tests/test_pudu.py
```

### Comparing `pudu-0.3.2/LICENSE` & `pudu-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pudu-0.3.2/PKG-INFO` & `pudu-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.3.2
+Version: 0.3.4
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,48 +15,57 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: spectrapepper
+Requires-Dist: scikit-learn
+Requires-Dist: tensorflow==2.11
 
 <img src="https://raw.githubusercontent.com/pudu-py/pudu/main/docs/_static/pudu-baner.png" width="70%">
 
 [![image](https://img.shields.io/pypi/v/pudu.svg)](https://pypi.python.org/pypi/pudu)
-[![image](https://img.shields.io/conda/vn/conda-forge/pudu.svg)](https://anaconda.org/conda-forge/pudu)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pudu/badges/version.svg)](https://anaconda.org/conda-forge/pudu)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![CodeQL](https://github.com/pudu-py/pudu/actions/workflows/codeql.yml/badge.svg)](https://github.com/pudu-py/pudu/actions/workflows/codeql.yml)
 [![image](https://github.com/pudu-py/pudu/workflows/docs/badge.svg)](https://pudu-py.github.io/pudu)
 [![codecov](https://codecov.io/gh/pudu-py/pudu/branch/main/graph/badge.svg?token=DC0QIwuYel)](https://codecov.io/gh/pudu-py/pudu)
 [![Downloads](https://static.pepy.tech/personalized-badge/pudu?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/pudu)
 [![image](https://img.shields.io/conda/dn/conda-forge/pudu?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/pudu)
 [![image](https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown?logo=stackoverflow&logoWidth=18&logoColor=white)](https://stackoverflow.com/questions/tagged/pudu)
+[![status](https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d/status.svg)](https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d)
 
-**A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.**
+**A Python library for explainability of machine learning algorithms for spectroscopic data in an agnostic, deterministic, and simple way.**
 
 * GitHub repo: https://github.com/pudu-py/pudu
 * Documentation: https://pudu-py.github.io/pudu
 * PyPI: https://pypi.python.org/pypi/pudu
 * Conda-forge: https://anaconda.org/conda-forge/pudu
 * Free software: MIT license
 
 # Introduction
 
-**pudu** is a Python package that helps intepret and explore the results of machinme learning algorythms. It does this by quantifying the change
-in probability according to the change in the features. This library works with any case that has a probability function, which is normally available in ``scikit-learn`` and ``keras`` methods, and works for both 1-d (vectrors) and 2-d problems (images). In order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
+**pudu** is a Python package that helps interpret and explore the results of machine learning algorithms with spectroscopic data. It does this by quantifying the change in the prediction according to the change in the features. This library works with classification and regression problems with both 1-d and 2-d problems. 
+actiIn order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
 
 # Features
 
-The following is a list of the main procedures that **pudu** package enables.
+The following is a list of the main features that **pudu** package enables.
 
-- Importance: estimates the absolute or relative importance of the features.
-- Speed: calculates how fast a preditcion changes according to the changes in the features.
+- Importance: measures the change in prediction according to perturbations in the features.
+- Speed: calculates how fast a prediction changes according to different perturbation levels.
 - Synergy: tests the synergy between features and the change in classification probability.
-- Easy plotting of the results from the above.
+- Re-activations: Evaluates how activations maps from CNN’s change according to perturbations in the data.
+- Easy plotting with ample personalization options for all the cases above.
+
 
 # Quickstart
 
 1. Install this library using ``pip``::
 
         pip install pudu
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pudu-0.3.2/README.md` & `pudu-0.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 <img src="https://raw.githubusercontent.com/pudu-py/pudu/main/docs/_static/pudu-baner.png" width="70%">
 
 [![image](https://img.shields.io/pypi/v/pudu.svg)](https://pypi.python.org/pypi/pudu)
-[![image](https://img.shields.io/conda/vn/conda-forge/pudu.svg)](https://anaconda.org/conda-forge/pudu)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pudu/badges/version.svg)](https://anaconda.org/conda-forge/pudu)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![CodeQL](https://github.com/pudu-py/pudu/actions/workflows/codeql.yml/badge.svg)](https://github.com/pudu-py/pudu/actions/workflows/codeql.yml)
 [![image](https://github.com/pudu-py/pudu/workflows/docs/badge.svg)](https://pudu-py.github.io/pudu)
 [![codecov](https://codecov.io/gh/pudu-py/pudu/branch/main/graph/badge.svg?token=DC0QIwuYel)](https://codecov.io/gh/pudu-py/pudu)
 [![Downloads](https://static.pepy.tech/personalized-badge/pudu?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/pudu)
 [![image](https://img.shields.io/conda/dn/conda-forge/pudu?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/pudu)
 [![image](https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown?logo=stackoverflow&logoWidth=18&logoColor=white)](https://stackoverflow.com/questions/tagged/pudu)
+[![status](https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d/status.svg)](https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d)
 
-**A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.**
+**A Python library for explainability of machine learning algorithms for spectroscopic data in an agnostic, deterministic, and simple way.**
 
 * GitHub repo: https://github.com/pudu-py/pudu
 * Documentation: https://pudu-py.github.io/pudu
 * PyPI: https://pypi.python.org/pypi/pudu
 * Conda-forge: https://anaconda.org/conda-forge/pudu
 * Free software: MIT license
 
 # Introduction
 
-**pudu** is a Python package that helps intepret and explore the results of machinme learning algorythms. It does this by quantifying the change
-in probability according to the change in the features. This library works with any case that has a probability function, which is normally available in ``scikit-learn`` and ``keras`` methods, and works for both 1-d (vectrors) and 2-d problems (images). In order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
+**pudu** is a Python package that helps interpret and explore the results of machine learning algorithms with spectroscopic data. It does this by quantifying the change in the prediction according to the change in the features. This library works with classification and regression problems with both 1-d and 2-d problems. 
+actiIn order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
 
 # Features
 
-The following is a list of the main procedures that **pudu** package enables.
+The following is a list of the main features that **pudu** package enables.
 
-- Importance: estimates the absolute or relative importance of the features.
-- Speed: calculates how fast a preditcion changes according to the changes in the features.
+- Importance: measures the change in prediction according to perturbations in the features.
+- Speed: calculates how fast a prediction changes according to different perturbation levels.
 - Synergy: tests the synergy between features and the change in classification probability.
-- Easy plotting of the results from the above.
+- Re-activations: Evaluates how activations maps from CNN’s change according to perturbations in the data.
+- Easy plotting with ample personalization options for all the cases above.
+
 
 # Quickstart
 
 1. Install this library using ``pip``::
 
         pip install pudu
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pudu-0.3.2/README.rst` & `pudu-0.3.4/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 ====
 pudu
 ====
 
 .. image:: https://img.shields.io/pypi/v/pudu.svg
         :target: https://pypi.python.org/pypi/pudu
-.. image:: https://img.shields.io/conda/vn/conda-forge/pudu.svg
+.. image:: https://anaconda.org/conda-forge/pudu/badges/version.svg   
         :target: https://anaconda.org/conda-forge/pudu
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
         :target: https://opensource.org/licenses/MIT
 .. image:: https://github.com/pudu-py/pudu/actions/workflows/codeql.yml/badge.svg
         :target: https://github.com/pudu-py/pudu/actions/workflows/codeql.yml
 .. image:: https://github.com/pudu-py/pudu/workflows/docs/badge.svg
         :target: https://pudu-py.github.io/pudu
 .. image:: https://codecov.io/gh/pudu-py/pudu/branch/main/graph/badge.svg?token=DC0QIwuYel
         :target: https://codecov.io/gh/pudu-py/pudu
-.. image:: https://img.shields.io/conda/dn/conda-forge/pudu.svg?color=blue&label=conda%20downloads
-        :target: https://pepy.tech/project/pudu
 .. image:: https://static.pepy.tech/personalized-badge/pudu?period=total&units=international_system&left_color=grey&left_text=pypi%20downloads&right_color=blue
         :target: https://pepy.tech/project/pudu
+.. image:: https://img.shields.io/conda/dn/conda-forge/pudu.svg?color=blue&label=conda%20downloads
+        :target: https://pepy.tech/project/pudu
 .. image:: https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown
         :target: https://stackoverflow.com/questions/tagged/pudu
+.. image:: https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d/status.svg
+        :target: https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d
 
-**A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.**
+**A Python library for explainability of machine learning algorithms for spectroscopic data in an agnostic, deterministic, and simple way.**
 * GitHub repo: https://github.com/pudu-py/pudu
 * Documentation: https://pudu-py.github.io/pudu
 * PyPI: https://pypi.python.org/pypi/pudu
 * Conda-forge: https://anaconda.org/conda-forge/pudu
 * Free software: MIT license
 
 Introduction
 ============
 
-**pudu** is a Python package that helps intepret and explore the results of machinme learning algorythms. It does this by quantifying the change
-in probability according to the change in the features. This library works with any case that has a probability function, which is normally available in ``scikit-learn`` and ``keras`` methods, and works for both 1-d (vectrors) and 2-d problems (images). In order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
+**pudu** is a Python package that helps interpret and explore the results of machine learning algorithms 
+with spectroscopic data. It does this by quantifying the change in the prediction according to the change 
+in the features. This library works with classification and regression problems with both 1-d and 2-d problems. 
+In order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
 
 Features
 --------
 
-The following is a list of the main procedures that **pudu** package enables.
+The following is a list of the main features that **pudu** package enables.
+
+- Importance: measures the change in prediction according to perturbations in the features.
+- Speed: calculates how fast a prediction changes according to different perturbation levels.
+- Synergy: tests the synergy between features and the change in classification probability.
+- Re-activations: Evaluates how activations maps from CNNs change according to perturbations in the data.
+- Easy plotting with ample personalization options for all the cases above.
 
-- Importance: estimates the absolute or relative importance oif the features.
-- Speed: calculates how fast a preditci0on changes according to the changes in the features.
-- Synergy: tests teh synergy between features and the change in classification probability.
-- Easy plotting of the results from the above.
 
 Quickstart
 ----------
 
 1. Install this library using ``pip``:
 
         pip install pudu
```

### Comparing `pudu-0.3.2/pudu/error_handler.py` & `pudu-0.3.4/pudu/error_handler.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.2/pudu/masks.py` & `pudu-0.3.4/pudu/masks.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.2/pudu/perturbation.py` & `pudu-0.3.4/pudu/perturbation.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,14 +358,31 @@
     def __init__(self, custom):
         self.custom = custom
     def apply(self, x, row, col, window, bias):
         x[0, row:row+window[0], col:col+window[1], 0] = x[0, row:row+window[0], col:col+window[1], 0]*self.custom[0, row:row+window[0], col:col+window[1], 0]
         return x, None
 
 
+class CustomSum:
+    """
+    Sums a custom vector as a perturbation to the array.
+
+    :type func: callable
+    :param func: A function that takes a single argument and returns a single value.
+
+    :rtype: 4d array
+    :return: Custom perturbated array
+    """
+    def __init__(self, custom):
+        self.custom = custom
+    def apply(self, x, row, col, window, bias):
+        x[0, row:row+window[0], col:col+window[1], 0] = x[0, row:row+window[0], col:col+window[1], 0] + self.custom[0, row:row+window[0], col:col+window[1], 0]
+        return x, None
+
+
 class UpperThreshold:
     """
     Sets values above a certain threshold to a specified value.
 
     :type threshold: float
     :param threshold: Threshold above which values will be set to a specific value.
     :type value: float
```

### Comparing `pudu-0.3.2/pudu/plots.py` & `pudu-0.3.4/pudu/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import matplotlib as mpl
 import numpy as np
 
 def plot(feature, image, axis=None, show_data=True, title='Importance', 
         xlabel='Feature', ylabel='Intensity', xticks=None, yticks=[], cmap='Greens',
         font_size=15, figsize=(14, 4), padding=(0, 0, 1, 1), cbar_pad=0.05, vmin=None,
         vmax=None, xlims=None):
+    
     """
     Easy plot function for `importance`, `speed`, or `synergy`. It shows the analyzed
         feature `feature` with a colormap overlay indicating the result along with
         a colorbar. Works for both vectors and images.
 
     :type feature: list
     :param feature: feature analyzed or any that the user whant to plot against.
```

### Comparing `pudu-0.3.2/pudu/pudu.py` & `pudu-0.3.4/pudu/pudu.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 import numpy as np
 import copy
 
 from . import error_handler, standards
 from . import masks as msk
 from . import perturbation as ptn
 
+# For Sphinx docs only:
+# import error_handler, standards
+# import masks as msk
+# import perturbation as ptn
+
+
 class pudu:
     def __init__(self, x, y, pf, model=None):
         """
         `pudu` constructor.
 
         :type x: list
         :param x: Features (input) to be analyzed. Must have same format as
```

### Comparing `pudu-0.3.2/pudu/standards.py` & `pudu-0.3.4/pudu/standards.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.2/pudu.egg-info/PKG-INFO` & `pudu-0.3.4/pudu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.3.2
+Version: 0.3.4
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,48 +15,57 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: spectrapepper
+Requires-Dist: scikit-learn
+Requires-Dist: tensorflow==2.11
 
 <img src="https://raw.githubusercontent.com/pudu-py/pudu/main/docs/_static/pudu-baner.png" width="70%">
 
 [![image](https://img.shields.io/pypi/v/pudu.svg)](https://pypi.python.org/pypi/pudu)
-[![image](https://img.shields.io/conda/vn/conda-forge/pudu.svg)](https://anaconda.org/conda-forge/pudu)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pudu/badges/version.svg)](https://anaconda.org/conda-forge/pudu)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![CodeQL](https://github.com/pudu-py/pudu/actions/workflows/codeql.yml/badge.svg)](https://github.com/pudu-py/pudu/actions/workflows/codeql.yml)
 [![image](https://github.com/pudu-py/pudu/workflows/docs/badge.svg)](https://pudu-py.github.io/pudu)
 [![codecov](https://codecov.io/gh/pudu-py/pudu/branch/main/graph/badge.svg?token=DC0QIwuYel)](https://codecov.io/gh/pudu-py/pudu)
 [![Downloads](https://static.pepy.tech/personalized-badge/pudu?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/pudu)
 [![image](https://img.shields.io/conda/dn/conda-forge/pudu?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/pudu)
 [![image](https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown?logo=stackoverflow&logoWidth=18&logoColor=white)](https://stackoverflow.com/questions/tagged/pudu)
+[![status](https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d/status.svg)](https://joss.theoj.org/papers/cacb5b6520209b0c940bf46638df251d)
 
-**A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.**
+**A Python library for explainability of machine learning algorithms for spectroscopic data in an agnostic, deterministic, and simple way.**
 
 * GitHub repo: https://github.com/pudu-py/pudu
 * Documentation: https://pudu-py.github.io/pudu
 * PyPI: https://pypi.python.org/pypi/pudu
 * Conda-forge: https://anaconda.org/conda-forge/pudu
 * Free software: MIT license
 
 # Introduction
 
-**pudu** is a Python package that helps intepret and explore the results of machinme learning algorythms. It does this by quantifying the change
-in probability according to the change in the features. This library works with any case that has a probability function, which is normally available in ``scikit-learn`` and ``keras`` methods, and works for both 1-d (vectrors) and 2-d problems (images). In order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
+**pudu** is a Python package that helps interpret and explore the results of machine learning algorithms with spectroscopic data. It does this by quantifying the change in the prediction according to the change in the features. This library works with classification and regression problems with both 1-d and 2-d problems. 
+actiIn order to see the exact procedure and format needed, please refer to the examples in the ``docs``.
 
 # Features
 
-The following is a list of the main procedures that **pudu** package enables.
+The following is a list of the main features that **pudu** package enables.
 
-- Importance: estimates the absolute or relative importance of the features.
-- Speed: calculates how fast a preditcion changes according to the changes in the features.
+- Importance: measures the change in prediction according to perturbations in the features.
+- Speed: calculates how fast a prediction changes according to different perturbation levels.
 - Synergy: tests the synergy between features and the change in classification probability.
-- Easy plotting of the results from the above.
+- Re-activations: Evaluates how activations maps from CNN’s change according to perturbations in the data.
+- Easy plotting with ample personalization options for all the cases above.
+
 
 # Quickstart
 
 1. Install this library using ``pip``::
 
         pip install pudu
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pudu-0.3.2/setup.py` & `pudu-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pudu',
     name='pudu',
     packages=find_packages(include=['pudu', 'pudu.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/pudu-py/pudu',
-    version='0.3.2',
+    version='0.3.4',
     zip_safe=False,
 )
```

