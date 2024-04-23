# Comparing `tmp/rydiqule-1.2.1.tar.gz` & `tmp/rydiqule-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rydiqule-1.2.1.tar", last modified: Tue Jan 23 16:15:43 2024, max compression
+gzip compressed data, was "rydiqule-1.2.2.tar", last modified: Tue Apr 23 20:26:30 2024, max compression
```

## Comparing `rydiqule-1.2.1.tar` & `rydiqule-1.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.046339 rydiqule-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-01-23 16:15:32.000000 rydiqule-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-01-23 16:15:43.046339 rydiqule-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-01-23 16:15:32.000000 rydiqule-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-23 16:15:32.000000 rydiqule-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-23 16:15:43.046339 rydiqule-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-23 16:15:32.000000 rydiqule-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.034339 rydiqule-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.038339 rydiqule-1.2.1/src/rydiqule/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/atom_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38909 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    15472 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/doppler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/rydiqule_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    93027 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/sensor_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/sensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.038339 rydiqule-1.2.1/src/rydiqule/slicing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/slicing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/slicing/slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.042339 rydiqule-1.2.1/src/rydiqule/stack_solvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/stack_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/stack_solvers/cyrk_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/stack_solvers/nbkode_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/stack_solvers/nbrk_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/stack_solvers/scipy_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    20031 2024-01-23 16:15:32.000000 rydiqule-1.2.1/src/rydiqule/timesolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.042339 rydiqule-1.2.1/src/rydiqule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-01-23 16:15:43.000000 rydiqule-1.2.1/src/rydiqule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-01-23 16:15:43.000000 rydiqule-1.2.1/src/rydiqule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 16:15:43.000000 rydiqule-1.2.1/src/rydiqule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 16:15:42.000000 rydiqule-1.2.1/src/rydiqule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-23 16:15:43.000000 rydiqule-1.2.1/src/rydiqule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-23 16:15:43.000000 rydiqule-1.2.1/src/rydiqule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:15:43.042339 rydiqule-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_EOMs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_calculate_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_detuning_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_level_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_numbakitode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_parameter_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_steady_state_ham_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_time_cyrk.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_time_ham_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-01-23 16:15:32.000000 rydiqule-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.024459 rydiqule-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-23 20:26:22.000000 rydiqule-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-23 20:26:30.024459 rydiqule-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-23 20:26:22.000000 rydiqule-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 20:26:22.000000 rydiqule-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 20:26:30.024459 rydiqule-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 20:26:22.000000 rydiqule-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.012458 rydiqule-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.016459 rydiqule-1.2.2/src/rydiqule/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/atom_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38909 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15472 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/doppler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/rydiqule_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93027 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/sensor_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/sensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.020459 rydiqule-1.2.2/src/rydiqule/slicing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/slicing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/slicing/slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12418 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.020459 rydiqule-1.2.2/src/rydiqule/stack_solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/stack_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/stack_solvers/cyrk_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/stack_solvers/nbkode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/stack_solvers/nbrk_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/stack_solvers/scipy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20031 2024-04-23 20:26:22.000000 rydiqule-1.2.2/src/rydiqule/timesolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.020459 rydiqule-1.2.2/src/rydiqule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-23 20:26:30.000000 rydiqule-1.2.2/src/rydiqule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-23 20:26:30.000000 rydiqule-1.2.2/src/rydiqule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:26:30.000000 rydiqule-1.2.2/src/rydiqule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:26:29.000000 rydiqule-1.2.2/src/rydiqule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 20:26:30.000000 rydiqule-1.2.2/src/rydiqule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 20:26:30.000000 rydiqule-1.2.2/src/rydiqule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:26:30.020459 rydiqule-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_EOMs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_calculate_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_detuning_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_level_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_numbakitode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_parameter_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_steady_state_ham_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_time_cyrk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_time_ham_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 20:26:22.000000 rydiqule-1.2.2/tests/test_utils.py
```

### Comparing `rydiqule-1.2.1/LICENSE` & `rydiqule-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/PKG-INFO` & `rydiqule-1.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rydiqule
-Version: 1.2.1
+Version: 1.2.2
 Summary: Rydberg Sensor Interactive Quantum Physics Module
 Author: ARL and NAWCWD
 License: Apache
 Keywords: rydberg,atomic-physics,quantum-optics,atomic-sensors,electrometry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -58,64 +58,76 @@
 B. N Miller, D. H. Meyer, T. Virtanen, C. M O'Brien, and K. C. Cox,
 RydIQule: A Graph-based paradigm for modeling Rydberg and atomic sensors,
 *Computer Physics Communications*, **294**, 108952 (2024)
 [https://doi.org/10.1016/j.cpc.2023.108952](https://doi.org/10.1016/j.cpc.2023.108952)
 
 ## Installation
 
-Presently, installation is done via pip.
+Installation is done via pip or conda.
 See below for detailed instructions.
 
 In all cases, it is highly recommended to install rydiqule in a virtual environment.
 
-### Conda/pip installation
+### Conda installation (recommended)
 
-If using a conda to provide the virtual environmnet,
-it can often be advantageous to install as many packages as possible via conda before running the pip installation command.
+Installation via conda is recommended for rydiqule.
+It handles dependency installation as well as a virtual environment to ensure packages do not conflict with other usages on the same system.
+Finally, the `numpy` provided by anaconda has been compiled against optimized BLAS/LAPACK implementations, which results in much better performance in rydiqule itself.
 
 Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
 ```shell
-(base) ~/> conda create -n rydiqule python=3.9
+(base) ~/> conda create -n rydiqule python=3.11
 (base) ~/> conda activate rydiqule
 ```
 RydIQule currently requires python >3.8.
+For a new installation, it is recommended to use the newest supported python.
 
-Now install dependencies that are available via conda.
-To capture as many dependencies as possible,
-we will add the `conda-forge` channel at a lower priority.
-```shell
-(rydiqule) ~/> conda config --env --append channels conda-forge
-(rydiqule) ~/> conda config --set channel_priority strict
-(rydiqule) ~/> conda install numpy scipy matplotlib networkx numba psutil
-# ARC specific dependencies available via conda
-(rydiqule) ~/> conda install sympy asteval lmfit uncertainties
-```
-
-Now use pip to install rydiqule and remaining dependencies.
-```shell
-# for normal installation
-(rydiqule) ~/> pip install rydiqule
-# for editable installation of cloned repo, so source can be modified locally
+Now install via rydiqule's anaconda channel.
+This channel provides rydiqule as well as its dependencies that are not available in the default anaconda channel.
+If one of these dependencies is outdated, please raise an issue with the [vendoring repository](https://github.com/QTC-UMD/rydiqule-vendored-conda-builds).
+```shell
+(rydiqule) ~/> conda install -c rydiqule rydiqule
+```
+
+If you would like to install rydiqule in editable mode to locally modify its source,
+this must be done using pip.
+Follow the above to install rydiqule and its dependencies,
+then run the following to uninstall rydiqule as provided by conda
+and install the editable local repository.
+```shell
+(rydiqule) ~/> conda remove rydiqule --force
+# following must be run from root of local repository
 (rydiqule) ~/> pip install -e .
 ```
 
+Note that editable installations require `git`.
+This can be provided by a system-wide installation or via conda in the virtual environment (`conda install git`).
+
+While rydiqule is a pure python package (ie it is platform independent), its core dependency ARC is not.
+If a pre-built package of ARC is not available for your platform in our anaconda channel,
+you will need to install ARC via `pip` to build it locally before installing `rydiqule`.
+To see what architectures are supported, please see the [vendoring repository](https://github.com/QTC-UMD/rydiqule-vendored-conda-builds).
+
+
 ### Pure pip installation
 
 To install normally, run:
 ```shell
 pip install rydiqule
 ```
 This command will use pip to install all necessary dependencies.
 
 To install in an editable way (which allows edits of the source code),
 run the following from the root directory of the cloned repository:
 ```shell
 pip install -e .
 ```
 
+Editable installation requires `git` to be installed.
+
 ### Confirm installation
 
 Proper installation can be confirmed by executing the following commands in a python terminal.
 ```shell
 >>> import rydiqule as rq
 >>> rq.about()
 
@@ -138,15 +150,22 @@
 CPU Count:            12
 Total System Memory:  128 GB
 ```
 
 ### Updating an existing installation
 
 Upgrading an existing installation is simple.
-Simply run the pip installation commands described above.
+Simply run the appropriate upgrade command for the installation method used.
+
+For conda installations, run the following command to upgrade rydiqule
+```shell
+conda upgrade rydiqule
+```
+
+For `pip`, you can use the installation command to upgrade.
 Optionally, include the update flag to greedily update dependencies as well.
 ```shell
 pip install -U rydiqule
 ```
 This command will also install any new dependencies that are required.
 
 If using an editable install, simply replacing the files in the same directory is sufficient.
@@ -155,30 +174,35 @@
 pip install -U -e .
 ```
 
 ### Dependencies
 
 This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
 It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
-These dependencies will be automatically installed by pip if not already present.
+These dependencies will be automatically installed if not already present.
 
 Rydiqule's performance does depend on these depedencies.
 In particular, `numpy` can be compiled with a variety of backends that implements
 BLAS and LAPACK routines that can have different performance for different computer architectures.
 When using Windows, it is recommended to install `numpy` from conda,
 which is built against the IntelMKL and has generally shown the best performance for Intel-based PCs.
 
 Optional timesolver backend dependencies include the [numbakit-ode](https://github.com/hgrecco/numbakit-ode)
 and [CyRK](https://github.com/jrenaud90/CyRK) packages.
-Both are available via `pip`.
+Both are available via `pip` or our anaconda channel.
 They can be installed automatically via the optional extras specification for the `pip` command.
 ```shell
 pip install rydiqule[backends]
 ```
 
+For conda installations, these dependencies must be installed manually.
+```shell
+conda install -c rydiqule CyRK numbakit-ode
+```
+
 ## Documentation
 
 Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
 PDF or EPUB formats of the documentation can be downloaded from the online documentation.
 
 ### Examples
```

### Comparing `rydiqule-1.2.1/README.md` & `rydiqule-1.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,64 +14,76 @@
 B. N Miller, D. H. Meyer, T. Virtanen, C. M O'Brien, and K. C. Cox,
 RydIQule: A Graph-based paradigm for modeling Rydberg and atomic sensors,
 *Computer Physics Communications*, **294**, 108952 (2024)
 [https://doi.org/10.1016/j.cpc.2023.108952](https://doi.org/10.1016/j.cpc.2023.108952)
 
 ## Installation
 
-Presently, installation is done via pip.
+Installation is done via pip or conda.
 See below for detailed instructions.
 
 In all cases, it is highly recommended to install rydiqule in a virtual environment.
 
-### Conda/pip installation
+### Conda installation (recommended)
 
-If using a conda to provide the virtual environmnet,
-it can often be advantageous to install as many packages as possible via conda before running the pip installation command.
+Installation via conda is recommended for rydiqule.
+It handles dependency installation as well as a virtual environment to ensure packages do not conflict with other usages on the same system.
+Finally, the `numpy` provided by anaconda has been compiled against optimized BLAS/LAPACK implementations, which results in much better performance in rydiqule itself.
 
 Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
 ```shell
-(base) ~/> conda create -n rydiqule python=3.9
+(base) ~/> conda create -n rydiqule python=3.11
 (base) ~/> conda activate rydiqule
 ```
 RydIQule currently requires python >3.8.
+For a new installation, it is recommended to use the newest supported python.
 
-Now install dependencies that are available via conda.
-To capture as many dependencies as possible,
-we will add the `conda-forge` channel at a lower priority.
-```shell
-(rydiqule) ~/> conda config --env --append channels conda-forge
-(rydiqule) ~/> conda config --set channel_priority strict
-(rydiqule) ~/> conda install numpy scipy matplotlib networkx numba psutil
-# ARC specific dependencies available via conda
-(rydiqule) ~/> conda install sympy asteval lmfit uncertainties
-```
-
-Now use pip to install rydiqule and remaining dependencies.
-```shell
-# for normal installation
-(rydiqule) ~/> pip install rydiqule
-# for editable installation of cloned repo, so source can be modified locally
+Now install via rydiqule's anaconda channel.
+This channel provides rydiqule as well as its dependencies that are not available in the default anaconda channel.
+If one of these dependencies is outdated, please raise an issue with the [vendoring repository](https://github.com/QTC-UMD/rydiqule-vendored-conda-builds).
+```shell
+(rydiqule) ~/> conda install -c rydiqule rydiqule
+```
+
+If you would like to install rydiqule in editable mode to locally modify its source,
+this must be done using pip.
+Follow the above to install rydiqule and its dependencies,
+then run the following to uninstall rydiqule as provided by conda
+and install the editable local repository.
+```shell
+(rydiqule) ~/> conda remove rydiqule --force
+# following must be run from root of local repository
 (rydiqule) ~/> pip install -e .
 ```
 
+Note that editable installations require `git`.
+This can be provided by a system-wide installation or via conda in the virtual environment (`conda install git`).
+
+While rydiqule is a pure python package (ie it is platform independent), its core dependency ARC is not.
+If a pre-built package of ARC is not available for your platform in our anaconda channel,
+you will need to install ARC via `pip` to build it locally before installing `rydiqule`.
+To see what architectures are supported, please see the [vendoring repository](https://github.com/QTC-UMD/rydiqule-vendored-conda-builds).
+
+
 ### Pure pip installation
 
 To install normally, run:
 ```shell
 pip install rydiqule
 ```
 This command will use pip to install all necessary dependencies.
 
 To install in an editable way (which allows edits of the source code),
 run the following from the root directory of the cloned repository:
 ```shell
 pip install -e .
 ```
 
+Editable installation requires `git` to be installed.
+
 ### Confirm installation
 
 Proper installation can be confirmed by executing the following commands in a python terminal.
 ```shell
 >>> import rydiqule as rq
 >>> rq.about()
 
@@ -94,15 +106,22 @@
 CPU Count:            12
 Total System Memory:  128 GB
 ```
 
 ### Updating an existing installation
 
 Upgrading an existing installation is simple.
-Simply run the pip installation commands described above.
+Simply run the appropriate upgrade command for the installation method used.
+
+For conda installations, run the following command to upgrade rydiqule
+```shell
+conda upgrade rydiqule
+```
+
+For `pip`, you can use the installation command to upgrade.
 Optionally, include the update flag to greedily update dependencies as well.
 ```shell
 pip install -U rydiqule
 ```
 This command will also install any new dependencies that are required.
 
 If using an editable install, simply replacing the files in the same directory is sufficient.
@@ -111,30 +130,35 @@
 pip install -U -e .
 ```
 
 ### Dependencies
 
 This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
 It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
-These dependencies will be automatically installed by pip if not already present.
+These dependencies will be automatically installed if not already present.
 
 Rydiqule's performance does depend on these depedencies.
 In particular, `numpy` can be compiled with a variety of backends that implements
 BLAS and LAPACK routines that can have different performance for different computer architectures.
 When using Windows, it is recommended to install `numpy` from conda,
 which is built against the IntelMKL and has generally shown the best performance for Intel-based PCs.
 
 Optional timesolver backend dependencies include the [numbakit-ode](https://github.com/hgrecco/numbakit-ode)
 and [CyRK](https://github.com/jrenaud90/CyRK) packages.
-Both are available via `pip`.
+Both are available via `pip` or our anaconda channel.
 They can be installed automatically via the optional extras specification for the `pip` command.
 ```shell
 pip install rydiqule[backends]
 ```
 
+For conda installations, these dependencies must be installed manually.
+```shell
+conda install -c rydiqule CyRK numbakit-ode
+```
+
 ## Documentation
 
 Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
 PDF or EPUB formats of the documentation can be downloaded from the online documentation.
 
 ### Examples
```

### Comparing `rydiqule-1.2.1/setup.cfg` & `rydiqule-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/__init__.py` & `rydiqule-1.2.2/src/rydiqule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from .solvers import solve_steady_state
 from .timesolvers import solve_time, solve_eom_stack, generate_eom_time
 from .doppler_utils import get_doppler_equations, generate_doppler_shift_eom, doppler_classes, doppler_mesh, apply_doppler_weights
 from .rydiqule_utils import about
 
 from .slicing.slicing import compute_grid, matrix_slice, memory_size, get_slice_num, get_slice_num_t
 
-__version__ = '1.2.1'
+__version__ = '1.2.2'
```

### Comparing `rydiqule-1.2.1/src/rydiqule/atom_utils.py` & `rydiqule-1.2.2/src/rydiqule/atom_utils.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/cell.py` & `rydiqule-1.2.2/src/rydiqule/cell.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/doppler_utils.py` & `rydiqule-1.2.2/src/rydiqule/doppler_utils.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/experiments.py` & `rydiqule-1.2.2/src/rydiqule/experiments.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/rydiqule_utils.py` & `rydiqule-1.2.2/src/rydiqule/rydiqule_utils.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/sensor.py` & `rydiqule-1.2.2/src/rydiqule/sensor.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/sensor_solution.py` & `rydiqule-1.2.2/src/rydiqule/sensor_solution.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/sensor_utils.py` & `rydiqule-1.2.2/src/rydiqule/sensor_utils.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/slicing/slicing.py` & `rydiqule-1.2.2/src/rydiqule/slicing/slicing.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/solvers.py` & `rydiqule-1.2.2/src/rydiqule/solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,17 +172,17 @@
         
     # get steady-state hamiltonians
     hamiltonians = sensor.get_hamiltonian()
     # add t=0 time-dependent parts of hamiltonian
     hamiltonians_time_r, hamiltonians_time_i = sensor.get_time_couplings()
     time_functions = sensor.get_time_dependence()
     hamiltonians_time = np.zeros_like(hamiltonians_time_i)
-    for func, htr, hti in zip(time_functions, hamiltonians_time_r, hamiltonians_time_i):
+    for i, (func, htr, hti) in enumerate(zip(time_functions, hamiltonians_time_r, hamiltonians_time_i)):
         f0 = func(0)
-        hamiltonians_time += f0.real*htr + f0.imag*hti
+        hamiltonians_time[i] += f0.real*htr + f0.imag*hti
     hamiltonians_total = hamiltonians + np.sum(hamiltonians_time, axis=0)
     # get decoherence matrix
     gamma = sensor.decoherence_matrix()
     # allocate solution array
     sols = np.zeros(out_sol_shape)
     
     # loop over individual slices of hamiltonian
```

### Comparing `rydiqule-1.2.1/src/rydiqule/stack_solvers/cyrk_solver.py` & `rydiqule-1.2.2/src/rydiqule/stack_solvers/cyrk_solver.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/stack_solvers/nbkode_solver.py` & `rydiqule-1.2.2/src/rydiqule/stack_solvers/nbkode_solver.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/stack_solvers/nbrk_solver.py` & `rydiqule-1.2.2/src/rydiqule/stack_solvers/nbrk_solver.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/stack_solvers/scipy_solver.py` & `rydiqule-1.2.2/src/rydiqule/stack_solvers/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule/timesolvers.py` & `rydiqule-1.2.2/src/rydiqule/timesolvers.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/src/rydiqule.egg-info/PKG-INFO` & `rydiqule-1.2.2/src/rydiqule.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rydiqule
-Version: 1.2.1
+Version: 1.2.2
 Summary: Rydberg Sensor Interactive Quantum Physics Module
 Author: ARL and NAWCWD
 License: Apache
 Keywords: rydberg,atomic-physics,quantum-optics,atomic-sensors,electrometry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -58,64 +58,76 @@
 B. N Miller, D. H. Meyer, T. Virtanen, C. M O'Brien, and K. C. Cox,
 RydIQule: A Graph-based paradigm for modeling Rydberg and atomic sensors,
 *Computer Physics Communications*, **294**, 108952 (2024)
 [https://doi.org/10.1016/j.cpc.2023.108952](https://doi.org/10.1016/j.cpc.2023.108952)
 
 ## Installation
 
-Presently, installation is done via pip.
+Installation is done via pip or conda.
 See below for detailed instructions.
 
 In all cases, it is highly recommended to install rydiqule in a virtual environment.
 
-### Conda/pip installation
+### Conda installation (recommended)
 
-If using a conda to provide the virtual environmnet,
-it can often be advantageous to install as many packages as possible via conda before running the pip installation command.
+Installation via conda is recommended for rydiqule.
+It handles dependency installation as well as a virtual environment to ensure packages do not conflict with other usages on the same system.
+Finally, the `numpy` provided by anaconda has been compiled against optimized BLAS/LAPACK implementations, which results in much better performance in rydiqule itself.
 
 Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
 ```shell
-(base) ~/> conda create -n rydiqule python=3.9
+(base) ~/> conda create -n rydiqule python=3.11
 (base) ~/> conda activate rydiqule
 ```
 RydIQule currently requires python >3.8.
+For a new installation, it is recommended to use the newest supported python.
 
-Now install dependencies that are available via conda.
-To capture as many dependencies as possible,
-we will add the `conda-forge` channel at a lower priority.
-```shell
-(rydiqule) ~/> conda config --env --append channels conda-forge
-(rydiqule) ~/> conda config --set channel_priority strict
-(rydiqule) ~/> conda install numpy scipy matplotlib networkx numba psutil
-# ARC specific dependencies available via conda
-(rydiqule) ~/> conda install sympy asteval lmfit uncertainties
-```
-
-Now use pip to install rydiqule and remaining dependencies.
-```shell
-# for normal installation
-(rydiqule) ~/> pip install rydiqule
-# for editable installation of cloned repo, so source can be modified locally
+Now install via rydiqule's anaconda channel.
+This channel provides rydiqule as well as its dependencies that are not available in the default anaconda channel.
+If one of these dependencies is outdated, please raise an issue with the [vendoring repository](https://github.com/QTC-UMD/rydiqule-vendored-conda-builds).
+```shell
+(rydiqule) ~/> conda install -c rydiqule rydiqule
+```
+
+If you would like to install rydiqule in editable mode to locally modify its source,
+this must be done using pip.
+Follow the above to install rydiqule and its dependencies,
+then run the following to uninstall rydiqule as provided by conda
+and install the editable local repository.
+```shell
+(rydiqule) ~/> conda remove rydiqule --force
+# following must be run from root of local repository
 (rydiqule) ~/> pip install -e .
 ```
 
+Note that editable installations require `git`.
+This can be provided by a system-wide installation or via conda in the virtual environment (`conda install git`).
+
+While rydiqule is a pure python package (ie it is platform independent), its core dependency ARC is not.
+If a pre-built package of ARC is not available for your platform in our anaconda channel,
+you will need to install ARC via `pip` to build it locally before installing `rydiqule`.
+To see what architectures are supported, please see the [vendoring repository](https://github.com/QTC-UMD/rydiqule-vendored-conda-builds).
+
+
 ### Pure pip installation
 
 To install normally, run:
 ```shell
 pip install rydiqule
 ```
 This command will use pip to install all necessary dependencies.
 
 To install in an editable way (which allows edits of the source code),
 run the following from the root directory of the cloned repository:
 ```shell
 pip install -e .
 ```
 
+Editable installation requires `git` to be installed.
+
 ### Confirm installation
 
 Proper installation can be confirmed by executing the following commands in a python terminal.
 ```shell
 >>> import rydiqule as rq
 >>> rq.about()
 
@@ -138,15 +150,22 @@
 CPU Count:            12
 Total System Memory:  128 GB
 ```
 
 ### Updating an existing installation
 
 Upgrading an existing installation is simple.
-Simply run the pip installation commands described above.
+Simply run the appropriate upgrade command for the installation method used.
+
+For conda installations, run the following command to upgrade rydiqule
+```shell
+conda upgrade rydiqule
+```
+
+For `pip`, you can use the installation command to upgrade.
 Optionally, include the update flag to greedily update dependencies as well.
 ```shell
 pip install -U rydiqule
 ```
 This command will also install any new dependencies that are required.
 
 If using an editable install, simply replacing the files in the same directory is sufficient.
@@ -155,30 +174,35 @@
 pip install -U -e .
 ```
 
 ### Dependencies
 
 This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
 It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
-These dependencies will be automatically installed by pip if not already present.
+These dependencies will be automatically installed if not already present.
 
 Rydiqule's performance does depend on these depedencies.
 In particular, `numpy` can be compiled with a variety of backends that implements
 BLAS and LAPACK routines that can have different performance for different computer architectures.
 When using Windows, it is recommended to install `numpy` from conda,
 which is built against the IntelMKL and has generally shown the best performance for Intel-based PCs.
 
 Optional timesolver backend dependencies include the [numbakit-ode](https://github.com/hgrecco/numbakit-ode)
 and [CyRK](https://github.com/jrenaud90/CyRK) packages.
-Both are available via `pip`.
+Both are available via `pip` or our anaconda channel.
 They can be installed automatically via the optional extras specification for the `pip` command.
 ```shell
 pip install rydiqule[backends]
 ```
 
+For conda installations, these dependencies must be installed manually.
+```shell
+conda install -c rydiqule CyRK numbakit-ode
+```
+
 ## Documentation
 
 Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
 PDF or EPUB formats of the documentation can be downloaded from the online documentation.
 
 ### Examples
```

### Comparing `rydiqule-1.2.1/src/rydiqule.egg-info/SOURCES.txt` & `rydiqule-1.2.2/src/rydiqule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_EOMs.py` & `rydiqule-1.2.2/tests/test_EOMs.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_calculate_snr.py` & `rydiqule-1.2.2/tests/test_calculate_snr.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_cell.py` & `rydiqule-1.2.2/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_detuning_sign.py` & `rydiqule-1.2.2/tests/test_detuning_sign.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_experiments.py` & `rydiqule-1.2.2/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_level_diagram.py` & `rydiqule-1.2.2/tests/test_level_diagram.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_numbakitode.py` & `rydiqule-1.2.2/tests/test_numbakitode.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_parameter_zip.py` & `rydiqule-1.2.2/tests/test_parameter_zip.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_sensor.py` & `rydiqule-1.2.2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_solvers.py` & `rydiqule-1.2.2/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_steady_state_ham_gen.py` & `rydiqule-1.2.2/tests/test_steady_state_ham_gen.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_time.py` & `rydiqule-1.2.2/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_time_cyrk.py` & `rydiqule-1.2.2/tests/test_time_cyrk.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_time_ham_gen.py` & `rydiqule-1.2.2/tests/test_time_ham_gen.py`

 * *Files identical despite different names*

### Comparing `rydiqule-1.2.1/tests/test_utils.py` & `rydiqule-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

