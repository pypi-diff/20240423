# Comparing `tmp/teneva_opti-0.5.3.tar.gz` & `tmp/teneva_opti-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_opti-0.5.3.tar", last modified: Tue Dec 19 09:12:02 2023, max compression
+gzip compressed data, was "teneva_opti-0.6.0.tar", last modified: Tue Apr 23 13:43:41 2024, max compression
```

## Comparing `teneva_opti-0.5.3.tar` & `teneva_opti-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-19 09:12:02.846956 teneva_opti-0.5.3/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-10-09 13:30:28.000000 teneva_opti-0.5.3/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       63 2023-10-09 11:44:01.000000 teneva_opti-0.5.3/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     4235 2023-12-19 09:12:02.846729 teneva_opti-0.5.3/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2409 2023-12-19 09:11:06.000000 teneva_opti-0.5.3/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      338 2023-12-19 09:10:08.000000 teneva_opti-0.5.3/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-12-19 09:12:02.847862 teneva_opti-0.5.3/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-10-09 13:29:52.000000 teneva_opti-0.5.3/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-19 09:12:02.832157 teneva_opti-0.5.3/teneva_opti/
--rw-r--r--   0 andrei     (501) staff       (20)      191 2023-12-19 09:11:10.000000 teneva_opti-0.5.3/teneva_opti/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    10367 2023-10-14 16:37:12.000000 teneva_opti-0.5.3/teneva_opti/bm_view.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-19 09:12:02.834827 teneva_opti-0.5.3/teneva_opti/func/
--rw-r--r--   0 andrei     (501) staff       (20)        0 2023-10-09 11:43:58.000000 teneva_opti-0.5.3/teneva_opti/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    15391 2023-10-13 17:28:14.000000 teneva_opti-0.5.3/teneva_opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      171 2023-10-13 10:23:42.000000 teneva_opti-0.5.3/teneva_opti/opti_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     9199 2023-10-14 17:29:10.000000 teneva_opti-0.5.3/teneva_opti/opti_manager.py
--rw-r--r--   0 andrei     (501) staff       (20)     2639 2023-10-13 17:46:20.000000 teneva_opti-0.5.3/teneva_opti/opti_tens.py
--rw-r--r--   0 andrei     (501) staff       (20)     2537 2023-10-14 18:00:17.000000 teneva_opti-0.5.3/teneva_opti/plot.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-19 09:12:02.845188 teneva_opti-0.5.3/teneva_opti/tens/
--rw-r--r--   0 andrei     (501) staff       (20)      344 2023-10-09 13:24:56.000000 teneva_opti-0.5.3/teneva_opti/tens/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      793 2023-10-09 13:29:07.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      865 2023-10-09 13:29:11.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)     1518 2023-10-13 10:15:37.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2603 2023-10-09 13:29:50.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)     2450 2023-10-13 10:34:24.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)     1518 2023-10-09 13:31:18.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)     1605 2023-10-13 10:10:00.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1471 2023-10-09 13:31:17.000000 teneva_opti-0.5.3/teneva_opti/tens/opti_tens_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2413 2023-10-13 10:26:02.000000 teneva_opti-0.5.3/teneva_opti/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-19 09:12:02.834469 teneva_opti-0.5.3/teneva_opti.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     4235 2023-12-19 09:12:02.000000 teneva_opti-0.5.3/teneva_opti.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      775 2023-12-19 09:12:02.000000 teneva_opti-0.5.3/teneva_opti.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-12-19 09:12:02.000000 teneva_opti-0.5.3/teneva_opti.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      262 2023-12-19 09:12:02.000000 teneva_opti-0.5.3/teneva_opti.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       12 2023-12-19 09:12:02.000000 teneva_opti-0.5.3/teneva_opti.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-04-23 13:43:41.021782 teneva_opti-0.6.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1106 2024-04-22 12:50:03.000000 teneva_opti-0.6.0/LICENSE
+-rw-r--r--   0 andrei     (501) staff       (20)       59 2024-04-23 13:26:18.000000 teneva_opti-0.6.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     4405 2024-04-23 13:43:41.021654 teneva_opti-0.6.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2409 2024-04-23 13:27:44.000000 teneva_opti-0.6.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      457 2024-04-23 13:36:09.000000 teneva_opti-0.6.0/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      103 2024-04-23 13:43:41.022228 teneva_opti-0.6.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2534 2024-04-23 13:23:53.000000 teneva_opti-0.6.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-04-23 13:43:41.015833 teneva_opti-0.6.0/teneva_opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      191 2024-04-23 13:26:57.000000 teneva_opti-0.6.0/teneva_opti/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)    10367 2023-10-14 16:37:12.000000 teneva_opti-0.6.0/teneva_opti/bm_view.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-04-23 13:43:41.017818 teneva_opti-0.6.0/teneva_opti/func/
+-rw-r--r--   0 andrei     (501) staff       (20)        0 2023-10-09 11:43:58.000000 teneva_opti-0.6.0/teneva_opti/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)    15391 2023-10-13 17:28:14.000000 teneva_opti-0.6.0/teneva_opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      171 2023-10-13 10:23:42.000000 teneva_opti-0.6.0/teneva_opti/opti_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     9199 2023-10-14 17:29:10.000000 teneva_opti-0.6.0/teneva_opti/opti_manager.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2639 2023-10-13 17:46:20.000000 teneva_opti-0.6.0/teneva_opti/opti_tens.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2537 2023-10-14 18:00:17.000000 teneva_opti-0.6.0/teneva_opti/plot.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-04-23 13:43:41.020671 teneva_opti-0.6.0/teneva_opti/tens/
+-rw-r--r--   0 andrei     (501) staff       (20)      344 2023-10-09 13:24:56.000000 teneva_opti-0.6.0/teneva_opti/tens/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)      793 2023-10-09 13:29:07.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      865 2023-10-09 13:29:11.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1518 2023-10-13 10:15:37.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2603 2023-10-09 13:29:50.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2450 2023-10-13 10:34:24.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1518 2023-10-09 13:31:18.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1605 2023-10-13 10:10:00.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1471 2023-10-09 13:31:17.000000 teneva_opti-0.6.0/teneva_opti/tens/opti_tens_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2413 2023-10-13 10:26:02.000000 teneva_opti-0.6.0/teneva_opti/utils.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-04-23 13:43:41.021062 teneva_opti-0.6.0/teneva_opti.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     4405 2024-04-23 13:43:40.000000 teneva_opti-0.6.0/teneva_opti.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      771 2024-04-23 13:43:40.000000 teneva_opti-0.6.0/teneva_opti.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2024-04-23 13:43:40.000000 teneva_opti-0.6.0/teneva_opti.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      316 2024-04-23 13:43:40.000000 teneva_opti-0.6.0/teneva_opti.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       12 2024-04-23 13:43:40.000000 teneva_opti-0.6.0/teneva_opti.egg-info/top_level.txt
```

### Comparing `teneva_opti-0.5.3/LICENSE.txt` & `teneva_opti-0.6.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Copyright (C) 2023 Andrei Chertkov, Gleb Ryzhakov, Ivan Oseledets
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Copyright (c) 2024 AIRI - Artificial Intelligence Research Institute
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `teneva_opti-0.5.3/PKG-INFO` & `teneva_opti-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: teneva_opti
-Version: 0.5.3
+Version: 0.6.0
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
-Home-page: https://github.com/AndreiChertkov/teneva_opti
+Home-page: https://github.com/AIRI-Institute/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
-Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
+Project-URL: Source, https://github.com/AIRI-Institute/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -18,60 +18,63 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
+Requires-Dist: contourpy==1.1.1; python_version == "3.8"
 Requires-Dist: matplotlib<3.7.1,>=3.7.0; python_version == "3.8"
 Requires-Dist: matplotlib>=3.7.0; python_version >= "3.9"
 Requires-Dist: ml_dtypes<=0.2.0; python_version == "3.8"
 Requires-Dist: ml_dtypes; python_version >= "3.9"
 Requires-Dist: nevergrad==0.8.0
 Requires-Dist: numpy<1.25,>=1.22; python_version == "3.8"
 Requires-Dist: numpy>=1.22; python_version >= "3.9"
 Requires-Dist: pandas<=1.5.3
 Requires-Dist: protes==0.3.6
+Requires-Dist: scikit-learn<=1.3.2; python_version == "3.8"
+Requires-Dist: scipy<1.11,>=1.9; python_version == "3.8"
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: teneva>=0.14.7
-Requires-Dist: teneva_bm==0.8.6
+Requires-Dist: teneva_bm==0.9.0
 Requires-Dist: ttopt==0.6.2
 
 # teneva_opti
 
 
 ## Description
 
-Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
+Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AIRI-Institute/teneva_bm).
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_opti==0.5.3
+    pip install teneva_opti==0.6.0
     ```
