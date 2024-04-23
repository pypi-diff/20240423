# Comparing `tmp/pyiron_potentialfit-0.3.0.tar.gz` & `tmp/pyiron_potentialfit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_potentialfit-0.3.0.tar", last modified: Tue Apr 16 05:40:13 2024, max compression
+gzip compressed data, was "pyiron_potentialfit-0.3.1.tar", last modified: Tue Apr 23 19:21:22 2024, max compression
```

## Comparing `pyiron_potentialfit-0.3.0.tar` & `pyiron_potentialfit-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.435933 pyiron_potentialfit-0.3.0/pyiron_potentialfit/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/atomicrex_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/function_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/general_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/potential_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    33964 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/structure_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
--rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/meamfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/potentialfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/cfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/masters.py
--rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlipdescriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.439934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/storageclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/projectflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 05:40:13.443934 pyiron_potentialfit-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-16 05:40:13.000000 pyiron_potentialfit-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-16 05:40:11.000000 pyiron_potentialfit-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.415804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/atomicrex_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/function_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/general_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/potential_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37753 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/structure_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/trainingcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/meamfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/potentialfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/cfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/masters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlipdescriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/storageclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/projectflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-23 19:21:21.000000 pyiron_potentialfit-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/versioneer.py
```

### Comparing `pyiron_potentialfit-0.3.0/LICENSE` & `pyiron_potentialfit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/PKG-INFO` & `pyiron_potentialfit-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -13,17 +13,18 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: ase>=3.22.1
-Requires-Dist: pyiron_atomistics>=0.5.1
-Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: pyiron_atomistics>=0.5.2
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyiron_base>=0.8.1
-Requires-Dist: scipy>=1.11.4
+Requires-Dist: pyiron_base>=0.8.2
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: runnerase>=0.3.3
-Requires-Dist: seaborn
-Requires-Dist: dill
+Requires-Dist: dill>=0.3.0
+Requires-Dist: seaborn<0.14,>=0.13.0
+Requires-Dist: pyxtal<0.7,>=0.6.0
 
 http://pyiron.org
```

### Comparing `pyiron_potentialfit-0.3.0/README.md` & `pyiron_potentialfit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/__init__.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/base.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/fit_properties.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/fit_properties.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/function_factory.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/function_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/general_input.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/general_input.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/interactive.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/parameter_constraints.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/potential_factory.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/potential_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/structure_list.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/structure_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -401,48 +401,62 @@
         identifiers = self._structures.get_array("identifier")
         if not np.all(np.char.find(identifiers, "/") == -1):
             raise ValueError(
                 "Structure identifiers must not contain '/'. "
                 "Use .structure_file_path to use existing POSCAR files"
             )
 
-    def write_xml_file(self, directory, name="structures.xml"):
+    def write_xml_with_poscars(
+        self,
+        directory,
+        name="structures.xml",
+    ):
         """
-        Internal helper function that writes an atomicrex style
-        xml file containg all structures.
+        Internal helper function that writes an atomicrex structure input
+        with POSCAR format structures. Not recommended normally.
 
         Args:
             directory (string): Working directory.
             name (str, optional): . Defaults to "structures.xml".
         """
         self._check_identifiers()
         self._shrink()
         root = ET.Element("group")
+        ### using poscar format. Not recommended normally.
         if self.structure_file_path is None and "atomic-forces" in self.fit_properties:
             # write POSCARs
             for i in range(self._structures.num_chunks):
                 vec_start = self._structures.start_index[i]
                 vec_end = self._structures.start_index[i] + self._structures.length[i]
                 forces = self.fit_properties["atomic-forces"]._per_element_arrays[
                     "target_val"
                 ][vec_start:vec_end]
                 if not self._structures._per_chunk_arrays["predefined"][i]:
