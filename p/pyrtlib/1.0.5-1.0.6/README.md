# Comparing `tmp/pyrtlib-1.0.5.tar.gz` & `tmp/pyrtlib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtlib-1.0.5.tar", last modified: Thu Feb 29 19:22:13 2024, max compression
+gzip compressed data, was "pyrtlib-1.0.6.tar", last modified: Tue Apr 23 08:31:02 2024, max compression
```

## Comparing `pyrtlib-1.0.5.tar` & `pyrtlib-1.0.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.404301 pyrtlib-1.0.5/pyrtlib/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.408301 pyrtlib-1.0.5/pyrtlib/_lineshape/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61798 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/h2o_lineshape.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/h2oll.py
--rw-r--r--   0 runner    (1001) docker     (127)   125023 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/o2_lineshape.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/o2ll.py
--rw-r--r--   0 runner    (1001) docker     (127)    91535 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/o3_lineshape.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/_lineshape/o3ll.py
--rw-r--r--   0 runner    (1001) docker     (127)    34895 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/absorption_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.408301 pyrtlib-1.0.5/pyrtlib/apiwebservices/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/apiwebservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/apiwebservices/eps_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/apiwebservices/erafive.py
--rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/apiwebservices/igra2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/apiwebservices/webservices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/apiwebservices/wyomingupperair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/pyrtlib/climatology/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/atmospheric_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/extrapolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26250 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/gas_minor.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/gas_trace.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/midlatitude_summer.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/midlatitude_winter.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/subarctic_summer.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/subarctic_winter.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/tropical.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/climatology/us_standard.dat
--rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/rt_equation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16955 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/tb_spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/pyrtlib/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/uncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/uncertainty/absmod_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R17/
--rw-r--r--   0 runner    (1001) docker     (127)   130507 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc
--rw-r--r--   0 runner    (1001) docker     (127)   134781 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R19/
--rw-r--r--   0 runner    (1001) docker     (127)   183368 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32209 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/pyrtlib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/pyrtlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-29 19:22:13.000000 pyrtlib-1.0.5/pyrtlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-29 19:22:13.000000 pyrtlib-1.0.5/pyrtlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 19:22:13.000000 pyrtlib-1.0.5/pyrtlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-29 19:22:13.000000 pyrtlib-1.0.5/pyrtlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-29 19:22:13.000000 pyrtlib-1.0.5/pyrtlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-29 19:22:13.412301 pyrtlib-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-29 19:22:02.000000 pyrtlib-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.621476 pyrtlib-1.0.6/pyrtlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.625476 pyrtlib-1.0.6/pyrtlib/_lineshape/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61798 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/h2o_lineshape.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/h2oll.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125023 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o2_lineshape.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o2ll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91535 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o3_lineshape.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o3ll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34466 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/absorption_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.625476 pyrtlib-1.0.6/pyrtlib/apiwebservices/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/eps_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/erafive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/igra2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/webservices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/wyomingupperair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/climatology/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/atmospheric_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27815 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/extrapolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26250 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/gas_minor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/gas_trace.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_summer.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_winter.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/subarctic_summer.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/subarctic_winter.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/tropical.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/us_standard.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/rt_equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16955 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/tb_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/absmod_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/
+-rw-r--r--   0 runner    (1001) docker     (127)   130507 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   134781 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R19/
+-rw-r--r--   0 runner    (1001) docker     (127)   183368 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32209 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/setup.py
```

### Comparing `pyrtlib-1.0.5/LICENSE` & `pyrtlib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/PKG-INFO` & `pyrtlib-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtlib
-Version: 1.0.5
+Version: 1.0.6
 Summary: pyrtlib - Radiative Transfer library
 Author: slarosa
 Author-email: salvatore-larosa@cnr.it
 License: GPLv3
 Project-URL: Documentation, https://satclop.github.io/pyrtlib
 Project-URL: Repository, https://github.com/SatCloP/pyrtlib
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,16 +22,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
-Requires-Dist: pytest==7.2.0
-Requires-Dist: pytest-datafiles>=2.0
 Requires-Dist: netCDF4
 Requires-Dist: requests
 Requires-Dist: bs4
 
 <img align="" src="https://raw.githubusercontent.com/SatCloP/pyrtlib/main/resources/logo/logo_large_new.png" width="400">
 
 # A Radiative Transfer Python Library (non-scattering)
@@ -131,13 +129,13 @@
 ## My first run with PyRTlib
 
 You can get started with PyRTlib by installing and executing the first radiative transfer calculation from the following Colab Notebook [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatCloP/pyrtlib/blob/main/docs/source/notebook/first_run.ipynb)
 
 
 ## Cite as
 
-Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., and Romano, F.: PyRTlib: an educational Python-based library for non-scattering atmospheric microwave Radiative Transfer computations, Geosci. Model Dev. Discuss. (preprint), https://doi.org/10.5194/gmd-2023-171, in review, 2023.
+Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., and Romano, F.: PyRTlib: an educational Python-based library for non-scattering atmospheric microwave radiative transfer computations, Geosci. Model Dev., 17, 2053–2076, https://doi.org/10.5194/gmd-17-2053-2024, 2024.
 
-Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., & Romano, F. (2023). PyRTlib: a python package for non-scattering line-by-line microwave Radiative Transfer simulations. (Computer software). https://doi.org/10.5281/zenodo.8219145
+Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., & Romano, F. (2024). PyRTlib: a python package for non-scattering line-by-line microwave Radiative Transfer simulations. (Computer software). https://doi.org/10.5281/zenodo.8219145
 
 ## Contributors
 <a href="https://github.com/SatCloP/pyrtlib/graphs/contributors"><img align="" src="https://contrib.rocks/image?repo=SatCloP/pyrtlib"></a>
```

### Comparing `pyrtlib-1.0.5/README.md` & `pyrtlib-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,13 +97,13 @@
 ## My first run with PyRTlib
 
 You can get started with PyRTlib by installing and executing the first radiative transfer calculation from the following Colab Notebook [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatCloP/pyrtlib/blob/main/docs/source/notebook/first_run.ipynb)
 
 
 ## Cite as
 
-Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., and Romano, F.: PyRTlib: an educational Python-based library for non-scattering atmospheric microwave Radiative Transfer computations, Geosci. Model Dev. Discuss. (preprint), https://doi.org/10.5194/gmd-2023-171, in review, 2023.
+Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., and Romano, F.: PyRTlib: an educational Python-based library for non-scattering atmospheric microwave radiative transfer computations, Geosci. Model Dev., 17, 2053–2076, https://doi.org/10.5194/gmd-17-2053-2024, 2024.
 
-Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., & Romano, F. (2023). PyRTlib: a python package for non-scattering line-by-line microwave Radiative Transfer simulations. (Computer software). https://doi.org/10.5281/zenodo.8219145
+Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., & Romano, F. (2024). PyRTlib: a python package for non-scattering line-by-line microwave Radiative Transfer simulations. (Computer software). https://doi.org/10.5281/zenodo.8219145
 
 ## Contributors
 <a href="https://github.com/SatCloP/pyrtlib/graphs/contributors"><img align="" src="https://contrib.rocks/image?repo=SatCloP/pyrtlib"></a>
```

### Comparing `pyrtlib-1.0.5/pyrtlib/_lineshape/h2o_lineshape.nc` & `pyrtlib-1.0.6/pyrtlib/_lineshape/h2o_lineshape.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/_lineshape/h2oll.py` & `pyrtlib-1.0.6/pyrtlib/_lineshape/h2oll.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/_lineshape/o2_lineshape.nc` & `pyrtlib-1.0.6/pyrtlib/_lineshape/o2_lineshape.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/_lineshape/o2ll.py` & `pyrtlib-1.0.6/pyrtlib/_lineshape/o2ll.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/_lineshape/o3_lineshape.nc` & `pyrtlib-1.0.6/pyrtlib/_lineshape/o3_lineshape.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/_lineshape/o3ll.py` & `pyrtlib-1.0.6/pyrtlib/_lineshape/o3ll.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/absorption_model.py` & `pyrtlib-1.0.6/pyrtlib/absorption_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 This class contains the absorption model used in pyrtlib.
 """
 
 import types
+import os
 from typing import Tuple, Union, List, Optional, Dict
+from netCDF4 import Dataset
 
 import numpy as np
 
 from pyrtlib.climatology import AtmosphericProfiles as atmp
 from .utils import dilec12, _dcerror, constants, gas_mass, import_lineshape
 
+PATH = os.path.dirname(os.path.abspath(__file__))
 
 class AbsModelError(Exception):
     """Exception raised for errors in the input model.
 
     Attributes:
         model -- input model which caused the error
         message -- explanation of the error
@@ -74,61 +77,44 @@
             List[str]: The list the implemented absorption models
 
         Example:
             .. code-block:: python
 
                 >>> from pyrtlib.absorption_model import AbsModel
                 >>> AbsModel.implemented_models()
