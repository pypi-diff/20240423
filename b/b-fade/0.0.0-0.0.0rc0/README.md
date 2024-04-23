# Comparing `tmp/b_fade-0.0.0.tar.gz` & `tmp/b_fade-0.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_fade-0.0.0.tar", last modified: Tue Apr 23 15:15:13 2024, max compression
+gzip compressed data, was "b_fade-0.0.0rc0.tar", last modified: Mon Apr 22 14:17:28 2024, max compression
```

## Comparing `b_fade-0.0.0.tar` & `b_fade-0.0.0rc0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-23 15:15:13.293426 b_fade-0.0.0/
--rw-rw-r--   0 ale       (1000) ale       (1000)    35149 2024-04-23 13:54:53.000000 b_fade-0.0.0/LICENSE
--rw-r--r--   0 ale       (1000) ale       (1000)     2010 2024-04-23 15:15:13.293426 b_fade-0.0.0/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1020 2024-04-23 13:54:53.000000 b_fade-0.0.0/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-04-23 13:54:53.000000 b_fade-0.0.0/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-04-23 15:15:13.293426 b_fade-0.0.0/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1136 2024-04-23 15:14:46.000000 b_fade-0.0.0/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-23 15:15:13.289426 b_fade-0.0.0/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-23 15:15:13.293426 b_fade-0.0.0/src/b_fade.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)     2010 2024-04-23 15:15:13.000000 b_fade-0.0.0/src/b_fade.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      360 2024-04-23 15:15:13.000000 b_fade-0.0.0/src/b_fade.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-04-23 15:15:13.000000 b_fade-0.0.0/src/b_fade.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      132 2024-04-23 15:15:13.000000 b_fade-0.0.0/src/b_fade.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        6 2024-04-23 15:15:13.000000 b_fade-0.0.0/src/b_fade.egg-info/top_level.txt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-23 15:15:13.293426 b_fade-0.0.0/src/bfade/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    24222 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/abstract.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    13909 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/dataset.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     6500 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/elhaddad.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7947 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/statistics.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    12287 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/util.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    19829 2024-04-23 13:54:53.000000 b_fade-0.0.0/src/bfade/viewers.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-22 14:17:28.362138 b_fade-0.0.0rc0/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    35149 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/LICENSE
+-rw-r--r--   0 ale       (1000) ale       (1000)     2083 2024-04-22 14:17:28.358138 b_fade-0.0.0rc0/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1090 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-04-22 14:17:28.362138 b_fade-0.0.0rc0/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1139 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-22 14:17:28.358138 b_fade-0.0.0rc0/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-22 14:17:28.358138 b_fade-0.0.0rc0/src/b_fade.egg-info/
+-rw-r--r--   0 ale       (1000) ale       (1000)     2083 2024-04-22 14:17:28.000000 b_fade-0.0.0rc0/src/b_fade.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      360 2024-04-22 14:17:28.000000 b_fade-0.0.0rc0/src/b_fade.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-04-22 14:17:28.000000 b_fade-0.0.0rc0/src/b_fade.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      132 2024-04-22 14:17:28.000000 b_fade-0.0.0rc0/src/b_fade.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        6 2024-04-22 14:17:28.000000 b_fade-0.0.0rc0/src/b_fade.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-04-22 14:17:28.358138 b_fade-0.0.0rc0/src/bfade/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    24222 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/abstract.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13909 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/dataset.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6500 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/elhaddad.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7947 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/statistics.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    12287 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/util.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    19829 2024-04-22 14:16:33.000000 b_fade-0.0.0rc0/src/bfade/viewers.py
```

### Comparing `b_fade-0.0.0/LICENSE` & `b_fade-0.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_fade-0.0.0/PKG-INFO` & `b_fade-0.0.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-fade
-Version: 0.0.0
+Version: 0.0.0rc0
 Summary: B-FADE: Bayesian FAtigue moDel Estimator
 Home-page: https://github.com/aletgn/b-fade
 Author: Alessandro Tognan
 Author-email: tognan.alessandro@spes.uniud.it
 Project-URL: Bug Tracker, https://github.com/aletgn/b-fade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,32 +27,32 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 # B-FADE: Bayesian FAtigue moDel Estimator
 
-The package implements Maximum a Posteriori Estimation (MAP) to accomplish the estimation of fatigue models' parameters. Currently the package is designed to identify the El Haddad (EH) curve given a fatigue & defectivity characterisation dataset. Other curves are foreseen in future developments.
+The package implements Maximum a Posteriori Estimation (MAP) to accomplish the estimation of fatigue models' parameters. Currently the package is designed to identify the El Haddad (EH) curve given a fatigue & defectivity characterisation dataset. Other curves are forseen in future developments.
 
 ## Features
 
 - Maximum a Posteriori Estimation and computation of the predictive posterior.
 - Monte Carlo Estimation of the prediction interval for the considered curve.
 - Data pre-processing & visualisation.
 
 ## Quick Setup
 
