# Comparing `tmp/cad_to_openmc-0.3.3.tar.gz` & `tmp/CAD_to_OpenMC-0.3.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cad_to_openmc-0.3.3.tar", last modified: Tue Apr 23 09:08:36 2024, max compression
+gzip compressed data, was "CAD_to_OpenMC-0.3.3a0.tar", last modified: Mon Mar 25 15:43:55 2024, max compression
```

## Comparing `cad_to_openmc-0.3.3.tar` & `CAD_to_OpenMC-0.3.3a0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-04-23 09:08:36.004194 cad_to_openmc-0.3.3/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1071 2022-04-21 08:49:34.000000 cad_to_openmc-0.3.3/LICENSE
--rw-r--r--   0 erkn      (1000) erkn      (1000)    16794 2024-04-23 09:08:36.004194 cad_to_openmc-0.3.3/PKG-INFO
--rw-r--r--   0 erkn      (1000) erkn      (1000)    15949 2024-04-23 09:04:37.000000 cad_to_openmc-0.3.3/README.md
--rw-r--r--   0 erkn      (1000) erkn      (1000)      894 2024-04-23 09:05:09.000000 cad_to_openmc-0.3.3/pyproject.toml
--rw-r--r--   0 erkn      (1000) erkn      (1000)       38 2024-04-23 09:08:36.004194 cad_to_openmc-0.3.3/setup.cfg
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-04-23 09:08:35.996194 cad_to_openmc-0.3.3/src/
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-04-23 09:08:36.000194 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/
--rw-r--r--   0 erkn      (1000) erkn      (1000)      610 2023-06-27 14:52:05.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/__init__.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)    42201 2024-04-23 09:04:37.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assembly.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      903 2023-11-21 09:53:06.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      203 2023-12-13 12:28:29.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_base.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     5550 2023-12-06 00:56:20.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_cq.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     7558 2024-02-26 23:06:01.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_cq2.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     7567 2024-01-30 16:17:19.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_cq3.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     6924 2024-02-26 23:06:01.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_gmsh.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1331 2024-04-23 09:04:37.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/check_step.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     2230 2023-11-21 09:53:06.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/cq_serialize.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      603 2024-02-26 23:06:01.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/datadirectory.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      589 2023-06-27 15:23:32.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/heal_h5m.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     3307 2023-04-17 16:03:40.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/meshutils.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      329 2022-08-23 06:16:29.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/object_factory.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     4131 2023-04-17 16:03:40.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC/stl_utils.py
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-04-23 09:08:36.004194 cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/
--rw-r--r--   0 erkn      (1000) erkn      (1000)    16794 2024-04-23 09:08:35.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/PKG-INFO
--rw-r--r--   0 erkn      (1000) erkn      (1000)      903 2024-04-23 09:08:35.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/SOURCES.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)        1 2024-04-23 09:08:35.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/dependency_links.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)       66 2024-04-23 09:08:35.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/requires.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)       14 2024-04-23 09:08:35.000000 cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/top_level.txt
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-04-23 09:08:36.004194 cad_to_openmc-0.3.3/tests/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     2724 2024-04-23 09:04:37.000000 cad_to_openmc-0.3.3/tests/test_OMC_DAGMC.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1951 2024-04-22 13:47:52.000000 cad_to_openmc-0.3.3/tests/test_OMC_DAGMC_test_msr.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      755 2024-02-26 23:06:01.000000 cad_to_openmc-0.3.3/tests/test_cqstl.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      839 2024-02-26 23:06:01.000000 cad_to_openmc-0.3.3/tests/test_cqstl2.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      527 2024-04-22 12:23:46.000000 cad_to_openmc-0.3.3/tests/test_gmsh.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      958 2024-04-23 09:04:37.000000 cad_to_openmc-0.3.3/tests/test_transform.py
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-03-25 15:43:55.485699 CAD_to_OpenMC-0.3.3a0/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1071 2022-04-21 08:49:34.000000 CAD_to_OpenMC-0.3.3a0/LICENSE
+-rw-r--r--   0 erkn      (1000) erkn      (1000)    16600 2024-03-25 15:43:55.485699 CAD_to_OpenMC-0.3.3a0/PKG-INFO
+-rw-r--r--   0 erkn      (1000) erkn      (1000)    15777 2024-03-25 10:38:54.000000 CAD_to_OpenMC-0.3.3a0/README.md
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      876 2024-03-25 15:40:37.000000 CAD_to_OpenMC-0.3.3a0/pyproject.toml
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       38 2024-03-25 15:43:55.485699 CAD_to_OpenMC-0.3.3a0/setup.cfg
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-03-25 15:43:55.481699 CAD_to_OpenMC-0.3.3a0/src/
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-03-25 15:43:55.485699 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      610 2023-06-27 14:52:05.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/__init__.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)    42246 2024-03-25 10:36:31.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assembly.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      903 2023-11-21 09:53:06.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      203 2023-12-13 12:28:29.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_base.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     5550 2023-12-06 00:56:20.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_cq.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     7558 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_cq2.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     7567 2024-01-30 16:17:19.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_cq3.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     6924 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_gmsh.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1331 2024-03-25 15:37:37.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/check_step.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     2230 2023-11-21 09:53:06.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/cq_serialize.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      603 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/datadirectory.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      589 2023-06-27 15:23:32.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/heal_h5m.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     3307 2023-04-17 16:03:40.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/meshutils.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      329 2022-08-23 06:16:29.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/object_factory.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     4131 2023-04-17 16:03:40.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/stl_utils.py
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-03-25 15:43:55.485699 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)    16600 2024-03-25 15:43:55.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/PKG-INFO
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      903 2024-03-25 15:43:55.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/SOURCES.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)        1 2024-03-25 15:43:55.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/dependency_links.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       57 2024-03-25 15:43:55.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/requires.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       14 2024-03-25 15:43:55.000000 CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/top_level.txt
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2024-03-25 15:43:55.485699 CAD_to_OpenMC-0.3.3a0/tests/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     2714 2024-03-25 15:40:04.000000 CAD_to_OpenMC-0.3.3a0/tests/test_OMC_DAGMC.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1957 2024-02-05 16:32:10.000000 CAD_to_OpenMC-0.3.3a0/tests/test_OMC_DAGMC_test_msr.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      755 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/tests/test_cqstl.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      839 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/tests/test_cqstl2.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      527 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/tests/test_gmsh.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      961 2024-02-26 23:06:01.000000 CAD_to_OpenMC-0.3.3a0/tests/test_transform.py
```

### Comparing `cad_to_openmc-0.3.3/LICENSE` & `CAD_to_OpenMC-0.3.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/PKG-INFO` & `CAD_to_OpenMC-0.3.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CAD_to_OpenMC
-Version: 0.3.3
+Version: 0.3.3a0
 Summary: Package to automagically convert step-geometries to h5m descriptions for neutronics by OpenMC
 Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
 Project-URL: Homepage, https://github.com/openmsr/CAD_to_OpenMC
 Project-URL: Bug Tracker, https://github.com/openmsr/CAD_to_OpenMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,23 +14,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gmsh
 Requires-Dist: pyparsing
 Requires-Dist: cadquery>=2
 Requires-Dist: cadquery-ocp>=7
 Requires-Dist: numpy