-                {
-                    'Oxygen': ['R98',
-                            'R03',
-                            'R16',
-                            'R17',
-                            'R18',
-                            'R19',
-                            'R19SD',
-                            'R20',
-                            'R20SD',
-                            'R22'],
+                {'Oxygen': ['R98',
+                    'R03',
+                    'R16',
+                    'R17',
+                    'R18',
+                    'R19',
+                    'R19SD',
+                    'R20',
+                    'R20SD',
+                    'R22'],
                     'WaterVapour': ['R98',
-                            'R03',
-                            'R16',
-                            'R17',
-                            'R18',
-                            'R19',
-                            'R19SD',
-                            'R20',
-                            'R20SD',
-                            'R21SD',
-                            'R22',
-                            'R22SD']}
+                    'R03',
+                    'R16',
+                    'R17',
+                    'R18',
+                    'R19',
+                    'R19SD',
+                    'R20',
+                    'R20SD',
+                    'R21SD',
+                    'R22SD'],
+                    'Ozone': ['R18', 'R22']}
         """
-        model = {"Oxygen": ['R98',
-                            'R03',
-                            'R16',
-                            'R17',
-                            'R18',
-                            'R19',
-                            'R19SD',
-                            'R20',
-                            'R20SD',
-                            'R22'], 
-                 "WaterVapour": ['R98',
-                            'R03',
-                            'R16',
-                            'R17',
-                            'R18',
-                            'R19',
-                            'R19SD',
-                            'R20',
-                            'R20SD',
-                            'R21SD',
-                            'R22',
-                            'R22SD'],  
-                 "Ozone": ['R18', 'R22']}
+        oxygen_netcdf =  Dataset(os.path.join(PATH, '_lineshape', 'o2_lineshape.nc'), mode='r')
+        wv_netcdf =  Dataset(os.path.join(PATH, '_lineshape', 'h2o_lineshape.nc'), mode='r')
+        ozone_netcdf =  Dataset(os.path.join(PATH, '_lineshape', 'o3_lineshape.nc'), mode='r')
+        
+        model = {"Oxygen": list(oxygen_netcdf.groups.keys()), 
+                 "WaterVapour": list(wv_netcdf.groups.keys()), 
+                 "Ozone": list(ozone_netcdf.groups.keys())}
 
         return model
 
 
 class LiqAbsModel(AbsModel):
     """This class contains the absorption model used in pyrtlib.
     """
```

### Comparing `pyrtlib-1.0.5/pyrtlib/apiwebservices/eps_sandbox.py` & `pyrtlib-1.0.6/pyrtlib/apiwebservices/eps_sandbox.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/apiwebservices/erafive.py` & `pyrtlib-1.0.6/pyrtlib/apiwebservices/erafive.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/apiwebservices/igra2.py` & `pyrtlib-1.0.6/pyrtlib/apiwebservices/igra2.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/apiwebservices/webservices.py` & `pyrtlib-1.0.6/pyrtlib/apiwebservices/webservices.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/apiwebservices/wyomingupperair.py` & `pyrtlib-1.0.6/pyrtlib/apiwebservices/wyomingupperair.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/atmospheric_profiles.py` & `pyrtlib-1.0.6/pyrtlib/climatology/atmospheric_profiles.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/extrapolation.py` & `pyrtlib-1.0.6/pyrtlib/climatology/extrapolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,39 +306,40 @@
             month (int): Month of the year
             z (np.ndarray): Height (km)
             q (Tuple[np.ndarray, np.ndarray, np.ndarray]): Pressure (hPa), Temperature (K) and Relative humisity (frac) profiles
 
         Returns:
             Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]: Height, Pressure, Temperature, RH extrapolated profiles
         """
+    
         if np.max(z) < 50:
-            h_km = np.append(z, np.arange(max(z)+5, 50, 5))
+            h_km = np.append(z, np.arange(max(z)+3.2, 50, 3.2))
             idx = np.where(self._height > np.max(h_km))
             self._height = np.append(h_km, self._height[idx])
         else:
             self._height = np.append(z, self._height[idx])
 
-        idx = np.where(self._height > np.max(z))
         season = self._get_season(lat, month)
+        idx = np.where(self._height > np.max(z))
 
         p, t, rh = q
 
         if season != 'standard':
-            tt = self.instance.temperature(lat, self._height, season)
-            pp = self.instance.pressure(lat, self._height, season)
-            wvd = self.instance.water_vapour_density(lat, self._height, season)
+            tt = self.temperature(lat, self._height, season)
+            pp = self.pressure(lat, self._height, season)
+            wvd = self.water_vapour_density(lat, self._height, season)
         else:
-            tt = self.instance.standard_temperature(self._height, season)
-            pp = self.instance.standard_pressure(self._height, season)
+            tt = self.instance.standard_temperature(self._height)
+            pp = self.instance.standard_pressure(self._height)
             wvd = self.instance.standard_water_vapour_density(
-                self._height, season)
+                self._height)
 
         pres = np.append(p, pp[idx])
         temp = np.append(t, tt[idx])
