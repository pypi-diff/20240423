# Comparing `tmp/wedap-0.0.9.tar.gz` & `tmp/wedap-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedap-0.0.9.tar", last modified: Fri Sep 22 19:15:53 2023, max compression
+gzip compressed data, was "wedap-1.0.0.tar", last modified: Tue Apr 23 20:11:17 2024, max compression
```

## Comparing `wedap-0.0.9.tar` & `wedap-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.281544 wedap-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-09-22 19:15:11.000000 wedap-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2023-09-22 19:15:53.277544 wedap-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2023-09-22 19:15:11.000000 wedap-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/mdap/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-09-22 19:15:11.000000 wedap-0.0.9/mdap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2023-09-22 19:15:11.000000 wedap-0.0.9/mdap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19591 2023-09-22 19:15:11.000000 wedap-0.0.9/mdap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/md_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/mdap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/styles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/mdap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/tests/make_md_pdist_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2023-09-22 19:15:12.000000 wedap-0.0.9/mdap/tests/test_md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 19:15:53.281544 wedap-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-09-22 19:15:12.000000 wedap-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.273544 wedap-0.0.9/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:12.000000 wedap-0.0.9/styles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-22 19:15:12.000000 wedap-0.0.9/wedap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-09-22 19:15:12.000000 wedap-0.0.9/wedap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21191 2023-09-22 19:15:12.000000 wedap-0.0.9/wedap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    54756 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21016 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/styles/default.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/make_h5_plot_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/test_h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2023-09-22 19:15:13.000000 wedap-0.0.9/wedap/tests/test_h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 19:15:53.277544 wedap-0.0.9/wedap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-22 19:15:53.000000 wedap-0.0.9/wedap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-23 20:10:54.000000 wedap-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-23 20:11:17.615585 wedap-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-23 20:10:54.000000 wedap-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.607585 wedap-1.0.0/mdap/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/md_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.607585 wedap-1.0.0/mdap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/mdap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/tests/make_md_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/tests/test_md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:11:17.615585 wedap-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-23 20:10:55.000000 wedap-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:55.000000 wedap-1.0.0/styles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/wedap/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 20:10:55.000000 wedap-1.0.0/wedap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-23 20:10:55.000000 wedap-1.0.0/wedap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28147 2024-04-23 20:10:55.000000 wedap-1.0.0/wedap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/h5_gif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69160 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/wedap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wedap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/make_h5_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/make_h5_plot_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/test_h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/test_h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wedap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/data/ppf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/error/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/error/GetAvg_CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/error/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/styles/default.mplstyle
```

### Comparing `wedap-0.0.9/LICENSE` & `wedap-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wedap-0.0.9/PKG-INFO` & `wedap-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 0.0.9
-Summary: weighted ensemble data analysis and plotting
+Version: 1.0.0
+Summary: Weighted Ensemble Data Analysis and Plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
         All rights reserved.
@@ -41,60 +41,61 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: h5py
-Requires-Dist: scipy
 Requires-Dist: gif
 Requires-Dist: tqdm
 
 <p align="left">
