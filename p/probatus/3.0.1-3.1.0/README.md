# Comparing `tmp/probatus-3.0.1.tar.gz` & `tmp/probatus-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probatus-3.0.1.tar", last modified: Tue Apr  2 14:13:53 2024, max compression
+gzip compressed data, was "probatus-3.1.0.tar", last modified: Tue Apr 23 07:37:02 2024, max compression
```

## Comparing `probatus-3.0.1.tar` & `probatus-3.1.0.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.550460 probatus-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-02 14:10:39.000000 probatus-3.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-02 14:13:53.550460 probatus-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-02 14:10:39.000000 probatus-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.538460 probatus-3.0.1/probatus/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/feature_elimination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67539 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/feature_elimination/feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/interpret/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/interpret/model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/interpret/shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/sample_similarity/resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/base_class_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/missing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/shap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/probatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-02 14:10:39.000000 probatus-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:13:53.550460 probatus-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.538460 probatus-3.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/docs/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/tests/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/feature_elimination/test_feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/tests/interpret/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/interpret/test_model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/interpret/test_shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/tests/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/sample_similarity/test_resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/utils/test_base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/utils/test_utils_array_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.327308 probatus-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-23 07:33:59.000000 probatus-3.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-23 07:37:02.327308 probatus-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-23 07:33:59.000000 probatus-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.319308 probatus-3.1.0/probatus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.319308 probatus-3.1.0/probatus/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/feature_elimination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/feature_elimination/early_stopping_feature_elimination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43744 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/feature_elimination/feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.319308 probatus-3.1.0/probatus/interpret/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19521 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/interpret/model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/interpret/shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.319308 probatus-3.1.0/probatus/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/sample_similarity/resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/probatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/base_class_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-23 07:33:59.000000 probatus-3.1.0/probatus/utils/shap_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/probatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-23 07:37:02.000000 probatus-3.1.0/probatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-23 07:37:02.000000 probatus-3.1.0/probatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:37:02.000000 probatus-3.1.0/probatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-23 07:37:02.000000 probatus-3.1.0/probatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 07:37:02.000000 probatus-3.1.0/probatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-23 07:33:59.000000 probatus-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:37:02.327308 probatus-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.319308 probatus-3.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/docs/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/tests/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/feature_elimination/test_feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/tests/interpret/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/interpret/test_model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/interpret/test_shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/tests/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/sample_similarity/test_resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:37:02.323308 probatus-3.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/utils/test_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-23 07:33:59.000000 probatus-3.1.0/tests/utils/test_utils_array_funcs.py
```

### Comparing `probatus-3.0.1/LICENCE` & `probatus-3.1.0/LICENCE`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2020 ING Bank N.V.
+Copyright (c) ING Bank N.V.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `probatus-3.0.1/PKG-INFO` & `probatus-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 3.0.1
-Summary: Validation of binary classifiers and data used to develop them
+Version: 3.1.0
+Summary: Validation of regression & classifiers and data used to develop them
 Author-email: "ING Bank N.V." <reinier.koops@ing.com>