+                    struct_xml = structure_meta_xml(
+                        identifier=self._structures.identifier[i],
+                        forces=forces,
+                        positions=self._structures.positions[vec_start:vec_end],
+                        symbols=self._structures.symbols[vec_start:vec_end],
+                        cell=self._structures.cell[i],
+                        directory=directory,
+                    )
+
                     write_modified_poscar(
                         identifier=self._structures.identifier[i],
                         forces=forces,
                         positions=self._structures.positions[vec_start:vec_end],
                         symbols=self._structures.symbols[vec_start:vec_end],
                         cell=self._structures.cell[i],
                         directory=directory,
                     )
                 # Maybe implement a check for forces when setting up a predefined structure?
                 # else:
                 #    if not np.all(np.isnan(forces)):
 
-        # write xml
+        # write meta xml for poscars
         for i in range(self._structures.num_chunks):
             fit_properties_xml = ET.Element("properties")
             if not self._structures._per_chunk_arrays["predefined"][i]:
                 for prop, flat_prop in self.fit_properties.items():
                     if not prop in ("lattice-parameter", "ca-ratio"):
                         fit_properties_xml.append(flat_prop.to_xml_element(i, prop))
                 struct_xml = structure_meta_xml(
@@ -473,14 +487,79 @@
                     fit_properties=fit_properties_xml,
                     fit=self._structures._per_chunk_arrays["fit"][i],
                 )
             root.append(struct_xml)
         filename = posixpath.join(directory, name)
         write_pretty_xml(root, filename)
 
+    def write_xml_file(self, directory, name="structures.xml", use_poscars=False):
+        """
+        Internal helper function that writes an atomicrex style
+        xml file containg all structures.
+
+        Args:
+            directory (string): Working directory.
+            name (str, optional): Defaults to "structures.xml".
+            use_poscars(bool, optional): whether to use poscars. Not recommneded anymore.
+        """
+        self._check_identifiers()
+        self._shrink()
+        root = ET.Element("group")
+        for i in range(self._structures.num_chunks):
+            fit_properties_xml = ET.Element("properties")
+            if not self._structures._per_chunk_arrays["predefined"][i]:
+                for prop, flat_prop in self.fit_properties.items():
+                    if not prop in ("lattice-parameter", "ca-ratio"):
+                        fit_properties_xml.append(flat_prop.to_xml_element(i, prop))
+
+                vec_start = self._structures.start_index[i]
+                vec_end = self._structures.start_index[i] + self._structures.length[i]
+                forces = self.fit_properties["atomic-forces"]._per_element_arrays[
+                    "target_val"
+                ][vec_start:vec_end]
+
+                struct_xml = user_structure_xml(
+                    identifier=self._structures.identifier[i],
+                    relative_weight=self._structures._per_chunk_arrays[
+                        "relative_weight"
+                    ][i],
+                    pbc=self._structures.pbc[i],
+                    forces=forces,
+                    positions=self._structures.positions[vec_start:vec_end],
+                    symbols=self._structures.symbols[vec_start:vec_end],
+                    cell=self._structures.cell[i],
+                    clamp=self._structures._per_chunk_arrays["clamp"][i],
+                    fit_properties=fit_properties_xml,
+                    fit=self._structures._per_chunk_arrays["fit"][i],
+                )
+
+            else:
+                for prop, flat_prop in self.fit_properties.items():
+                    fit_properties_xml.append(flat_prop.to_xml_element(i, prop))
+
+                data = self._predefined_storage[self._structures.identifier[i]]
+                struct_xml = predefined_structure_xml(
+                    identifier=self._structures.identifier[i],
+                    lattice=data["lattice"],
+                    lattice_param=data["lattice_parameter"],
+                    ca_ratio=data["ca_ratio"],
+                    atom_type_A=data["atom_type_A"],
+                    atom_type_B=data["atom_type_B"],
+                    relative_weight=self._structures._per_chunk_arrays[
+                        "relative_weight"
+                    ][i],
+                    clamp=self._structures._per_chunk_arrays["clamp"][i],
+                    fit_properties=fit_properties_xml,
+                    fit=self._structures._per_chunk_arrays["fit"][i],
+                )
+
+            root.append(struct_xml)
+        filename = posixpath.join(directory, name)
+        write_pretty_xml(root, filename)
+
     def _parse_final_properties(self, struct_lines):
         """
         Internal function that parses the values of fitted properties
         calculated with the final iteration of the fitted potential.
 
         Args:
             struct_lines (list[str]): lines from atomicrex output that contain structure information.
@@ -615,50 +694,14 @@
         return self.get_training_data()
 
     @property
     def predicted_data(self):
         return self.get_predicted_data()
 
 
-### This is probably useless like this in most cases because forces can't be passed.
-def user_structure_to_xml_element(structure):
-    """
-    Converts an ase/pyiron atoms object to an atomicrex xml element
-    Right now forces can't be passed in the xml file, so this is not really helpful.
-    Args:
-        structure (Atoms): ase or pyiron Atoms
-
-    Returns:
-        (ET.Element, ET.Element): atomicrex structure xml
-    """
-    pbc = ET.Element("pbc")
-    pbc.set("x", f"{structure.pbc[0]}".lower())
-    pbc.set("y", f"{structure.pbc[1]}".lower())
-    pbc.set("z", f"{structure.pbc[2]}".lower())
-
-    c = structure.cell
-    cell = ET.Element("cell")
-    for i in range(3):
-        a = ET.SubElement(cell, f"a{i+1}")
-        a.set("x", f"{c[i][0]}")
-        a.set("y", f"{c[i][1]}")
-        a.set("z", f"{c[i][2]}")
-
-    atoms = ET.SubElement(cell, "atoms")
-    for at in structure:
-        a = ET.SubElement(atoms, "atom")
-        a.set("type", at.symbol)
-        a.set("x", f"{at.a}")
-        a.set("y", f"{at.b}")
-        a.set("z", f"{at.c}")
-        a.set("reduced", "false")
-
-    return pbc, cell
-
-
 def write_modified_poscar(
     identifier,
     forces,
     directory,
     structure=None,
     positions=None,
     cell=None,
@@ -737,16 +780,16 @@
 
 
 def structure_meta_xml(
     identifier,
     relative_weight,
     clamp,  ## Not sure if and how this combines with relax in the ARFitParameter sets
     fit_properties,
-    struct_file_path,
-    fit,
+    struct_file_path=None,
+    fit=True,
     mod_poscar=True,
 ):
     """
     Internal function. Creates xml element with
     scalar properties, weight and reference to POSCAR
     containg structure and forces.
 