-    <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap.jpeg?raw=true" alt="wedap logo" width="400">
+    <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap_logo.png?raw=true" alt="wedap logo" width="400">
 </p>
 
 ![tests](https://github.com/darianyang/wedap/actions/workflows/tests.yml/badge.svg)
 [![docs](https://img.shields.io/website?label=docs&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdarianyang.github.io%2Fwedap%2Fdocs%2Fhtml%2Findex.html)](https://darianyang.github.io/wedap/docs/html/index.html)
 [![PyPI version](https://badge.fury.io/py/wedap.svg)](https://badge.fury.io/py/wedap)
 [![Downloads](https://static.pepy.tech/badge/wedap)](https://pepy.tech/project/wedap)
 [![GitHub license](https://img.shields.io/github/license/darianyang/wedap)](https://github.com/darianyang/wedap/blob/master/LICENSE)
 
-**wedap** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
+**WEDAP** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
 
 `wedap` is primarily used to plot H5 files produced from running [WESTPA](https://github.com/westpa/westpa).
 
 `mdap` can be used to plot data files from analysis of standard MD simulations.
 
+`wekap` can be used to plot flux values as rates from a WESTPA created direct.h5 file. 
+
 For a demo and summary of features, see this [jupyter notebook](docs/notebook/wedap_demo.ipynb).
 
 Or view the same demo notebook on the [documentation web page](https://darianyang.github.io/wedap/docs/html/notebook/wedap_demo.html).
 
 ### Requirements
 
 - numpy
 - matplotlib
 - h5py
-- scipy
 - tqdm
+- gif
 
 ### Optional
 
 - gif (optional for making gifs)
 - gooey (optional for GUI)
 
 ## Installation
 
 If you don't need the GUI, then installing `Gooey` is not required and you can just pip install.
 ``` bash
 pip install wedap
 ```
 Otherwise you can install with `Gooey`, e.g. into a new conda env:
 ``` bash
-conda env create --name wedap python=3.8+
+conda env create --name wedap python=3.10+
 conda activate wedap
 conda install -c conda-forge gooey
 pip install wedap
 ```
 Or update an existing environmnent:
 ``` bash
 conda activate ENV_NAME
@@ -102,23 +103,30 @@
 pip install wedap
 ```
 
 Note that `Gooey` is kindof troublesome to pip install in some systems, which is also why it's not included in the requirements (although it is required for the GUI). For now, I recommend conda installing `Gooey`.
 
 ## GUI
 
-`wedap` has a GUI built using [Gooey](https://github.com/chriskiehl/Gooey) which can be launched by running `wedap` or `python wedap` if you're in the main `wedap` directory of this repository. If you're using MacOSX, you'll need to run `pythonw wedap` in the main directory since conda prevents wxPython from accessing the display on Mac. 
+`wedap` has a GUI built using [Gooey](https://github.com/chriskiehl/Gooey) which can be launched from the command line by simply running 
+``` bash
+wedap
+```
+or 
+`python wedap` if you're in the main `wedap` directory of this repository. 
+
+
+If you're using MacOSX, you'll need to run `pythonw wedap` in the main directory since conda prevents wxPython from accessing the display on Mac. 
 If you pip install (instead of conda installing) `wxPython` and `Gooey` on Mac you may be able to just run `wedap`. 
-If you wish to use the command line interface instead include any amount of arguments and include `-h` or `--help` to see the available options.
 
 For MacOSX, you can set up an alias in your `.bash_profile` by running the following:
-```
+``` bash
 echo "alias wedap=pythonw /Path/to/wedap/git/repo/wedap/wedap" >> ~/.bash_profile
 ```
-Then simply type `wedap` on the terminal to run the wedap GUI.
+Then simply type `wedap` in the terminal to run the wedap GUI.
 
 ## Examples
 
 After installation, to run the CLI version and view available options:
 ``` bash
 wedap --help
 ```
```

### Comparing `wedap-0.0.9/README.md` & `wedap-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 <p align="left">
-    <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap.jpeg?raw=true" alt="wedap logo" width="400">
+    <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap_logo.png?raw=true" alt="wedap logo" width="400">
 </p>
 
 ![tests](https://github.com/darianyang/wedap/actions/workflows/tests.yml/badge.svg)
 [![docs](https://img.shields.io/website?label=docs&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdarianyang.github.io%2Fwedap%2Fdocs%2Fhtml%2Findex.html)](https://darianyang.github.io/wedap/docs/html/index.html)
 [![PyPI version](https://badge.fury.io/py/wedap.svg)](https://badge.fury.io/py/wedap)
 [![Downloads](https://static.pepy.tech/badge/wedap)](https://pepy.tech/project/wedap)
 [![GitHub license](https://img.shields.io/github/license/darianyang/wedap)](https://github.com/darianyang/wedap/blob/master/LICENSE)
 
-**wedap** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
+**WEDAP** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
 
 `wedap` is primarily used to plot H5 files produced from running [WESTPA](https://github.com/westpa/westpa).
 
 `mdap` can be used to plot data files from analysis of standard MD simulations.
 
+`wekap` can be used to plot flux values as rates from a WESTPA created direct.h5 file. 
+
 For a demo and summary of features, see this [jupyter notebook](docs/notebook/wedap_demo.ipynb).
 
 Or view the same demo notebook on the [documentation web page](https://darianyang.github.io/wedap/docs/html/notebook/wedap_demo.html).
 
 ### Requirements
 
 - numpy
 - matplotlib
 - h5py
-- scipy
 - tqdm
+- gif
 
 ### Optional
 
 - gif (optional for making gifs)
 - gooey (optional for GUI)
 
 ## Installation
 
 If you don't need the GUI, then installing `Gooey` is not required and you can just pip install.
 ``` bash
 pip install wedap
 ```
 Otherwise you can install with `Gooey`, e.g. into a new conda env:
 ``` bash
-conda env create --name wedap python=3.8+
+conda env create --name wedap python=3.10+
 conda activate wedap
 conda install -c conda-forge gooey
 pip install wedap
 ```
 Or update an existing environmnent:
 ``` bash
 conda activate ENV_NAME
@@ -51,23 +53,30 @@
 pip install wedap
 ```
 
 Note that `Gooey` is kindof troublesome to pip install in some systems, which is also why it's not included in the requirements (although it is required for the GUI). For now, I recommend conda installing `Gooey`.
 
 ## GUI
 
-`wedap` has a GUI built using [Gooey](https://github.com/chriskiehl/Gooey) which can be launched by running `wedap` or `python wedap` if you're in the main `wedap` directory of this repository. If you're using MacOSX, you'll need to run `pythonw wedap` in the main directory since conda prevents wxPython from accessing the display on Mac. 
+`wedap` has a GUI built using [Gooey](https://github.com/chriskiehl/Gooey) which can be launched from the command line by simply running 
+``` bash
+wedap
+```
+or 
+`python wedap` if you're in the main `wedap` directory of this repository. 
+
+
+If you're using MacOSX, you'll need to run `pythonw wedap` in the main directory since conda prevents wxPython from accessing the display on Mac. 
 If you pip install (instead of conda installing) `wxPython` and `Gooey` on Mac you may be able to just run `wedap`. 
-If you wish to use the command line interface instead include any amount of arguments and include `-h` or `--help` to see the available options.
 
 For MacOSX, you can set up an alias in your `.bash_profile` by running the following:
-```
+``` bash
 echo "alias wedap=pythonw /Path/to/wedap/git/repo/wedap/wedap" >> ~/.bash_profile
 ```
-Then simply type `wedap` on the terminal to run the wedap GUI.
+Then simply type `wedap` in the terminal to run the wedap GUI.
 
 ## Examples
 
 After installation, to run the CLI version and view available options:
 ``` bash
 wedap --help
 ```
```

### Comparing `wedap-0.0.9/mdap/__main__.py` & `wedap-1.0.0/mdap/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,19 @@
     argument_parser = create_cmd_arguments()
     # Retrieve list of args
     args = handle_command_line(argument_parser)
 
     """
     Generate pdist and plot it
     """
+    # if not using screen use agg to be compatible with no display envs
+    if args.no_output_to_screen:
+        import matplotlib
+        matplotlib.use('agg')
+
     if args.style == "default":
         # get the style parameters from package data
         # currently writes into temp file, could be more efficient (TODO)
         style = pkgutil.get_data(__name__, "styles/default.mplstyle")
         # pkgutil returns binary string, decode it first and make temp file
         with open("style.temp", "w+") as f:
             f.write(style.decode())
@@ -96,15 +101,15 @@
     elif args.p_units == "kcal":
         cbar_label = "$-RT\ \ln\, P\ (kcal\ mol^{-1})$"
     elif args.p_units == "raw":
         cbar_label = "Counts"
     elif args.p_units == "raw_norm":
         cbar_label = "Normalized Counts"
     # if using scatter3d and no label is given, create default label
-    if args.plot_mode == "scatter3d" and args.cbar_label is None:
+    if (args.plot_mode == "scatter3d" or args.plot_mode == "hexbin3d") and args.cbar_label is None:
         cbar_label = plot.Zname[0] + " i" + str(plot.Zindex)
     # if there is a cbar object set label
     if hasattr(plot, "cbar"):
         plot.cbar.set_label(cbar_label, labelpad=14)
     # if using proj3d, add z axis label
     if args.proj3d is True:
         plot.ax.set_zlabel(cbar_label)
@@ -123,14 +128,18 @@
         # if Y data is given
         elif args.Yname:
             plot.ax.set_ylabel(plot.Yname[0] + " i" + str(plot.Yindex))
         # otherwise it will be something like 1d pdist
         else:
             plot.ax.set_ylabel(cbar_label)
 
+    # run postprocessing function if requested
+    if args.postprocess_func is not None:
+        plot._run_postprocessing()
+
     """
     Show and/or save the final plot
     """
     # fig vs plt shouldn't matter here (needed to go plt for mosaic)
     #plot.fig.tight_layout()
     plt.tight_layout()
     if args.output_path is not None:
```

### Comparing `wedap-0.0.9/mdap/command_line.py` & `wedap-1.0.0/mdap/command_line.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ArgumentParser = argparse.ArgumentParser
 
     def gui_decorator(f):
         return f
 else:
     ArgumentParser = gooey.GooeyParser
     gui_decorator = gooey.Gooey(
-        program_name='mdap',
+        program_name='MDAP',
         #navigation='TABBED',
         #advanced=True,
         suppress_gooey_flag=True,
         optional_cols=4, 
         default_size=(1000, 600),
         #tabbed_groups=True,
     )
@@ -57,15 +57,15 @@
 
     Returns
     -------
     argparse.ArgumentParser: 
         An ArgumentParser that is used to retrieve command line arguments. 
     """
     mdap_desc = "======================================================= \n" + \
-                "=== molecular dynamics analysis and plotting (mdap) === \n" + \
+                "=== Molecular Dynamics Analysis and Plotting (MDAP) === \n" + \
                 "======================================================= \n" + \
                 "\nGiven an input (pre-calcualated) dataset from standard MD simulations, " + \
                 "prepare probability distributions and plots. " + \
                 "Input data must be in >=2 column format: \n" + \
                 "# use hashs at top of data file to indicate comments (skipped) \n" + \
                 "COL1:Frame | COL2:Data | COL3:Data... \n\n" + \
                 "\nSee the documentation for usage and examples: https://darianyang.github.io/wedap " + \
@@ -140,15 +140,15 @@
     main.add_argument("-dt", "--data-type", "--datatype", default="pdist", nargs="?",
                         dest="data_type", choices=("time", "pdist"),
                         help="Type of pdist dataset to generate, options are ",
                              # TODO
                         type=str) 
     main.add_argument("-pm", "--plot-mode", "--plotmode", default="hist", nargs="?",
                         dest="plot_mode", choices=("hist", "hist_l", "contour", "contour_l", 
-                                                   "contour_f", "bar", "line", "scatter3d"),
+                                                   "contour_f", "bar", "line", "scatter3d", "hexbin3d"),
                         help="The type of plot desired.  "
                              "e.g. line for 1D, hist or contour for 2D and scatter3d for 3D.",
                         type=str)
     # TODO: allow a list of files, then multiple replicates can be addressed
     # * args is flexible number of values, which will be gathered into a list
     main.add_argument("-X", "-x", "--Xname", "--xname", default=None, nargs="*",
                         dest="Xname",
@@ -251,40 +251,51 @@
                         type=float)
     optional.add_argument("-sl", "--smoothing-level", default=None, 
                         dest="smoothing_level",
                         help="Smooth data (plotted as histogram or contour"
                              " levels) using a gaussian filter with sigma="
                              "SMOOTHING_LEVEL.",
                         type=float)
+    optional.add_argument("-sci", "--scatter-iterval", default=10, nargs="?",
+                        dest="scatter_interval",
+                        help="Adjust to use less data for scatter plots.",
+                        type=int)
+    optional.add_argument("-scs", "--scatter-s", default=1, nargs="?",
+                        dest="scatter_s",
+                        help="Adjust scatter plot marker size",
+                        type=float)
+    optional.add_argument("-hbg", "--hexbin-grid", default=100, nargs="?",
+                        dest="hexbin_grid",
+                        help="Adjusts hexbin gridsize parameters.",
+                        type=int)
     optional.add_argument("-T", "--temp", default=298, nargs="?",
                         dest="T", help="Used with kcal/mol 'p-units'.",
                         type=int)
     optional.add_argument("-jp", "--joint-plot", default=False,
                           dest="jointplot",
                           help="Optionally include marginal plots to create "
                                "a joint plot from 2D pdist.",
                           action="store_true")
     optional.add_argument("-3d", "--proj3d", default=False,
                           dest="proj3d",
-                          help="Make a 3d projection plot",
+                          help="Make a 3d projection plot, works with contour or scatter plots.",
                           action="store_true")
-    optional.add_argument("--style", default="default", nargs="?",
-                        dest="style",
-                        help="mpl style, can use default, None, or custom. "
-                             "Edit the wedap/styles/default.mplstyle file to "
-                             "change default wedap plotting style options.",
-                        type=str)
-    # TODO: prob cant use custom outside of list
-    optional.add_argument("--cmap", default="viridis", nargs="?",
-                        dest="cmap",
-                        help="mpl colormap name.",
-                        type=str)
-    optional.add_argument("--color",
-                        dest="color", help="Color for 1D plots and trace plots.",
-                        widget="ColourChooser")
+    optional.add_argument("-4d", "--proj4d", default=False,
+                          dest="proj4d",
+                          help="Make a 4d projection plot, must have Cname. " +
+                               "only works with scatter plots.",
+                          action="store_true")
+    optional.add_argument("-C", "-c", "--Cname", "--cname", default=None, nargs="?",
+                         dest="Cname", 
+                         help="Target data name for cbar of proj3d. Must use 'scatter3d' "
+                         "for 'plot_mode'. Can be 'pcoord' or any aux dataset name "
+                         "in your h5 file.",
+                         type=str)
+    optional.add_argument("-Ci", "--Cindex", "--cindex", default=0, nargs="?", type=int,
+                           dest="Cindex", help="Index in third dimension for >2D datasets.")
 
     # create optional flag to not output plot to console screen
     optional.add_argument("-nots", "--no-output-to-screen",
                         dest = "no_output_to_screen",
                         help = "Include this argument to not output the plot to "
                         "your display.", 
                         action= "store_true") 
@@ -312,23 +323,55 @@
 
     ##########################################################
     ############### FORMATTING ARGUMENTS #####################
     ##########################################################
 
     formatting = parser.add_argument_group("Plot Formatting Arguments") 
 
+    formatting.add_argument("--style", default="default", nargs="?",
+                        dest="style",
+                        help="mpl style, can leave blank to use default, "
+                             "input `None` for basic mpl settings, can use a custom "
+                             "path to a mpl.style text file, or could use a mpl included "
+                             "named style, e.g. `ggplot`. "
+                             "Edit the wedap/styles/default.mplstyle file to "
+                             "change default wedap plotting style options.",
+                        type=str)
+    # TODO: prob cant use custom outside of list
+    formatting.add_argument("--cmap", default="viridis", nargs="?",
+                        dest="cmap", help="mpl colormap name.", type=str)
+    formatting.add_argument("--color",
+                        dest="color", help="Color for 1D plots, contour lines, and trace plots.",
+                        widget="ColourChooser")
+    formatting.add_argument("--linewidth", "-lw", default=None, nargs="?",
+                        dest="linewidth", help="Linewidth for 1D plots, contour lines, and trace plots.",
+                        type=float)
+    formatting.add_argument("--linestyle", "-ls", default="-", nargs="?",
+                        dest="linestyle", help="Linestyle for 1D plots, contour lines, and trace plots.",
+                        type=str)
     formatting.add_argument("--xlabel", dest="xlabel", type=str)
     formatting.add_argument("--xlim", help="LB UB", dest="xlim", nargs=2, type=float)
     formatting.add_argument("--ylabel", dest="ylabel", type=str)
     formatting.add_argument("--ylim", help="LB UB", dest="ylim", nargs=2, type=float)
     formatting.add_argument("--title", dest="title", type=str)
     formatting.add_argument("--suptitle", dest="suptitle", type=str)
     formatting.add_argument("--cbar-label", dest="cbar_label", type=str)
     formatting.add_argument("--grid", dest="grid", default=False, action="store_true")
-
+    formatting.add_argument("--axvline", "-vl", help="Can be a single value or a list of lines.", 
+                            dest="axvline", nargs="*", type=float)
+    formatting.add_argument("--axhline", "-hl", help="Can be a single value or a list of lines.",
+                            dest="axhline", nargs="*", type=float)
+    formatting.add_argument('--postprocess', '--postprocess-function', '-ppf', default=None,
+                            dest='postprocess_func',
+                            help='After plotting data, load and execute the '
+                                 'Python function specified by '
+                                 'POSTPROCESS_FUNC. POSTPROCESS_FUNC should be '
+                                 'a string of the form ``mymodule.myfunction``.'
+                                 'Example: '
+                                 '``--postprocess mymodule.myfunction``.')
     # return the argument parser
     return parser 
 
 
 # TODO: adjust all to fix str/int/type auto
 def handle_command_line(argument_parser): 
     """
```

### Comparing `wedap-0.0.9/mdap/md_pdist.py` & `wedap-1.0.0/mdap/md_pdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,24 +118,37 @@
         # if the input file isn't already a list, make it a 1 item list
         if not isinstance(names, list):
             names = [names]
 
         # handle multiple file name list
         # TODO: handle direct ndarray inputs as well as file str
         for name in names:
+            # if the input is a numpy array
+            if isinstance(name, np.ndarray):
+                data_item = name
+
             # for .npy binary files or pkl files
-            if name[-4:] in [".npy", ".npz", ".pkl"]:
+            elif name[-4:] in [".npy", ".npz", ".pkl"]:
                 data_item = np.load(name, allow_pickle=True)
             else:
                 # TODO: note that genfromtxt can handle multiple items in list, could this help?
                 data_item = np.genfromtxt(name)
             # for 1D datasets, need to standardize to 2D, but as a new column
             if data_item.ndim < 2:
                 data_item = data_item[:, np.newaxis]
-            data.append(data_item[::interval, index])
+
+            # if indexing is wrong (e.g. 1 for 1 column dataset when 0 index is needed)
+            try:
+                data.append(data_item[::interval, index])
+            except IndexError as e:
+                print(f"{e}: Note that by default MDAP uses the 2nd column of the input data, \
+                        which cooresponds to an X/Y/Zindex of 1. Your dataset may only have 1 column, \
+                        and in that case the X/Y/Zindex should be set to 0. Exiting...")
+                sys.exit(0)
+
         # combine into a single array
         data = np.concatenate(data)
 
         return data
 
     def timeseries(self):
         """
@@ -146,15 +159,15 @@
         """
         # could get time from frame column
         #time = np.concatenate([np.genfromtxt(i)[::self.Xinterval, 0] for i in self.Xname])
 
         X = self._get_md_data(self.Xname, self.Xindex, self.Xinterval)
 
         # or can just get it from n rows
-        time = np.arange(0, X.shape[0], self.Xinterval)
+        time = np.arange(0, X.shape[0])
         time = np.divide(time, self.timescale)
 
         return time, X
 
     def pdist_1d(self):
         """
         Returns
```

### Comparing `wedap-0.0.9/mdap/md_plot.py` & `wedap-1.0.0/mdap/md_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,9 +46,11 @@
                     kwargs["p_units"] = og_p_units
                     self.p_units = og_p_units
                 # otherwise default to kT
                 else:
                     kwargs["p_units"] = "kT"
                     self.p_units = "kT"
 
+        # don't use weights, e.g. for hexbin plots (TODO: might be a better way to account for this)
+        self.weighted = False
         # run H5_Plot initialization
         H5_Plot.__init__(self, self.X, self.Y, self.Z, *args, **kwargs)
```

### Comparing `wedap-0.0.9/mdap/tests/make_md_pdist_test_data.py` & `wedap-1.0.0/mdap/tests/make_md_pdist_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.9/mdap/tests/test_md_pdist.py` & `wedap-1.0.0/mdap/tests/test_md_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-0.0.9/setup.py` & `wedap-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 with open('./LICENSE') as f:
     lic = f.read()
 
 packages = find_packages()
 
 setup(
     name='wedap',
-    version='0.0.9',
-    description='weighted ensemble data analysis and plotting',
+    version='1.0.0',
+    description='Weighted Ensemble Data Analysis and Plotting',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='Darian T. Yang',
     author_email='dty7@pitt.edu',
-    install_requires=['numpy', 'matplotlib', 'h5py', 'scipy', 'gif', 'tqdm'],
+    install_requires=['numpy', 'matplotlib', 'h5py', 'gif', 'tqdm'],
     url='https://github.com/darianyang/wedap',
     project_urls={'Documentation' : 'https://darianyang.github.io/wedap'},
     license=lic,
     #packages = find_packages(where = 'src'),
     #Packages=find_packages(exclude="docs"),
     packages=find_packages(exclude="docs"),
-    package_data={"wedap": ["styles/*"]},
+    package_data={"wedap":["styles/*"], "mdap":["styles/*"], "wekap":["styles/*"]},
     #py_modules=["wedap"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Chemistry"
     ],
     entry_points={"console_scripts" : ["wedap=wedap.__main__:main",
-                                       "mdap=mdap.__main__:main"]}
+                                       "mdap=mdap.__main__:main",
+                                       "wekap=wekap.__main__:main"]}
 )
```

### Comparing `wedap-0.0.9/wedap/__main__.py` & `wedap-1.0.0/wedap/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Main call.
 """
 from wedap.h5_pdist import *
 from wedap.h5_plot import *
 from wedap.command_line import *
+from wedap.h5_gif import *
 
 # TODO: change to logging style instead of stdout
 #import logging
 
 # for accessing package data: mpl styles
 import pkgutil 
 import os
@@ -21,14 +22,19 @@
     argument_parser = create_cmd_arguments()
     # Retrieve list of args
     args = handle_command_line(argument_parser)
 
     """
     Generate pdist and plot it
     """
+    # if not using screen use agg to be compatible with no display envs
+    if args.no_output_to_screen:
+        import matplotlib
+        matplotlib.use('agg')
+
     if args.style == "default":
         # get the style parameters from package data
         # currently writes into temp file, could be more efficient (TODO)
         style = pkgutil.get_data(__name__, "styles/default.mplstyle")
         # pkgutil returns binary string, decode it first and make temp file
         with open("style.temp", "w+") as f:
             f.write(style.decode())
@@ -40,17 +46,30 @@
 
     # a poor workaround for now for the weighted arg
     # this is only to make the gooey formatting look nicer in terms of the checkbox
     if args.not_weighted is True:
         args.weighted = False
     elif args.not_weighted is False:
         args.weighted = True
-    
-    # vars converts from Namespace object to dict
-    plot = H5_Plot(**vars(args))
+
+    #  make a gif instead of a single plot if gif_out is given
+    # e.g. $ wedap -h5 wedap/data/p53.h5 -y pcoord -yi 1 -dt average --last-iter 16 
+    #              --avg-plus 2 --gif-out test.gif --xlim 0 6 --ylim 0 36 --pmax 20
+    if args.gif_out is not None:
+        make_gif(**vars(args))
+        # exit prematurely since gif making
+        return
+    # otherwise carry on as normal for a single plot
+    else:
+        # vars converts from Namespace object to dict
+        plot = H5_Plot(**vars(args))
+
+    # for 4d projected, adjust cbar position (this is a class attr)
+    if args.proj4d is True:
+        plot.cbar_pad = 0.2
 
     # 2D plot with cbar
     # TODO: can this be done better?
     if args.Yname or args.data_type == "evolution":
         try:
             plot.plot(cbar=True)
         except AttributeError as e:
@@ -66,15 +85,15 @@
     """
     # default to white if no color provided
     if args.color is None:
         args.color = "white"
     if args.trace_seg is not None:
         plot.plot_trace(args.trace_seg, color=args.color, ax=plot.ax)
     if args.trace_val is not None:
-        iter, seg = plot.search_aux_xy_nn(args.trace_val[0], args.trace_val[1])
+        iter, seg = plot.find_iter_seg_from_xy_vals(args.trace_val[0], args.trace_val[1])
         plot.plot_trace((iter,seg), color=args.color, ax=plot.ax)
 
     """
     Plot formatting
     """
     # if no xlabel is given, create default label
     if args.xlabel is None:
@@ -87,22 +106,30 @@
         if args.Yname:
             plot.ax.set_ylabel(args.Yname + " i" + str(plot.Yindex))
 
     # if cbar_label is given set as cbar_label
     if args.cbar_label:
         plot.cbar.set_label(args.cbar_label, labelpad=14)
     # if using scatter3d and no label is given, create default label
-    elif args.plot_mode == "scatter3d":
+    elif args.plot_mode == "scatter3d" or args.plot_mode == "hexbin3d":
         # for 3d projected
         if args.proj3d is True:
             plot.ax.set_zlabel(args.Zname + " i" + str(plot.Zindex))
+        # for 4d projected
+        elif args.proj4d is True:
+            plot.ax.set_zlabel(args.Zname + " i" + str(plot.Zindex))
+            plot.cbar.set_label(args.Cname + " i" + str(plot.Cindex))
         # for 2d scatter with cbar
         else:
             plot.cbar.set_label(args.Zname + " i" + str(plot.Zindex))
     
+    # run postprocessing function if requested
+    if args.postprocess_func is not None:
+        plot._run_postprocessing()
+
     """
     Show and/or save the final plot
     """
     # fig vs plt shouldn't matter here (needed to go plt for mosaic)
     #plot.fig.tight_layout()
     plt.tight_layout()
     if args.output_path is not None:
```

### Comparing `wedap-0.0.9/wedap/command_line.py` & `wedap-1.0.0/wedap/command_line.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 try:
     import gooey
     #from gooey import Gooey
     #from gooey import GooeyParser
 except ImportError:
     gooey = None
 
+import pkg_resources
+
+# for auto filling version arg
+def get_version():
+    try:
+        return pkg_resources.get_distribution('wedap').version
+    except pkg_resources.DistributionNotFound:
+        return None
+
 def flex_add_argument(f):
     """Make the add_argument accept (and ignore) the widget option."""
 
     def f_decorated(*args, **kwargs):
         kwargs.pop('widget', None)
         return f(*args, **kwargs)
 
@@ -37,15 +46,15 @@
     ArgumentParser = argparse.ArgumentParser
 
     def gui_decorator(f):
         return f
 else:
     ArgumentParser = gooey.GooeyParser
     gui_decorator = gooey.Gooey(
-        program_name='wedap',
+        program_name='WEDAP',
         #navigation='TABBED',
         #advanced=True,
         suppress_gooey_flag=True,
         optional_cols=4, 
         default_size=(1000, 600),
         #tabbed_groups=True,
     )
@@ -62,15 +71,15 @@
 
     Returns
     -------
     argparse.ArgumentParser: 
         An ArgumentParser that is used to retrieve command line arguments. 
     """
     wedap_desc = "============================================================ \n" + \
-                 "=== weighted ensemble data analysis and plotting (wedap) === \n" + \
+                 "=== Weighted Ensemble Data Analysis and Plotting (WEDAP) === \n" + \
                  "============================================================ \n" + \
                  "\nGiven an input west.h5 file from a successful WESTPA simulation, " + \
                  "prepare probability distributions and plots." + \
                  "\nSee the documentation for usage and examples: https://darianyang.github.io/wedap" + \
                  "\n\n" + \
                  "wedap can be used with 3 different --data-type (-dt) args: " + \
                  "\n\t`evolution` (default), `average`, and `instant`" + \
@@ -144,18 +153,24 @@
     main.add_argument("-dt", "--data-type", "--datatype", default="evolution", nargs="?",
                         dest="data_type", choices=("evolution", "average", "instant"),
                         help="Type of pdist dataset to generate, options are "
                              "'evolution' (1 dataset); " 
                              "'average' or 'instance' (1 or 2 or 3 datasets).",
                         type=str) 
     main.add_argument("-pm", "--plot-mode", "--plotmode", default="hist", nargs="?",
-                        dest="plot_mode", choices=("hist", "hist_l", "contour", "contour_l", 
-                                                   "contour_f", "bar", "line", "scatter3d"),
+                        dest="plot_mode", choices=("bar", "line", "hist", "hist_l", "contour", 
+                                                   "contour_l", "contour_f", "scatter3d", "hexbin3d"),
                         help="The type of plot desired.  "
-                             "e.g. line for 1D, hist or contour for 2D and scatter3d for 3D.",
+                             "For 1D: bar or line. "
+                             "For 2D: hist or contour, hist_l is a hist with contour lines, "
+                             "contour_l is just contour lines, contour_f is just the fill, "
+                             "contour is both lines and fill, note that any contour lines "
+                             "plotted will default to cmap colors, so to have more distinctive "
+                             "contour lines, include a --color arg, e.g. `--color k`. \n"
+                             "For 3D, scatter3d or hexbin3d.",
                         type=str)
     main.add_argument("-X", "-x", "--Xname", "--xname", default="pcoord", nargs="?",
                         dest="Xname", 
                         help="Target data name for x axis. Default 'pcoord', "
                         "can also be any aux dataset name in your h5 file.",
                         type=str)
     main.add_argument("-Y", "-y", "--Yname", "--yname", default=None, nargs="?",
@@ -177,15 +192,15 @@
                         dest="Zindex", help="Index in third dimension for >2D datasets.")
     main.add_argument("-o", "--output", default=None,
                         dest="output_path",
                         help="The filename to which the plot will be saved. "
                              "Various image formats are available. You " 
                              "may choose one by specifying an extension. "
                              "\nLeave this empty if you don't want to save "
-                             "the plot to a serperate file.",
+                             "the plot to a serparate file.",
                         type=str)
     # begin optional arg group
     optional.add_argument("-fi", "--first-iter", default=1, nargs="?",
                         dest="first_iter",
                         help="Plot data starting at iteration FIRST_ITER. "
                              "By default, plot data starting at the first "
                              "iteration in the specified west.h5 file.",
@@ -252,51 +267,89 @@
                         type=float)
     optional.add_argument("-sl", "--smoothing-level", default=None, 
                         dest="smoothing_level",
                         help="Smooth data (plotted as histogram or contour"
                              " levels) using a gaussian filter with sigma="
                              "SMOOTHING_LEVEL.",
                         type=float)
+    optional.add_argument("-sci", "--scatter-int", "--scatter-interval", default=10, nargs="?",
+                        dest="scatter_interval",
+                        help="Adjust to use less data for scatter plots.",
+                        type=int)
+    optional.add_argument("-scs", "--scatter-s", "--scatter-size",
+                        default=1, nargs="?",
+                        dest="scatter_s",
+                        help="Adjust scatter plot marker size",
+                        type=float)
+    optional.add_argument("-hbg", "--hexbin-grid", default=100, nargs="?",
+                        dest="hexbin_grid",
+                        help="Adjusts hexbin gridsize parameters.",
+                        type=int)
     # TODO: is there a better way to do this? 
     #optional.add_argument("--weighted", default=True, action="store_true",
     #                      help="Use weights from WE.")
     optional.add_argument("-nw", "--not-weighted",
                           help="Include this to not use WE weights.",
                           dest="not_weighted", action="store_true")
     # optional.add_argument("--weighted", default=True, 
     #                       action=argparse.BooleanOptionalAction)
     # * args is flexible number of values, which will be gathered into a list
     optional.add_argument("-sb", "--skip-basis", default=None, nargs="*",
                           dest="skip_basis",
                           help="List of binary values for skipping basis states, "
                                "e.g. 0 1 1 to skip all bstates except for first.",
                           type=int)
+    optional.add_argument("-so", "--succ-only", "--succonly", default=False,
+                          dest="succ_only",
+                          help="Filter weights to only use successfull trajectories ",
+                          action="store_true")
+    optional.add_argument("--h5saveout", "--h5-save-out", "--H5save_out", default=None, nargs="?",
+                          dest="H5save_out",
+                          help="Optionally output updated west.h5 file. Use if you are "
+                               "weight filtering with skip_basis or succ_only.",
+                          type=str)
+     # TODO: eventually include XYZsavename?
     optional.add_argument("-jp", "--jointplot", "--joint-plot", default=False,
                           dest="jointplot",
                           help="Optionally include marginal plots to create "
                                "a joint plot from 2D pdist.",
                           action="store_true")
     optional.add_argument("-3d", "--proj3d", default=False,
                           dest="proj3d",
-                          help="Make a 3d projection plot",
+                          help="Make a 3d projection plot, works with contour or scatter plots.",
+                          action="store_true")
+    optional.add_argument("-4d", "--proj4d", default=False,
+                          dest="proj4d",
+                          help="Make a 4d projection plot, must have Cname. " +
+                               "only works with scatter plots.",
                           action="store_true")
+    optional.add_argument("-C", "-c", "--Cname", "--cname", default=None, nargs="?",
+                         dest="Cname", 
+                         help="Target data name for cbar of proj3d. Must use 'scatter3d' "
+                         "for 'plot_mode'. Can be 'pcoord' or any aux dataset name "
+                         "in your h5 file.",
+                         type=str)
+    optional.add_argument("-Ci", "--Cindex", "--cindex", default=0, nargs="?", type=int,
+                           dest="Cindex", help="Index in third dimension for >2D datasets.")
+
     # create optional flag to output everything to console screen
     # optional.add_argument("-ots", "--output_to_screen", default=True,
     #                     dest = "output_to_screen",
     #                     help = "Outputs plot to screen. True (default) or False", 
     #                     action= "store_true") 
     optional.add_argument("-nots", "--no-output-to-screen",
                         dest = "no_output_to_screen",
                         help = "Include this argument to not output the plot to "
                         "your display.", 
                         action= "store_true") 
     optional.add_argument("-npb", "--no-progress-bar",
                         dest = "no_pbar",
                         help = "Include this argument to not output the tqdm progress bar.",
                         action= "store_true")
+    optional.add_argument('--version', '-V', action='version', version='%(prog)s ' + get_version())
 
     # plot tracing arg group
     trace = parser.add_argument_group("Optional Plot Tracing", 
                                        description="Plot a trace on top of the pdist.")
     trace_group = trace.add_mutually_exclusive_group()
     # type to float for val inside tuple, 
     # and nargs to 2 since it is interpreted as a 2 item tuple or list
@@ -328,22 +381,77 @@
                         type=str)
     # TODO: prob cant use custom outside of list
     formatting.add_argument("--cmap", default="viridis", nargs="?",
                         dest="cmap", help="mpl colormap name.", type=str)
     formatting.add_argument("--color",
                         dest="color", help="Color for 1D plots, contour lines, and trace plots.",
                         widget="ColourChooser")
+    formatting.add_argument("--linewidth", "-lw", default=None, nargs="?",
+                        dest="linewidth", help="Linewidth for 1D plots, contour lines, and trace plots.",
+                        type=float)
+    formatting.add_argument("--linestyle", "-ls", default="-", nargs="?",
+                        dest="linestyle", help="Linestyle for 1D plots, contour lines, and trace plots.",
+                        type=str)
     formatting.add_argument("--xlabel", dest="xlabel", type=str)
     formatting.add_argument("--xlim", help="LB UB", dest="xlim", nargs=2, type=float)
     formatting.add_argument("--ylabel", dest="ylabel", type=str)
     formatting.add_argument("--ylim", help="LB UB", dest="ylim", nargs=2, type=float)
+    formatting.add_argument("--zlabel", dest="zlabel", type=str)
     formatting.add_argument("--title", dest="title", type=str)
     formatting.add_argument("--suptitle", dest="suptitle", type=str)
     formatting.add_argument("--cbar-label", dest="cbar_label", type=str)
     formatting.add_argument("--grid", dest="grid", default=False, action="store_true")
+    formatting.add_argument("--axvline", "-vl", help="Can be a single value or a list of lines.", 
+                            dest="axvline", nargs="*", type=float)
+    formatting.add_argument("--axhline", "-hl", help="Can be a single value or a list of lines.",
+                            dest="axhline", nargs="*", type=float)
+#     formatting.add_argument("--text", help="3 args for ax.text: x, y, string",
+#                             dest="text", nargs="3", type=float)
+#     formatting.add_argument("--figsize", default=None, nargs=2,
+#                             dest="figsize",
+#                             help="Matplotlib figure size, e.g. (6,4)",
+#                             type=float)
+    formatting.add_argument('--postprocess', '--postprocess-function', '-ppf', default=None,
+                            dest='postprocess_func',
+                            help='After plotting data, load and execute the '
+                                 'Python function specified by '
+                                 'POSTPROCESS_FUNC. POSTPROCESS_FUNC should be '
+                                 'a string of the form ``mymodule.myfunction``.'
+                                 'Example: '
+                                 '``--postprocess mymodule.myfunction``.')
+
+    #########################################################
+    ##################### GIF ARGUMENTS #####################
+    #########################################################
+
+    gif_maker = parser.add_argument_group("Gif Making Arguments",
+                                          description="Only needed if making a gif. "
+                                                      "Currently somewhat of an experimental feature, "
+                                                      "only tested with 1D or 2D avg pdist plots.",
+                                                      ) 
+    # avg_plus, duration, output path
+    gif_maker.add_argument("--avg-plus", default=100, nargs="?",
+                        dest="avg_plus",
+                        help="The +range of interations for each iter in range(first,last,step). "
+                             "So as the loop progresses, avg_plus is added to each iter to make the "
+                             "range that the average pdist is taken from. Important here is that you "
+                             "make sure avg_plus + last_iter does not exceed the total amount of iters "
+                             "you have available in the h5 file. If you set avg_plus to 0, it will "
+                             "make instant plots of each iter in the range requested. Default 100.",
+                        type=int)
+    gif_maker.add_argument("--duration", default=50, nargs="?",
+                        dest="duration", 
+                        help="Duration in milliseconds between frames of the gif, default 50ms.",
+                        type=int)
+    gif_maker.add_argument("--gif-out", default=None, nargs="?",
+                        dest="gif_out", 
+                        help="Out path to created gif file, e.g. 'example.gif'. "
+                             "Note this arg needs to be specified and not None for "
+                             "gif creation to begin.",
+                        type=str)
 
     # return the argument parser
     return parser 
 
 
 # TODO: adjust all to fix str/int/type auto
 def handle_command_line(argument_parser):
```

### Comparing `wedap-0.0.9/wedap/h5_pdist.py` & `wedap-1.0.0/wedap/h5_pdist.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,106 +5,130 @@
 This script effectively replaces the need to use the native WESTPA plotting pipeline:
 west.h5 --w_pdist(with --construct-dataset module.py)--> 
 pdist.h5 --plothist(with --postprocess-functions hist_settings.py)--> plot.pdf
 
 TODO: 
     - maybe add option to output pdist as file, this would speed up subsequent plotting
         of the same data. H5_Plot could then use this data.
-    - add option for a list of equivalent h5 files, alternative to w_multi_west.
     - method to return pdist of a single trace, leading into option to plot all succ traces.
 """
 
 # TEMP for trace plot (TODO)
 import matplotlib.pyplot as plt
 ######
 
+import os
 import h5py
 import numpy as np
 from tqdm.auto import tqdm
 
-from scipy.spatial import KDTree
-
 from warnings import warn
 
 # for copying h5 file
 import shutil
 
 # Suppress divide-by-zero in log
 np.seterr(divide='ignore', invalid='ignore')
 
 class H5_Pdist():
     """
     These class methods generate probability distributions from a WESTPA H5 file.
     """
     def __init__(self, h5="west.h5", data_type=None, Xname="pcoord", Xindex=0, Yname=None, 
-                 Yindex=0, Zname=None, Zindex=0, H5save_out=None, Xsave_name=None, Ysave_name=None,
-                 Zsave_name=None, data_proc=None, first_iter=1, last_iter=None, bins=(100,100), 
-                 p_units='kT', T=298, weighted=True, skip_basis=None, skip_basis_out=None,
-                 histrange_x=None, histrange_y=None, no_pbar=False, step_iter=1, *args, **kwargs):
-        """
+                 Yindex=0, Zname=None, Zindex=0, Cname=None, Cindex=0, 
+                 H5save_out=None, Xsave_name=None, Ysave_name=None, Zsave_name=None, 
+                 data_proc=None, first_iter=1, last_iter=None, step_iter=1, bins=(100,100), 
+                 p_units='kT', T=298, weighted=True, skip_basis=None, succ_only=False,
+                 histrange_x=None, histrange_y=None, no_pbar=False, *args, **kwargs):
+        """
+        Initialize this class with an `h5` file and `data_type`. The `X/Y/Zname` args
+        Can be a pcoord or aux dataset name in a west.h5 file, a 1D or 2D numpy array,
+        or the path to and name of a file (with a .dat, .txt, .pkl, .npz, .npy ending).
+
+        After instantiating this class, input args are saved as instance attributes.
+
+        These can then be updated if needed. The main method you will call is the
+        H5_Pdist.pdist() method, which will return the X, Y, and Z arrays to be plotted.
+        The X and Y arrays are 1D and represent the X and Y axis values to be plotted.
+        The Z array is empty with 2D output but otherwise will be a 2D array.
+
         Parameters
         ----------
         h5 : str or list of str
             Path(s) to west.h5 file(s).
         data_type : str
             'evolution' (1 dataset); 'average' or 'instant' (1 or 2 datasets)
-        Xname : str
-            Target data for x axis, default pcoord.
+        Xname : str or array
+            Target data for x axis, default pcoord. Can be a pcoord or aux dataset name 
+            in a west.h5 file, a 1D or 2D numpy array, or the path to and name of a file 
+            (with a .dat, .txt, .pkl, .npz, .npy ending).
         Xindex : int
             If X.ndim > 2, use this to index.
-        Yname : str
-            Target data for y axis, default None.
+        Yname : str or array
+            Target data for y axis, default None. Can be a pcoord or aux dataset name 
+            in a west.h5 file, a 1D or 2D numpy array, or the path to and name of a file 
+            (with a .dat, .txt, .pkl, .npz, .npy ending).
         Yindex : int
             If Y.ndim > 2, use this to index.
-        Zname : str
-            Target data for z axis, default None. 
+        Zname : str or array
+            Target data for z axis, default None. Can be a pcoord or aux dataset name 
+            in a west.h5 file, a 1D or 2D numpy array, or the path to and name of a file 
+            (with a .dat, .txt, .pkl, .npz, .npy ending).
             Use this if you want to use a dataset instead of pdist for Z axis.
             This will be best plotted as a scatter plot with Z as the marker color.
             Instead of returning the pdist, only the XYZ datasets will be returned.
             This is becasue the weights/pdist isn't considered.
         Zindex : int
             If Z.ndim > 2, use this to index.
+        Cname : str or array
+            Target data for cbar axis when using 3d projection scatter, default None. 
+            Can be a pcoord or aux dataset name in a west.h5 file, a 1D or 2D numpy array, 
+            or the path to and name of a file (with a .dat, .txt, .pkl, .npz, .npy ending).
+        Cindex : int
+            If C.ndim > 2, use this to index.
         H5save_out : str
             Paths to save a new H5 file with this dataset name.
             Right now it saves the requested X Y or Z data into a new aux_name.
             Note if you use this feature the input data must be the same shape and formatting as the other
             H5 file datasets. (TODO: organization?)
+            Also can be name of the outfile h5 file for optionally outputting new skipped basis or succ_only
+            h5 dataset with updated weights.
         Xsave_name, Ysave_name, Zsave_name : str
             Respective names to call the new dataset saved into the new H5 file.
         data_proc : function or tuple of functions
             Of the form f(data) where data has rows=segments, columns=frames until tau, depth=data dims.
             The input function must return a processed array of the same shape and formatting.
         first_iter : int
-            Default start plot at iteration 1 data.
+            Default start pdist at iteration 1 data.
         last_iter : int
             Last iteration data to include, default is the last recorded iteration in the west.h5 file. 
             Note that `instant` type pdists only depend on last_iter.
+        step_iter : int
+            Only use every step_iter size iteration intervals of the input data,
+            e.g. step_iter=10 for every 10 iterations.
         bins : tuple of ints (TODO: maybe the tuple isn't user friendly for 1 dim? Could check items like md_pdist)
             Histogram bins in pdist data to be generated for x and y datasets, default both 100.
         p_units : str
             Can be 'kT' (default), 'kcal', 'raw', or 'raw_norm'.
             kT = -lnP, kcal/mol = -RT(lnP), where RT = 0.5922 at `T` Kelvin.
             'raw' is the raw probabilities and 'raw_norm' is the raw probabilities P(max) normalized.
         T : int
             Temperature if using kcal/mol.
         weighted : bool
             Default True, use WE segment weights in pdist calculation.
         skip_basis : list
             List of binaries for each basis state to determine if it is skipped.
             e.g. [0, 0, 1] would only consider the trajectory data from basis 
             states 1 and 2 but would skip basis state 3, applying zero weights.
-        skip_basis_out : str
-            Name of the outfile h5 file for optionally outputting new skipped basis h5 dataset.
+        succ_only : bool
+            Default False, set True to filter weights to show only successfull trajectories.
         histrange_x, histrange_y : list or tuple of 2 floats or ints
             Optionally put custom bin ranges.
         no_pbar : bool
             Optionally do not include the progress bar for pdist generation.
-        step_iter : int
-            Only use every step_iter size iteration intervals of the input data,
-            e.g. step_iter=10 for every 10 iterations.
         TODO: maybe also binsfromexpression?
         """
         # standard case where the input h5 file is a single string
         if isinstance(h5, str):
             self.h5_list = [h5]
         # when input is a list one or many h5 files
         elif isinstance(h5, list):
@@ -126,27 +150,33 @@
             self.data_type = data_type
 
         self.p_units = str(p_units)
 
         self.T = int(T)
         self.weighted = weighted
 
-        # process XYZ names and indicies
+        # process XYZ names and indicies (TODO: maybe a more efficient way to go about this)
         self.Xname, self.Xindex = self._process_name_and_index(Xname, Xindex, Xname, Yname)
         self.Yname, self.Yindex = self._process_name_and_index(Yname, Yindex, Xname, Yname)
         self.Zname, self.Zindex = self._process_name_and_index(Zname, Zindex, Xname, Yname)
 
+        # for 3d proj plot cbar
+        self.Cname, self.Cindex = self._process_name_and_index(Cname, Cindex, Xname, Yname)
+
+        # check to make sure none of the Name / Index pairs are identical
+        self._check_duplicate_name_index_pairs()
+
         # XYZ save into new h5 file options
         self.H5save_out = H5save_out
         self.Xsave_name = Xsave_name
         self.Ysave_name = Ysave_name
         self.Zsave_name = Zsave_name
-        if H5save_out is not None:
-            shutil.copyfile(self.h5_name, H5save_out)
-            self.H5save_out = h5py.File(H5save_out, "r+")
+        # if H5save_out is not None:
+        #     shutil.copyfile(self.h5_name, str(H5save_out))
+        #     self.H5save_out = h5py.File(H5save_out, "r+")
         
         # raw data processing function
         # TODO: allow for 2-3 functions as tuple input, right now one function only
         self.data_proc = data_proc
 
         # default to last
         if last_iter is not None:
@@ -156,17 +186,30 @@
 
         if data_type == "instant":
             self.first_iter = self.last_iter
         else:
             self.first_iter = int(first_iter)
 
         self.step_iter = step_iter
-        self.bins = bins
+        
+        # standardize bins input
+        # case where the input bins is a single int
+        if isinstance(bins, int):
+            # convert single int to 1 element list to be indexable later
+            self.bins = [bins]
+            # if there is a 2 dimensional pdist requested, make same int bins each dim
+            if Yname is not None:
+                self.bins = [bins, bins]
+        # when input is already a list of bins with an item for each dimension
+        elif isinstance(bins, (list, tuple)):
+            self.bins = bins
+        else:
+            raise ValueError(f"Something may be wrong with bins input: {bins}")
+
         self.skip_basis = skip_basis
-        self.skip_basis_out = skip_basis_out
 
         # initialize weights
         self._init_weights()
 
         # n_particles for each iteration
         self.n_particles = self.h5["summary"]["n_particles"]
 
@@ -179,14 +222,15 @@
 
         # integer for the amount of frames saved (length) per tau (e.g. 101 for 100 ps tau)
         self.tau = self._get_data_array("pcoord", 0, self.first_iter).shape[1]
 
         self.histrange_x = histrange_x
         self.histrange_y = histrange_y
         self.no_pbar = no_pbar
+        self.succ_only = succ_only
 
         # accounts for array and filename input XYZnames
         self._check_XYZnames()
 
     def _process_name_and_index(self, name, index, Xname, Yname):
         """
         Consolidated logic for taking input XYZnames and outputting the 
@@ -196,49 +240,58 @@
         ----------
         name : str
             Input XYZ name.
         index : int
             Input XYZ index 
         Xname : str
         Yname : str
+        # usingY : bool
+        #     Set to True when returning name/index for Yname, default False.
         
         Returns
         -------
         name : str
             Corrected XYZ name.
         index : int
             Corrected XYZ index.
         """
         if name is not None and isinstance(name, str):
             # add auxdata prefix if not using "pcoord" and not using array or filename input
-            if name != "pcoord" and name[-4:] != ".":
+            # instead of checking for '.', check for filename
+            #if name != "pcoord" and name[-4] != ".":
+            if name != "pcoord" and not os.path.isfile(name):
                 name = "auxdata/" + name
             # for common case of evolution with extra Yname input
-            if self.data_type == "evolution":
+            if self.data_type == "evolution" and Yname is not None:
                 warn("\nDefaulting to evolution plot for --data-type, since you put a --Yname arg.\n"
                     "Did you mean to use --data-type of `average` or `instant`?")
-            # for common case where one plots "pcoord/aux 0" and "pcoord/aux 1"
-            elif isinstance(name, str) and name == Yname and Xname == Yname and index == 0:
-                index = 1
-                warn("\nSetting --Yindex to 1 (2nd dimension) since Xname/Yname and Xindex/Yindex were the same.")
+            # for case with "pcoord/aux 0" and "pcoord/aux 0": same name and index will auto change index
+            # Note: this didnt really work if you set -xi 1 or other index and -yi 0 
+            #       need to actually compare the xindex and yindex within this function
+            #       instead, just not going to include this check.
+            # elif isinstance(name, str) and usingY and Xname == Yname and index == 0:
+            #     index = 1
+            #     warn("\nSetting --Yindex to 1 (2nd dimension) since Xname/Yname and Xindex/Yindex were the same.")
         return name, index
 
     def _check_XYZnames(self):
         """
         Check XYZnames for array and filename input (if found, initialize).
         Replaces self.Xname, self.Yname, and self.Zname attrs as needed.
         """
-        XYZnames = ["Xname", "Yname", "Zname"]
+        XYZnames = ["Xname", "Yname", "Zname", "Cname"]
         for name in XYZnames:
             attr_value = getattr(self, name)
             # reshape 1d input raw data array (if given) into 3d array
             if isinstance(attr_value, np.ndarray):
                 setattr(self, name, self.reshape_total_data_array(attr_value))
             # if input isn't an auxname but an allowed filename for input
-            elif isinstance(attr_value, str) and attr_value[-4] == ".":
+            # instead of checking for '.', check for filename
+            #elif isinstance(attr_value, str) and attr_value[-4] == ".":
+            elif isinstance(attr_value, str) and os.path.isfile(attr_value):
                 # for .npy binary files or pkl files
                 if attr_value[-4:] in [".npy", ".npz", ".pkl"]:
                     data = np.load(attr_value, allow_pickle=True)
                 # text files
                 elif attr_value[-4:] in [".dat", ".txt"]:
                     data = np.genfromtxt(attr_value)
                 else:
@@ -260,20 +313,64 @@
         elif self.skip_basis:
             weight_start = 1
 
         # make a (TODO: pre-allocated?) list for each iteration weight array
         #weights = [None] * (self.last_iter - weight_start + 1)
         weights = []
         # fill out the weight list
-        for iter in range(weight_start, self.last_iter + 1, self.step_iter):
+        # can't use step-iter here since the entire weight array needs to be indexed by step-iter later
+        #for iter in range(weight_start, self.last_iter + 1, self.step_iter):
+        for iter in range(weight_start, self.last_iter + 1):
             #weights[iter - weight_start] = self.h5[f"iterations/iter_{iter:08d}/seg_index"]["weight"]
             weights.append(self.h5[f"iterations/iter_{iter:08d}/seg_index"]["weight"])
         # 1D array of variably shaped arrays
         self.weights = np.array(weights, dtype=object)
 
+    def _check_duplicate_name_index_pairs(self):
+        """
+        Warnings if there are duplicate XYZ name/index pairs.
+        """
+        # only check all of them if Cname is not None
+        if self.Cname is not None:
+            pairs = [(self.Xname, self.Xindex), (self.Yname, self.Yindex), 
+                     (self.Zname, self.Zindex), (self.Cname, self.Cindex)]
+        # only check if Zname is not None
+        elif self.Zname is not None:
+            pairs = [(self.Xname, self.Xindex), (self.Yname, self.Yindex), (self.Zname, self.Zindex)]
+        else:
+            pairs = [(self.Xname, self.Xindex), (self.Yname, self.Yindex)]
+        seen_pairs = set()
+        duplicates = set()
+
+        for pair in pairs:
+            # for input numpy arrays, skip this checking
+            if isinstance(pair[0], np.ndarray):
+                pass
+
+            # otherwise check if the pair has been seen before
+            elif pair in seen_pairs:
+                duplicates.add(pair)
+            else:
+                seen_pairs.add(pair)
+
+        if duplicates:
+            # Handle duplicates
+            # For example, you can print a message or perform any desired action
+            message = "Duplicate name and index pairs found, "
+            message += "check to make sure XYZname and XYZindex values are unique:\n" 
+            message += f"Xname: {self.Xname}, Xindex: {self.Xindex}\n"
+            message += f"Yname: {self.Yname}, Yindex: {self.Yindex}\n"
+            message += f"Zname: {self.Zname}, Zindex: {self.Zindex}\n" 
+            warn(message)
+            # for pair in duplicates:
+            #     print(f"Name: {pair[0]}, Index: {pair[1]}")
+        #else:
+            # No duplicates found
+            #print("No duplicate name and index pairs found")
+
     def _get_data_array(self, name, index, iteration, h5_create=None, h5_create_name=None):
         """
         Extract, index, and return the aux/data array of interest.
         Rows are segments, columns are frames until tau, depth is ndimensional datasets.
 
         Parameters
         ----------
@@ -302,17 +399,23 @@
             n_segs_including_iter = np.sum(self.n_particles[self.first_iter-1:iteration])
             data = name[n_segs_up_to_iter:n_segs_including_iter,:,:]
 
         # name should be a string for the h5 file dataset name
         elif isinstance(name, str):
             # this t/e block is to catch non-existent aux data names
             try:
-                data = np.array(self.h5[f"iterations/iter_{iteration:08d}/{name}"])
-            except KeyError:
-                message = f"{name} is not a valid object in the h5 file. \n" + \
+                #data = np.array(self.h5[f"iterations/iter_{iteration:08d}/{name}"])
+                #data = self.h5[f"iterations/iter_{iteration:08d}/{name}"][:]
+                # seems like data is okay left as type: <class 'h5py._hl.dataset.Dataset'>
+                # doesn't need to be an array, I guess array indexing already works so it's compatible
+                # speeds seem pretty similar for both though
+                # and the np.atleast_3d will convert to array anyway
+                data = self.h5[f"iterations/iter_{iteration:08d}/{name}"]
+            except KeyError as e:
+                message = f"{e}: {name} is not a valid object in the h5 file. \n" + \
                           f"Available datasets are: 'pcoord' "
                 # this t/e block is to catch the case where there are no aux datasets at all
                 try:
                     auxnames = list(self.h5[f"iterations/iter_{self.first_iter:08d}/auxdata"])
                     message += f"and the following aux datasets {auxnames}"
                 except KeyError:
                     message += "and no aux datasets were found"
@@ -443,15 +546,15 @@
 
     def _new_weights_from_skip_basis(self):
         """
         Make a new temp h5 file with zero weights for skipped basis state walkers.
 
         Returns
         -------
-        self.weights : array
+        new_weights : array
             Updated weight array with zero values for skipped basis states.
         """
         # TODO: doesn't work with --first-iter
         
         # copy of weights to edit
         new_weights = self.weights
 
@@ -510,105 +613,25 @@
 
                             # make new empty list to store the iteration's skipped
                             skip_parents_c.clear()
                             skip_parents_c += skip_parents_n
                             skip_parents_n.clear()
 
         # TODO: prob can do better than these print statements
-        print("pdist calculation: ")
+        #print("pdist calculation: ")
         # write new weights into skip_basis_out h5 file
-        if self.skip_basis_out is not None:
-            shutil.copyfile(self.h5_name, self.skip_basis_out)
-            h5_skip_basis = h5py.File(self.skip_basis_out, "r+")
-            for idx, weight in enumerate(new_weights):
-                h5_skip_basis[f"iterations/iter_{idx+1:08d}/seg_index"]["weight"] = weight
+        # TODO: wrap this into h5saveout and include succ_only
+        # if self.skip_basis_out is not None:
+        #     shutil.copyfile(self.h5_name, self.skip_basis_out)
+        #     h5_skip_basis = h5py.File(self.skip_basis_out, "r+")
+        #     for idx, weight in enumerate(new_weights):
+        #         h5_skip_basis[f"iterations/iter_{idx+1:08d}/seg_index"]["weight"] = weight
             
         # only return portion of weights requested by user
-        return new_weights[self.first_iter-1:self.last_iter]
-
-    # TODO: clean up and optimize
-    def search_aux_xy_nn(self, val_x, val_y):
-        """
-        Originally adapted from code by Jeremy Leung.
-        Tree search to find closest datapoint to input data value(s).
-
-        # TODO: add step size for searching, right now gets the last frame
-
-        Parameters
-        ----------
-        val_x : int or float
-            X dataset value to search for.
-        val_y : int or float
-            Y dataset value to search for.
-        """
-        # iter is already known when searching evo data
-        if self.data_type == "evolution":
-            iter_num = int(val_y)
-            
-            # These are the auxillary coordinates you're looking for
-            r1 = self._get_data_array(self.Xname, self.Xindex, iter_num)[:,-1]
-
-            # phase 2: finding seg number
-
-            # TODO: numpy array this
-            small_array2 = []
-            for j in range(0,len(r1)):
-                small_array2.append([r1[j]])
-            tree2 = KDTree(small_array2)
-
-            # TODO: these can be multiple points, maybe can parse these and filter later
-            d2, i2 = tree2.query([val_x],k=1)
-            seg_num = int(i2)
-
-        else:
-            # phase 1: finding iteration number
-            distances = []
-            indices = []
-
-            # change indices to number of iteration
-            #for i in range(self.first_iter, self.last_iter + 1): 
-            # always use iteration 1 to get full trace path
-            for i in range(1, self.last_iter + 1): 
-
-                # These are the auxillary coordinates you're looking for
-                r1 = self._get_data_array(self.Xname, self.Xindex, i)[:,-1]
-                r2 = self._get_data_array(self.Yname, self.Yindex, i)[:,-1]
-
-                small_array = []
-                for j in range(0,len(r1)):
-                    small_array.append([r1[j],r2[j]])
-                tree = KDTree(small_array)
-
-                # Outputs are distance from neighbour (dd) and indices of output (ii)
-                dd, ii = tree.query([val_x, val_y],k=1) 
-                distances.append(dd) 
-                indices.append(ii)
-
-            minimum = np.argmin(distances)
-            iter_num = int(minimum+1)
-
-            # These are the auxillary coordinates you're looking for
-            r1 = self._get_data_array(self.Xname, self.Xindex, iter_num)[:,-1]
-            r2 = self._get_data_array(self.Yname, self.Yindex, iter_num)[:,-1]
-
-            # phase 2: finding seg number
-
-            # TODO: numpy array this
-            small_array2 = []
-            for j in range(0,len(r1)):
-                small_array2.append([r1[j],r2[j]])
-            tree2 = KDTree(small_array2)
-
-            # TODO: these can be multiple points, maybe can parse these and filter later
-            d2, i2 = tree2.query([val_x, val_y],k=1)
-            seg_num = int(i2)
-
-        #print("go to iter " + str(iter_num) + ", " + "and seg " + str(seg_num))
-        print(f"Go to ITERATION: {iter_num} and SEGMENT: {seg_num}")
-        return iter_num, seg_num
+        return new_weights[self.first_iter-1:self.last_iter:self.step_iter]
 
     ##################### TODO: update or organize this #############################
     def get_parents(self, walker_tuple):
         """
         Get parent of an input (iteration, walker).
 
         Parameters
@@ -620,120 +643,271 @@
         -------
         parent : iteration, walker
         """
         it, wlk = walker_tuple
         parent = self.h5[f"iterations/iter_{it:08d}"]["seg_index"]["parent_id"][wlk]
         return it-1, parent
 
-    def trace_walker(self, walker_tuple):
+    def trace_walker(self, walker_tuple, first_iter=1):
         """
         Get trace path of an input (iteration, walker).
 
         Parameters
         ----------
         walker_tuple : tuple
             (iteration, walker)
+        first_iter : int
+            Iter to trace back to. Default 1.
 
         Returns
         -------
         trace : list of tuples
             Tuples are (iteration, walker) traces.
         """
         # Unroll the tuple into iteration/walker 
         it, wlk = walker_tuple
         # Initialize our path
         path = [(it,wlk)]
         # And trace it
-        while it > 1: 
+        while it > first_iter: 
             it, wlk = self.get_parents((it, wlk))
             path.append((it,wlk))
         return np.array(sorted(path, key=lambda x: x[0]))
 
     def get_coords(self, path, data_name, data_index):
         """
         Get a list of data coordinates for plotting traces.
+        Only grabs the last frames.
 
         Parameters
         ----------
         path : list of tuples
             Tuples are (iteration, walker) traces.
         data_name : str
             Name of dataset.
         data_index : int
             Index of dataset.
 
         Returns
         -------
-        coordinates : array
+        coordinates : 1d array
+            Array of coordinates from the list of (iteration, walker) tuples.
+        """
+        # Initialize an array for the pcoords
+        coords = np.zeros((len(path)))
+        # Loop over the path and get the pcoords for each walker
+        for idx, (it, wlk) in enumerate(path):
+            coords[idx] = (self._get_data_array(data_name, data_index, it)[wlk][-1])
+        return coords
+    
+    def get_full_coords(self, walker_tuple, data_name, data_index=0, first_iter=1):
+        """
+        Returns a full 1D set of data for a single trace (path).
+        This will be ordered from the first iter to the last.
+
+        Parameters
+        ----------
+        walker_tuple : tuple
+            (iteration, walker) start point to trace from.
+        data_name : str
+            Name of dataset.
+        data_index : int
+            Index of dataset.
+        first_iter : int
+            Iter to trace back to. Default 1.
+            
+        Returns
+        -------
+        coordinates : 1d array
             Array of coordinates from the list of (iteration, walker) tuples.
         """
-        # Initialize a list for the pcoords
-        coords = []
+        # account for non-pcoord input strings
+        if data_name != "pcoord":
+            data_name = "auxdata/" + data_name
+
+        path = self.trace_walker(walker_tuple, first_iter)
+        # Initialize an array for the pcoords (each iter * tau)
+        coords = np.zeros((len(path)*self.tau))
+        
         # Loop over the path and get the pcoords for each walker
-        for it, wlk in path:
-            coords.append(self._get_data_array(data_name, data_index, it)[wlk][::10])
-        return np.array(coords)
+        # path will be ordered from the first iter to the last.
+        for idx, (it, wlk) in enumerate(path):
+            # fill out the array in self.tau chunks
+            coords[idx*self.tau:(idx+1)*self.tau] = self._get_data_array(data_name, data_index, it)[wlk]
+
+        return coords            
+
+    def find_iter_seg_from_xy_vals(self, val_x, val_y):
+        """
+        Find and return (iter, seg) closest to input data value(s).
+
+        Parameters
+        ----------
+        val_x : int or float
+            X dataset value to search for.
+        val_y : int or float
+            Y dataset value to search for.
+
+        Returns
+        -------
+        iter_num, seg_num : int, int
+            Iteration, segment number.
+        """
+        # for evolution plots, only need to search one iteration
+        if self.data_type == "evolution":
+            # convert to int since it is an iteration number
+            val_y = int(val_y)
+            # Extract x values for the val_y iteration
+            x_data = self._get_data_array(self.Xname, self.Xindex, val_y)[:,-1]
+            # Calculate distances between input x values and all data points in the current iteration
+            dist = np.abs(x_data - val_x)
+            min_dist_idx = np.argmin(dist)
+            min_dist = dist[min_dist_idx]
+            # iter, seg return: iter is from y value, seg is from min dist
+            return val_y, min_dist_idx
+
+        # for e.g. average plots, search all iterations of both x and y values
+        distances = []
+        # always use iteration 1 to get full trace path
+        for i in tqdm(range(1, self.last_iter + 1, self.step_iter), 
+                      desc="Trace Search", disable=self.no_pbar): 
+            # Extract x and y values for the current iteration
+            x_data = self._get_data_array(self.Xname, self.Xindex, i)[:,-1]
+            y_data = self._get_data_array(self.Yname, self.Yindex, i)[:,-1]
+            # Calculate distances between input values and all data points in the current iteration
+            dist = np.sqrt((x_data - val_x)**2 + (y_data - val_y)**2)
+
+            # Find the minimum distance and its index
+            min_dist_idx = np.argmin(dist)
+            min_dist = dist[min_dist_idx]
+
+            distances.append((min_dist, i, min_dist_idx))
+
+        # Find the iteration and segment with the minimum distance
+        min_distance, iter_num, seg_num = min(distances)
 
-    def plot_trace(self, walker_tuple, color="white", ax=None):
+        print(f"Tracing ITERATION: {iter_num}, SEGMENT: {seg_num}")
+        return iter_num, seg_num
+
+    # TODO: alot of the self refs are not even in h5_pdist, but in h5_plot
+    #       need to do some rearrangement and refactoring at some point
+    def plot_trace(self, walker_tuple, color="white", linewidth=1.0, linestyle='-', ax=None, 
+                   find_iter_seg=False, **kwargs):
         """
         Plot trace.
 
         Parameters
         ----------
         walker_tuple : tuple
             (iteration, walker) start point to trace from.
+            Can also find the closest iteration/seg using input as (X_value,Y_value).
+            `find_iter_seg` must be True to use this setting.
         color : str
+        linewidth : int
+        linestyle : str
         ax : mpl axes object
+        find_iter_seg : bool
+            Default False and use walker tuple as (iter, seg). 
+            Set True to look for (iter, seg) using walker_tuple input as (X_value,Y_value).
+        **kwargs
+            Passed to mpl plt.plot line plots. E.g. alpha parameter.
         """
         # TODO: update/streamline this
         if ax is None:
-            fig, ax = plt.subplots(figsize=(7,5))
+            fig, ax = plt.subplots()
         else:
             fig = plt.gcf()
 
+        # TODO: temp linestyle check, eventually move this whole method elsewhere
+        #       need to be able to use cli and pass linestyle, while being able to use API
+        #       where linestyle might not always be available if using h5_pdist and h5_plot separately
+        # if object has linestyle specified, use it, otherwise use arg
+        if hasattr(self, 'linestyle'):
+            linestyle = self.linestyle
+
+        # search for iter_seg if specified
+        if find_iter_seg:
+            walker_tuple = self.find_iter_seg_from_xy_vals(walker_tuple[0], walker_tuple[1])
+
         path = self.trace_walker(walker_tuple)
         # adjustments for plothist evolution of only aux_x data
         if self.data_type == "evolution":
             # split iterations up to provide y-values for each x-value (pcoord)
             aux = self.get_coords(path, self.Xname, self.Xindex)
-            iters = np.arange(1, len(aux)+1)
-            ax.plot(aux[:,0], iters, c="black", lw=2)
-            ax.plot(aux[:,0], iters, c=color, lw=1)
+            iters = np.arange(1, len(aux)+1, self.step_iter)
+            ax.plot(aux[::self.step_iter], iters, c="black", lw=linewidth+1, linestyle=linestyle, **kwargs)
+            ax.plot(aux[::self.step_iter], iters, c=color, lw=linewidth, linestyle=linestyle, **kwargs)
             return
 
         # And pull aux_coords for the path calculated
         aux_x = self.get_coords(path, self.Xname, self.Xindex)
         aux_y = self.get_coords(path, self.Yname, self.Yindex)
 
-        ax.plot(aux_x[:,0], aux_y[:,0], c="black", lw=2)
-        ax.plot(aux_x[:,0], aux_y[:,0], c=color, lw=1)
+        ax.plot(aux_x[::self.step_iter], aux_y[::self.step_iter], c="black", lw=linewidth+1, linestyle=linestyle, **kwargs)
+        ax.plot(aux_x[::self.step_iter], aux_y[::self.step_iter], c=color, lw=linewidth, linestyle=linestyle, **kwargs)
 
     def w_succ(self):
         """
         Find and return all successfully recycled (iter, seg) pairs.
-        TODO eventually can use this to plot pdist of succ only trajs
-        note that I would have to norm by the overall pmax (not just succ pmax)
-        Could have this be an optional feature.
+
+        Returns
+        -------
+        succ : list of tuples (iter,wlk)
         """
         succ = []
-        for iter in range(self.last_iter):
+        for iter in tqdm(range(self.first_iter, self.last_iter + 1), 
+                         desc="Running w_succ", disable=self.no_pbar):
             # if the new_weights group exists in the h5 file
             if f"iterations/iter_{iter:08d}/new_weights" in self.h5:
                 prev_segs = self.h5[f"iterations/iter_{iter:08d}/new_weights/index"]["prev_seg_id"]
                 # append the previous iter and previous seg id recycled
                 for seg in prev_segs:
                     succ.append((iter-1, seg))
         # TODO: order this by iter and seg vals? currently segs not sorted but is iter ordered
         return succ
-    def succ_pdist(self):
+    
+    def succ_pdist_weight_filter(self):
         """
         TODO: Filter weights to be zero for all non successfull trajectories.
         Make an array of zero weights and fill out weights for succ trajs only.
+        option to output new h5?
+
+        Returns
+        -------
+        succ_weights : numpy object array
+            Updated weight array.
         """
-        pass
+        # start with zero weight array and fill it with succ traj traces
+        #succ_weights = np.zeros_like(self.weights, dtype=object)
+        #succ_weights = np.vstack((np.zeros_like(w) for w in self.weights), dtype=object)
+
+        # find the per iter n_seg lengths along axis 1 for weights
+        seg_lengths = [len(arr) for arr in self.weights]
+        #print(seg_lengths)
+
+        # Create a new array filled with zeros with the same variable shape
+        succ_weights = np.array([np.zeros(length) for length in seg_lengths], dtype=object)
+    
+        #print(succ_weights.shape)
+        #print(self.weights.shape)
+
+        # trace through each succ traj and fill in weights
+        # TODO: there is some redundancy here, no need to fill weight when previously filled
+        succ_trajs = self.w_succ()
+        for succ in tqdm(succ_trajs, disable=self.no_pbar,
+                         desc="Creating succ only weight array"):
+            trace_path = self.trace_walker(succ)
+            for it, wlk in trace_path:
+                #print(succ_weights[it][wlk], self.weights[it][wlk])
+                # -1 for indexing iters but regular indexing walkers
+                succ_weights[it-1][wlk] = self.weights[it-1][wlk]
+
+        # only return portion of weights requested by user
+        return succ_weights[self.first_iter-1:self.last_iter:self.step_iter]
+
     ###############################################################################
 
     def aux_to_pdist_1d(self, iteration):
         """
         Take the auxiliary dataset for a single iteration and generate a weighted
         1D probability distribution. 
 
@@ -968,28 +1142,70 @@
         X = np.zeros((self.current_particles, self.tau))
         Y = np.zeros((self.current_particles, self.tau))
         Z = np.zeros((self.current_particles, self.tau))
 
         # loop each iteration
         seg_start = 0
         for iter in tqdm(range(self.first_iter, self.last_iter + 1, self.step_iter), 
-                         desc="Average 3D", disable=self.no_pbar):
+                         desc="Data 3D", disable=self.no_pbar):
             # then go through and add all segments/walkers in the iteration
             X[seg_start:seg_start + self.n_particles[iter - 1]] = \
                 self._get_data_array(self.Xname, self.Xindex, iter)
             Y[seg_start:seg_start + self.n_particles[iter - 1]] = \
                 self._get_data_array(self.Yname, self.Yindex, iter)
             Z[seg_start:seg_start + self.n_particles[iter - 1]] = \
                 self._get_data_array(self.Zname, self.Zindex, iter)
 
             # keeps track of position in the seg_total length based arrays
             seg_start += self.n_particles[iter - 1]
 
-        # 3D average datasets using all available data (can more managable with interval)
+        # 3D datasets using all available data (can be more managable with interval)
         return X[::interval], Y[::interval], Z[::interval]
+    
+    # TODO: very similar method to avg_datasets_3d, also could combine with code from get_total_dataset
+    def average_datasets_4d(self, interval=1):
+        """
+        Unique case where `Zname` is specified and the XYZ datasets are returned.
+        Averaged over the iteration range. With `Cname`, 4d.
+        
+        Returns
+        -------
+        X, Y, Z, C : arrays 
+            Raw data for each named coordinate.
+        """
+        if self.Yname is None:
+            warn("`Zname` is defined but not `Yname`, using Yname=`pcoord`")
+            self.Yname = "pcoord"
+
+        # arrays to be filled with values from each iteration
+        # rows are for all segments, columns are each segment datapoint
+        X = np.zeros((self.current_particles, self.tau))
+        Y = np.zeros((self.current_particles, self.tau))
+        Z = np.zeros((self.current_particles, self.tau))
+        C = np.zeros((self.current_particles, self.tau))
+
+        # loop each iteration
+        seg_start = 0
+        for iter in tqdm(range(self.first_iter, self.last_iter + 1, self.step_iter), 
+                         desc="Data 4D", disable=self.no_pbar):
+            # then go through and add all segments/walkers in the iteration
+            X[seg_start:seg_start + self.n_particles[iter - 1]] = \
+                self._get_data_array(self.Xname, self.Xindex, iter)
+            Y[seg_start:seg_start + self.n_particles[iter - 1]] = \
+                self._get_data_array(self.Yname, self.Yindex, iter)
+            Z[seg_start:seg_start + self.n_particles[iter - 1]] = \
+                self._get_data_array(self.Zname, self.Zindex, iter)
+            C[seg_start:seg_start + self.n_particles[iter - 1]] = \
+                self._get_data_array(self.Cname, self.Cindex, iter)
+
+            # keeps track of position in the seg_total length based arrays
+            seg_start += self.n_particles[iter - 1]
+
+        # 4D datasets using all available data (can be more managable with interval)
+        return X[::interval], Y[::interval], Z[::interval], C[::interval]
 
     def get_all_weights(self):
         """
         Returns an 1D array of the weight for every frame of each tau 
         for all segments of all iterations specified.
 
         Returns
@@ -1080,95 +1296,134 @@
         # which can be the correct shape if pulled from westpa (e.g. 100 ps + 1)
         # or if from agg MD sim, will just be (e.g. 100 ps)
         # also adding -1 in z dim for extra depth dimension compatibility
 
         # TODO: change total particles to iteration range to be able to use iter args with data arrays
 
         try:
-            array = array.reshape(self.total_particles, self.tau, -1)
+            array = array.reshape(self.current_particles, self.tau, -1)
         # e.g. ValueError: cannot reshape array of size 303000 into shape (3000,100,newaxis)
         except ValueError as e:
-            array = array.reshape(self.total_particles, self.tau - 1, -1)
-            message = "\nYou may be using an input data array which did not include the rst file datapoints. " + \
-                      "\nThis will work, but note that you shouldn't create a new H5 file using this array."
-            warn(f"{e} {message}")
-            # the case where the array does not have rst data included
-            # put the new first column as the first value of each row (segment)
-            # TODO: this is a temp hack for the no rst shape data
-            # noting that both arrays must have same ndims for hstack
-            #print(f"original shape: {array.shape}")
-            #print(f"to stack shape: {np.atleast_3d(array[:,0,:]).shape}")
-            # make array for all first col vals reshape so that the columns go depth wise
-            firstcols = array[:,0,:].reshape(array.shape[0], 1, -1)
-            array = np.hstack((firstcols, array))
-            #print(f"new shape: {array.shape}")
+            try:
+                array = array.reshape(self.current_particles, self.tau - 1, -1)
+                message = "\nYou may be using an input data array which did not include the rst file datapoints. " + \
+                        "\nThis will work, but note that you shouldn't create a new H5 file using this array."
+                warn(f"{e} {message}")
+                # the case where the array does not have rst data included
+                # put the new first column as the first value of each row (segment)
+                # TODO: this is a temp hack for the no rst shape data
+                # noting that both arrays must have same ndims for hstack
+                #print(f"original shape: {array.shape}")
+                #print(f"to stack shape: {np.atleast_3d(array[:,0,:]).shape}")
+                # make array for all first col vals reshape so that the columns go depth wise
+                firstcols = array[:,0,:].reshape(array.shape[0], 1, -1)
+                array = np.hstack((firstcols, array))
+                #print(f"new shape: {array.shape}")
+            # for cases where the WE simulation didn't exit and make next empty iteration
+            except ValueError:
+                array = array.reshape(np.sum(self.h5["summary"]["n_particles"][self.first_iter-1:self.last_iter-1]), 
+                                      self.tau - 1, -1)
+                
 
         # TODO: the above works to solve the shape issue but if I wanted to fill out a new dataset in
         # the h5 file, it would be missing the first value, which links walkers.
         # maybe I can use the parent IDs to link it manually, but note I would have to
         # go through and parse by my self.n_particles array to separate iterations.
         # put conditional if shape[1] = tau vs tau - 1 for creating dataset (to add parent data point)
         # note that the first iteration I need to pull from somewhere else? It's calculated from the
         # original bstate file
 
         # Note, if the user includes the rst files like WESTPA does, it should look and process fine
 
         return array
 
+    def make_new_h5(self, new_weights=None):
+        """
+        TODO: actually make a new h5 file, see bstate filter code, integrate all.
+        If self.H5save_out is not None and X/Y/Zsave_name is not None.
+        Saves out a new h5 file of name self.H5save_out with the current
+        X/Y/Zname data into auxdata of h5 file with name of X/Y/Zsave_name.
+
+        Parameters
+        ----------
+        new_weights : numpy object array
+            Updated weight values, e.g. from skip_basis or succ_only.
+        """
+        # make copy of h5 file and open copy
+        shutil.copyfile(self.h5_name, self.H5save_out)
+        self.H5save_out = h5py.File(self.H5save_out, "r+")
+        # replace weights
+        if new_weights is not None:
+            for idx, weight in enumerate(new_weights):
+                self.H5save_out[f"iterations/iter_{idx+1:08d}/seg_index"]["weight"] = weight
+
+        # create new dataset based on input XYZ data
+        for iter in tqdm(range(self.first_iter, self.last_iter + 1, self.step_iter), 
+                         desc="Creating new h5 dataset(s)", disable=self.no_pbar):
+            if self.Xsave_name:
+                self._get_data_array(self.Xname, self.Xindex, iter, self.H5save_out, self.Xsave_name)
+            if self.Ysave_name:
+                self._get_data_array(self.Yname, self.Yindex, iter, self.H5save_out, self.Ysave_name)
+            if self.Zsave_name:
+                self._get_data_array(self.Zname, self.Zindex, iter, self.H5save_out, self.Zsave_name)
+
     def pdist(self, normalize=True):
         """
         Main public method with pdist generation controls.
 
         Parameters
         ----------
         normalize : bool
             By default (True), normalizes the output pdist.
             Must be True when using multiple h5 input files.
         
         Returns
         -------
         X, Y, Z : arrays
+            Output probability distributions.
         """ 
+        # empty object to pass to make_new_h5
+        new_weights = None
         # option to zero weight out specific basis states
         if self.skip_basis is not None:
             self.n_bstates = self.h5["ibstates/index"]["n_bstates"]
             try: 
-                self.weights = self._new_weights_from_skip_basis()
+                new_weights = self.weights = self._new_weights_from_skip_basis()
             # if the wrong amount of args are input and != n_bstates
             except IndexError as e:
                 message = f"IndexError ({e}) for bstate input ({self.skip_basis}): " + \
                           f"Did you use the correct amount of bstates {self.n_bstates}?"
                 warn(message)
 
-        # TODO: could make this it's own method
+        # option to only use weights for succ trajs
+        if self.succ_only is True:
+            # replace the original weight array with succ only
+            new_weights = self.weights = self.succ_pdist_weight_filter()
+
         # if requested, save out a new H5 file with the input data array in new aux name
         if self.H5save_out is not None:
-            for iter in range(self.first_iter, self.last_iter + 1):
-                if self.Xsave_name:
-                    self._get_data_array(self.Xname, self.Xindex, iter, self.H5save_out, self.Xsave_name)
-                if self.Ysave_name:
-                    self._get_data_array(self.Yname, self.Yindex, iter, self.H5save_out, self.Ysave_name)
-                if self.Zsave_name:
-                    self._get_data_array(self.Zname, self.Zindex, iter, self.H5save_out, self.Zsave_name)
+            self.make_new_h5(new_weights)
 
         # TODO: need to consolidate the Y 2d vs 1d stuff somehow
 
         # multi_h5: putting the whole thing in a loop over each h5 file
         # loop histranges to find the best hist range for all input h5 files
         # loop each pdist return, sum and normalize at the end
 
         # collect each histrange for each file 
         xranges = []
         yranges = []
         # go through each file and find a consistent histrange if histrangeXY is None
-        for h5 in self.h5_list:
-            # close and re-open, keeping the class attribute for method calls
-            # but allowing the loop to propagate through each file
-            self.h5.close()
-            self.h5 = h5py.File(h5, mode="r")
+        for i, h5 in enumerate(self.h5_list):
+            # only needs to be done for non-first dataset in h5_list
+            if i != 0:
+                # close and re-open, keeping the class attribute for method calls
+                # but allowing the loop to propagate through each file
+                self.h5.close()
+                self.h5 = h5py.File(h5, mode="r")
             if self.histrange_x is None:
                 # get the optimal histrange
                 xranges.append(self._get_histrange(self.Xname, self.Xindex))
                 histrange_x = (min(i[0] for i in xranges),
                                max(i[1] for i in xranges))
             # 2D pdist: needs to handle array input or None input
             if isinstance(self.Yname, (str, np.ndarray)) and self.histrange_y is None:
@@ -1182,35 +1437,38 @@
         if isinstance(self.Yname, (str, np.ndarray)) and self.histrange_y is None:
             self.histrange_y = histrange_y
 
         # collect each iteration's XYZ arrays for potential summation
         Xs = []
         Ys = []
         Zs = []
+        Cs = []
         # same loop but now use the optimized histrange for pdist gen of all h5 files in list
-        for h5 in self.h5_list:
-            # close and re-open, keeping the class attribute for method calls
-            # but allowing the loop to propagate through each file
-            self.h5.close()
-            self.h5 = h5py.File(h5, mode="r")
-            self._init_weights()
-            
-            # TODO: instead of just opening h5 and re-init weights, need to also account for
-            # cases like with 3D dataset returns which use self.n_particles (segs per iter)
-            # perhaps I can just reinit the entire set of attrs
-            #self.h5 = h5
-            #self.__init__(self)
-            
-            # TODO: maybe this could go into a _particle_init method?
-            # for now just going to save a new self.n_particles attribute
-            self.n_particles = self.h5["summary"]["n_particles"]
-            # these may not be needed, 
-            self.current_particles = np.sum(self.h5["summary"]["n_particles"][self.first_iter-1:self.last_iter])
-            # do not include the final (empty) iteration
-            self.total_particles = np.sum(self.h5["summary"]["n_particles"][:-1])
+        for i, h5 in enumerate(self.h5_list):
+            # only needs to be done for non-first dataset in h5_list
+            if i != 0:
+                # close and re-open, keeping the class attribute for method calls
+                # but allowing the loop to propagate through each file
+                self.h5.close()
+                self.h5 = h5py.File(h5, mode="r")
+                self._init_weights()
+                
+                # TODO: instead of just opening h5 and re-init weights, need to also account for
+                # cases like with 3D dataset returns which use self.n_particles (segs per iter)
+                # perhaps I can just reinit the entire set of attrs
+                #self.h5 = h5
+                #self.__init__(self)
+                
+                # TODO: maybe this could go into a _particle_init method?
+                # for now just going to save a new self.n_particles attribute
+                self.n_particles = self.h5["summary"]["n_particles"]
+                # these may not be needed, 
+                self.current_particles = np.sum(self.h5["summary"]["n_particles"][self.first_iter-1:self.last_iter])
+                # do not include the final (empty) iteration
+                self.total_particles = np.sum(self.h5["summary"]["n_particles"][:-1])
 
             # scale weights by n h5 files
             self.weights /= len(self.h5_list)
 
             # TODO: need a better way to always return XYZ (currently using ones)
             #       this is needed for easy testing with uniform XYZ 3 array returns
             #       but maybe a different test strategy would also work
@@ -1224,25 +1482,32 @@
                     x, y, z = self.instant_pdist_2d()
                 else:
                     x, y = self.instant_pdist_1d()
                     z = np.ones((self.first_iter, self.last_iter))
             elif self.data_type == "average":
                 # attemts to say, if not None, but has to be compatible with str and arrays
                 if isinstance(self.Yname, (str, np.ndarray)) and isinstance(self.Zname, (str, np.ndarray)):
-                    x, y, z = self.average_datasets_3d()
+                    # for 4d plots
+                    if isinstance(self.Cname, (str, np.ndarray)):
+                        x, y, z, c = self.average_datasets_4d()
+                    else:
+                        x, y, z = self.average_datasets_3d()
                 elif isinstance(self.Yname, (str, np.ndarray)):
                     x, y, z = self.average_pdist_2d()
                 else:
                     x, y = self.average_pdist_1d()
                     z = np.ones((self.first_iter, self.last_iter))
         
             # append to master lists
             Xs.append(x)
             Ys.append(y)
             Zs.append(z)
+            # optional C
+            if 'c' in locals():
+                Cs.append(c)
 
         # selectively normalize final probabilities (sometimes Y and sometimes Z)
         # no normalization needed with 3D data returns (Zname) for 3D scatter plots
         if self.data_type == "evolution" or self.Yname is not None and self.Zname is None:
             # for XY, just use the first file array
             X = Xs[0]
             Y = Ys[0]
@@ -1261,16 +1526,28 @@
         else:
             # for 3d data returns for scatter3d, stack list of XYZs
             X = np.concatenate(Xs)
             Y = np.concatenate(Ys)
             Z = np.concatenate(Zs)
 
         # safely close h5 file
-        self.h5.close()
-        return X, Y, Z
+        # TODO: not doing this since methods e.g. for tracing need access to h5 file
+        #self.h5.close()
 
-#if __name__ == "__main__":
+        # for optional Cname 4D returns
+        if isinstance(self.Cname, (str, np.ndarray)):
+            C = np.concatenate(Cs)
+            return X, Y, Z, C
+        else:
+            return X, Y, Z
+
+if __name__ == "__main__":
     # total_array_out = np.loadtxt("p53_X_array.txt")
     # original_array = np.loadtxt("p53_X_array_noreshape.txt")
-    
-    # h5 = H5_Pdist("data/p53.h5", data_type="evolution")
-    # TODO: test Zname with data_array
+    # TODO: test Zname with data_array
+
+    #h5pd = H5_Pdist("wedap/data/nacl.h5", data_type="evolution")
+    #print(h5pd.w_succ())
+    #h5pd.succ_pdist_weight_filter()
+
+    h5pd = H5_Pdist("wedap/data/nacl.h5", data_type="average")
+    print(h5pd.get_full_coords((10,1), "pcoord").shape)
```

### Comparing `wedap-0.0.9/wedap/h5_plot.py` & `wedap-1.0.0/wedap/h5_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,50 +5,73 @@
 * line -- plot 1D lines.
 * hist -- plot histogram (default).
 * hist_l -- plot histogram and contour lines.
 * contour -- plot contour levels and lines.
 * contour_f -- plot contour levels
 * contour_l -- plot contour lines only.
 * scatter3d -- plot 3 datasets in a scatter plot.
+* hexbin3d -- plot 3 datasets in a hexbin plot.
 
 maybe a ridgeline plot?
 - This would be maybe for 1D avg of every 100 iterations
 - https://matplotlib.org/matplotblog/posts/create-ridgeplots-in-matplotlib/
 Option to overlay different datasets, could be done easily with python but maybe a cli option?                
 
-TODO: plot clustering centroids option?
-      can then grab the search_aux at the centroid
-
 TODO: bin visualizer? and maybe show the trajectories as just dots?
-Add postprocess function for quick fixes when using CLI? see feplotter
 """
 
 import sys
 import numpy as np
 import matplotlib.pyplot as plt
-import scipy.ndimage
 from warnings import warn
 from numpy import inf
+import importlib
 
 from .h5_pdist import *
 
 # TODO: maybe put the pdist object into the plot class and have this object be flexible
 # so it could just be a pdist.h5 file from westpa or make your own
 # or read in a pdist.h5 and create pdist object using that dataset
 
 class H5_Plot(H5_Pdist):
     """
     These methods provide various plotting options for pdist data.
+
+    Attributes
+    ----------
+    cbar_pad : float
+        Default 0.05, can update this attribute to change cbar padding.
     """
+    cbar_pad = 0.05
     def __init__(self, X=None, Y=None, Z=None, plot_mode="hist", cmap=None, smoothing_level=None,
         color=None, ax=None, p_min=None, p_max=None, contour_interval=1, contour_levels=None,
-        cbar_label=None, cax=None, jointplot=False, data_label=None, proj3d=False, 
-        *args, **kwargs):
+        cbar_label=None, cax=None, jointplot=False, data_label=None, proj3d=False, proj4d=False, 
+        C=None, scatter_interval=10, scatter_s=1, hexbin_grid=100, linewidth=None, linestyle="-",
+        postprocess_func=None, *args, **kwargs):
         """
         Plotting of pdists generated from H5 datasets.
+        
+        After instantiating this class, input args are all saved as instance attributes.
+        
+        These can then be updated if needed. Note that if the X, Y, and Z input arrays are 
+        not provided, they will be generated using the parent H5_Pdist class using super()
+        and initializing with the input *args and **kwargs lists. So you can input the same
+        args to be passed to H5_Pdist such as `h5`, `data_type`, `Xname`, `Yname`, `Xindex`, etc.
+        The raw data arrays being used by H5_Plot and generated by H5_Pdist can be accessed as
+        updated instance attributes (self.X, self.Y, self.Z).
+
+        Alternatively the X, Y, and Z arrays can be generated in a separate line by H5_Pdist 
+        and then passed to H5_Plot.
+        ``` Python
+        X, Y, Z = H5_Pdist(**kwargs).pdist()
+        H5_Plot(X, Y, Z, **kwargs).plot()
+        ```
+
+        The main method you will call is the H5_Plot.plot() method, which will update the 
+        self.ax and self.fig instance attributes with the desired plotting options specified.
 
         Parameters
         ----------
         X, Y : arrays
             x and y axis values, and if using aux_y or evolution (with only aux_x), also must input Z.
         Z : 2darray
             Z is a 2-D matrix of the normalized histogram values.
@@ -74,14 +97,34 @@
         cax : MPL axes object
             Optionally define axes object to place colorbar.
         jointplot : bool
             Whether or not to include marginal plots. Note to use this argument, 
             probabilities for Z or from H5_Pdist must be in `raw` p_units.
         data_label : str
             Optionally label the data, e.g. for multiple 1D plots.
+        proj3d : bool
+            Optionally use a 3d projection plot, defaut False.
+            Only works with contour and scatter plots.
+        proj4d : bool
+            Optionally use a 4d projection plot, defaut False.
+            Only works with scatter plots.
+        C : array
+            For color mapping of 3d projection plots.
+        scatter_interval : int
+            Interval for displaying scatter plot data, default 1.
+        scatter_s : float
+            Int for displaying scatter plot data marker size, default 1.
+        hexbin_grid : int
+            Determines gridsize for hexbin plots.
+        linewidth : float
+            Linewidth for 1D plots, contour lines, and hexbin edges.
+        linestyle : str
+            Linestyle for 1D plots, contour lines, and hexbin edges.
+        postprocess_func : func
+            User function to import.
         ** args
         ** kwargs
         """
         # include the init args for H5_Pdist
         # TODO: how to make some of the args optional if I want to use classes seperately?
         #super().__init__(*args, **kwargs)
 
@@ -89,33 +132,37 @@
         self.smoothing_level = smoothing_level
         self.jointplot = jointplot
 
         # TODO: option if you want to generate pdist
         # also need option of just using the input X Y Z args
         # or getting them from w_pdist h5 file, or from H5_Pdist output file
         # user inputs XYZ
-        if X is None and Y is None and Z is None:
+        if X is None and Y is None and Z is None and C is None:
             super().__init__(*args, **kwargs)
             # save the user requested p_units and changes p_units to raw
             if self.jointplot:
                 # will be re-normed later on
                 X, Y, Z = self.pdist(normalize=False)
+            # when requesting a projection plot with 4d cbar additional dataset
+            elif proj4d:
+                X, Y, Z, C = self.pdist()
             else:
                 # TODO: tuple unpacking to deal with variable item return
                 X, Y, Z = self.pdist()
         # need to set this when using mdap, shouldn't affect anything else
         # since joint plot dists must be changed from raw to requested p_units
         if self.jointplot and "p_units" in kwargs:
             self.requested_p_units = kwargs["p_units"]
         else:
             self.requested_p_units = "kT"
 
         self.X = X
         self.Y = Y
         self.Z = Z
+        self.C = C
 
         self.p_min = p_min
         self.p_max = p_max
         self.contour_interval = contour_interval
         self.contour_levels = contour_levels
 
         self.plot_mode = plot_mode
@@ -127,32 +174,39 @@
         if cbar_label is None:
             self.cbar_label = ""
 
         # if no p_units are there then no label is fine
         # otherwise check if p_units are there
         if hasattr(self, "p_units"):
             if self.p_units == "kT":
-                self.cbar_label = "$-\ln\,P(x)$"
+                self.cbar_label = r"$-\ln\,P(x)$"
                 #self.cbar_label = "-ln (P(x))"
             elif self.p_units == "kcal":
-                self.cbar_label = "$-RT\ \ln\, P\ (kcal\ mol^{-1})$"
+                self.cbar_label = r"$-RT\ \ln\, P\ (kcal\ mol^{-1})$"
             elif self.p_units == "raw":
                 self.cbar_label = "Counts"
             elif self.p_units == "raw_norm":
                 self.cbar_label = "Normalized Counts"
         # if using 3 datasets, put blank name as default cbar
-        if self.plot_mode == "scatter3d":
+        if self.plot_mode == "scatter3d" or self.plot_mode == "hexbin3d":
             self.cbar_label = ""
         # overwrite and apply cbar_label attr if available/specified
         if cbar_label:
             self.cbar_label = cbar_label
 
         self.cax = cax
         self.data_label = data_label
         self.proj3d = proj3d
+        self.proj4d = proj4d
+        self.scatter_interval = scatter_interval
+        self.scatter_s = scatter_s
+        self.hexbin_grid = hexbin_grid
+        self.linewidth = linewidth
+        self.linestyle = linestyle
+        self.postprocess_func = postprocess_func
         self.kwargs = kwargs
 
     # TODO: load from w_pdist, also can add method to load from wedap pdist output
     # def _load_from_pdist_file(self):
     #     '''
     #     Load data from a w_pdist output file. This includes bin boundaries. 
     #     '''
@@ -181,26 +235,28 @@
     #     self.axis_list = self._get_bins_from_expr(self.args.pdist_axes)
     #     self.H         = self._sum_except_along(histogram, self.axis_list) 
 
     #     # Make sure that the axis ordering is correct.
     #     if self.axis_list[0] > self.axis_list[1]:
     #         self.H = self.H.transpose()
 
-    def add_cbar(self, cax=None):
+    def add_cbar(self, cax=None, pad=0.05):
         """
         Add cbar.
 
         Parameters
         ----------
         cax : mpl cbar axis
             Optionally specify the cbar axis.
+        pad : float
+            cbar padding level.
         """
         # fig vs plt should be the same, tests run fine (needed to go plt for mosaic)
         #cbar = self.fig.colorbar(self.plot, cax=cax)
-        cbar = plt.colorbar(self.plot_obj, cax=cax)
+        cbar = plt.colorbar(self.plot_obj, cax=cax, pad=pad)
         # if contour lines are present
         if hasattr(self, "lines"):
             cbar.add_lines(self.lines)
 
         # TODO: move labelpad here to style?
         cbar.set_label(self.cbar_label, labelpad=14)
 
@@ -240,18 +296,22 @@
     def plot_contour_l(self):
         """
         2d contour plot, lines.
         """
         Warning("contour_l lines are set to mpl defaults, set can be changed with `--color` or `--cmap`")
         # can control linewidths using rc params (lines.linewidths (default 1.5))
         if self.color:
-            self.lines = self.ax.contour(self.X, self.Y, self.Z, levels=self.contour_levels, colors=self.color)
+            self.lines = self.ax.contour(self.X, self.Y, self.Z, levels=self.contour_levels, 
+                                         colors=self.color, linewidths=self.linewidth, linestyles=self.linestyle)
             #self.lines = self.ax.contour(self.X, self.Y, self.Z, levels=[5], colors=self.color)
         else:
-            self.lines = self.ax.contour(self.X, self.Y, self.Z, levels=self.contour_levels, cmap=self.cmap)
+            self.lines = self.ax.contour(self.X, self.Y, self.Z, levels=self.contour_levels, 
+                                         cmap=self.cmap, linewidths=self.linewidth, linestyles=self.linestyle)
+        # set to call both lines and cbar plot_obj
+        self.plot_obj = self.lines
 
     def plot_contour_f(self):
         """
         2d contour plot, fill.
         """
         self.plot_obj = self.ax.contourf(self.X, self.Y, self.Z, levels=self.contour_levels, cmap=self.cmap)
 
@@ -266,48 +326,90 @@
     def plot_line(self):
         """
         1d line plot.
         """
         # 1D data
         if self.p_max:
             self.Y[self.Y > self.p_max] = inf
-        self.ax.plot(self.X, self.Y, color=self.color, label=self.data_label)
+        self.ax.plot(self.X, self.Y, color=self.color, label=self.data_label, 
+                     linewidth=self.linewidth, linestyle=self.linestyle)
         self.ax.set_ylabel(self.cbar_label)
     
     def plot_scatter3d(self, interval=10, s=1):
         """
         3d scatter plot.
 
         Parameters
         ----------
         interval : int
             Interval to consider the XYZ datasets, increase to use less data.
         s : float
             mpl scatter marker size.
         """
-        if self.proj3d:
+        if self.proj3d or self.proj4d:
+            if isinstance(self.C, np.ndarray):
+                C = self.C[::interval]
+            else:
+                C = self.Z[::interval]
             self.plot_obj = self.ax.scatter(self.X[::interval], 
                                             self.Y[::interval], 
                                             self.Z[::interval],
-                                            c=self.Z[::interval],
+                                            c=C,
                                             cmap=self.cmap, s=s,
                                             vmin=self.p_min, vmax=self.p_max)
         else:
             self.plot_obj = self.ax.scatter(self.X[::interval], 
                                             self.Y[::interval], 
                                             c=self.Z[::interval], 
                                             cmap=self.cmap, s=s,
                                             vmin=self.p_min, vmax=self.p_max)
 
-    def plot_hexbin3d(self):
+    def plot_hexbin3d(self, gridsize=100):
         """
-        Hexbin plot?
+        Hexbin plot.
         """
         # TODO: test this and add grid?
-        self.plot_obj = self.ax.hexbin(self.X, self.Y, C=self.Z,
+        # reshape to 1D and then get rid of extra dimension
+        self.X = np.squeeze(self.X.reshape(1, -1))
+        self.Y = np.squeeze(self.Y.reshape(1, -1))
+        # self.Z = np.squeeze(self.Z.reshape(1, -1))
+        
+        # if weighted attr is passed as False, don't weight hexbins
+        try:
+            if self.weighted is False:
+                reduce_C_function = np.mean
+                Zindices = self.Z
+            else:
+                # for building a weighted C
+                flat_weights = np.concatenate([sub_array.flatten() for sub_array in self.weights])
+                full_flat_weights = np.repeat(flat_weights, repeats=self.Z.shape[1])
+                self.Z = np.squeeze(self.Z.reshape(1, -1))
+                Z_and_weights = np.vstack((self.Z, full_flat_weights)).T
+                Zindices = list(range(len(self.X)))
+                #print(Z_and_weights.shape)
+
+                def reduce_C_function(C):
+                    '''
+                    Custom C function to account for weights in hexbins.
+                    In this case, C is the Zindices.
+                    '''
+                    # when I have a zeroed weight h5 e.g. from succ_only, this doesn't work
+                    # need an extra checking step here (for all zero weights)
+                    try:
+                        return np.average(Z_and_weights[C, 0], weights=Z_and_weights[C, 1])
+                    except ZeroDivisionError:
+                        return np.nan
+        # account for when self.weighted does not exist (TODO: this is only for MDAP, can probably separate it out)
+        except AttributeError:
+            pass
+
+        #print(self.X.shape, self.Y.shape, self.Z.shape)
+        self.plot_obj = self.ax.hexbin(self.X, self.Y, C=Zindices, gridsize=gridsize, 
+                                       edgecolors=self.color, reduce_C_function=reduce_C_function,
+                                       linewidths=self.linewidth, linestyles=self.linestyle,
                                        cmap=self.cmap, vmin=self.p_min, vmax=self.p_max)
 
     def plot_margins(self):
         """
         Joint plot of heatmap (pcolormesh).
         Must input raw probabilities from H5_Pdist(p_units = 'raw').
         """
@@ -330,52 +432,177 @@
         # TODO: put all in ax.set()?
         #for key, item in self.plot_options.items():
         for key, item in self.kwargs.items():
             if key == "xlabel" and item:
                 self.ax.set_xlabel(item)
             if key == "ylabel" and item:
                 self.ax.set_ylabel(item)
+            if key == "zlabel" and item:
+                self.ax.set_zlabel(item)
             if key == "xlim" and item:
                 self.ax.set_xlim(item)
                 if self.jointplot:
                     self.fig["x"].set_xlim(item)
             if key == "ylim"and item:
                 self.ax.set_ylim(item)
                 if self.jointplot:
                     self.fig["y"].set_ylim(item)
             if key == "title" and item:
                 self.ax.set_title(item)
             if key == "suptitle" and item:
                 plt.suptitle(item)
+            # if key == "style" and item:
+            #     plt.style.use(item)
             if key == "grid" and item:
                 self.ax.grid(item, alpha=0.5)
                 if self.jointplot:
                     # grid the margins
                     for ax in ["x", "y"]:
                         self.fig[ax].grid(item, alpha=0.5)
             if key == "minima" and item: # TODO: this is essentially bstate, also put maxima?
                 # reorient transposed hist matrix
                 Z = np.rot90(np.flip(self.Z, axis=0), k=3)
                 # get minima coordinates index (inverse maxima since min = 0)
                 maxima = np.where(1 / Z ==  np.amax(1 / Z, axis=(0, 1)))
                 # plot point at x and y bin midpoints that correspond to mimima
                 self.ax.plot(self.X[maxima[0]], self.Y[maxima[1]], 'ko')
                 print(f"Minima: ({self.X[maxima[0]][0]}, {self.Y[maxima[1]][0]})")
+            
+            # now allowing for a list of line inputs
+            if key == "axvline" and item:
+                # make into list if not already
+                if not isinstance(item, list):
+                    item = [item]
+                # loop each list item and plot line
+                for line in item:
+                    self.ax.axvline(line, color=self.color, linewidth=self.linewidth, linestyle=self.linestyle)
+            if key == "axhline" and item:
+                # make into list if not already
+                if not isinstance(item, list):
+                    item = [item]
+                # loop each list item and plot line
+                for line in item:
+                    self.ax.axhline(line, color=self.color, linewidth=self.linewidth, linestyle=self.linestyle)
+
+    def _run_postprocessing(self):
+        """
+        Run the user-specified postprocessing function.
+        """
+        # Parse the user-specifed string for the module and class/function name.
+        module_name, attr_name = self.postprocess_func.split('.', 1) 
+        # import the module ``module_name`` and make the function/class 
+        # accessible as ``attr``.
+        #attr = getattr(importlib.import_module(module_name), attr_name) 
+        attr = getattr(self.load_module(module_name, '.'), attr_name)
+        # Call ``attr``.
+        attr()
+
+    @staticmethod
+    def load_module(module_name, path=None):
+        """Load and return the given module, recursively loading containing packages as necessary."""
+        if module_name in sys.modules:
+            return sys.modules[module_name]
+
+        if path is None:
+            return importlib.import_module(module_name)
+
+        spec_components = list(reversed(module_name.split('.')))
+        qname_components = []
+        mod_chain = []
+        while spec_components:
+            next_component = spec_components.pop(-1)
+            qname_components.append(next_component)
+
+            try:
+                parent = mod_chain[-1]
+                path = parent.__path__
+            except IndexError:
+                parent = None
+
+            qname = '.'.join(qname_components)
+
+            if qname in sys.modules:
+                module = sys.modules[qname]
+            else:
+                spec = importlib.machinery.PathFinder().find_spec(qname, path)
+
+                if spec is None:
+                    raise ImportError(f'No module named {qname}')
+
+                module = importlib.util.module_from_spec(spec)
+
+                if spec.name not in sys.modules:
+                    sys.modules[spec.name] = module
+
+                spec.loader.exec_module(module)
+
+                # Make the module appear in the parent module's namespace
+                if parent:
+                    setattr(parent, next_component, module)
+
+            mod_chain.append(module)
+
+        return module
+
+    @staticmethod
+    def gaussian_filter(data, sigma):
+        """
+        Apply Gaussian smoothing to a 2D array.
+
+        Parameters
+        ----------
+        data : ndarray 
+            Input 2D array.
+        sigma : float 
+            Standard deviation of the Gaussian filter.
+
+        Returns
+        -------
+        ndarray
+            Smoothed 2D array.
+        """
+        # Create a Gaussian filter kernel
+        size = int(2 * np.ceil(3 * sigma) + 1)
+        kernel = np.fromfunction(lambda x, y: (1/(2*np.pi*sigma**2)) * 
+                                 np.exp(-((x - size//2)**2 + (y - size//2)**2)/(2*sigma**2)), 
+                                 (size, size))
+
+        # Normalize the kernel
+        kernel /= np.sum(kernel)
+
+        # Determine padding size
+        pad_width = size // 2
+
+        # Pad the input data array
+        padded_data = np.pad(data, pad_width, mode='constant')
+
+        # Convolve the padded data with the Gaussian kernel
+        smoothed_data = np.zeros_like(data)
+        for i in range(data.shape[0]):
+            for j in range(data.shape[1]):
+                smoothed_data[i, j] = np.sum(padded_data[i:i+size, j:j+size] * kernel)
+
+        return smoothed_data
 
     # TODO: cbar issues with 1d plots
     def plot(self, cbar=True):
         """
         Main public method.
         Master plotting run function
         Parse plot type and add cbars/tightlayout/plot_options/smoothing
 
         Parameters
         ----------
         cbar : bool
             Whether or not to include a colorbar.
+        
+        Returns
+        -------
+        self.fig, self.ax : mpl figure and axes objects
+            Generates, updates, and returns figure and axes objects.
         """
         # special settings for joint plots
         if self.jointplot:
             # can't use custom ax objects with jointplot, must create new fig and ax using mosaic
             if self.ax:
                 message = "Can't use custom mpl axes objects with jointplot option, " + \
                           "creating new fig and ax using mpl subplot_mosaic."
@@ -414,40 +641,38 @@
             self.fig["x"].set_xticklabels([])
             self.fig["y"].set_yticklabels([])
             # put pmax as lims on margin plots
             self.fig["x"].set_ylim(self.p_min, self.p_max)
             self.fig["y"].set_xlim(self.p_min, self.p_max)
 
         # 3dprojection test, not going to be compatible with jp
-        elif self.proj3d:
+        elif self.proj3d or self.proj4d:
             self.fig = plt.figure()
             self.ax = self.fig.add_subplot(projection='3d')
-            # don't need cbar since 3d projected
-            cbar = False
-            # but add cbar label to z axis
-            self.ax.set_zlabel(self.cbar_label)
+            # don't need 4d cbar when 3d projected
+            if self.proj3d:
+                cbar = False
+                # but add cbar label to z axis
+                self.ax.set_zlabel(self.cbar_label)
+            # elif self.proj4d:
+            #     self.ax.set_zlabel(self.cbar_label)
 
         else:
             if self.ax is None:
                 self.fig, self.ax = plt.subplots()
             else:
                 self.fig = plt.gcf()
 
         # smooth the data if specified
         if self.smoothing_level:
             # make into a smooth style e.g. contour with 0 as base instead of negative or inf
             #self.Z = np.ma.masked_invalid(self.Z)
             self.Z[self.Z < 0] = 0
             self.Z[self.Z == np.inf] = 0
-            self.Z = scipy.ndimage.gaussian_filter(self.Z, sigma=self.smoothing_level)
-            #self.Z[self.Z == 0] = np.inf
-            # get rid of any negatives --> 0
-            #self.Z[self.Z < 0] = np.inf
-            #self.Z[self.Z == np.inf] = 0
-            #self.Z[self.Z < 0] = 0
+            self.Z = self.gaussian_filter(self.Z, sigma=self.smoothing_level)
 
         # get contour levels if needed
         if self.plot_mode in ["contour", "contour_l", "contour_f", "hist_l"]:
             self._get_contour_levels()
 
         if self.plot_mode == "contour":
             self.plot_contour_l()
@@ -477,33 +702,60 @@
             Warning("'bar' plot_mode is still under development")
 
         elif self.plot_mode == "line":
             self.plot_line()
             #self.ax.set_ylabel(self.cbar_label)
 
         elif self.plot_mode == "scatter3d":
-            self.plot_scatter3d()
+            self.plot_scatter3d(interval=self.scatter_interval, s=self.scatter_s)
 
         elif self.plot_mode == "hexbin3d":
-            self.plot_hexbin3d()
+            self.plot_hexbin3d(gridsize=self.hexbin_grid)
 
         # error if unknown plot_mode
         else:
             raise ValueError(f"plot_mode = '{self.plot_mode}' is not valid.")
 
         # TODO: can this work with non H5_Pdist input?
         # if self.Xname == "pcoord":
         #     self.ax.set_xlabel(f"Progress Coordinate {self.Xindex}")
         # if self.Yname == "pcoord":
         #     self.ax.set_ylabel(f"Progress Coordinate {self.Yindex}")
 
         # don't add cbar if not specified or if using a 1D plot
-        if cbar and self.plot_mode not in ["line", "bar", "contour_l"]:
-            self.add_cbar(cax=self.cax)
+        if cbar and self.plot_mode not in ["line", "bar"]:
+            self.add_cbar(cax=self.cax, pad=self.cbar_pad)
 
         # take kwargs and unpack to look for plot option items
         if self.kwargs is not None:
             self._unpack_plot_options()
 
+        # optionally run post processing function
+        # commented out, likely if you're using the API, no need for postproc
+        # only gets called during CLI/GUI use
+        # if self.postprocess_func is not None:
+        #     self._run_postprocessing()
+
         # fig vs plt shouldn't matter here (needed to go plt for mosaic)
         #self.fig.tight_layout()
         plt.tight_layout()
+
+        return self.fig, self.ax
+
+if __name__ == "__main__":
+    # testing of postprocess function
+    import types
+    x = types.SimpleNamespace()
+    import os
+    print(os.getcwd())
+    x.postprocess_func = "postprocess_test.adjust_plot"
+    #H5_Plot._run_postprocessing(x)
+
+    #import importlib
+    # # Parse the user-specifed string for the module and class/function name.
+    # module_name, attr_name = x.postprocess_func.split('.', 1) 
+    # # import the module ``module_name`` and make the function/class 
+    # # accessible as ``attr``.
+    # attr = getattr(importlib.import_module(module_name), attr_name) 
+    # # Call ``attr``.
+    # attr()
+
```

### Comparing `wedap-0.0.9/wedap/tests/test_h5_pdist.py` & `wedap-1.0.0/wedap/tests/test_h5_pdist.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,14 +41,31 @@
         # Y data is just the WE iterations
         np.testing.assert_allclose(Y, 
             np.arange(evolution.first_iter, evolution.last_iter + 1, 1))
 
         # Z data is the pdist values of each iteration
         np.testing.assert_allclose(Z, np.loadtxt(f"wedap/tests/data/evolution_{Xname}_Z.txt"))
 
+    # this repeat test is needed since I want to test both pcoord vs aux and multiple indices
+    @pytest.mark.parametrize("Xname", ["pcoord"])
+    @pytest.mark.parametrize("Xindex", [0, 1])
+    def test_evolution_idx(self, Xname, Xindex):
+        evolution = wedap.H5_Pdist(h5=self.h5, data_type="evolution", Xname=Xname, Xindex=Xindex)
+        X, Y, Z = evolution.pdist()
+
+        # X data is the variably filled array of instance pdist x values
+        np.testing.assert_allclose(X, np.loadtxt(f"wedap/tests/data/evolution_{Xname}{Xindex}_X.txt"))
+
+        # Y data is just the WE iterations
+        np.testing.assert_allclose(Y, 
+            np.arange(evolution.first_iter, evolution.last_iter + 1, 1))
+
+        # Z data is the pdist values of each iteration
+        np.testing.assert_allclose(Z, np.loadtxt(f"wedap/tests/data/evolution_{Xname}{Xindex}_Z.txt"))
+
     @pytest.mark.parametrize("Xname", ["pcoord", "dihedral_2"])
     def test_instant_1d(self, Xname):
         X, Y, Z = wedap.H5_Pdist(h5=self.h5, data_type="instant", Xname=Xname).pdist()
         np.testing.assert_allclose(X, np.loadtxt(f"wedap/tests/data/instant_{Xname}_X.txt"))
         np.testing.assert_allclose(Y, np.loadtxt(f"wedap/tests/data/instant_{Xname}_Y.txt"))
         
     @pytest.mark.parametrize("Xname", ["pcoord", "dihedral_2"])
@@ -57,16 +74,30 @@
         X, Y, Z = wedap.H5_Pdist(h5=self.h5, data_type="instant", Xname=Xname, Yname=Yname).pdist()
         np.testing.assert_allclose(X, 
             np.loadtxt(f"wedap/tests/data/instant_{Xname}_{Yname}_X.txt"))
         np.testing.assert_allclose(Y, 
             np.loadtxt(f"wedap/tests/data/instant_{Xname}_{Yname}_Y.txt"))
         np.testing.assert_allclose(Z, 
             np.loadtxt(f"wedap/tests/data/instant_{Xname}_{Yname}_Z.txt"))
+
+    @pytest.mark.parametrize("Xname", ["pcoord"])
+    #@pytest.mark.parametrize("Yname", ["dihedral_3", "pcoord"])
+    @pytest.mark.parametrize("Yname", ["dihedral_3"])
+    @pytest.mark.parametrize("Xindex", [0, 1])
+    def test_instant_2d_idx(self, Xname, Yname, Xindex):
+        X, Y, Z = wedap.H5_Pdist(h5=self.h5, data_type="instant", Xindex=Xindex,
+                                 Xname=Xname, Yname=Yname).pdist()
+        np.testing.assert_allclose(X, 
+            np.loadtxt(f"wedap/tests/data/instant_{Xname}{Xindex}_{Yname}_X.txt"))
+        np.testing.assert_allclose(Y, 
+            np.loadtxt(f"wedap/tests/data/instant_{Xname}{Xindex}_{Yname}_Y.txt"))
+        np.testing.assert_allclose(Z, 
+            np.loadtxt(f"wedap/tests/data/instant_{Xname}{Xindex}_{Yname}_Z.txt"))
     
-    # TODO along with average (but this is kinda taken care of in H5_Plot scatter3d tests)
+    # TODO along with average 3D (but this is kinda taken care of in H5_Plot scatter3d tests)
     # def test_instant_3d(self):
     #     X, Y, Z = wedap.H5_Pdist(h5=self.h5, data_type="instant", Xname=Xname, Yname=Yname).pdist()
     #     np.testing.assert_allclose(X, 
     #         np.loadtxt(f"wedap/data/instant_{Xname}_{Yname}_X.txt"))
     #     np.testing.assert_allclose(Y, 
     #         np.loadtxt(f"wedap/data/instant_{Xname}_{Yname}_Y.txt"))
     #     np.testing.assert_allclose(Z, 
@@ -84,7 +115,21 @@
         X, Y, Z = wedap.H5_Pdist(h5=self.h5, data_type="average", Xname=Xname, Yname=Yname).pdist()
         np.testing.assert_allclose(X, 
             np.loadtxt(f"wedap/tests/data/average_{Xname}_{Yname}_X.txt"))
         np.testing.assert_allclose(Y, 
             np.loadtxt(f"wedap/tests/data/average_{Xname}_{Yname}_Y.txt"))
         np.testing.assert_allclose(Z, 
             np.loadtxt(f"wedap/tests/data/average_{Xname}_{Yname}_Z.txt"))
+        
+    #@pytest.mark.parametrize("Xname", ["dihedral_3", "pcoord"])
+    @pytest.mark.parametrize("Xname", ["dihedral_3"])
+    @pytest.mark.parametrize("Yname", ["pcoord"])
+    @pytest.mark.parametrize("Yindex", [0, 1])
+    def test_average_2d_idx(self, Xname, Yname, Yindex):
+        X, Y, Z = wedap.H5_Pdist(h5=self.h5, data_type="average", Yindex=Yindex,
+                                 Xname=Xname, Yname=Yname).pdist()
+        np.testing.assert_allclose(X, 
+            np.loadtxt(f"wedap/tests/data/average_{Xname}_{Yname}{Yindex}_X.txt"))
+        np.testing.assert_allclose(Y, 
+            np.loadtxt(f"wedap/tests/data/average_{Xname}_{Yname}{Yindex}_Y.txt"))
+        np.testing.assert_allclose(Z, 
+            np.loadtxt(f"wedap/tests/data/average_{Xname}_{Yname}{Yindex}_Z.txt"))
```

### Comparing `wedap-0.0.9/wedap.egg-info/PKG-INFO` & `wedap-1.0.0/wedap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 0.0.9
-Summary: weighted ensemble data analysis and plotting
+Version: 1.0.0
+Summary: Weighted Ensemble Data Analysis and Plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
         All rights reserved.
@@ -41,60 +41,61 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: h5py
-Requires-Dist: scipy
 Requires-Dist: gif
 Requires-Dist: tqdm
 
 <p align="left">
-    <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap.jpeg?raw=true" alt="wedap logo" width="400">
+    <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap_logo.png?raw=true" alt="wedap logo" width="400">
 </p>
 
 ![tests](https://github.com/darianyang/wedap/actions/workflows/tests.yml/badge.svg)
 [![docs](https://img.shields.io/website?label=docs&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdarianyang.github.io%2Fwedap%2Fdocs%2Fhtml%2Findex.html)](https://darianyang.github.io/wedap/docs/html/index.html)
 [![PyPI version](https://badge.fury.io/py/wedap.svg)](https://badge.fury.io/py/wedap)
 [![Downloads](https://static.pepy.tech/badge/wedap)](https://pepy.tech/project/wedap)
 [![GitHub license](https://img.shields.io/github/license/darianyang/wedap)](https://github.com/darianyang/wedap/blob/master/LICENSE)
 
-**wedap** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
+**WEDAP** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
 
 `wedap` is primarily used to plot H5 files produced from running [WESTPA](https://github.com/westpa/westpa).
 
 `mdap` can be used to plot data files from analysis of standard MD simulations.
 
+`wekap` can be used to plot flux values as rates from a WESTPA created direct.h5 file. 
+
 For a demo and summary of features, see this [jupyter notebook](docs/notebook/wedap_demo.ipynb).
 
 Or view the same demo notebook on the [documentation web page](https://darianyang.github.io/wedap/docs/html/notebook/wedap_demo.html).
 
 ### Requirements
 
 - numpy
 - matplotlib
 - h5py
-- scipy
 - tqdm
+- gif
 
 ### Optional
 
 - gif (optional for making gifs)
 - gooey (optional for GUI)
 
 ## Installation
 
 If you don't need the GUI, then installing `Gooey` is not required and you can just pip install.
 ``` bash
 pip install wedap
 ```
 Otherwise you can install with `Gooey`, e.g. into a new conda env:
 ``` bash
-conda env create --name wedap python=3.8+
+conda env create --name wedap python=3.10+
 conda activate wedap
 conda install -c conda-forge gooey
 pip install wedap
 ```
 Or update an existing environmnent:
 ``` bash
 conda activate ENV_NAME
@@ -102,23 +103,30 @@
 pip install wedap
 ```
 
 Note that `Gooey` is kindof troublesome to pip install in some systems, which is also why it's not included in the requirements (although it is required for the GUI). For now, I recommend conda installing `Gooey`.
 
 ## GUI
 
-`wedap` has a GUI built using [Gooey](https://github.com/chriskiehl/Gooey) which can be launched by running `wedap` or `python wedap` if you're in the main `wedap` directory of this repository. If you're using MacOSX, you'll need to run `pythonw wedap` in the main directory since conda prevents wxPython from accessing the display on Mac. 
+`wedap` has a GUI built using [Gooey](https://github.com/chriskiehl/Gooey) which can be launched from the command line by simply running 
+``` bash
+wedap
+```
+or 
+`python wedap` if you're in the main `wedap` directory of this repository. 
+
+
+If you're using MacOSX, you'll need to run `pythonw wedap` in the main directory since conda prevents wxPython from accessing the display on Mac. 
 If you pip install (instead of conda installing) `wxPython` and `Gooey` on Mac you may be able to just run `wedap`. 
-If you wish to use the command line interface instead include any amount of arguments and include `-h` or `--help` to see the available options.
 
 For MacOSX, you can set up an alias in your `.bash_profile` by running the following:
-```
+``` bash
 echo "alias wedap=pythonw /Path/to/wedap/git/repo/wedap/wedap" >> ~/.bash_profile
 ```
-Then simply type `wedap` on the terminal to run the wedap GUI.
+Then simply type `wedap` in the terminal to run the wedap GUI.
 
 ## Examples
 
 After installation, to run the CLI version and view available options:
 ``` bash
 wedap --help
 ```
```

### Comparing `wedap-0.0.9/wedap.egg-info/SOURCES.txt` & `wedap-1.0.0/wedap.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,28 +3,43 @@
 setup.py
 mdap/__init__.py
 mdap/__main__.py
 mdap/command_line.py
 mdap/md_pdist.py
 mdap/md_plot.py
 mdap/styles/__init__.py
+mdap/styles/default.mplstyle
 mdap/tests/__init__.py
 mdap/tests/make_md_pdist_test_data.py
 mdap/tests/test_md_pdist.py
 styles/__init__.py
 wedap/__init__.py
 wedap/__main__.py
 wedap/command_line.py
+wedap/h5_gif.py
 wedap/h5_pdist.py
 wedap/h5_plot.py
 wedap.egg-info/PKG-INFO
 wedap.egg-info/SOURCES.txt
 wedap.egg-info/dependency_links.txt
 wedap.egg-info/entry_points.txt
 wedap.egg-info/requires.txt
 wedap.egg-info/top_level.txt
 wedap/styles/__init__.py
 wedap/styles/default.mplstyle
 wedap/tests/__init__.py
+wedap/tests/make_h5_pdist_test_data.py
 wedap/tests/make_h5_plot_test_data.py
 wedap/tests/test_h5_pdist.py
-wedap/tests/test_h5_plot.py
+wedap/tests/test_h5_plot.py
+wekap/__init__.py
+wekap/__main__.py
+wekap/bootstrap.py
+wekap/command_line.py
+wekap/kinetics.py
+wekap/data/__init__.py
+wekap/data/ppf.py
+wekap/error/GetAvg_CR.py
+wekap/error/__init__.py
+wekap/error/bootstrap.py
+wekap/styles/__init__.py
+wekap/styles/default.mplstyle
```