-    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
+    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
 
-2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script; note that you don't need to use environment in colab):
+2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AIRI-Institute/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script; note that you don't need to use environment in colab):
     ```bash
-    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
+    wget https://raw.githubusercontent.com/AIRI-Institute/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
     ```
-    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`. If you have problems downloading the script via wget, you can download it manually from the root folder of the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
+    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`. If you have problems downloading the script via wget, you can download it manually from the root folder of the repository [teneva_bm](https://github.com/AIRI-Institute/teneva_bm).
 
 
 ## Documentation and examples (in progress...)
 
-Please, run the demo script from the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository:
+Please, run the demo script from the root of the [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) repository:
 ```bash
 clear && python demo/base.py
 ```
 
-> See also other demo scripts in the folder `demo` of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository.
+> See also other demo scripts in the folder `demo` of the [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) repository.
 
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_opti-0.5.3/README.md` & `teneva_opti-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # teneva_opti
 
 
 ## Description
 
-Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
+Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AIRI-Institute/teneva_bm).
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_opti==0.5.3
+    pip install teneva_opti==0.6.0
     ```
-    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
+    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
 
-2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script; note that you don't need to use environment in colab):
+2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AIRI-Institute/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script; note that you don't need to use environment in colab):
     ```bash
-    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
+    wget https://raw.githubusercontent.com/AIRI-Institute/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
     ```
-    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`. If you have problems downloading the script via wget, you can download it manually from the root folder of the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
+    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`. If you have problems downloading the script via wget, you can download it manually from the root folder of the repository [teneva_bm](https://github.com/AIRI-Institute/teneva_bm).
 
 
 ## Documentation and examples (in progress...)
 
-Please, run the demo script from the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository:
+Please, run the demo script from the root of the [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) repository:
 ```bash
 clear && python demo/base.py
 ```
 
-> See also other demo scripts in the folder `demo` of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository.
+> See also other demo scripts in the folder `demo` of the [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) repository.
 
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_opti-0.5.3/setup.py` & `teneva_opti-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     name='teneva_opti',
     version=version,
     description=desc,
     long_description=desc_long,
     long_description_content_type='text/markdown',
     author='Andrei Chertkov',
     author_email='andre.chertkov@gmail.com',
-    url='https://github.com/AndreiChertkov/teneva_opti',
+    url='https://github.com/AIRI-Institute/teneva_opti',
     classifiers=[
         'Development Status :: 3 - Alpha', # 4 - Beta, 5 - Production/Stable
         'License :: OSI Approved :: MIT License',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
@@ -55,18 +55,18 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy',
     packages=find_packages('teneva_opti', './teneva_opti/'),
     python_requires='>=3.8',
     project_urls={
-        'Source': 'https://github.com/AndreiChertkov/teneva_opti',
+        'Source': 'https://github.com/AIRI-Institute/teneva_opti',
     },
     license='MIT',
-    license_files = ('LICENSE.txt',),
+    license_files = ('LICENSE',),
 )
 
 
 if __name__ == '__main__':
     setup(
         **setup_args,
         install_requires=requirements,
```