@@ -774,34 +817,85 @@
 
     if mod_poscar:
         poscar_file = ET.SubElement(struct_xml, "poscar-file")
         if struct_file_path is None:
             poscar_file.text = f"POSCAR_{identifier}"
         else:
             poscar_file.text = f"{struct_file_path}POSCAR_{identifier}"
-    else:
-        #    struct_xml.extend(structure_to_xml_element(structure))
-        raise NotImplementedError(
-            "Only writing structure meta information, \n"
-            "not structure data for now because this is not implemented in atomicrex"
-        )
 
     if not clamp:
         relax_dof = ET.SubElement(struct_xml, "relax-dof")
         atom_coordinates = ET.SubElement(relax_dof, "atom-coordinates")
 
     if isinstance(fit_properties, ARFitPropertyList):
         properties = ET.SubElement(struct_xml, "properties")
         for prop in fit_properties.values():
             properties.append(prop.to_xml_element())
     else:
         struct_xml.append(fit_properties)
     return struct_xml
 
 
+def user_structure_xml(
+    identifier,
+    fit_properties,
+    pbc,
+    cell,
+    positions,
+    symbols,
+    forces=None,
+    fit=True,
+    relative_weight=1,
+    clamp=True,
+):
+
+    struct_xml = structure_meta_xml(
+        identifier=identifier,
+        relative_weight=relative_weight,
+        clamp=clamp,
+        fit_properties=fit_properties,
+        fit=fit,
+        mod_poscar=False,
+    )
+
+    xmlpbc = ET.SubElement(struct_xml, "pbc")
+    xmlpbc.set("x", f"{pbc[0]}".lower())
+    xmlpbc.set("y", f"{pbc[1]}".lower())
+    xmlpbc.set("z", f"{pbc[2]}".lower())
+
+    xmlcell = ET.SubElement(struct_xml, "cell")
+    for i in range(3):
+        a = ET.SubElement(xmlcell, f"a{i+1}")
+        a.set("x", f"{cell[i][0]}")
+        a.set("y", f"{cell[i][1]}")
+        a.set("z", f"{cell[i][2]}")
+
+    xmlatoms = ET.SubElement(xmlcell, "atoms")
+    for sym, pos in zip(symbols, positions):
+        a = ET.SubElement(xmlatoms, "atom")
+        a.set("type", sym)
+        a.set("x", f"{pos[0]}")
+        a.set("y", f"{pos[1]}")
+        a.set("z", f"{pos[2]}")
+        a.set("reduced", "false")
+
+    if forces is not None:
+        idx = 0
+        xmlforces = ET.SubElement(struct_xml, "atomic-forces")
+        for f in forces:
+            xmlf = ET.SubElement(xmlforces, "force")
+            xmlf.set("x", f"{f[0]}")
+            xmlf.set("y", f"{f[1]}")
+            xmlf.set("z", f"{f[2]}")
+            xmlf.set("i", f"{idx}")
+            idx += 1
+
+    return struct_xml
+
+
 def predefined_structure_xml(
     identifier,
     lattice,
     lattice_param,
     ca_ratio,
     atom_type_A,
     atom_type_B,
```

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomicrex/utility_functions.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/trainingcontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/meamfit/meamfit.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/meamfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/ml/potentialfit.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/potentialfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/cfgs.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/cfgs.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/lammps.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/masters.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/masters.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlip.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlip.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/mlipdescriptors.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlipdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/parser.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/mlip/potential.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/pacemaker/job.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 raise ValueError(
                     "Provided potential filename ({}) doesn't exists".format(
                         self.input["potential"]
                     )
                 )
 
         with open(os.path.join(self.working_directory, "input.yaml"), "w") as f:
-            yaml.dump(input_yaml_dict, f)
+            yaml.YAML(typ="unsafe", pure=True).dump(input_yaml_dict, f)
 
     def _analyse_log(self, logfile="metrics.txt"):
         metrics_filename = os.path.join(self.working_directory, logfile)
 
         metrics_df = pd.read_csv(metrics_filename, sep="\s+")
         res_dict = metrics_df.to_dict(orient="list")
         return res_dict
```

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/job.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/storageclasses.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/storageclasses.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/runner/utils.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/utils.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/calculations.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/calculations.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/learn.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/learn.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pyiron_base import Project
 from pyiron_potentialfit.atomistics.job.trainingcontainer import TrainingContainer
 from typing import Iterable, Union
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 import numpy as np
+import pandas as pd
 from tqdm.auto import tqdm
 
 from .util import get_table, read_generic_parameters
 
 
 def broadcast(*names):
     """
@@ -57,76 +58,76 @@
             func(*boundargs.args, **boundargs.kwargs)
 
         return f
 
     return wrapper
 
 
-@broadcast("min_dist", "max_dist", "level")
+@broadcast("rmin", "rmax", "level")
 def fit(
     fit_pr: Project,
     train: TrainingContainer,
-    min_dist: Union[float, Iterable[float]],
-    max_dist: Union[float, Iterable[float]],
+    rmin: Union[float, Iterable[float]],
+    rmax: Union[float, Iterable[float]],
     level: Union[int, Iterable[int]],
     iterations: int = 5000,
     energy_weight: float = None,
     force_weight: float = None,
     stress_weight: float = None,
     refit: bool = True,
     delete_existing_job=False,
 ) -> Project:
     """
     Fit a potential to the given structures.
 
-    If min_dist, max_dist or level are iterables the function is broadcasted
+    If rmin, rmax or level are iterables the function is broadcasted
     over them.
 
     Args:
         fit_pr (Project): project that contains the fitting jobs
         train (TrainingContainer): container that keeps all the structures
-        min_dist (float, Iterable[float]): lower cut off of the potential
-        max_dist (float, Iterable[float]): upper cut off of the potential
+        rmin (float, Iterable[float]): lower cut off of the potential
+        rmax (float, Iterable[float]): upper cut off of the potential
         level (int, Iterable[int]): level of the potential
         energy_weight (float): relative weight of energy error in cost function
         force_weight (float): relative weight of force error in cost function
         stress_weight (float): relative weight of stress error in cost function
         refit (bool): if True and the fit to be created already exists, start a
                       refit
         delete_existing_job (float): remove old job before creating new one
     """
     pr = fit_pr.create_group(train.name)
 
-    name = [f"MTP{level:02}", round(min_dist, 2), round(max_dist, 2)]
+    name = [f"MTP{level:02}", round(rmin, 2), round(rmax, 2)]
     if iterations is not None:
         name += ["I", iterations]
     if energy_weight is not None:
         name += ["E", energy_weight]
     if force_weight is not None:
         name += ["F", force_weight]
     if stress_weight is not None:
         name += ["S", stress_weight]
 
     j = pr.create.job.Mlip(
         name, delete_existing_job=delete_existing_job, delete_aborted_job=True
     )
     j["user/level"] = level
-    j["user/rmax"] = max_dist
-    j["user/rmin"] = min_dist
+    j["user/rmax"] = rmax
+    j["user/rmin"] = rmin
     if iterations is not None:
         j["user/iterations"] = iterations
     if energy_weight is not None:
         j["user/energy_weight"] = energy_weight
     if force_weight is not None:
         j["user/force_weight"] = force_weight
     if stress_weight is not None:
         j["user/stress_weight"] = stress_weight
     if j.status.finished and refit and not j.name.endswith("_restart"):
         j = j.restart()
-        j["user/restart"] = True
+        j["user/refit"] = True
         j.server.queue = "cmti"
         if level < 16:
             j.server.cores = 40
         if level < 24:
             j.server.cores = 80
         else:
             j.server.cores = 120
@@ -134,16 +135,16 @@
         j.run()
         return pr
     if not j.status.initialized:
         return pr
 
     j.add_job_to_fitting(train.id, 0, train.number_of_structures - 1, 1)
     j.input["potential"] = level
-    j.input["min_dist"] = min_dist
-    j.input["max_dist"] = max_dist
+    j.input["rmin"] = rmin
+    j.input["rmax"] = rmax
     if iterations is not None:
         j.input["iteration"] = iterations
     if energy_weight is not None:
         j.input["energy-weight"] = energy_weight
     if force_weight is not None:
         j.input["force-weight"] = force_weight
     if stress_weight is not None:
@@ -319,17 +320,17 @@
         tab.analysis_project = fit_pr
         tab.filter_function = tab.filter.job_type("Mlip")
         # GOTCHA: technically this can be anything; but we only ever fit() Alex' predefined potentials where the
         # name corresponds exactly to the level
         tab.add["level"] = lambda j: int(
             read_generic_parameters(j["mlip_inp"], "potential")
         )
-        tab.add["rmin"] = lambda j: read_generic_parameters(j["mlip_inp"], "min_dist")
-        tab.add["rmax"] = lambda j: read_generic_parameters(j["mlip_inp"], "max_dist")
-        tab.add["restart"] = lambda j: j.name.endswith("restart")
+        tab.add["rmin"] = lambda j: read_generic_parameters(j["mlip_inp"], "rmin")
+        tab.add["rmax"] = lambda j: read_generic_parameters(j["mlip_inp"], "rmax")
+        tab.add["refit"] = lambda j: j.name.endswith("refit")
         tab.add["energy_spread"] = energy_spread
         tab.add["energy_rmse"] = energy_rmse
         tab.add["energy_mae"] = energy_mae
         tab.add["force_rmse"] = force_rmse
         tab.add["force_mae"] = force_mae
         tab.add["stress_hydro_rmse"] = stress_hydro_rmse
         tab.add["stress_hydro_mae"] = stress_hydro_mae
@@ -376,32 +377,32 @@
         data=df,
         kind="line",
         marker="o",
         x="level",
         y="error",
         col="quantity",
         row="metric",
-        hue="max_dist",
-        style="min_dist",
+        hue="rmax",
+        style="rmin",
         facet_kws={"sharey": "col"},
         **kwargs,
     ).set(yscale="log" if logy else "linear")
 
 
-def plot_error_vs_max_dist(df, logy=True, **kwargs):
+def plot_error_vs_rmax(df, logy=True, **kwargs):
     return sns.relplot(
         data=df,
         kind="line",
         marker="o",
-        x="max_dist",
+        x="rmax",
         y="error",
         col="quantity",
         row="metric",
         hue="level",
-        style="min_dist",
+        style="rmin",
         facet_kws={"sharey": "col"},
         **kwargs,
     ).set(yscale="log" if logy else "linear")
 
 
 epilog = """
 We lay out the project like this,
@@ -485,16 +486,16 @@
     fit_pr = Project(args.project)
     train_pr = fit_pr[".."].create_group(args.calculations_project)
     for contname in args.containers:
         cont = train_pr.load(contname)
         fit(
             fit_pr,
             cont,
-            min_dist=args.rmin,
-            max_dist=args.rmax,
+            rmin=args.rmin,
+            rmax=args.rmax,
             level=args.level,
             iterations=args.iterations,
             refit=args.refit,
             energy_weight=args.energy_weight,
             force_weight=args.force_weight,
             stress_weight=args.stress_weight,
         )
```

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/projectflow.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/projectflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/structures.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/structures.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit/spgfit/util.py` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/PKG-INFO` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -13,17 +13,18 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: ase>=3.22.1
-Requires-Dist: pyiron_atomistics>=0.5.1
-Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: pyiron_atomistics>=0.5.2
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyiron_base>=0.8.1
-Requires-Dist: scipy>=1.11.4
+Requires-Dist: pyiron_base>=0.8.2
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: runnerase>=0.3.3
-Requires-Dist: seaborn
-Requires-Dist: dill
+Requires-Dist: dill>=0.3.0
+Requires-Dist: seaborn<0.14,>=0.13.0
+Requires-Dist: pyxtal<0.7,>=0.6.0
 
 http://pyiron.org
```

### Comparing `pyiron_potentialfit-0.3.0/pyiron_potentialfit.egg-info/SOURCES.txt` & `pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.0/setup.py` & `pyiron_potentialfit-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,24 @@
         'Programming Language :: Python :: 3.11',
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
         'ase>=3.22.1',
-        'pyiron_atomistics>=0.5.1',
-        'matplotlib>=3.8.3',
+        'pyiron_atomistics>=0.5.2',
+        'matplotlib>=3.8.4',
         'numpy>=1.26.4',
-        'pyiron_base>=0.8.1',
-        'scipy>=1.11.4',
+        'pyiron_base>=0.8.2',
+        'scipy>=1.13.0',
         'runnerase>=0.3.3',
         # spgfit
-        'seaborn',
-        'dill'
+        'dill>=0.3.0',
+        'seaborn>=0.13.0,<0.14',
+        'pyxtal>=0.6.0,<0.7',
     ],
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
         "console_scripts": [
             "spgfit-structures = pyiron_potentialfit.spgfit.structures:main",
             "spgfit-calculations = pyiron_potentialfit.spgfit.calculations:main",
             "spgfit-learn = pyiron_potentialfit.spgfit.learn:main"
```

### Comparing `pyiron_potentialfit-0.3.0/versioneer.py` & `pyiron_potentialfit-0.3.1/versioneer.py`

 * *Files identical despite different names*