-        _rh = rho2rh(wvd, tt, pp)[0]
+        _rh = rho2rh(wvd, temp, pres)[0]
         rh = np.append(rh, _rh[idx])
 
         return self._height, pres, temp, rh
 
 
 class _ITU835_6():
     """Class to model the ITU-R P.835_6 recommendation.
@@ -428,15 +429,15 @@
         return P
 
     @staticmethod
     def standard_water_vapour_density(h, h_0=2, rho_0=7.5):
         """
 
         """
-        return rho_0 * np.exp(-h / h_0)
+        return rho_0 * np.exp(-h / float(h_0))
 
     def standard_water_vapour_pressure(self, h, h_0=2, rho_0=7.5):
         """
 
         """
         rho_h = self.standard_water_vapour_density(h, h_0, rho_0)
         T_h = self.standard_temperature(h)
```

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/gas_minor.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/gas_minor.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/gas_trace.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/gas_trace.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/midlatitude_summer.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_summer.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/midlatitude_winter.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_winter.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/subarctic_summer.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/subarctic_summer.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/subarctic_winter.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/subarctic_winter.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/tropical.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/tropical.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/climatology/us_standard.dat` & `pyrtlib-1.0.6/pyrtlib/climatology/us_standard.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/rt_equation.py` & `pyrtlib-1.0.6/pyrtlib/rt_equation.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/tb_spectrum.py` & `pyrtlib-1.0.6/pyrtlib/tb_spectrum.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/uncertainty/absmod_uncertainty.py` & `pyrtlib-1.0.6/pyrtlib/uncertainty/absmod_uncertainty.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc` & `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc` & `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc` & `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/uncertainty/covariance_matrix/__init__.py` & `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib/utils.py` & `pyrtlib-1.0.6/pyrtlib/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/pyrtlib.egg-info/PKG-INFO` & `pyrtlib-1.0.6/pyrtlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtlib
-Version: 1.0.5
+Version: 1.0.6
 Summary: pyrtlib - Radiative Transfer library
 Author: slarosa
 Author-email: salvatore-larosa@cnr.it
 License: GPLv3
 Project-URL: Documentation, https://satclop.github.io/pyrtlib
 Project-URL: Repository, https://github.com/SatCloP/pyrtlib
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,16 +22,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
-Requires-Dist: pytest==7.2.0
-Requires-Dist: pytest-datafiles>=2.0
 Requires-Dist: netCDF4
 Requires-Dist: requests
 Requires-Dist: bs4
 
 <img align="" src="https://raw.githubusercontent.com/SatCloP/pyrtlib/main/resources/logo/logo_large_new.png" width="400">
 
 # A Radiative Transfer Python Library (non-scattering)
@@ -131,13 +129,13 @@
 ## My first run with PyRTlib
 
 You can get started with PyRTlib by installing and executing the first radiative transfer calculation from the following Colab Notebook [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SatCloP/pyrtlib/blob/main/docs/source/notebook/first_run.ipynb)
 
 
 ## Cite as
 
-Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., and Romano, F.: PyRTlib: an educational Python-based library for non-scattering atmospheric microwave Radiative Transfer computations, Geosci. Model Dev. Discuss. (preprint), https://doi.org/10.5194/gmd-2023-171, in review, 2023.
+Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., and Romano, F.: PyRTlib: an educational Python-based library for non-scattering atmospheric microwave radiative transfer computations, Geosci. Model Dev., 17, 2053–2076, https://doi.org/10.5194/gmd-17-2053-2024, 2024.
 
-Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., & Romano, F. (2023). PyRTlib: a python package for non-scattering line-by-line microwave Radiative Transfer simulations. (Computer software). https://doi.org/10.5281/zenodo.8219145
+Larosa, S., Cimini, D., Gallucci, D., Nilo, S. T., & Romano, F. (2024). PyRTlib: a python package for non-scattering line-by-line microwave Radiative Transfer simulations. (Computer software). https://doi.org/10.5281/zenodo.8219145
 
 ## Contributors
 <a href="https://github.com/SatCloP/pyrtlib/graphs/contributors"><img align="" src="https://contrib.rocks/image?repo=SatCloP/pyrtlib"></a>
```

### Comparing `pyrtlib-1.0.5/pyrtlib.egg-info/SOURCES.txt` & `pyrtlib-1.0.6/pyrtlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.5/setup.py` & `pyrtlib-1.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,19 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='pyrtlib',
-    version='1.0.5',
+    version='1.0.6',
     include_package_data=True,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     package_data={'pyrtlib': ['_lineshape/*', 'climatology/*', 'uncertainty/covariance_matrix/*/*']},
-    # package_dir={'': 'pyrtlib'},
     python_requires='>=3.8',
-    setup_requires=['pytest-runner'],
-    tests_require=['pytest'],
     install_requires=required,
     project_urls={
         'Documentation': 'https://satclop.github.io/pyrtlib',
         'Repository': 'https://github.com/SatCloP/pyrtlib'
     },
     license='GPLv3',
     author='slarosa',
```