### Comparing `teneva_opti-0.5.3/teneva_opti/bm_view.py` & `teneva_opti-0.6.0/teneva_opti/bm_view.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/opti.py` & `teneva_opti-0.6.0/teneva_opti/opti.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/opti_manager.py` & `teneva_opti-0.6.0/teneva_opti/opti_manager.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/opti_tens.py` & `teneva_opti-0.6.0/teneva_opti/opti_tens.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/plot.py` & `teneva_opti-0.6.0/teneva_opti/plot.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_nb.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_nb.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_opo.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_opo.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_optimatt.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_optimatt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_portfolio.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_portfolio.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_protes.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_protes.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_pso.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_pso.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_spsa.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_spsa.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/tens/opti_tens_ttopt.py` & `teneva_opti-0.6.0/teneva_opti/tens/opti_tens_ttopt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti/utils.py` & `teneva_opti-0.6.0/teneva_opti/utils.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.5.3/teneva_opti.egg-info/PKG-INFO` & `teneva_opti-0.6.0/teneva_opti.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: teneva-opti
-Version: 0.5.3
+Name: teneva_opti
+Version: 0.6.0
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
-Home-page: https://github.com/AndreiChertkov/teneva_opti
+Home-page: https://github.com/AIRI-Institute/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
-Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
+Project-URL: Source, https://github.com/AIRI-Institute/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -18,60 +18,63 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
+Requires-Dist: contourpy==1.1.1; python_version == "3.8"
 Requires-Dist: matplotlib<3.7.1,>=3.7.0; python_version == "3.8"
 Requires-Dist: matplotlib>=3.7.0; python_version >= "3.9"
 Requires-Dist: ml_dtypes<=0.2.0; python_version == "3.8"
 Requires-Dist: ml_dtypes; python_version >= "3.9"
 Requires-Dist: nevergrad==0.8.0
 Requires-Dist: numpy<1.25,>=1.22; python_version == "3.8"
 Requires-Dist: numpy>=1.22; python_version >= "3.9"
 Requires-Dist: pandas<=1.5.3
 Requires-Dist: protes==0.3.6