-B-FADE is available at [PyPI](https://pypi.org/project/b-fade/), so it can be installed using common package managers, such as `pip` or `conda`:
+B-FADE is available on [PyPI](https://pypi.org/) at (**add link when available**), therefore it can be installed using common package managers, such as `pip` or `conda`:
 
 ```
 pip install --user b-fade
 ```
 
 ```
 conda install b-fade
 ```
 
 For further instructions, please take a look at the documentation.
 
 ## Documentation
 
-Please refer to [ReadTheDocs](https://b-fade.readthedocs.io/en/latest/) for detailed instructions about installing, utilising B-FADE and working examples.
+Please refer to https://github.com/aletgn/b-fade/blob/master/README.md (**Update with readthedocs when it is ready**) for detailed instructions about installing, utilising B-FADE and working examples.
```

### Comparing `b_fade-0.0.0/README.md` & `b_fade-0.0.0rc0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # B-FADE: Bayesian FAtigue moDel Estimator
 
-The package implements Maximum a Posteriori Estimation (MAP) to accomplish the estimation of fatigue models' parameters. Currently the package is designed to identify the El Haddad (EH) curve given a fatigue & defectivity characterisation dataset. Other curves are foreseen in future developments.
+The package implements Maximum a Posteriori Estimation (MAP) to accomplish the estimation of fatigue models' parameters. Currently the package is designed to identify the El Haddad (EH) curve given a fatigue & defectivity characterisation dataset. Other curves are forseen in future developments.
 
 ## Features
 
 - Maximum a Posteriori Estimation and computation of the predictive posterior.
 - Monte Carlo Estimation of the prediction interval for the considered curve.
 - Data pre-processing & visualisation.
 
 ## Quick Setup
 
-B-FADE is available at [PyPI](https://pypi.org/project/b-fade/), so it can be installed using common package managers, such as `pip` or `conda`:
+B-FADE is available on [PyPI](https://pypi.org/) at (**add link when available**), therefore it can be installed using common package managers, such as `pip` or `conda`:
 
 ```
 pip install --user b-fade
 ```
 
 ```
 conda install b-fade
 ```
 
 For further instructions, please take a look at the documentation.
 
 ## Documentation
 
-Please refer to [ReadTheDocs](https://b-fade.readthedocs.io/en/latest/) for detailed instructions about installing, utilising B-FADE and working examples.
+Please refer to https://github.com/aletgn/b-fade/blob/master/README.md (**Update with readthedocs when it is ready**) for detailed instructions about installing, utilising B-FADE and working examples.
```

### Comparing `b_fade-0.0.0/setup.py` & `b_fade-0.0.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="b-fade",
-    version="0.0.0",
+    version="0.0.0.rc0",
     description="B-FADE: Bayesian FAtigue moDel Estimator",
     long_description=long_description,
     long_description_content_type="text/markdown",
         
     author="Alessandro Tognan",
     author_email="tognan.alessandro@spes.uniud.it",
     url="https://github.com/aletgn/b-fade",
@@ -25,8 +25,8 @@
     packages=find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=["numpy", "scipy", "matplotlib", 
                       "pandas", "odfpy", "openpyxl",
                       "scikit-learn", "numdifftools", "PyYAML"],
     extras_require={"test" : ["notebook"],
                     "dev" : ["pytest", "twine", "setuptools", "build"]}
-)
+)
```

### Comparing `b_fade-0.0.0/src/b_fade.egg-info/PKG-INFO` & `b_fade-0.0.0rc0/src/b_fade.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-fade
-Version: 0.0.0
+Version: 0.0.0rc0
 Summary: B-FADE: Bayesian FAtigue moDel Estimator
 Home-page: https://github.com/aletgn/b-fade
 Author: Alessandro Tognan
 Author-email: tognan.alessandro@spes.uniud.it
 Project-URL: Bug Tracker, https://github.com/aletgn/b-fade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,32 +27,32 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 # B-FADE: Bayesian FAtigue moDel Estimator
 
-The package implements Maximum a Posteriori Estimation (MAP) to accomplish the estimation of fatigue models' parameters. Currently the package is designed to identify the El Haddad (EH) curve given a fatigue & defectivity characterisation dataset. Other curves are foreseen in future developments.
+The package implements Maximum a Posteriori Estimation (MAP) to accomplish the estimation of fatigue models' parameters. Currently the package is designed to identify the El Haddad (EH) curve given a fatigue & defectivity characterisation dataset. Other curves are forseen in future developments.
 
 ## Features
 
 - Maximum a Posteriori Estimation and computation of the predictive posterior.
 - Monte Carlo Estimation of the prediction interval for the considered curve.
 - Data pre-processing & visualisation.
 
 ## Quick Setup
 
-B-FADE is available at [PyPI](https://pypi.org/project/b-fade/), so it can be installed using common package managers, such as `pip` or `conda`:
+B-FADE is available on [PyPI](https://pypi.org/) at (**add link when available**), therefore it can be installed using common package managers, such as `pip` or `conda`:
 
 ```
 pip install --user b-fade
 ```
 
 ```
 conda install b-fade
 ```
 
 For further instructions, please take a look at the documentation.
 
 ## Documentation
 
-Please refer to [ReadTheDocs](https://b-fade.readthedocs.io/en/latest/) for detailed instructions about installing, utilising B-FADE and working examples.
+Please refer to https://github.com/aletgn/b-fade/blob/master/README.md (**Update with readthedocs when it is ready**) for detailed instructions about installing, utilising B-FADE and working examples.
```

### Comparing `b_fade-0.0.0/src/bfade/abstract.py` & `b_fade-0.0.0rc0/src/bfade/abstract.py`

 * *Files identical despite different names*

### Comparing `b_fade-0.0.0/src/bfade/dataset.py` & `b_fade-0.0.0rc0/src/bfade/dataset.py`

 * *Files identical despite different names*

### Comparing `b_fade-0.0.0/src/bfade/elhaddad.py` & `b_fade-0.0.0rc0/src/bfade/elhaddad.py`

 * *Files identical despite different names*

### Comparing `b_fade-0.0.0/src/bfade/statistics.py` & `b_fade-0.0.0rc0/src/bfade/statistics.py`

 * *Files identical despite different names*

### Comparing `b_fade-0.0.0/src/bfade/util.py` & `b_fade-0.0.0rc0/src/bfade/util.py`

 * *Files identical despite different names*

### Comparing `b_fade-0.0.0/src/bfade/viewers.py` & `b_fade-0.0.0rc0/src/bfade/viewers.py`

 * *Files identical despite different names*