-Requires-Dist: networkx
 Requires-Dist: trimesh
 
-|Main | Development|
-|---|---|
-|[![Main branch](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)| [![Development branch](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg?branch=develop)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)|
-
+[![Python application](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)
 ![GitHub License](https://img.shields.io/github/license/openmsr/CAD_to_OpenMC)
-[![Python 3.9](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 
 # CAD_to_OpenMC
 This is a python package intended to establish an open source link between CAD tools in general and the nuetron and photon transport code OpenMC. It is inspired by [Paramak](https://github.com/fusion-energy/paramak), and borrows concepts from [step_to_h5m]( https://github.com/fusion-energy/step_to_h5m).
 
 Although most CAD-tools use some other internal and/or native representation for geometry, most, if not all, will be able to export to the STEP-file format. Therefore this is the format we use
 
 CAD_to_OpenMC uses cadQuery and its links to OCCT
@@ -65,28 +60,29 @@
       sudo python setup.py install
     ```
 4. Install the main package: ```pip install CAD_to_OpenMC```. This will pip-install all the required python packages in the virtual environment. This ensures that no additional conflicts are introduced with the system python.
 
 Should you wish to install the development version of this package you may do so by cloning this repository and replace the last command by: ```pip install <path/to/repo>```. This procedure will build and install the python package locally directly from source.
 
 5. Optionally install the msh refinement tool mmg (https://www.mmgtools.org), which may be run in conjunction with the cq/stl-mesher backend to avoid the high aspect ratio triangles that this backend tends to produce. Arch-linux users may install this from the AUR, otherwise get the source (and build from that) or binary builds from the mmg-site.
-
 # To install in a conda environment
 _replace \<name\> with an arbitrary name for your virtual environment_
 
-If instead you prefer to use a conda-environment, this is now as simple as:
+If instead you prefer to use a conda-environment, this can also be done. There's no native conda-package for CAD_to_OpenMC yet, but we've had good mileage from using pip within a conda-environment. First install conda, mamba, or micromamba.
 1. create an environment, e.g. ```conda create -n <name>```
 2. activate it: ```conda activate <name>```
-3. install CAD_to_OpenMC: ```conda install cad-to-openmc```
+3. install moab (and a supportng library for gmsh) using native conda packaging: ```conda install moab libglu -c conda_forge```
+4. pip-install the main package along with dependencies: ```pip install CAD_to_OpenMC```
+
+This procedure has proven to work quite well, and avoid the bother of building moab from source. The team is working on getting a native conda-package up and running.
 
 # Known problems 
 - At present the parallel meshing option is buggy - it is therefore highly recommended to set the mesher to only use 1 thread. The team is working on a solution for this. See issue [#80](https://github.com/openmsr/CAD_to_OpenMC/issues/80)
 - Geometries which lead to degenerate toroidal surfaces in the step-files, can have problems. See issue [#94](https://github.com/openmsr/CAD_to_OpenMC/issues/94)
-- As is reported in [#98](https://github.com/openmsr/CAD_to_OpenMC/issues/98) on Ubuntu 22.04 there's a problem with python 3.12. Specifically with installing "nlopt", which is used by one of the dependencies of CAD_to_OpenMC. We recommend to stay with python < 3.11 until this has been fixed upstream.
- 
+
 # Use cases
 
 We will show a few very simple uses-cases below to get you started using CAD_to_OpenMC, starting with a simply utility script, and then some more examples showing a few of the options later.
 
 ## Simple utility script
 This is the fastest way of getting up and running. A very basic script to process the file 'geometry.step' into a geometry useful for OpenMC in the 'geometry.h5m':
 ```python
@@ -225,14 +221,15 @@
 Two = ab.Assembly(['two.step])
 Two.run(backend='stl2', merge=True, h5m_filename='two.h5m')
 
 ab.merge2h5m([One,Two],h5m_file='three.h5')
 ```
 This will run the normal triangulization procedure for one and two separately, but also create a single h5m-file: three.h5m which contains both of the geometries.
 
+
 # Advanced example
 For a more advanced example of the use of CAD_to_OpenMC and OpenMC we may turn to the Zero Power Reactor Experiment. This was a full-scale reactor experiment that was carried out at Oak Rodge TN in the 1960's. Copenhagen Atomics provides a CAD-drawn model of this experiment, extracted from the original reports and drawings from the original experiment, in the form of a step-file. To get access simply clone the zpre github repository and run the scripts:
 ```bash
 git clone https://www.github.com/openmsr/zpre
 cd zpre
 bash run.sh
 ```
```

### Comparing `cad_to_openmc-0.3.3/README.md` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,31 @@
-|Main | Development|
-|---|---|
-|[![Main branch](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)| [![Development branch](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg?branch=develop)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)|
+Metadata-Version: 2.1
+Name: CAD_to_OpenMC
+Version: 0.3.3a0
+Summary: Package to automagically convert step-geometries to h5m descriptions for neutronics by OpenMC
+Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
+Project-URL: Homepage, https://github.com/openmsr/CAD_to_OpenMC
+Project-URL: Bug Tracker, https://github.com/openmsr/CAD_to_OpenMC/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gmsh
+Requires-Dist: pyparsing
+Requires-Dist: cadquery>=2
+Requires-Dist: cadquery-ocp>=7
+Requires-Dist: numpy
+Requires-Dist: trimesh
 
+[![Python application](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)
 ![GitHub License](https://img.shields.io/github/license/openmsr/CAD_to_OpenMC)
-[![Python 3.9](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 
 # CAD_to_OpenMC
 This is a python package intended to establish an open source link between CAD tools in general and the nuetron and photon transport code OpenMC. It is inspired by [Paramak](https://github.com/fusion-energy/paramak), and borrows concepts from [step_to_h5m]( https://github.com/fusion-energy/step_to_h5m).
 
 Although most CAD-tools use some other internal and/or native representation for geometry, most, if not all, will be able to export to the STEP-file format. Therefore this is the format we use
 
 CAD_to_OpenMC uses cadQuery and its links to OCCT
@@ -42,28 +60,29 @@
       sudo python setup.py install
     ```
 4. Install the main package: ```pip install CAD_to_OpenMC```. This will pip-install all the required python packages in the virtual environment. This ensures that no additional conflicts are introduced with the system python.
 
 Should you wish to install the development version of this package you may do so by cloning this repository and replace the last command by: ```pip install <path/to/repo>```. This procedure will build and install the python package locally directly from source.
 
 5. Optionally install the msh refinement tool mmg (https://www.mmgtools.org), which may be run in conjunction with the cq/stl-mesher backend to avoid the high aspect ratio triangles that this backend tends to produce. Arch-linux users may install this from the AUR, otherwise get the source (and build from that) or binary builds from the mmg-site.
-
 # To install in a conda environment
 _replace \<name\> with an arbitrary name for your virtual environment_
 
-If instead you prefer to use a conda-environment, this is now as simple as:
+If instead you prefer to use a conda-environment, this can also be done. There's no native conda-package for CAD_to_OpenMC yet, but we've had good mileage from using pip within a conda-environment. First install conda, mamba, or micromamba.
 1. create an environment, e.g. ```conda create -n <name>```
 2. activate it: ```conda activate <name>```
-3. install CAD_to_OpenMC: ```conda install cad-to-openmc```
+3. install moab (and a supportng library for gmsh) using native conda packaging: ```conda install moab libglu -c conda_forge```
+4. pip-install the main package along with dependencies: ```pip install CAD_to_OpenMC```
+
+This procedure has proven to work quite well, and avoid the bother of building moab from source. The team is working on getting a native conda-package up and running.
 
 # Known problems 
 - At present the parallel meshing option is buggy - it is therefore highly recommended to set the mesher to only use 1 thread. The team is working on a solution for this. See issue [#80](https://github.com/openmsr/CAD_to_OpenMC/issues/80)
 - Geometries which lead to degenerate toroidal surfaces in the step-files, can have problems. See issue [#94](https://github.com/openmsr/CAD_to_OpenMC/issues/94)
-- As is reported in [#98](https://github.com/openmsr/CAD_to_OpenMC/issues/98) on Ubuntu 22.04 there's a problem with python 3.12. Specifically with installing "nlopt", which is used by one of the dependencies of CAD_to_OpenMC. We recommend to stay with python < 3.11 until this has been fixed upstream.
- 
+
 # Use cases
 
 We will show a few very simple uses-cases below to get you started using CAD_to_OpenMC, starting with a simply utility script, and then some more examples showing a few of the options later.
 
 ## Simple utility script
 This is the fastest way of getting up and running. A very basic script to process the file 'geometry.step' into a geometry useful for OpenMC in the 'geometry.h5m':
 ```python
@@ -202,14 +221,15 @@
 Two = ab.Assembly(['two.step])
 Two.run(backend='stl2', merge=True, h5m_filename='two.h5m')
 
 ab.merge2h5m([One,Two],h5m_file='three.h5')
 ```
 This will run the normal triangulization procedure for one and two separately, but also create a single h5m-file: three.h5m which contains both of the geometries.
 
+
 # Advanced example
 For a more advanced example of the use of CAD_to_OpenMC and OpenMC we may turn to the Zero Power Reactor Experiment. This was a full-scale reactor experiment that was carried out at Oak Rodge TN in the 1960's. Copenhagen Atomics provides a CAD-drawn model of this experiment, extracted from the original reports and drawings from the original experiment, in the form of a step-file. To get access simply clone the zpre github repository and run the scripts:
 ```bash
 git clone https://www.github.com/openmsr/zpre
 cd zpre
 bash run.sh
 ```
```

### Comparing `cad_to_openmc-0.3.3/pyproject.toml` & `CAD_to_OpenMC-0.3.3a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="CAD_to_OpenMC"
-version="0.3.3"
+version="0.3.3a0"
 authors = [
   { name="Erik B Knudsen", email="erik.knudsen@copenhagenatomics.com" },
 ]
 description = "Package to automagically convert step-geometries to h5m descriptions for neutronics by OpenMC"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -16,15 +16,14 @@
 ]
 dependencies=[
         'gmsh',
         'pyparsing',
         'cadquery>=2',
         'cadquery-ocp>=7',
         'numpy',
-        'networkx',
         'trimesh',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/openmsr/CAD_to_OpenMC"
 "Bug Tracker" = "https://github.com/openmsr/CAD_to_OpenMC/issues"
```

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/__init__.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/__init__.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assembly.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import CAD_to_OpenMC.assemblymesher as am
 from CAD_to_OpenMC.datadirectory import mesher_datadir
 from CAD_to_OpenMC.check_step import has_degenerate_toroids
 
 try:
     import gmsh
+
     nogmsh = False
 except ImportError as e:
     print(f"Warning: import gmsh failed ({e})- material tag-list, must be supplied.")
     nogmsh = True
 
 mesher_config = {
     # general opts
@@ -36,15 +37,15 @@
     "tolerance": 0.1,
     "angular_tolerance": 0.2,
     # gmsh-backend opts
     "min_mesh_size": 0.1,
     "max_mesh_size": 10,
     "curve_samples": 20,
     "mesh_algorithm": 1,
-    "threads": 1,
+    "threads": 4,
     "radial_threshold": 0,
     "refine": 0,
     "verbose": 0,
 }
 
 
 # these are dummies that we still need to have defined
@@ -320,43 +321,44 @@
                                 f"INFO: Tagging volume #{vid} label:{s} with material {tag}"
                             )
                     except Exception as _e:
                         tag = default_tag
                     e.tag = tag
                     tags_set = tags_set + 1
                 gmsh.finalize()
-
-            if tags:
+            elif tags:
                 # tag objects according to the tags dictionary.
                 gmsh.initialize()
                 vols = gmsh.model.occ.importShapes(stp)
                 gmsh.model.occ.synchronize()
                 for e, v in zip(ents, vols):
                     vid = v[1]
-                    s = gmsh.model.getEntityName(3, vid)
-                    part = s.split("/")[-1]
-                    tag = None
-                    for k in tags.keys():
-                        if match_anywhere:
-                            g = re.search(k, part)
-                        else:
-                            g = re.match(k, part)
-                        if g is not None:
-                            tag = tags[k]
-                            break
-                    #if tag is still not set at this point we will either leave it or set it to the default.
-                    if tag is None:
-                        if e.tag is None or self.noextract_tags:
+                    try:
+                        s = gmsh.model.getEntityName(3, vid)
+                        part = s.split("/")[-1]
+                        tag = None
+                        for k in tags.keys():
+                            if match_anywhere:
+                                g = re.search(k, part)
+                            else:
+                                g = re.match(k, part)
+                            if g:
+                                tag = tags[k]
+                                break
+                        if tag is None:
                             tag = self.default_tag
-                    else:
-                        tag = tag
-                    if self.verbose > 1:
-                        print(
-                            f"INFO: Tagging volume #{vid} label:{s} with material {tag}"
-                        )
+                        else:
+                            tags_set = tags_set + 1
+                        if self.verbose > 1:
+                            print(
+                                f"INFO: Tagging volume #{vid} label:{s} with material {tag}"
+                            )
+                    except Exception as _e:
+                        tag = default_tag
+                    e.tag = tag
                 gmsh.finalize()
             elif sequential_tags:
                 for e, t in zip_longest(
                     ents, sequential_tags[tags_set:], fillvalue=self.default_tag
                 ):
                     # Apply tags to the imported volumes in the sequence they get imported.
                     if e == default_tag:
```

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_cq.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_cq.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_cq2.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_cq2.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_cq3.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_cq3.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/assemblymesher_gmsh.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/assemblymesher_gmsh.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/check_step.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/check_step.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/cq_serialize.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/cq_serialize.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/datadirectory.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/datadirectory.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/heal_h5m.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/heal_h5m.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/meshutils.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/meshutils.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC/stl_utils.py` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC/stl_utils.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/PKG-INFO` & `CAD_to_OpenMC-0.3.3a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,9 @@
-Metadata-Version: 2.1
-Name: CAD_to_OpenMC
-Version: 0.3.3
-Summary: Package to automagically convert step-geometries to h5m descriptions for neutronics by OpenMC
-Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
-Project-URL: Homepage, https://github.com/openmsr/CAD_to_OpenMC
-Project-URL: Bug Tracker, https://github.com/openmsr/CAD_to_OpenMC/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: gmsh
-Requires-Dist: pyparsing
-Requires-Dist: cadquery>=2
-Requires-Dist: cadquery-ocp>=7
-Requires-Dist: numpy
-Requires-Dist: networkx
-Requires-Dist: trimesh
-
-|Main | Development|
-|---|---|
-|[![Main branch](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)| [![Development branch](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg?branch=develop)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)|
-
+[![Python application](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)
 ![GitHub License](https://img.shields.io/github/license/openmsr/CAD_to_OpenMC)
-[![Python 3.9](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 
 # CAD_to_OpenMC
 This is a python package intended to establish an open source link between CAD tools in general and the nuetron and photon transport code OpenMC. It is inspired by [Paramak](https://github.com/fusion-energy/paramak), and borrows concepts from [step_to_h5m]( https://github.com/fusion-energy/step_to_h5m).
 
 Although most CAD-tools use some other internal and/or native representation for geometry, most, if not all, will be able to export to the STEP-file format. Therefore this is the format we use
 
 CAD_to_OpenMC uses cadQuery and its links to OCCT
@@ -65,28 +38,29 @@
       sudo python setup.py install
     ```
 4. Install the main package: ```pip install CAD_to_OpenMC```. This will pip-install all the required python packages in the virtual environment. This ensures that no additional conflicts are introduced with the system python.
 
 Should you wish to install the development version of this package you may do so by cloning this repository and replace the last command by: ```pip install <path/to/repo>```. This procedure will build and install the python package locally directly from source.
 
 5. Optionally install the msh refinement tool mmg (https://www.mmgtools.org), which may be run in conjunction with the cq/stl-mesher backend to avoid the high aspect ratio triangles that this backend tends to produce. Arch-linux users may install this from the AUR, otherwise get the source (and build from that) or binary builds from the mmg-site.
-
 # To install in a conda environment
 _replace \<name\> with an arbitrary name for your virtual environment_
 
-If instead you prefer to use a conda-environment, this is now as simple as:
+If instead you prefer to use a conda-environment, this can also be done. There's no native conda-package for CAD_to_OpenMC yet, but we've had good mileage from using pip within a conda-environment. First install conda, mamba, or micromamba.
 1. create an environment, e.g. ```conda create -n <name>```
 2. activate it: ```conda activate <name>```
-3. install CAD_to_OpenMC: ```conda install cad-to-openmc```
+3. install moab (and a supportng library for gmsh) using native conda packaging: ```conda install moab libglu -c conda_forge```
+4. pip-install the main package along with dependencies: ```pip install CAD_to_OpenMC```
+
+This procedure has proven to work quite well, and avoid the bother of building moab from source. The team is working on getting a native conda-package up and running.
 
 # Known problems 
 - At present the parallel meshing option is buggy - it is therefore highly recommended to set the mesher to only use 1 thread. The team is working on a solution for this. See issue [#80](https://github.com/openmsr/CAD_to_OpenMC/issues/80)
 - Geometries which lead to degenerate toroidal surfaces in the step-files, can have problems. See issue [#94](https://github.com/openmsr/CAD_to_OpenMC/issues/94)
-- As is reported in [#98](https://github.com/openmsr/CAD_to_OpenMC/issues/98) on Ubuntu 22.04 there's a problem with python 3.12. Specifically with installing "nlopt", which is used by one of the dependencies of CAD_to_OpenMC. We recommend to stay with python < 3.11 until this has been fixed upstream.
- 
+
 # Use cases
 
 We will show a few very simple uses-cases below to get you started using CAD_to_OpenMC, starting with a simply utility script, and then some more examples showing a few of the options later.
 
 ## Simple utility script
 This is the fastest way of getting up and running. A very basic script to process the file 'geometry.step' into a geometry useful for OpenMC in the 'geometry.h5m':
 ```python
@@ -225,14 +199,15 @@
 Two = ab.Assembly(['two.step])
 Two.run(backend='stl2', merge=True, h5m_filename='two.h5m')
 
 ab.merge2h5m([One,Two],h5m_file='three.h5')
 ```
 This will run the normal triangulization procedure for one and two separately, but also create a single h5m-file: three.h5m which contains both of the geometries.
 
+
 # Advanced example
 For a more advanced example of the use of CAD_to_OpenMC and OpenMC we may turn to the Zero Power Reactor Experiment. This was a full-scale reactor experiment that was carried out at Oak Rodge TN in the 1960's. Copenhagen Atomics provides a CAD-drawn model of this experiment, extracted from the original reports and drawings from the original experiment, in the form of a step-file. To get access simply clone the zpre github repository and run the scripts:
 ```bash
 git clone https://www.github.com/openmsr/zpre
 cd zpre
 bash run.sh
 ```
```

### Comparing `cad_to_openmc-0.3.3/src/CAD_to_OpenMC.egg-info/SOURCES.txt` & `CAD_to_OpenMC-0.3.3a0/src/CAD_to_OpenMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/tests/test_OMC_DAGMC.py` & `CAD_to_OpenMC-0.3.3a0/tests/test_OMC_DAGMC.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,47 +23,47 @@
     self.aa.run(backend='stl2', merge = True, h5m_filename = self.h5m)
     assert self.h5m.exists()
     self.tt.run()
     self.tt.check_results()
     self.tt.cleanup()
     self.cleanup()
 
-#@pytest.mark.skipif(sys.version_info >= (3, 11), reason="requires python3.10 or lower")
+@pytest.mark.skipif(sys.version_info > (3, 10), reason="requires python3.10 or lower")
 def test_h5m_neutronics_p1():
   o = OMC_DAGMC_harness('examples/step_files/pincell1.step')
   openmc.config['cross_sections']=str(o.nuclear_lib)
   o.tt.results={'keff':(0.07944,0.00070)}
   o.run()
 
-#@pytest.mark.skipif(sys.version_info >= (3, 11), reason="requires python3.10 or lower")
+@pytest.mark.skipif(sys.version_info > (3, 10), reason="requires python3.10 or lower")
 def test_h5m_neutronics_p2():
   o = OMC_DAGMC_harness('examples/step_files/pincell2.step')
   openmc.config['cross_sections']=str(o.nuclear_lib)
   o.tt.results={'keff':(0.07786,0.0008)}
   o.run()
 
-#@pytest.mark.skipif(sys.version_info >= (3, 11), reason="requires python3.10 or lower")
+@pytest.mark.skipif(sys.version_info > (3, 10), reason="requires python3.10 or lower")
 def test_h5m_neutronics_tors():
   o = OMC_DAGMC_harness('examples/step_files/toroids.step')
   # override source spatial distribution
   o.tt.settings.source.space=openmc.stats.CylindricalIndependent(
     openmc.stats.Discrete([100,85,77.5],[1.0/3.0,1.0/3.0, 1.0/3.0]), openmc.stats.Uniform(0.0,2.0*math.pi), openmc.stats.Discrete([0.0],[1.0])
   )
   openmc.config['cross_sections']=str(o.nuclear_lib)
   o.tt.results={'keff':(1.61936,0.08562)}
   o.run()
 
-#@pytest.mark.skipif(sys.version_info >= (3, 11), reason="requires python3.10 or lower")
+@pytest.mark.skipif(sys.version_info > (3, 10), reason="requires python3.10 or lower")
 def test_h5m_neutronics_spheroids():
   o = OMC_DAGMC_harness('examples/step_files/spheroids.step')
   openmc.config['cross_sections']=str(o.nuclear_lib)
   o.tt.results={'keff':(1.39082,0.01622)}
   o.run()
 
-#@pytest.mark.skipif(sys.version_info >= (3, 10), reason="requires python3.10 or lower")
+@pytest.mark.skipif(sys.version_info > (3, 10), reason="requires python3.10 or lower")
 def test_h5m_neutronics_ellipsoids():
   o = OMC_DAGMC_harness('examples/step_files/oblate_ellipsoids.step')
   openmc.config['cross_sections']=str(o.nuclear_lib)
   o.tt.results={'keff':(1.05396,0.01514)}
   o.run()
 
 if __name__=='__main__':
```

### Comparing `cad_to_openmc-0.3.3/tests/test_OMC_DAGMC_test_msr.py` & `CAD_to_OpenMC-0.3.3a0/tests/test_OMC_DAGMC_test_msr.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 from tests.OMC_DAGMC_run import DAGMC_template
 from tests.harnessRun import HarnessRun
 
 class msr_DAGMC(DAGMC_template):
     def bld_mats(self):
         uf4 = openmc.Material(name='uf4')
         uf4.set_density('g/cm3', 4.5)
-        uf4.add_nuclide('U231', 1.)
+        uf4.add_element('U', 1., enrichment=5)
         uf4.add_element('F', 4.)
 
         helium = openmc.Material(name='he')
         helium.set_density('g/cm3', 0.001598)
-        helium.add_nuclide('He4', 2.4044e-4)
+        helium.add_element('He', 2.4044e-4)
 
         zircaloy = openmc.Material(name='zr4')
         zircaloy.set_density('g/cm3', 6.55)
-        zircaloy.add_nuclide('Sn114', 0.014, 'wo')
+        zircaloy.add_element('Sn', 0.014, 'wo')
         zircaloy.add_element('Fe', 0.00165, 'wo')
         zircaloy.add_element('Cr', 0.001, 'wo')
         zircaloy.add_element('Zr', 0.98335, 'wo')
 
         water = openmc.Material(name='h2o')
         water.set_density('g/cm3', 1)
         water.add_nuclide('H2', 2)
         water.add_element('O', 1)
         water.add_s_alpha_beta('c_D_in_D2O')
 
         # Define overall material
-        self.materials = openmc.Materials([uf4, helium, zircaloy, water])
+        self.material = openmc.Materials([uf4, helium, zircaloy, water])
 
 class OMC_DAGMC_harness(HarnessRun):
   def __init__(self, step):
     self.path = pathlib.Path(step)
     self.h5m = self.path.with_suffix('.h5m')
     self.nuclear_lib = pathlib.Path('tests/nuclear_data_testlib/cross_sections.xml').absolute()
     self.aa = ab.Assembly([str(self.path)], verbose = 2)
```

### Comparing `cad_to_openmc-0.3.3/tests/test_cqstl.py` & `CAD_to_OpenMC-0.3.3a0/tests/test_cqstl.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/tests/test_cqstl2.py` & `CAD_to_OpenMC-0.3.3a0/tests/test_cqstl2.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/tests/test_gmsh.py` & `CAD_to_OpenMC-0.3.3a0/tests/test_gmsh.py`

 * *Files identical despite different names*

### Comparing `cad_to_openmc-0.3.3/tests/test_transform.py` & `CAD_to_OpenMC-0.3.3a0/tests/test_transform.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import CAD_to_OpenMC.assembly as ab
 from tests.harnessRun import HarnessRun
 import pathlib as pl
 
 class HarnessTrans(HarnessRun):
   def __init__(self):
-    self.infile = 'tests/7pin.step'
+    self.infile = 'examples/7pin.step'
     self.a = ab.Assembly(verbose=2)
 
   def run(self,merge=False, **kwargs):
     self.a.stp_files=[self.infile]
     print(f'stl: {self.a.stp_files})')
     self.a.import_stp_files(**kwargs)
```