+Requires-Dist: scikit-learn<=1.3.2; python_version == "3.8"
+Requires-Dist: scipy<1.11,>=1.9; python_version == "3.8"
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: teneva>=0.14.7
-Requires-Dist: teneva_bm==0.8.6
+Requires-Dist: teneva_bm==0.9.0
 Requires-Dist: ttopt==0.6.2
 
 # teneva_opti
 
 
 ## Description
 
-Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
+Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AIRI-Institute/teneva_bm).
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_opti==0.5.3
+    pip install teneva_opti==0.6.0
     ```
-    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
+    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
 
-2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script; note that you don't need to use environment in colab):
+2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AIRI-Institute/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script; note that you don't need to use environment in colab):
     ```bash
-    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
+    wget https://raw.githubusercontent.com/AIRI-Institute/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
     ```
-    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`. If you have problems downloading the script via wget, you can download it manually from the root folder of the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
+    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`. If you have problems downloading the script via wget, you can download it manually from the root folder of the repository [teneva_bm](https://github.com/AIRI-Institute/teneva_bm).
 
 
 ## Documentation and examples (in progress...)
 
-Please, run the demo script from the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository:
+Please, run the demo script from the root of the [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) repository:
 ```bash
 clear && python demo/base.py
 ```
 
-> See also other demo scripts in the folder `demo` of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository.
+> See also other demo scripts in the folder `demo` of the [teneva_opti](https://github.com/AIRI-Institute/teneva_opti) repository.
 
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_opti-0.5.3/teneva_opti.egg-info/SOURCES.txt` & `teneva_opti-0.6.0/teneva_opti.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.txt
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 teneva_opti/__init__.py
 teneva_opti/bm_view.py
```