-License: Copyright (c) 2020 ING Bank N.V.
+License: Copyright (c) ING Bank N.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://ing-bank.github.io/probatus/
@@ -78,15 +78,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
 ![GitHub contributors](https://img.shields.io/github/contributors/ing-bank/probatus)
 
 # Probatus
 
 ## Overview
 
-**Probatus** is a python package that helps validate binary classification models and the data used to develop them. Main features:
+**Probatus** is a python package that helps validate regression & (multiclass) classification models and the data used to develop them. Main features:
 
 - [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools
 - [probatus.sample_similarity](https://ing-bank.github.io/probatus/api/sample_similarity.html) to compare two datasets using resemblance modelling, f.e. `train` with out-of-time `test`.
 - [probatus.feature_elimination.ShapRFECV](https://ing-bank.github.io/probatus/api/feature_elimination.html) provides cross-validated Recursive Feature Elimination using shap feature importance.
 
 ## Installation
```

### Comparing `probatus-3.0.1/README.md` & `probatus-3.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
 ![GitHub contributors](https://img.shields.io/github/contributors/ing-bank/probatus)
 
 # Probatus
 
 ## Overview
 
-**Probatus** is a python package that helps validate binary classification models and the data used to develop them. Main features:
+**Probatus** is a python package that helps validate regression & (multiclass) classification models and the data used to develop them. Main features:
 
 - [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools
 - [probatus.sample_similarity](https://ing-bank.github.io/probatus/api/sample_similarity.html) to compare two datasets using resemblance modelling, f.e. `train` with out-of-time `test`.
 - [probatus.feature_elimination.ShapRFECV](https://ing-bank.github.io/probatus/api/feature_elimination.html) provides cross-validated Recursive Feature Elimination using shap feature importance.
 
 ## Installation
```

### Comparing `probatus-3.0.1/probatus/__init__.py` & `probatus-3.1.0/probatus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 ING Bank N.V.
+# Copyright (c) ING Bank N.V.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `probatus-3.0.1/probatus/interpret/model_interpret.py` & `probatus-3.1.0/probatus/interpret/model_interpret.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,21 @@
-# Copyright (c) 2020 ING Bank N.V.
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of
-# this software and associated documentation files (the "Software"), to deal in
-# the Software without restriction, including without limitation the rights to
-# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-# the Software, and to permit persons to whom the Software is furnished to do so,
-# subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from shap import summary_plot
 from shap.plots._waterfall import waterfall_legacy
 
 from probatus.interpret import DependencePlotter
 from probatus.utils import (
     BaseFitComputePlotClass,
     assure_list_of_strings,
     calculate_shap_importance,
-    get_single_scorer,
     preprocess_data,
     preprocess_labels,
+    get_single_scorer,
     shap_calc,
 )
 
 
 class ShapModelInterpreter(BaseFitComputePlotClass):
     """
     This class is a wrapper that allows to easily analyse a model's features.
@@ -56,19 +36,19 @@
 
     # Prepare two samples
     X, y = make_classification(n_samples=5000, n_features=4, random_state=0)
     X = pd.DataFrame(X, columns=feature_names)
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 
     # Prepare and fit model. Remember about class_weight="balanced" or an equivalent.
-    clf = RandomForestClassifier(class_weight='balanced', n_estimators = 100, max_depth=2, random_state=0)
-    clf.fit(X_train, y_train)
+    model = RandomForestClassifier(class_weight='balanced', n_estimators = 100, max_depth=2, random_state=0)
+    model.fit(X_train, y_train)
 
     # Train ShapModelInterpreter
-    shap_interpreter = ShapModelInterpreter(clf)
+    shap_interpreter = ShapModelInterpreter(model)
     feature_importance = shap_interpreter.fit_compute(X_train, X_test, y_train, y_test)
 
     # Make plots
     ax1 = shap_interpreter.plot('importance')
     ax2 = shap_interpreter.plot('summary')
     ax3 = shap_interpreter.plot('dependence', target_columns=['f1', 'f2'])
     ax4 = shap_interpreter.plot('sample', samples_index=[X_test.index.tolist()[0]])
@@ -76,20 +56,20 @@
 
     <img src="../img/model_interpret_importance.png" width="320" />
     <img src="../img/model_interpret_summary.png" width="320" />
     <img src="../img/model_interpret_dep.png" width="320" />
     <img src="../img/model_interpret_sample.png" width="320" />
     """
 
-    def __init__(self, clf, scoring="roc_auc", verbose=0, random_state=None):
+    def __init__(self, model, scoring="roc_auc", verbose=0, random_state=None):
         """
         Initializes the class.
 
         Args:
-            clf (binary classifier):
+            model (classifier or regressor):
                 Model fitted on X_train.
 
             scoring (string or probatus.utils.Scorer, optional):
                 Metric for which the model performance is calculated. It can be either a metric name  aligned with
                 predefined classification scorers names in sklearn
                 ([link](https://scikit-learn.org/stable/modules/model_evaluation.html)).
                 Another option is using probatus.utils.Scorer to define a custom metric.
@@ -101,59 +81,52 @@
                 - 1 - only most important warnings
                 - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set for the nr of samples. If it is None, the results will not be reproducible. For
                 reproducible results set it to an integer.
         """
-        self.clf = clf
+        self.model = model
         self.scorer = get_single_scorer(scoring)
         self.verbose = verbose
         self.random_state = random_state
 
     def fit(
         self,
         X_train,
         X_test,
         y_train,
         y_test,
         column_names=None,
         class_names=None,
-        shap_variance_penalty_factor=None,
         **shap_kwargs,
     ):
         """
         Fits the object and calculates the shap values for the provided datasets.
 
         Args:
             X_train (pd.DataFrame):
                 Dataframe containing training data.
 
             X_test (pd.DataFrame):
                 Dataframe containing test data.
 
             y_train (pd.Series):
-                Series of binary labels for train data.
+                Series of labels for train data.
 
             y_test (pd.Series):
-                Series of binary labels for test data.
+                Series of labels for test data.
 
             column_names (None, or list of str, optional):
                 List of feature names for the dataset. If None, then column names from the X_train dataframe are used.
 
             class_names (None, or list of str, optional):
                 List of class names e.g. ['neg', 'pos']. If none, the default ['Negative Class', 'Positive Class'] are
                 used.
 
-            shap_variance_penalty_factor (int or float, optional):
-                Apply aggregation penalty when computing average of shap values for a given feature.
-                Results in a preference for features that have smaller standard deviation of shap
-                values (more coherent shap importance). Recommend value 0.5 - 1.0.
-                Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
-
             **shap_kwargs:
                 keyword arguments passed to
                 [shap.Explainer](https://shap.readthedocs.io/en/latest/generated/shap.Explainer.html#shap.Explainer).
                 It also enables `approximate` and `check_additivity` parameters, passed while calculating SHAP values.
                 The `approximate=True` causes less accurate, but faster SHAP values calculation, while
                 `check_additivity=False` disables the additivity check inside SHAP.
         """
@@ -167,57 +140,57 @@
 
         # Set class names
         self.class_names = class_names
         if self.class_names is None:
             self.class_names = ["Negative Class", "Positive Class"]
 
         # Calculate Metrics
-        self.train_score = self.scorer.score(self.clf, self.X_train, self.y_train)
-        self.test_score = self.scorer.score(self.clf, self.X_test, self.y_test)
+        self.train_score = self.scorer.score(self.model, self.X_train, self.y_train)
+        self.test_score = self.scorer.score(self.model, self.X_test, self.y_test)
 
         self.results_text = (
             f"Train {self.scorer.metric_name}: {np.round(self.train_score, 3)},\n"
             f"Test {self.scorer.metric_name}: {np.round(self.test_score, 3)}."
         )
 
         (
             self.shap_values_train,
             self.expected_value_train,
             self.tdp_train,
         ) = self._prep_shap_related_variables(
-            clf=self.clf,
+            model=self.model,
             X=self.X_train,
             y=self.y_train,
             column_names=self.column_names,
             class_names=self.class_names,
             verbose=self.verbose,
             random_state=self.random_state,
             **shap_kwargs,
         )
 
         (
             self.shap_values_test,
             self.expected_value_test,
             self.tdp_test,
         ) = self._prep_shap_related_variables(
-            clf=self.clf,
+            model=self.model,
             X=self.X_test,
             y=self.y_test,
             column_names=self.column_names,
             class_names=self.class_names,
             verbose=self.verbose,
             random_state=self.random_state,
             **shap_kwargs,
         )
 
         self.fitted = True
 
     @staticmethod
     def _prep_shap_related_variables(
-        clf,
+        model,
         X,
         y,
         approximate=False,
         verbose=0,
         random_state=None,
         column_names=None,
         class_names=None,
@@ -227,15 +200,15 @@
         The function prepares the variables related to shap that are used to interpret the model.
 
         Returns:
             (np.array, int, DependencePlotter):
                 Shap values, expected value of the explainer, and fitted TreeDependencePlotter for a given dataset.
         """
         shap_values, explainer = shap_calc(
-            clf,
+            model,
             X,
             approximate=approximate,
             verbose=verbose,
             random_state=random_state,
             return_explainer=True,
             **shap_kwargs,
         )
@@ -243,15 +216,15 @@
         expected_value = explainer.expected_value
 
         # For sklearn models the expected values consists of two elements (negative_class and positive_class)
         if isinstance(expected_value, list) or isinstance(expected_value, np.ndarray):
             expected_value = expected_value[1]
 
         # Initialize tree dependence plotter
-        tdp = DependencePlotter(clf, verbose=verbose).fit(
+        tdp = DependencePlotter(model, verbose=verbose).fit(
             X,
             y,
             column_names=column_names,
             class_names=class_names,
             precalc_shap=shap_values,
         )
         return shap_values, expected_value, tdp
@@ -330,18 +303,18 @@
             X_train (pd.DataFrame):
                 Dataframe containing training data.
 
             X_test (pd.DataFrame):
                 Dataframe containing test data.
 
             y_train (pd.Series):
-                Series of binary labels for train data.
+                Series of labels for train data.
 
             y_test (pd.Series):
-                Series of binary labels for test data.
+                Series of labels for test data.
 
             column_names (None, or list of str, optional):
                 List of feature names for the dataset.
                 If None, then column names from the X_train dataframe are used.
 
             class_names (None, or list of str, optional):
                 List of class names e.g. ['neg', 'pos'].
@@ -376,18 +349,17 @@
         self.fit(
             X_train=X_train,
             X_test=X_test,
             y_train=y_train,
             y_test=y_test,
             column_names=column_names,
             class_names=class_names,
-            shap_variance_penalty_factor=shap_variance_penalty_factor,
             **shap_kwargs,
         )
-        return self.compute(shap_variance_penalty_factor=shap_variance_penalty_factor)
+        return self.compute(return_scores=return_scores, shap_variance_penalty_factor=shap_variance_penalty_factor)
 
     def plot(self, plot_type, target_set="test", target_columns=None, samples_index=None, show=True, **plot_kwargs):
         """
         Plots the appropriate SHAP plot.
 
         Args:
             plot_type (str):
```

### Comparing `probatus-3.0.1/probatus/interpret/shap_dependence.py` & `probatus-3.1.0/probatus/interpret/shap_dependence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2020 ING Bank N.V.
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of
-# this software and associated documentation files (the "Software"), to deal in
-# the Software without restriction, including without limitation the rights to
-# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-# the Software, and to permit persons to whom the Software is furnished to do so,
-# subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import KBinsDiscretizer
 
 from probatus.utils import BaseFitComputePlotClass, preprocess_data, preprocess_labels, shap_to_df
 
@@ -38,52 +18,52 @@
     Example:
     ```python
     from sklearn.datasets import make_classification
     from sklearn.ensemble import RandomForestClassifier
     from probatus.interpret import DependencePlotter
 
     X, y = make_classification(n_samples=15, n_features=3, n_informative=3, n_redundant=0, random_state=42)
-    clf = RandomForestClassifier().fit(X, y)
-    bdp = DependencePlotter(clf)
+    model = RandomForestClassifier().fit(X, y)
+    bdp = DependencePlotter(model)
     shap_values = bdp.fit_compute(X, y)
 
     bdp.plot(feature=2)
     ```
 
     <img src="../img/model_interpret_dep.png"/>
     """
 
-    def __init__(self, clf, verbose=0, random_state=None):
+    def __init__(self, model, verbose=0, random_state=None):
         """
         Initializes the class.
 
         Args:
-            clf (model object):
-                Binary classification model or pipeline.
+            model (model object):
+                regression or classification model or pipeline.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
                 - 1 - only most important warnings
                 - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set for the nr of samples. If it is None, the results will not be reproducible. For
                 reproducible results set it to an integer.
         """
-        self.clf = clf
+        self.model = model
         self.verbose = verbose
         self.random_state = random_state
 
     def __repr__(self):
         """
         Represent string method.
         """
-        return f"Shap dependence plotter for {self.clf.__class__.__name__}"
+        return f"Shap dependence plotter for {self.model.__class__.__name__}"
 
     def fit(self, X, y, column_names=None, class_names=None, precalc_shap=None, **shap_kwargs):
         """
         Fits the plotter to the model and data by computing the shap values.
 
         If the shap_values are passed, they do not need to be computed.
 
@@ -114,15 +94,15 @@
 
         # Set class names
         self.class_names = class_names
         if self.class_names is None:
             self.class_names = ["Negative Class", "Positive Class"]
 
         self.shap_vals_df = shap_to_df(
-            self.clf,
+            self.model,
             self.X,
             precalc_shap=precalc_shap,
             verbose=self.verbose,
             random_state=self.random_state,
             **shap_kwargs,
         )
 
@@ -147,15 +127,15 @@
         If the shap_values are passed, they do not need to be computed
 
         Args:
             X (pd.DataFrame):
                 Provided dataset.
 
             y (pd.Series):
-                Binary labels for X.
+                Labels for X.
 
             column_names (None, or list of str, optional):
                 List of feature names for the dataset. If None, then column names from the X_train dataframe are used.
 
             class_names (None, or list of str, optional):
                 List of class names e.g. ['neg', 'pos']. If none, the default ['Negative Class', 'Positive Class'] are
                 used.
```

### Comparing `probatus-3.0.1/probatus/sample_similarity/resemblance_model.py` & `probatus-3.1.0/probatus/sample_similarity/resemblance_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,18 @@
-# Copyright (c) 2020 ING Bank N.V.
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of
-# this software and associated documentation files (the "Software"), to deal in
-# the Software without restriction, including without limitation the rights to
-# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-# the Software, and to permit persons to whom the Software is furnished to do so,
-# subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
 import warnings
 
 import matplotlib.pyplot as plt
-from loguru import logger
 import numpy as np
 import pandas as pd
+from loguru import logger
 from shap import summary_plot
 from sklearn.inspection import permutation_importance
 from sklearn.model_selection import train_test_split
 
-from probatus.utils import BaseFitComputePlotClass, get_single_scorer, preprocess_data, preprocess_labels
+from probatus.utils import BaseFitComputePlotClass, preprocess_data, preprocess_labels, get_single_scorer
 from probatus.utils.shap_helpers import calculate_shap_importance, shap_calc
 
 
 class BaseResemblanceModel(BaseFitComputePlotClass):
     """
     This model checks for the similarity of two samples.
 
@@ -42,27 +22,27 @@
     This is a base class and needs to be extended by a fit() method, which implements how the data is split,
     how the model is trained and evaluated.
     Further, inheriting classes need to implement how feature importance should be indicated.
     """
 
     def __init__(
         self,
-        clf,
+        model,
         scoring="roc_auc",
         test_prc=0.25,
         n_jobs=1,
         verbose=0,
         random_state=None,
     ):
         """
         Initializes the class.
 
         Args:
-            clf (model object):
-                Binary classification model or pipeline.
+            model (model object):
+                Regression or classification model or pipeline.
 
             scoring (string or probatus.utils.Scorer, optional):
                 Metric for which the model performance is calculated. It can be either a metric name aligned with
                 predefined
                 [classification scorers names in sklearn](https://scikit-learn.org/stable/modules/model_evaluation.html).
                 Another option is using probatus.utils.Scorer to define a custom metric. The recommended option for this
                 class is 'roc_auc'.
@@ -81,15 +61,15 @@
                 - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to an integer.
         """  # noqa
-        self.clf = clf
+        self.model = model
         self.test_prc = test_prc
         self.n_jobs = n_jobs
         self.random_state = random_state
         self.verbose = verbose
         self.scorer = get_single_scorer(scoring)
 
     def _init_output_variables(self):
@@ -124,18 +104,14 @@
                 List of class names assigned, in this case provided samples e.g. ['sample1', 'sample2']. If none, the
                 default ['First Sample', 'Second Sample'] are used.
 
         Returns:
             (BaseResemblanceModel):
                 Fitted object
         """
-        # Set seed for results reproducibility
-        if self.random_state is not None:
-            np.random.seed(self.random_state)
-
         # Set class names
         self.class_names = class_names
         if self.class_names is None:
             self.class_names = ["First Sample", "Second Sample"]
 
         # Ensure inputs are correct
         self.X1, self.column_names = preprocess_data(X1, X_name="X1", column_names=column_names, verbose=self.verbose)
@@ -165,18 +141,18 @@
             self.X,
             self.y,
             test_size=self.test_prc,
             random_state=self.random_state,
             shuffle=True,
             stratify=self.y,
         )
-        self.clf.fit(self.X_train, self.y_train)
+        self.model.fit(self.X_train, self.y_train)
 
-        self.train_score = np.round(self.scorer.score(self.clf, self.X_train, self.y_train), 3)
-        self.test_score = np.round(self.scorer.score(self.clf, self.X_test, self.y_test), 3)
+        self.train_score = np.round(self.scorer.score(self.model, self.X_train, self.y_train), 3)
+        self.test_score = np.round(self.scorer.score(self.model, self.X_test, self.y_test), 3)
 
         self.results_text = (
             f"Train {self.scorer.metric_name}: {np.round(self.train_score, 3)},\n"
             f"Test {self.scorer.metric_name}: {np.round(self.test_score, 3)}."
         )
         if self.verbose > 1:
             logger.info(f"Finished model training: \n{self.results_text}")
@@ -293,38 +269,38 @@
     Examples:
     ```python
     from sklearn.datasets import make_classification
     from sklearn.ensemble import RandomForestClassifier
     from probatus.sample_similarity import PermutationImportanceResemblance
     X1, _ = make_classification(n_samples=100, n_features=5)
     X2, _ = make_classification(n_samples=100, n_features=5, shift=0.5)
-    clf = RandomForestClassifier(max_depth=2)
-    perm = PermutationImportanceResemblance(clf)
+    model = RandomForestClassifier(max_depth=2)
+    perm = PermutationImportanceResemblance(model)
     feature_importance = perm.fit_compute(X1, X2)
     perm.plot()
     ```
     <img src="../img/sample_similarity_permutation_importance.png" width="500" />
     """
 
     def __init__(
         self,
-        clf,
+        model,
         iterations=100,
         scoring="roc_auc",
         test_prc=0.25,
         n_jobs=1,
         verbose=0,
         random_state=None,
     ):
         """
         Initializes the class.
 
         Args:
-            clf (model object):
-                Binary classification model or pipeline.
+            model (model object):
+                Regression or classification model or pipeline.
 
             iterations (int, optional):
                 Number of iterations performed to calculate permutation importance. By default 100 iterations per
                 feature are done.
 
             scoring (string or probatus.utils.Scorer, optional):
                 Metric for which the model performance is calculated. It can be either a metric name aligned with
@@ -348,15 +324,15 @@
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to integer.
         """  # noqa
         super().__init__(
-            clf=clf,
+            model=model,
             scoring=scoring,
             test_prc=test_prc,
             n_jobs=n_jobs,
             verbose=verbose,
             random_state=random_state,
         )
 
@@ -397,15 +373,15 @@
         Returns:
             (PermutationImportanceResemblance):
                 Fitted object.
         """
         super().fit(X1=X1, X2=X2, column_names=column_names, class_names=class_names)
 
         permutation_result = permutation_importance(
-            self.clf,
+            self.model,
             self.X_test,
             self.y_test,
             scoring=self.scorer.scorer,
             n_repeats=self.iterations,
             n_jobs=self.n_jobs,
         )
 
@@ -524,39 +500,39 @@
     Examples:
     ```python
     from sklearn.datasets import make_classification
     from sklearn.ensemble import RandomForestClassifier
     from probatus.sample_similarity import SHAPImportanceResemblance
     X1, _ = make_classification(n_samples=100, n_features=5)
     X2, _ = make_classification(n_samples=100, n_features=5, shift=0.5)
-    clf = RandomForestClassifier(max_depth=2)
-    rm = SHAPImportanceResemblance(clf)
+    model = RandomForestClassifier(max_depth=2)
+    rm = SHAPImportanceResemblance(model)
     feature_importance = rm.fit_compute(X1, X2)
     rm.plot()
     ```
 
     <img src="../img/sample_similarity_shap_importance.png" width="320" />
     <img src="../img/sample_similarity_shap_summary.png" width="320" />
     """
 
     def __init__(
         self,
-        clf,
+        model,
         scoring="roc_auc",
         test_prc=0.25,
         n_jobs=1,
         verbose=0,
         random_state=None,
     ):
         """
         Initializes the class.
 
         Args:
-            clf (model object):
-                Binary classification model or pipeline.
+            model (model object):
+                Regression or classification model or pipeline.
 
             scoring (string or probatus.utils.Scorer, optional):
                 Metric for which the model performance is calculated. It can be either a metric name aligned with
                 predefined
                 [classification scorers names in sklearn](https://scikit-learn.org/stable/modules/model_evaluation.html).
                 Another option is using probatus.utils.Scorer to define a custom metric. Recommended option for this
                 class is 'roc_auc'.
@@ -576,15 +552,15 @@
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to integer.
         """  # noqa
         super().__init__(
-            clf=clf,
+            model=model,
             scoring=scoring,
             test_prc=test_prc,
             n_jobs=n_jobs,
             verbose=verbose,
             random_state=random_state,
         )
 
@@ -625,15 +601,15 @@
         Returns:
             (SHAPImportanceResemblance):
                 Fitted object.
         """
         super().fit(X1=X1, X2=X2, column_names=column_names, class_names=class_names)
 
         self.shap_values_test = shap_calc(
-            self.clf, self.X_test, verbose=self.verbose, random_state=self.random_state, **shap_kwargs
+            self.model, self.X_test, verbose=self.verbose, random_state=self.random_state, **shap_kwargs
         )
         self.report = calculate_shap_importance(self.shap_values_test, self.column_names)
         return self
 
     def plot(self, plot_type="bar", show=True, **summary_plot_kwargs):
         """
         Plots the resulting AUC of the model as well as the feature importances.
```

### Comparing `probatus-3.0.1/probatus/utils/shap_helpers.py` & `probatus-3.1.0/probatus/utils/shap_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-# Copyright (c) 2020 ING Bank N.V.
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of
-# this software and associated documentation files (the "Software"), to deal in
-# the Software without restriction, including without limitation the rights to
-# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-# the Software, and to permit persons to whom the Software is furnished to do so,
-# subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
 import warnings
 
 import numpy as np
 import pandas as pd
 from shap import Explainer
 from shap.explainers import TreeExplainer
 from shap.utils import sample
@@ -39,15 +19,15 @@
     check_additivity=True,
     **shap_kwargs,
 ):
     """
     Helper function to calculate the shapley values for a given model.
 
     Args:
-        model (binary model):
+        model (model):
             Trained model.
 
         X (pd.DataFrame or np.ndarray):
             features set.
 
         return_explainer (boolean):
             if True, returns a a tuple (shap_values, explainer).
@@ -73,43 +53,41 @@
 
     Returns:
         (np.ndarray or tuple(np.ndarray, shap.Explainer)):
             shapley_values for the model, optionally also returns the explainer.
 
     """
     if isinstance(model, Pipeline):
-        raise (
-            TypeError(
-                "The provided model is a Pipeline. Unfortunately, the features based on SHAP do not support "
-                "pipelines, because they cannot be used in combination with shap.Explainer. Please apply any "
-                "data transformations before running the probatus module."
-            )
+        raise TypeError(
+            "The provided model is a Pipeline. Unfortunately, the features based on SHAP do not support "
+            "pipelines, because they cannot be used in combination with shap.Explainer. Please apply any "
+            "data transformations before running the probatus module."
         )
+
     # Suppress warnings regarding XGboost and Lightgbm models.
     with warnings.catch_warnings():
-        if verbose <= 1:
-            warnings.simplefilter("ignore")
+        warnings.simplefilter("ignore" if verbose <= 1 else "default")
 
         # For tree explainers, do not pass masker when feature_perturbation is
         # tree_path_dependent, or when X contains categorical features
         # related to issue:
         # https://github.com/slundberg/shap/issues/480
         if shap_kwargs.get("feature_perturbation") == "tree_path_dependent" or X.select_dtypes("category").shape[1] > 0:
             # Calculate Shap values.
-            explainer = Explainer(model, **shap_kwargs)
+            explainer = Explainer(model, seed=random_state, **shap_kwargs)
         else:
             # Create the background data,required for non tree based models.
             # A single datapoint can passed as mask
             # (https://github.com/slundberg/shap/issues/955#issuecomment-569837201)
             if X.shape[0] < sample_size:
                 sample_size = int(np.ceil(X.shape[0] * 0.2))
             else:
                 pass
             mask = sample(X, sample_size, random_state=random_state)
-            explainer = Explainer(model, masker=mask, **shap_kwargs)
+            explainer = Explainer(model, seed=random_state, masker=mask, **shap_kwargs)
 
         # For tree-explainers allow for using check_additivity and approximate arguments
         if isinstance(explainer, TreeExplainer):
             shap_values = explainer.shap_values(X, check_additivity=check_additivity, approximate=approximate)
 
             # From SHAP version 0.43+ https://github.com/shap/shap/pull/3121 required to
             # get the second dimension of calculated Shap values.
@@ -131,41 +109,38 @@
 
 
 def shap_to_df(model, X, precalc_shap=None, **kwargs):
     """
     Calculates the shap values and return the pandas DataFrame with the columns and the index of the original.
 
     Args:
-        model (binary model):
+        model (model):
             Pretrained model (Random Forest of XGBoost at the moment).
 
         X (pd.DataFrame or np.ndarray):
             Dataset on which the SHAP importance is calculated.
 
         precalc_shap (np.array):
             Precalculated SHAP values. If None, they are computed.
 
         **kwargs: for the function shap_calc
 
     Returns:
         (pd.DataFrame):
             Dataframe with SHAP feature importance per features on X dataset.
     """
-    if precalc_shap is not None:
-        shap_values = precalc_shap
-    else:
-        shap_values = shap_calc(model, X, **kwargs)
-    if isinstance(X, pd.DataFrame):
-        return pd.DataFrame(shap_values, columns=X.columns, index=X.index)
-
-    elif isinstance(X, np.ndarray) and len(X.shape) == 2:
-        return pd.DataFrame(shap_values, columns=[f"col_{ix}" for ix in range(X.shape[1])])
+    shap_values = precalc_shap if precalc_shap is not None else shap_calc(model, X, **kwargs)
 
-    else:
-        raise NotImplementedError("X must be a dataframe or a 2d array")
+    try:
+        return pd.DataFrame(shap_values, columns=X.columns, index=X.index)
+    except AttributeError:
+        if isinstance(X, np.ndarray) and len(X.shape) == 2:
+            return pd.DataFrame(shap_values, columns=[f"col_{ix}" for ix in range(X.shape[1])])
+        else:
+            raise TypeError("X must be a dataframe or a 2d array")
 
 
 def calculate_shap_importance(shap_values, columns, output_columns_suffix="", shap_variance_penalty_factor=None):
     """
     Returns the average shapley value for each column of the dataframe, as well as the average absolute shap value.
 
     Args:
@@ -185,60 +160,44 @@
             Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
 
     Returns:
         (pd.DataFrame):
             Mean absolute shap values and Mean shap values of features.
 
     """
-    if shap_variance_penalty_factor is None:
-        _shap_variance_penalty_factor = 0
-    elif (
-        isinstance(shap_variance_penalty_factor, float) or isinstance(shap_variance_penalty_factor, int)
-    ) and shap_variance_penalty_factor >= 0:
-        _shap_variance_penalty_factor = shap_variance_penalty_factor
-    else:
+    if shap_variance_penalty_factor is None or shap_variance_penalty_factor < 0:
+        shap_variance_penalty_factor = 0
+    elif not isinstance(shap_variance_penalty_factor, (float, int)):
         warnings.warn(
-            "shap_variance_penalty_factor must be None, int or float. " "Setting shap_variance_penalty_factor = 0"
+            "shap_variance_penalty_factor must be None, int, or float. Setting shap_variance_penalty_factor = 0"
         )
-        _shap_variance_penalty_factor = 0
+        shap_variance_penalty_factor = 0
 
+    abs_shap_values = np.abs(shap_values)
     if np.ndim(shap_values) > 2:  # multi-class case
-        shap_abs_mean = np.mean(np.sum(np.abs(shap_values), axis=0), axis=0)
-        shap_mean = np.mean(np.sum(shap_values, axis=0), axis=0)
-        penalized_shap_abs_mean = np.mean(np.sum(np.abs(shap_values), axis=0), axis=0) - (
-            np.std(np.sum(np.abs(shap_values), axis=0), axis=0) * _shap_variance_penalty_factor
-        )
+        sum_abs_shap = np.sum(abs_shap_values, axis=0)
+        sum_shap = np.sum(shap_values, axis=0)
+        shap_abs_mean = np.mean(sum_abs_shap, axis=0)
+        shap_mean = np.mean(sum_shap, axis=0)
+        penalized_shap_abs_mean = shap_abs_mean - (np.std(sum_abs_shap, axis=0) * shap_variance_penalty_factor)
     else:
         # Find average shap importance for neg and pos class
-        shap_abs_mean = np.mean(np.abs(shap_values), axis=0)
+        shap_abs_mean = np.mean(abs_shap_values, axis=0)
         shap_mean = np.mean(shap_values, axis=0)
-        penalized_shap_abs_mean = np.mean(np.abs(shap_values), axis=0) - (
-            np.std(np.abs(shap_values), axis=0) * _shap_variance_penalty_factor
-        )
+        penalized_shap_abs_mean = shap_abs_mean - (np.std(abs_shap_values, axis=0) * shap_variance_penalty_factor)
 
-    # Prepare importance values in a handy df
+    # Prepare the values in a df and set the correct column types
     importance_df = pd.DataFrame(
         {
-            f"mean_abs_shap_value{output_columns_suffix}": shap_abs_mean.tolist(),
-            f"mean_shap_value{output_columns_suffix}": shap_mean.tolist(),
-            f"penalized_mean_abs_shap_value{output_columns_suffix}": penalized_shap_abs_mean.tolist(),
+            f"mean_abs_shap_value{output_columns_suffix}": shap_abs_mean,
+            f"mean_shap_value{output_columns_suffix}": shap_mean,
+            f"penalized_mean_abs_shap_value{output_columns_suffix}": penalized_shap_abs_mean,
         },
         index=columns,
-    )
-
-    # Set the correct column types
-    importance_df[f"mean_abs_shap_value{output_columns_suffix}"] = importance_df[
-        f"mean_abs_shap_value{output_columns_suffix}"
-    ].astype(float)
-    importance_df[f"mean_shap_value{output_columns_suffix}"] = importance_df[
-        f"mean_shap_value{output_columns_suffix}"
-    ].astype(float)
-    importance_df[f"penalized_mean_abs_shap_value{output_columns_suffix}"] = importance_df[
-        f"penalized_mean_abs_shap_value{output_columns_suffix}"
-    ].astype(float)
+    ).astype(float)
 
     importance_df = importance_df.sort_values(f"penalized_mean_abs_shap_value{output_columns_suffix}", ascending=False)
 
     # Drop penalized column
     importance_df = importance_df.drop(columns=[f"penalized_mean_abs_shap_value{output_columns_suffix}"])
 
     return importance_df
```

### Comparing `probatus-3.0.1/probatus.egg-info/PKG-INFO` & `probatus-3.1.0/probatus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 3.0.1
-Summary: Validation of binary classifiers and data used to develop them
+Version: 3.1.0
+Summary: Validation of regression & classifiers and data used to develop them
 Author-email: "ING Bank N.V." <reinier.koops@ing.com>
-License: Copyright (c) 2020 ING Bank N.V.
+License: Copyright (c) ING Bank N.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://ing-bank.github.io/probatus/
@@ -78,15 +78,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
 ![GitHub contributors](https://img.shields.io/github/contributors/ing-bank/probatus)
 
 # Probatus
 
 ## Overview
 
-**Probatus** is a python package that helps validate binary classification models and the data used to develop them. Main features:
+**Probatus** is a python package that helps validate regression & (multiclass) classification models and the data used to develop them. Main features:
 
 - [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools
 - [probatus.sample_similarity](https://ing-bank.github.io/probatus/api/sample_similarity.html) to compare two datasets using resemblance modelling, f.e. `train` with out-of-time `test`.
 - [probatus.feature_elimination.ShapRFECV](https://ing-bank.github.io/probatus/api/feature_elimination.html) provides cross-validated Recursive Feature Elimination using shap feature importance.
 
 ## Installation
```

### Comparing `probatus-3.0.1/probatus.egg-info/SOURCES.txt` & `probatus-3.1.0/probatus.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 probatus/__init__.py
 probatus.egg-info/PKG-INFO
 probatus.egg-info/SOURCES.txt
 probatus.egg-info/dependency_links.txt
 probatus.egg-info/requires.txt
 probatus.egg-info/top_level.txt
 probatus/feature_elimination/__init__.py
+probatus/feature_elimination/early_stopping_feature_elimination.py
 probatus/feature_elimination/feature_elimination.py
 probatus/interpret/__init__.py
 probatus/interpret/model_interpret.py
 probatus/interpret/shap_dependence.py
 probatus/sample_similarity/__init__.py
 probatus/sample_similarity/resemblance_model.py
 probatus/utils/__init__.py
 probatus/utils/_utils.py
 probatus/utils/arrayfuncs.py
 probatus/utils/base_class_interface.py
 probatus/utils/exceptions.py
-probatus/utils/missing_helpers.py
-probatus/utils/plots.py
 probatus/utils/scoring.py
 probatus/utils/shap_helpers.py
-probatus/utils/warnings.py
 tests/docs/__init__.py
 tests/docs/test_docstring.py
 tests/docs/test_notebooks.py
 tests/feature_elimination/test_feature_elimination.py
 tests/interpret/__init__.py
 tests/interpret/test_model_interpret.py
 tests/interpret/test_shap_dependence.py
```

### Comparing `probatus-3.0.1/probatus.egg-info/requires.txt` & `probatus-3.1.0/probatus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `probatus-3.0.1/pyproject.toml` & `probatus-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "probatus"
-version = "3.0.1"
+version = "3.1.0"
 requires-python= ">=3.8"
-description = "Validation of binary classifiers and data used to develop them"
+description = "Validation of regression & classifiers and data used to develop them"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "ING Bank N.V.", email = "reinier.koops@ing.com" }
 ]
 license = { file = "LICENCE" }
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `probatus-3.0.1/tests/docs/test_docstring.py` & `probatus-3.1.0/tests/docs/test_docstring.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.1/tests/feature_elimination/test_feature_elimination.py` & `probatus-3.1.0/tests/feature_elimination/test_feature_elimination.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-import os
-
 import pandas as pd
 import pytest
 from lightgbm import LGBMClassifier
-from sklearn.datasets import make_classification
+from sklearn.datasets import load_diabetes, make_classification
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import RandomizedSearchCV, StratifiedGroupKFold, StratifiedKFold
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import StandardScaler
 from sklearn.svm import SVC
-from xgboost import XGBClassifier
+from xgboost import XGBClassifier, XGBRegressor
 
 from probatus.feature_elimination import EarlyStoppingShapRFECV, ShapRFECV
 from probatus.utils import preprocess_labels
 
 
 @pytest.fixture(scope="function")
 def X():
-    """
-    Fixture for X.
-    """
     return pd.DataFrame(
         {
             "col_1": [1, 1, 1, 1, 1, 1, 1, 0],
             "col_2": [0, 0, 0, 0, 0, 0, 0, 1],
             "col_3": [1, 0, 1, 0, 1, 0, 1, 0],
         },
         index=[1, 2, 3, 4, 5, 6, 7, 8],
     )
 
 
 @pytest.fixture(scope="function")
 def y():
-    """
-    Fixture for y.
-    """
     return pd.Series([1, 0, 1, 0, 1, 0, 1, 0], index=[1, 2, 3, 4, 5, 6, 7, 8])
 
 
 @pytest.fixture(scope="function")
 def sample_weight():
-    """
-    Fixture for sample_weight.
-    """
     return pd.Series([1, 1, 1, 1, 1, 1, 1, 1], index=[1, 2, 3, 4, 5, 6, 7, 8])
 
 
 @pytest.fixture(scope="function")
 def groups():
-    """
-    Fixture for groups.
-    """
     return pd.Series(["grp1", "grp1", "grp1", "grp1", "grp2", "grp2", "grp2", "grp2"], index=[1, 2, 3, 4, 5, 6, 7, 8])
 
 
 @pytest.fixture(scope="function")
 def XGBoost_classifier(random_state):
-    """This fixture allows to reuse the import of the XGBClassifier class across different tests."""
     model = XGBClassifier(n_estimators=200, max_depth=3, random_state=random_state)
     return model
 
 
+@pytest.fixture(scope="function")
+def XGBoost_regressor(random_state):
+    model = XGBRegressor(n_estimators=200, max_depth=3, random_state=random_state)
+    return model
+
+
+def test_shap_rfe_regressor(XGBoost_regressor, random_state):
+    diabetes = load_diabetes()
+    X = pd.DataFrame(diabetes.data, columns=diabetes.feature_names)
+    y = diabetes.target
+
+    shap_elimination = ShapRFECV(XGBoost_regressor, step=0.8, cv=2, scoring="r2", n_jobs=4, random_state=random_state)
+    report = shap_elimination.fit_compute(X, y)
+
+    assert report.shape[0] == 3
+    assert shap_elimination.get_reduced_features_set(1) == ["bmi"]
+
+    _ = shap_elimination.plot(show=False)
+
+
 def test_shap_rfe_randomized_search(X, y, randomized_search_decision_tree_classifier, random_state):
-    """
-    Test with RandomizedSearchCV.
-    """
     search = randomized_search_decision_tree_classifier
     shap_elimination = ShapRFECV(search, step=0.8, cv=2, scoring="roc_auc", n_jobs=4, random_state=random_state)
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == 2
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
@@ -87,17 +89,14 @@
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
 def test_shap_rfe(X, y, sample_weight, decision_tree_classifier, random_state):
-    """
-    Test with ShapRFECV.
-    """
     shap_elimination = ShapRFECV(
         decision_tree_classifier,
         random_state=random_state,
         step=1,
         cv=2,
         scoring="roc_auc",
         n_jobs=4,
@@ -105,17 +104,14 @@
     report = shap_elimination.fit_compute(X, y, sample_weight=sample_weight, approximate=True, check_additivity=False)
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
 def test_shap_rfe_group_cv(X, y, groups, sample_weight, decision_tree_classifier, random_state):
-    """
-    Test ShapRFECV with StratifiedGroupKFold.
-    """
     cv = StratifiedGroupKFold(n_splits=2, shuffle=True, random_state=random_state)
     shap_elimination = ShapRFECV(
         decision_tree_classifier,
         random_state=random_state,
         step=1,
         cv=cv,
         scoring="roc_auc",
@@ -126,64 +122,52 @@
     )
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
 def test_shap_pipeline_error(X, y, decision_tree_classifier, random_state):
-    """
-    Test with ShapRFECV for pipelines.
-    """
-    clf = Pipeline(
+    model = Pipeline(
         [
             ("scaler", StandardScaler()),
             ("dt", decision_tree_classifier),
         ]
     )
     with pytest.raises(TypeError):
         shap_elimination = ShapRFECV(
-            clf,
+            model,
             random_state=random_state,
             step=1,
             cv=2,
             scoring="roc_auc",
             n_jobs=4,
         )
         shap_elimination = shap_elimination.fit(X, y, approximate=True, check_additivity=False)
 
 
 def test_shap_rfe_linear_model(X, y, random_state):
-    """
-    Test ShapRFECV with linear model.
-    """
-    clf = LogisticRegression(C=1, random_state=random_state)
-    shap_elimination = ShapRFECV(clf, random_state=random_state, step=1, cv=2, scoring="roc_auc", n_jobs=4)
+    model = LogisticRegression(C=1, random_state=random_state)
+    shap_elimination = ShapRFECV(model, random_state=random_state, step=1, cv=2, scoring="roc_auc", n_jobs=4)
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
 def test_shap_rfe_svm(X, y, random_state):
-    """
-    Test with ShapRFECV with SVM.
-    """
-    clf = SVC(C=1, kernel="linear", probability=True, random_state=random_state)
-    shap_elimination = ShapRFECV(clf, random_state=random_state, step=1, cv=2, scoring="roc_auc", n_jobs=4)
+    model = SVC(C=1, kernel="linear", probability=True, random_state=random_state)
+    shap_elimination = ShapRFECV(model, random_state=random_state, step=1, cv=2, scoring="roc_auc", n_jobs=4)
     shap_elimination = shap_elimination.fit(X, y)
     report = shap_elimination.compute()
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
 def test_shap_rfe_cols_to_keep(X, y, decision_tree_classifier, random_state):
-    """
-    Test for shap_rfe_cv with features to keep parameter.
-    """
     shap_elimination = ShapRFECV(
         decision_tree_classifier,
         random_state=random_state,
         step=2,
         cv=2,
         scoring="roc_auc",
         n_jobs=4,
@@ -193,30 +177,24 @@
 
     assert report.shape[0] == 2
     reduced_feature_set = set(shap_elimination.get_reduced_features_set(num_features=2))
     assert reduced_feature_set == {"col_2", "col_3"}
 
 
 def test_shap_rfe_randomized_search_cols_to_keep(X, y, randomized_search_decision_tree_classifier, random_state):
-    """
-    Test with ShapRFECV with column to keep param.
-    """
     search = randomized_search_decision_tree_classifier
     shap_elimination = ShapRFECV(search, step=0.8, cv=2, scoring="roc_auc", n_jobs=4, random_state=random_state)
     report = shap_elimination.fit_compute(X, y, columns_to_keep=["col_2", "col_3"])
 
     assert report.shape[0] == 2
     reduced_feature_set = set(shap_elimination.get_reduced_features_set(num_features=2))
     assert reduced_feature_set == {"col_2", "col_3"}
 
 
 def test_calculate_number_of_features_to_remove():
-    """
-    Test with ShapRFECV with n features to remove.
-    """
     assert 3 == ShapRFECV._calculate_number_of_features_to_remove(
         current_num_of_features=10, num_features_to_remove=3, min_num_features_to_keep=5
     )
     assert 3 == ShapRFECV._calculate_number_of_features_to_remove(
         current_num_of_features=8, num_features_to_remove=5, min_num_features_to_keep=5
     )
     assert 0 == ShapRFECV._calculate_number_of_features_to_remove(
@@ -224,17 +202,14 @@
     )
     assert 4 == ShapRFECV._calculate_number_of_features_to_remove(
         current_num_of_features=5, num_features_to_remove=7, min_num_features_to_keep=1
     )
 
 
 def test_shap_automatic_num_feature_selection(decision_tree_classifier, random_state):
-    """
-    Test automatic num feature selection methods
-    """
     X = pd.DataFrame(
         {
             "col_1": [1, 0, 1, 0, 1, 0, 1, 0],
             "col_2": [0, 0, 0, 0, 0, 1, 1, 1],
             "col_3": [1, 1, 1, 0, 0, 0, 0, 0],
         }
     )
@@ -258,17 +233,14 @@
 
     assert best_features == ["col_2"]
     assert best_coherent_features == ["col_1", "col_2", "col_3"]
     assert best_parsimonious_features == ["col_2"]
 
 
 def test_get_feature_shap_values_per_fold(X, y, decision_tree_classifier, random_state):
-    """
-    Test with ShapRFECV with features per fold.
-    """
     shap_elimination = ShapRFECV(decision_tree_classifier, scoring="roc_auc", random_state=random_state)
     (
         shap_values,
         train_score,
         test_score,
     ) = shap_elimination._get_feature_shap_values_per_fold(
         X,
@@ -343,17 +315,14 @@
         "f18",
         "f19",
         "f20",
     ] == kept_features
 
 
 def test_shap_rfe_penalty_factor(X, y, decision_tree_classifier, random_state):
-    """
-    Test ShapRFECV with shap_variance_penalty_factor
-    """
     shap_elimination = ShapRFECV(
         decision_tree_classifier,
         random_state=random_state,
         step=1,
         cv=2,
         scoring="roc_auc",
         n_jobs=1,
@@ -362,65 +331,53 @@
         X, y, shap_variance_penalty_factor=1.0, approximate=True, check_additivity=False
     )
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_1"]
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_complex_dataset(complex_data, complex_lightgbm, random_state_1):
-    """
-    Test on complex dataset.
-    """
     X, y = complex_data
 
     param_grid = {
         "n_estimators": [5, 7, 10],
         "num_leaves": [3, 5, 7, 10],
     }
     search = RandomizedSearchCV(complex_lightgbm, param_grid, n_iter=1, random_state=random_state_1)
 
     shap_elimination = ShapRFECV(
-        clf=search, step=1, cv=10, scoring="roc_auc", n_jobs=3, verbose=1, random_state=random_state_1
+        model=search, step=1, cv=10, scoring="roc_auc", n_jobs=3, verbose=1, random_state=random_state_1
     )
 
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == X.shape[1]
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_shap_rfe_early_stopping_lightGBM(complex_data, random_state):
-    """
-    Test EarlyStoppingShapRFECV with a LGBMClassifier.
-    """
-    clf = LGBMClassifier(n_estimators=200, max_depth=3, random_state=random_state)
+    model = LGBMClassifier(n_estimators=200, max_depth=3, random_state=random_state)
     X, y = complex_data
 
     shap_elimination = EarlyStoppingShapRFECV(
-        clf,
+        model,
         random_state=random_state,
         step=1,
         cv=10,
         scoring="roc_auc",
         n_jobs=4,
         early_stopping_rounds=5,
         eval_metric="auc",
     )
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 5
     assert shap_elimination.get_reduced_features_set(1) == ["f5"]
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_shap_rfe_early_stopping_XGBoost(XGBoost_classifier, complex_data, random_state):
-    """
-    Test EarlyStoppingShapRFECV with a LGBMClassifier.
-    """
     X, y = complex_data
     X["f1_categorical"] = X["f1_categorical"].astype(float)
 
     shap_elimination = EarlyStoppingShapRFECV(
         XGBoost_classifier,
         random_state=random_state,
         step=1,
@@ -432,19 +389,17 @@
     )
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 5
     assert shap_elimination.get_reduced_features_set(1) == ["f4"]
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
+#
+#
 def test_shap_rfe_early_stopping_CatBoost(complex_data_with_categorical, catboost_classifier, random_state):
-    """
-    Test EarlyStoppingShapRFECV with a CatBoostClassifier.
-    """
     X, y = complex_data_with_categorical
 
     shap_elimination = EarlyStoppingShapRFECV(
         catboost_classifier,
         random_state=random_state,
         step=1,
         cv=10,
@@ -455,26 +410,22 @@
     )
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 5
     assert shap_elimination.get_reduced_features_set(1)[0] in ["f4", "f5"]
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_shap_rfe_randomized_search_early_stopping_lightGBM(complex_data, random_state):
-    """
-    Test EarlyStoppingShapRFECV with RandomizedSearchCV and a LGBMClassifier on complex dataset.
-    """
-    clf = LGBMClassifier(n_estimators=200, random_state=random_state)
+    model = LGBMClassifier(n_estimators=200, random_state=random_state)
     X, y = complex_data
 
     param_grid = {
         "max_depth": [3, 4, 5],
     }
-    search = RandomizedSearchCV(clf, param_grid, cv=2, n_iter=2, random_state=random_state)
+    search = RandomizedSearchCV(model, param_grid, cv=2, n_iter=2, random_state=random_state)
     shap_elimination = EarlyStoppingShapRFECV(
         search,
         step=1,
         cv=10,
         scoring="roc_auc",
         early_stopping_rounds=5,
         eval_metric="auc",
@@ -486,49 +437,41 @@
 
     assert report.shape[0] == X.shape[1]
     assert shap_elimination.get_reduced_features_set(1) == ["f5"]
 
     _ = shap_elimination.plot(show=False)
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_get_feature_shap_values_per_fold_early_stopping_lightGBM(complex_data, random_state):
-    """
-    Test with ShapRFECV with features per fold.
-    """
-    clf = LGBMClassifier(n_estimators=200, max_depth=3, random_state=random_state)
+    model = LGBMClassifier(n_estimators=200, max_depth=3, random_state=random_state)
     X, y = complex_data
     y = preprocess_labels(y, y_name="y", index=X.index)
 
     shap_elimination = EarlyStoppingShapRFECV(
-        clf, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
+        model, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
     )
     (
         shap_values,
         train_score,
         test_score,
     ) = shap_elimination._get_feature_shap_values_per_fold(
         X,
         y,
-        clf,
+        model,
         train_index=list(range(5, 50)),
         val_index=[0, 1, 2, 3, 4],
     )
     assert test_score > 0.6
     assert train_score > 0.6
     assert shap_values.shape == (5, 5)
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_get_feature_shap_values_per_fold_early_stopping_CatBoost(
     complex_data_with_categorical, catboost_classifier, random_state
 ):
-    """
-    Test with ShapRFECV with features per fold.
-    """
     X, y = complex_data_with_categorical
     y = preprocess_labels(y, y_name="y", index=X.index)
 
     shap_elimination = EarlyStoppingShapRFECV(
         catboost_classifier, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
     )
     (
@@ -543,19 +486,15 @@
         val_index=[0, 1, 2, 3, 4],
     )
     assert test_score > 0
     assert train_score > 0.6
     assert shap_values.shape == (5, 5)
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_get_feature_shap_values_per_fold_early_stopping_XGBoost(XGBoost_classifier, complex_data, random_state):
-    """
-    Test with ShapRFECV with features per fold.
-    """
     X, y = complex_data
     y = preprocess_labels(y, y_name="y", index=X.index)
 
     shap_elimination = EarlyStoppingShapRFECV(
         XGBoost_classifier, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
     )
     (
@@ -570,21 +509,19 @@
         val_index=[0, 1, 2, 3, 4],
     )
     assert test_score > 0
     assert train_score > 0.6
     assert shap_values.shape == (5, 5)
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_EarlyStoppingShapRFECV_no_categorical(complex_data, random_state):
-    """Test EarlyStoppingShapRFECV when no categorical features are present."""
-    clf = LGBMClassifier(n_estimators=50, max_depth=3, num_leaves=3, random_state=random_state)
+    model = LGBMClassifier(n_estimators=50, max_depth=3, num_leaves=3, random_state=random_state)
 
     shap_elimination = EarlyStoppingShapRFECV(
-        clf=clf,
+        model=model,
         step=0.33,
         cv=5,
         scoring="accuracy",
         eval_metric="logloss",
         early_stopping_rounds=5,
         random_state=random_state,
     )
@@ -594,15 +531,14 @@
 
     assert report.shape[0] == X.shape[1]
     assert shap_elimination.get_reduced_features_set(1) == ["f5"]
 
     _ = shap_elimination.plot(show=False)
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_LightGBM_stratified_kfold(random_state):
     """
     Test added to check for https://github.com/ing-bank/probatus/issues/170.
     """
     X = pd.DataFrame(
         [
             [1, 2, 3, 4, 5, 101, 102, 103, 104, 105],
@@ -611,22 +547,22 @@
         ]
     ).transpose()
     X[2] = X[2].astype("category")
     X[1] = X[1].astype("float")
     X[0] = X[0].astype("float")
     y = [0] * 5 + [1] * 5
 
-    clf = LGBMClassifier(random_state=random_state)
+    model = LGBMClassifier(random_state=random_state)
     n_iter = 2
     n_folds = 3
 
     for _ in range(n_iter):
         skf = StratifiedKFold(n_folds, shuffle=True, random_state=random_state)
         shap_elimination = EarlyStoppingShapRFECV(
-            clf=clf,
+            model=model,
             step=1 / (n_iter + 1),
             cv=skf,
             scoring="accuracy",
             eval_metric="logloss",
             early_stopping_rounds=5,
             random_state=random_state,
         )
```

### Comparing `probatus-3.0.1/tests/interpret/test_model_interpret.py` & `probatus-3.1.0/tests/interpret/test_model_interpret.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,41 @@
-import os
-
 import numpy as np
 import pandas as pd
 import pytest
 
 from probatus.interpret import ShapModelInterpreter
 
 
 @pytest.fixture(scope="function")
 def expected_feature_importance():
-    """
-    Fixture.
-    """
     return pd.DataFrame(
         {
             "mean_abs_shap_value_test": [0.5, 0.0, 0.0],
             "mean_abs_shap_value_train": [0.5, 0.0, 0.0],
             "mean_shap_value_test": [-0.5, 0.0, 0.0],
             "mean_shap_value_train": [-0.5, 0.0, 0.0],
         },
         index=["col_3", "col_1", "col_2"],
     )
 
 
 @pytest.fixture(scope="function")
 def expected_feature_importance_lin_models():
-    """
-    Test.
-    """
     return pd.DataFrame(
         {
             "mean_abs_shap_value_test": [0.4, 0.0, 0.0],
             "mean_abs_shap_value_train": [0.4, 0.0, 0.0],
             "mean_shap_value_test": [-0.4, 0.0, 0.0],
             "mean_shap_value_train": [-0.4, 0.0, 0.0],
         },
         index=["col_3", "col_1", "col_2"],
     )
 
 
 def test_shap_interpret(fitted_tree, X_train, y_train, X_test, y_test, expected_feature_importance, random_state):
-    """
-    Test.
-    """
     class_names = ["neg", "pos"]
 
     shap_interpret = ShapModelInterpreter(fitted_tree, random_state=random_state)
     shap_interpret.fit(X_train, X_test, y_train, y_test, class_names=class_names)
 
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
@@ -80,17 +69,14 @@
     assert isinstance(ax7, list) and len(ax7) == 2
     assert isinstance(ax8, list) and len(ax8) == 2
 
 
 def test_shap_interpret_lin_models(
     fitted_logistic_regression, X_train, y_train, X_test, y_test, expected_feature_importance_lin_models, random_state
 ):
-    """
-    Test.
-    """
     class_names = ["neg", "pos"]
 
     shap_interpret = ShapModelInterpreter(fitted_logistic_regression, random_state=random_state)
     shap_interpret.fit(X_train, X_test, y_train, y_test, class_names=class_names)
 
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
@@ -125,17 +111,14 @@
     assert isinstance(ax7, list) and len(ax7) == 2
     assert isinstance(ax8, list) and len(ax8) == 2
 
 
 def test_shap_interpret_fit_compute_lin_models(
     fitted_logistic_regression, X_train, y_train, X_test, y_test, expected_feature_importance_lin_models, random_state
 ):
-    """
-    Test.
-    """
     class_names = ["neg", "pos"]
 
     shap_interpret = ShapModelInterpreter(fitted_logistic_regression, random_state=random_state)
     importance_df = shap_interpret.fit_compute(X_train, X_test, y_train, y_test, class_names=class_names)
     importance_df = importance_df.round(2)
 
     assert shap_interpret.class_names == class_names
@@ -149,17 +132,14 @@
 
     pd.testing.assert_frame_equal(expected_feature_importance_lin_models, importance_df)
 
 
 def test_shap_interpret_fit_compute(
     fitted_tree, X_train, y_train, X_test, y_test, expected_feature_importance, random_state
 ):
-    """
-    Test.
-    """
     class_names = ["neg", "pos"]
 
     shap_interpret = ShapModelInterpreter(fitted_tree, random_state=random_state)
     importance_df = shap_interpret.fit_compute(X_train, X_test, y_train, y_test, class_names=class_names)
 
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
@@ -168,19 +148,15 @@
     # Check expected shap values
     assert (np.mean(np.abs(shap_interpret.shap_values_test), axis=0) == [0, 0, 0.5]).all()
     assert (np.mean(np.abs(shap_interpret.shap_values_train), axis=0) == [0, 0, 0.5]).all()
 
     pd.testing.assert_frame_equal(expected_feature_importance, importance_df)
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_shap_interpret_complex_data(complex_data_split_with_categorical, complex_fitted_lightgbm, random_state):
-    """
-    Test lightgbm.
-    """
     class_names = ["neg", "pos"]
     X_train, X_test, y_train, y_test = complex_data_split_with_categorical
 
     shap_interpret = ShapModelInterpreter(complex_fitted_lightgbm, verbose=1, random_state=random_state)
     importance_df = shap_interpret.fit_compute(
         X_train, X_test, y_train, y_test, class_names=class_names, approximate=False, check_additivity=False
     )
```

### Comparing `probatus-3.0.1/tests/interpret/test_shap_dependence.py` & `probatus-3.1.0/tests/interpret/test_shap_dependence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 from sklearn.ensemble import RandomForestClassifier
 
@@ -13,17 +11,14 @@
 # Turn off interactive mode in plots
 plt.ioff()
 matplotlib.use("Agg")
 
 
 @pytest.fixture(scope="function")
 def X_y():
-    """
-    Fixture.
-    """
     return (
         pd.DataFrame(
             [
                 [1.72568193, 2.21070436, 1.46039061],
                 [-1.48382902, 2.88364928, 0.22323996],
                 [-0.44947744, 0.85434638, -2.54486421],
                 [-1.38101231, 1.77505901, -1.36000132],
@@ -42,17 +37,14 @@
         ),
         pd.Series([1, 1, 0, 0, 1, 1, 0, 1, 1, 0, 1, 0, 0, 0, 0]),
     )
 
 
 @pytest.fixture(scope="function")
 def expected_shap_vals():
-    """
-    Fixture.
-    """
     return pd.DataFrame(
         [
             [0.176667, 0.005833, 0.284167],
             [-0.042020, 0.224520, 0.284167],
             [-0.092020, -0.135480, -0.205833],
             [-0.092020, -0.135480, -0.205833],
             [0.002424, 0.000909, 0.263333],
@@ -67,74 +59,58 @@
             [-0.108687, 0.081187, -0.205833],
             [-0.092020, -0.164646, -0.176667],
         ]
     )
 
 
 @pytest.fixture(scope="function")
-def clf(X_y, random_state):
-    """
-    Fixture.
-    """
+def model(X_y, random_state):
     X, y = X_y
 
     model = RandomForestClassifier(random_state=random_state, n_estimators=10, max_depth=5)
 
     model.fit(X, y)
     return model
 
 
 @pytest.fixture(scope="function")
 def expected_feat_importances():
-    """
-    Test.
-    """
     return pd.DataFrame(
         {
             "Feature Name": {0: 2, 1: 1, 2: 0},
             "Shap absolute importance": {0: 0.2199, 1: 0.1271, 2: 0.1022},
             "Shap signed importance": {0: 0.0292, 1: -0.0149, 2: -0.0076},
         }
     )
 
 
-def test_not_fitted(clf, random_state):
-    """
-    Test.
-    """
-    plotter = DependencePlotter(clf, random_state)
+def test_not_fitted(model, random_state):
+    plotter = DependencePlotter(model, random_state)
     assert plotter.fitted is False
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_fit_complex(complex_data_split, complex_fitted_lightgbm, random_state):
-    """
-    Test.
-    """
     _, X_test, _, y_test = complex_data_split
 
     plotter = DependencePlotter(complex_fitted_lightgbm, random_state=random_state)
 
     plotter.fit(X_test, y_test)
 
     pd.testing.assert_frame_equal(plotter.X, X_test)
     pd.testing.assert_series_equal(plotter.y, pd.Series(y_test, index=X_test.index))
     assert plotter.fitted is True
 
     # Check if plotting does not cause errors
     _ = plotter.plot(feature="f2_missing", show=False)
 
 
-def test_get_X_y_shap_with_q_cut_normal(X_y, clf, random_state):
-    """
-    Test.
-    """
+def test_get_X_y_shap_with_q_cut_normal(X_y, model, random_state):
     X, y = X_y
 
-    plotter = DependencePlotter(clf, random_state).fit(X, y)
+    plotter = DependencePlotter(model, random_state).fit(X, y)
     plotter.min_q, plotter.max_q = 0, 1
 
     X_cut, y_cut, _ = plotter._get_X_y_shap_with_q_cut(0)
     assert np.isclose(X[0], X_cut).all()
     assert y.equals(y_cut)
 
     plotter.min_q = 0.2
@@ -154,61 +130,46 @@
             -2.10917352,
             -1.25945582,
         ],
     ).all()
     assert np.equal(y_cut.values, [1, 0, 0, 1, 1, 0, 0, 0, 0]).all()
 
 
-def test_get_X_y_shap_with_q_cut_unfitted(clf, random_state):
-    """
-    Test.
-    """
-    plotter = DependencePlotter(clf, random_state)
+def test_get_X_y_shap_with_q_cut_unfitted(model, random_state):
+    plotter = DependencePlotter(model, random_state)
     with pytest.raises(NotFittedError):
         plotter._get_X_y_shap_with_q_cut(0)
 
 
-def test_get_X_y_shap_with_q_cut_input(X_y, clf, random_state):
-    """
-    Test.
-    """
-    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1])
+def test_get_X_y_shap_with_q_cut_input(X_y, model, random_state):
+    plotter = DependencePlotter(model, random_state).fit(X_y[0], X_y[1])
     with pytest.raises(ValueError):
         plotter._get_X_y_shap_with_q_cut("not a feature")
 
 
-def test_plot_normal(X_y, clf, random_state):
-    """
-    Test.
-    """
-    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1])
+def test_plot_normal(X_y, model, random_state):
+    plotter = DependencePlotter(model, random_state).fit(X_y[0], X_y[1])
     _ = plotter.plot(feature=0)
 
 
-def test_plot_class_names(X_y, clf, random_state):
-    """
-    Test.
-    """
-    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1], class_names=["a", "b"])
+def test_plot_class_names(X_y, model, random_state):
+    plotter = DependencePlotter(model, random_state).fit(X_y[0], X_y[1], class_names=["a", "b"])
     _ = plotter.plot(feature=0)
     assert plotter.class_names == ["a", "b"]
 
 
-def test_plot_input(X_y, clf, random_state):
-    """
-    Test.
-    """
-    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1])
+def test_plot_input(X_y, model, random_state):
+    plotter = DependencePlotter(model, random_state).fit(X_y[0], X_y[1])
     with pytest.raises(ValueError):
         plotter.plot(feature="not a feature")
     with pytest.raises(TypeError):
         plotter.plot(feature=0, bins=5.0)
     with pytest.raises(ValueError):
         plotter.plot(feature=0, min_q=1, max_q=0)
 
 
-def test__repr__(clf, random_state):
+def test__repr__(model, random_state):
     """
     Test string representation.
     """
-    plotter = DependencePlotter(clf, random_state)
+    plotter = DependencePlotter(model, random_state)
     assert str(plotter) == "Shap dependence plotter for RandomForestClassifier"
```

### Comparing `probatus-3.0.1/tests/sample_similarity/test_resemblance_model.py` & `probatus-3.1.0/tests/sample_similarity/test_resemblance_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.api.types import is_numeric_dtype
 
@@ -12,32 +10,23 @@
 # Turn off interactive mode in plots
 plt.ioff()
 matplotlib.use("Agg")
 
 
 @pytest.fixture(scope="function")
 def X1():
-    """
-    Fixture.
-    """
     return pd.DataFrame({"col_1": [1, 1, 1, 1], "col_2": [0, 0, 0, 0], "col_3": [0, 0, 0, 0]}, index=[1, 2, 3, 4])
 
 
 @pytest.fixture(scope="function")
 def X2():
-    """
-    Fixture.
-    """
     return pd.DataFrame({"col_1": [0, 0, 0, 0], "col_2": [0, 0, 0, 0], "col_3": [0, 0, 0, 0]}, index=[1, 2, 3, 4])
 
 
 def test_base_class(X1, X2, decision_tree_classifier, random_state):
-    """
-    Test.
-    """
     rm = BaseResemblanceModel(decision_tree_classifier, test_prc=0.5, n_jobs=1, random_state=random_state)
 
     actual_report, train_score, test_score = rm.fit_compute(X1, X2, return_scores=True)
 
     assert train_score == 1
     assert test_score == 1
     assert actual_report is None
@@ -59,17 +48,14 @@
     assert list(rm.X.index) == list(rm.y.index)
 
     with pytest.raises(NotImplementedError) as _:
         rm.plot()
 
 
 def test_base_class_lin_models(X1, X2, logistic_regression, random_state):
-    """
-    Test.
-    """
     # Test class BaseResemblanceModel for linear models.
     rm = BaseResemblanceModel(logistic_regression, test_prc=0.5, n_jobs=1, random_state=random_state)
 
     actual_report, train_score, test_score = rm.fit_compute(X1, X2, return_scores=True)
 
     assert train_score == 1
     assert test_score == 1
@@ -92,17 +78,14 @@
     assert list(rm.X.index) == list(rm.y.index)
 
     with pytest.raises(NotImplementedError) as _:
         rm.plot()
 
 
 def test_shap_resemblance_class(X1, X2, decision_tree_classifier, random_state):
-    """
-    Test.
-    """
     rm = SHAPImportanceResemblance(decision_tree_classifier, test_prc=0.5, n_jobs=1, random_state=random_state)
 
     actual_report, train_score, test_score = rm.fit_compute(X1, X2, return_scores=True)
 
     assert train_score == 1
     assert test_score == 1
 
@@ -123,17 +106,14 @@
 
     # Run plots
     rm.plot(plot_type="bar")
     rm.plot(plot_type="dot")
 
 
 def test_shap_resemblance_class_lin_models(X1, X2, logistic_regression, random_state):
-    """
-    Test.
-    """
     # Test SHAP Resemblance Model for linear models.
     rm = SHAPImportanceResemblance(logistic_regression, test_prc=0.5, n_jobs=1, random_state=random_state)
 
     actual_report, train_score, test_score = rm.fit_compute(
         X1, X2, return_scores=True, approximate=True, check_additivity=False
     )
 
@@ -156,19 +136,15 @@
     assert actual_shap_values_test.shape == (4, 3)
 
     # Run plots
     rm.plot(plot_type="bar")
     rm.plot(plot_type="dot")
 
 
-@pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_shap_resemblance_class2(complex_data_with_categorical, complex_lightgbm, random_state):
-    """
-    Test.
-    """
     X1, _ = complex_data_with_categorical
     X2 = X1.copy()
     X2["f4"] = X2["f4"] + 100
 
     rm = SHAPImportanceResemblance(
         complex_lightgbm, scoring="accuracy", test_prc=0.5, n_jobs=1, random_state=random_state
     )
@@ -197,17 +173,14 @@
 
     # Run plots
     rm.plot(plot_type="bar", show=True)
     rm.plot(plot_type="dot", show=False)
 
 
 def test_permutation_resemblance_class(X1, X2, decision_tree_classifier, random_state):
-    """
-    Test.
-    """
     rm = PermutationImportanceResemblance(
         decision_tree_classifier, test_prc=0.5, n_jobs=1, random_state=random_state, iterations=20
     )
 
     actual_report, train_score, test_score = rm.fit_compute(X1, X2, return_scores=True)
 
     assert train_score == 1
@@ -229,17 +202,14 @@
     # Check plot size
     fig = plt.gcf()
     size = fig.get_size_inches()
     assert size[0] == 10 and size[1] == 10
 
 
 def test_base_class_same_data(X1, decision_tree_classifier, random_state):
-    """
-    Test.
-    """
     rm = BaseResemblanceModel(decision_tree_classifier, test_prc=0.5, n_jobs=1, random_state=random_state)
 
     actual_report, train_score, test_score = rm.fit_compute(X1, X1, return_scores=True)
 
     assert train_score == 0.5
     assert test_score == 0.5
     assert actual_report is None
```

### Comparing `probatus-3.0.1/tests/utils/test_base_class.py` & `probatus-3.1.0/tests/utils/test_base_class.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from probatus.interpret import ShapModelInterpreter
 import pytest
 from probatus.utils import NotFittedError
 
 
 def test_fitted_exception(fitted_tree, X_train, y_train, X_test, y_test, random_state):
-    """
-    Test if fitted works..
-    """
     class_names = ["neg", "pos"]
 
     shap_interpret = ShapModelInterpreter(fitted_tree, random_state=random_state)
 
     # Before fit it should raise an exception
     with pytest.raises(NotFittedError) as _:
         shap_interpret._check_if_fitted()
@@ -20,13 +17,10 @@
     # Check parameters
     assert shap_interpret.fitted
     shap_interpret._check_if_fitted
 
 
 @pytest.mark.xfail
 def test_fitted_exception_is_raised(fitted_tree, random_state):
-    """
-    Test if fitted works fails when not fitted.
-    """
     shap_interpret = ShapModelInterpreter(fitted_tree, random_state=random_state)
 
     shap_interpret._check_if_fitted
```

