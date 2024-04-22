# Comparing `tmp/pymatgen-analysis-defects-2024.2.9.tar.gz` & `tmp/pymatgen_analysis_defects-2024.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2024.2.9.tar", last modified: Fri Feb  9 21:31:13 2024, max compression
+gzip compressed data, was "pymatgen_analysis_defects-2024.4.22.tar", last modified: Mon Apr 22 22:35:07 2024, max compression
```

## Comparing `pymatgen-analysis-defects-2024.2.9.tar` & `pymatgen_analysis_defects-2024.4.22.tar`

### file list

```diff
@@ -1,44 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.197259 pymatgen-analysis-defects-2024.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-02-09 21:31:13.197259 pymatgen-analysis-defects-2024.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.189259 pymatgen-analysis-defects-2024.2.9/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.189259 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.193259 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    31179 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    39114 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.193259 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    21485 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.193259 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/plotting/optics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/plotting/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    48901 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (127)    40842 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.197259 pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-02-09 21:31:13.000000 pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-09 21:31:13.000000 pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 21:31:13.000000 pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-09 21:31:13.000000 pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-09 21:31:13.000000 pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 21:31:13.197259 pymatgen-analysis-defects-2024.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:31:13.197259 pymatgen-analysis-defects-2024.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-02-09 21:31:01.000000 pymatgen-analysis-defects-2024.2.9/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-09 21:31:02.000000 pymatgen-analysis-defects-2024.2.9/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-02-09 21:31:02.000000 pymatgen-analysis-defects-2024.2.9/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-09 21:31:02.000000 pymatgen-analysis-defects-2024.2.9/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-09 21:31:02.000000 pymatgen-analysis-defects-2024.2.9/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    13830 2024-02-09 21:31:02.000000 pymatgen-analysis-defects-2024.2.9/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-09 21:31:02.000000 pymatgen-analysis-defects-2024.2.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.396712 pymatgen_analysis_defects-2024.4.22/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-04-22 22:35:07.396712 pymatgen_analysis_defects-2024.4.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.388712 pymatgen_analysis_defects-2024.4.22/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.388712 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.392712 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26337 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40256 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.392712 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.392712 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/plotting/optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/plotting/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51742 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:35:07.396712 pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-04-22 22:35:07.000000 pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 22:35:07.000000 pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:35:07.000000 pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-22 22:35:07.000000 pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 22:35:07.000000 pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-22 22:34:59.000000 pymatgen_analysis_defects-2024.4.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:35:07.396712 pymatgen_analysis_defects-2024.4.22/setup.cfg
```

### Comparing `pymatgen-analysis-defects-2024.2.9/LICENSE` & `pymatgen_analysis_defects-2024.4.22/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-atomate2 Copyright (c) 2015, The Regents of the University of
+pymatgen-analysis-defects Copyright (c) 2015, The Regents of the University of
 California, through Lawrence Berkeley National Laboratory (subject
 to receipt of any required approvals from the U.S. Dept. of Energy).
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
```

### Comparing `pymatgen-analysis-defects-2024.2.9/PKG-INFO` & `pymatgen_analysis_defects-2024.4.22/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2024.2.9
+Version: 2024.4.22
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
@@ -14,151 +14,159 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymatgen
 Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: numpy
+Requires-Dist: mp-pyrho>=0.4.4
 Provides-Extra: finder
 Requires-Dist: dscribe>=2.0.0; extra == "finder"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: jupyter-book>=0.13.1; extra == "docs"
 Provides-Extra: optional
 Requires-Dist: pydefect>=0.6.2; extra == "optional"
 Requires-Dist: dscribe>=2.0.0; extra == "optional"
 Requires-Dist: numba; extra == "optional"
 Provides-Extra: strict
-Requires-Dist: pymatgen==2023.10.11; extra == "strict"
+Requires-Dist: pymatgen==2024.3.1; extra == "strict"
 Requires-Dist: dscribe==2.1.0; extra == "strict"
-Requires-Dist: scikit-image==0.21.0; extra == "strict"
+Requires-Dist: scikit-image==0.22.0; extra == "strict"
+Requires-Dist: mp-pyrho==0.4.4; extra == "strict"
 Provides-Extra: tests
-Requires-Dist: pytest==7.4.2; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0; extra == "tests"
-Requires-Dist: nbmake==1.4.6; extra == "tests"
+Requires-Dist: nbmake==1.5.3; extra == "tests"
 
-pymatgen-analysis-defects
-=========================
+# pymatgen-analysis-defects
 
-|testing| |codecov| |zenodo| |pypi|
+[![testing](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml)
+[![codecov](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects/branch/main/graph/badge.svg?token=FOKXRCZTXZ)](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects)
+[![zenodo](https://zenodo.org/badge/452872799.svg)](https://zenodo.org/badge/latestdoi/452872799)
+[![pypi](https://badge.fury.io/py/pymatgen-analysis-defects.svg)](https://badge.fury.io/py/pymatgen-analysis-defects)
+
+📄 [Full
+Documentation](https://materialsproject.github.io/pymatgen-analysis-defects/)
+[Paper](https://joss.theoj.org/papers/10.21105/joss.05941)
+
+This package is an extension to `pymatgen` for performing defect
+analysis. The package is designed to work with VASP inputs and output
+files and is meant to be used as a namespace package extension to the
+main `pymatgen` library. The new module has been redesigned to work
+closely with `atomate2`.
+
+While the `atomate2` automation framework is not required for this code
+to be useful, users are strongly encouraged to to adopt the `atomate2`
+framework as it contains codified \"best practices\" for running defect
+calculations as well as orchestrating the running of calculations and
+storing the results.
+
+The package serves as an object-oriented interface to defect physics and
+is capable of generating a list of non-equivalent defect objects
+directly from the Materials Project API.
+
+``` python
+from pymatgen.analysis.defects.generators import ChargeInterstitialGenerator, generate_all_native_defects
+from pymatgen.ext.matproj import MPRester
+with MPRester() as mpr:
+chgcar = mpr.get_charge_density_from_material_id("mp-804")
+for defect in generate_all_native_defects(chgcar):
+    print(defect)
+```
 
-📄 `Full Documentation <https://materialsproject.github.io/pymatgen-analysis-defects/>`_
+# Non-exhaustive list of features:
 
-
-This package is an extension to ``pymatgen`` for performing defect analysis.
-The package is designed to work with VASP inputs and output files and is meant
-to be used as a namespace package extension to the main ``pymatgen`` library.
-The new module has been redesigned to work closely with ``atomate2``.
-
-While the ``atomate2`` automation framework is not required for this code to be useful, users are strongly encouraged to
-to adopt the ``atomate2`` framework as it contains codified "best practices" for running defect calculations
-as well as orchestrating the running of calculations and storing the results.
-
-
-Non-exhaustive list of features:
---------------------------------
-
-Reproducible definition of defects
-++++++++++++++++++++++++++++++++++
+## Reproducible definition of defects
 
 Defects are defined based on the physical concept they represent,
-independent of the calculation details such as simulation cell size.
-As an example, a Vacancy defect is defined by the primitive cell of the
+independent of the calculation details such as simulation cell size. As
+an example, a Vacancy defect is defined by the primitive cell of the
 pristine material plus a single site that represents the vacancy site in
 the unit cell.
 
-
-Formation energy calculations
-+++++++++++++++++++++++++++++
+## Formation energy calculations
 
 The formation energy diagram is a powerful tool for understanding the
 thermodynamics of defects. This package provides a simple interface for
 calculating the formation energy diagram from first-principles results.
-This package handles the energy accounting of the chemical species for the chemical
-potential calculations, which determines the y-offset of the formation energy.
-This package also performs finite-size corrections for the formation energy which is required
-when studying charged defects in periodic simulation cells.
-
-Defect Position
-+++++++++++++++
-
-Identification of the defect positions in a simulation cell after atomic relaxation
-is not trivial since the many atoms can collectively shift in response to the creation of
-the defect.
-Yet the exact location of the defect is required for the calculation of finite-size corrections
-as well as other physical properties.
-We devised a method based on calculating a SOAP-based distortion field that can be used to
-identify the defect position in a simulation cell.
-Note, this method only requires the reference pristine supercell and does not need prior knowledge
-of how the defect was created.
-
-Defect Complexes
-++++++++++++++++
-
-Multiple defects can be composed into defect complexes.
-The complex is can be treated as a normal defect object for subsequent analysis.
-
-Defect Interactions
-+++++++++++++++++++
-
-Simulation of defect-photon and defect-phonon interactions under the independent particle approximation.
+This package handles the energy accounting of the chemical species for
+the chemical potential calculations, which determines the y-offset of
+the formation energy. This package also performs finite-size corrections
+for the formation energy which is required when studying charged defects
+in periodic simulation cells.
 
-Previous versions of the defects code
--------------------------------------
+## Defect Position
 
-This package replaces the older ``pymatgen.analysis.defects`` modules.
-The previous module was used by ``pyCDT`` code which will continue to work with version ``2022.7.8`` of ``pymatgen``.
+Identification of the defect positions in a simulation cell after atomic
+relaxation is not trivial since the many atoms can collectively shift in
+response to the creation of the defect. Yet the exact location of the
+defect is required for the calculation of finite-size corrections as
+well as other physical properties. We devised a method based on
+calculating a SOAP-based distortion field that can be used to identify
+the defect position in a simulation cell. Note, this method only
+requires the reference pristine supercell and does not need prior
+knowledge of how the defect was created.
 
-Contributing
-------------
+## Defect Complexes
 
-The source code can be downloaded from the GitHub repository at
+Multiple defects can be composed into defect complexes. The complex is
+can be treated as a normal defect object for subsequent analysis.
 
-.. code-block:: bash
+## Defect Interactions
 
-    $ git clone https://github.com/materialsproject/pymatgen-analysis-defects.git
+Simulation of defect-photon and defect-phonon interactions under the
+independent particle approximation.
 
-All code contributions are welcome. Please submit a pull request on GitHub.
-To make maintenance easier, please use a workflow similar to the automated CI
-`workflow <https://github.com/materialsproject/pymatgen-analysis-defects/blob/main/.github/workflows/testing.yml>`_.
+# Previous versions of the defects code
 
-Specifically, please make sure to run the following commands for linting:
+This package replaces the older `pymatgen.analysis.defects` modules. The
+previous module was used by `pyCDT` code which will continue to work
+with version `2022.7.8` of `pymatgen`.
 
-.. code-block:: bash
+# Contributing
 
-    $ pip install -e .[strict]
-    $ pip install -e .[dev]
-    $ pre-commit install
-    $ pre-commit run --all-files
+The source code can be downloaded from the GitHub repository at
 
-And run these commands for testing:
+``` bash
+$ git clone https://github.com/materialsproject/pymatgen-analysis-defects.git
+```
+
+All code contributions are welcome. Please submit a pull request on
+GitHub. To make maintenance easier, please use a workflow similar to the
+automated CI
+[workflow](https://github.com/materialsproject/pymatgen-analysis-defects/blob/main/.github/workflows/testing.yml).
+
+Specifically, please make sure to run the following commands for
+linting:
+
+``` bash
+$ pip install -e .[strict]
+$ pip install -e .[dev]
+$ pre-commit install
+$ pre-commit run --all-files
+```
 
-.. code-block:: bash
+And run these commands for testing:
 
-    $ pip install -e .[strict]
-    $ pip install -e .[tests]
-    $ pytest --cov=pymatgen
-    $ pytest --nbmake ./docs/source/content
-
-For more details about what is actually installed with each of the ``pip install .[arg]`` commands, please inspect the
-``pyproject.toml`` file.
-
-Contributors
-------------
-
-* Lead developer: Dr. Jimmy-Xuan Shen
-* This code contains contributions from the original defects analysis module of ``pymatgen`` from Dr. Danny Broberg and Dr. Shyam Dwaraknath.
-
-.. |testing| image:: https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml/badge.svg?branch=main
-   :target: https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml
-.. |codecov| image:: https://codecov.io/gh/materialsproject/pymatgen-analysis-defects/branch/main/graph/badge.svg?token=FOKXRCZTXZ
-   :target: https://codecov.io/gh/materialsproject/pymatgen-analysis-defects
-.. |zenodo| image:: https://zenodo.org/badge/452872799.svg
-   :target: https://zenodo.org/badge/latestdoi/452872799
-.. |pypi| image:: https://badge.fury.io/py/pymatgen-analysis-defects.svg
-    :target: https://badge.fury.io/py/pymatgen-analysis-defects
+``` bash
+$ pip install -e .[strict]
+$ pip install -e .[tests]
+$ pytest --cov=pymatgen
+$ pytest --nbmake ./docs/source/content
+```
+
+For more details about what is actually installed with each of the
+`pip install .[arg]` commands, please inspect the `pyproject.toml` file.
+
+# Contributors
+
+-   Lead developer: Dr. Jimmy-Xuan Shen
+-   This code contains contributions from the original defects analysis
+    module of `pymatgen` from Dr. Danny Broberg and Dr. Shyam
+    Dwaraknath.
```

### Comparing `pymatgen-analysis-defects-2024.2.9/README.rst` & `pymatgen_analysis_defects-2024.4.22/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 to be used as a namespace package extension to the main ``pymatgen`` library.
 The new module has been redesigned to work closely with ``atomate2``.
 
 While the ``atomate2`` automation framework is not required for this code to be useful, users are strongly encouraged to
 to adopt the ``atomate2`` framework as it contains codified "best practices" for running defect calculations
 as well as orchestrating the running of calculations and storing the results.
 
+The package serves as an object-oriented interface to defect physics and is capable of generating a list of 
+non-equivalent defect objects directly from the Materials Project API.
+
+.. code-block:: python
+    from pymatgen.analysis.defects.generators import ChargeInterstitialGenerator, generate_all_native_defects
+    from pymatgen.ext.matproj import MPRester
+    with MPRester() as mpr:
+        chgcar = mpr.get_charge_density_from_material_id("mp-804")
+        
+    for defect in generate_all_native_defects(chgcar):
+        print(defect)
 
 Non-exhaustive list of features:
 --------------------------------
 
 Reproducible definition of defects
 ++++++++++++++++++++++++++++++++++
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/ccd.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/ccd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Configuration-coordinate diagram analysis."""
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from itertools import groupby
-from typing import TYPE_CHECKING, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING
 
 import numpy as np
 from monty.json import MSONable
 from pymatgen.electronic_structure.core import Spin
 from pymatgen.io.vasp.optics import DielectricFunctionCalculator
 from pymatgen.io.vasp.outputs import WSWQ, Procar, Vasprun
 from scipy.optimize import curve_fit
 
 from .constants import AMU2KG, ANGS2M, EV2J, HBAR_EV, KB
 from .recombination import get_SRH_coef
 from .utils import get_localized_states, get_zfile, sort_positive_definite
 
 if TYPE_CHECKING:
+    from collections.abc import Sequence
     from ctypes import Structure
     from pathlib import Path
 
     import numpy.typing as npt
     from matplotlib.axes import Axes
     from pymatgen.io.vasp.outputs import BandStructure, Waveder
 
@@ -60,23 +62,23 @@
         wswqs: Dict of WSWQ objects for each distortion. The key is the distortion.
         waveder: The Waveder object for the relaxed defect structure.
     """
 
     omega: float
     charge_state: int
     ispin: int
-    vrun: Optional[Vasprun] = None
-    distortions: Optional[list[float]] = None
-    structures: Optional[list[Structure]] = None
-    energies: Optional[list[float]] = None
-    defect_band: Optional[Sequence[tuple]] = None
-    relaxed_index: Optional[int] = None
-    relaxed_bandstructure: Optional[BandStructure] = None
-    wswqs: Optional[list[dict]] = None
-    waveder: Optional[Waveder] = None
+    vrun: Vasprun | None = None
+    distortions: Sequence[float] | None = None
+    structures: Sequence[Structure] | None = None
+    energies: Sequence[float] | None = None
+    defect_band: Sequence[tuple] | None = None
+    relaxed_index: int | None = None
+    relaxed_bandstructure: BandStructure | None = None
+    wswqs: list[dict] | None = None
+    waveder: Waveder | None = None
 
     def __repr__(self) -> str:
         """String representation of the harmonic defect."""
         return (
             f"HarmonicDefect("
             f"omega={self.omega_eV:.3f} eV, "
             f"charge={self.charge_state}, "
@@ -87,38 +89,40 @@
         )
 
     @property
     def defect_band_index(self) -> int:
         """The index of the defect band."""
         bands = {band for band, _, _ in self.defect_band}
         if len(bands) != 1:
-            raise ValueError("Defect band index is not unique.")
+            msg = "Defect band index is not unique."
+            raise ValueError(msg)
         return bands.pop()
 
     @property
     def spin_index(self) -> int:
         """The spin index of the defect.
 
         The integer spin index the defect state belongs to.
         0 for spin up and 1 for spin down. If ISPIN=1, this is always 0.
         """
         spins = {spin for _, _, spin in self.defect_band}
         if len(spins) != 1:
-            raise ValueError("Spin index is not unique.")
+            msg = "Spin index is not unique."
+            raise ValueError(msg)
         return spins.pop()
 
     @property
     def spin(self) -> Spin:
         """The spin of the defect returned as an Spin Enum."""
         if self.spin_index == 0:
             return Spin.up
-        elif self.spin_index == 1:
+        if self.spin_index == 1:
             return Spin.down
-        else:
-            raise ValueError(f"Invalid spin index: {self.spin_index}")
+        msg = f"Invalid spin index: {self.spin_index}"
+        raise ValueError(msg)
 
     @property
     def relaxed_structure(self) -> Structure:
         """The relaxed structure."""
         return self.structures[self.relaxed_index]
 
     @classmethod
@@ -158,15 +162,15 @@
             band_window: The number of bands above and below the defect band to include when searching for the defect band.
             **kwargs: Additional keyword arguments to pass to the constructor.
 
         Returns:
             A HarmonicDefect object.
         """
 
-        def _parse_vasprun(vasprun: Vasprun):
+        def _parse_vasprun(vasprun: Vasprun) -> tuple[float, Structure]:
             energy = vasprun.final_energy
             struct = vasprun.final_structure
             return (energy, struct)
 
         energy_struct = list(map(_parse_vasprun, vaspruns))
         unsorted_e = [e for e, _ in energy_struct]
 
@@ -178,45 +182,46 @@
             energy_struct,
             energy_struct[relaxed_index],
             energy_struct[-1],
             lambda x, y: get_dQ(x[1], y[1]),
         )
         energies, structures = list(zip(*sorted_list))
 
-        if not np.allclose(unsorted_e, energies, atol=1e-99):
-            raise ValueError("The vaspruns should already be in order.")
+        if not np.allclose(unsorted_e, energies, atol=1e-99):  # pragma: no cover
+            msg = "The vaspruns should already be in order."
+            raise ValueError(msg)
 
         omega = _get_omega(
             Q=distortions,
             E=energies,
             Q0=distortions[relaxed_index],
             E0=energies[relaxed_index],
         )
 
         get_band_structure_kwargs = get_band_structure_kwargs or {}
         bandstructure = vaspruns[relaxed_index].get_band_structure(
-            **get_band_structure_kwargs
+            **get_band_structure_kwargs,
         )
         ispin = vaspruns[relaxed_index].parameters["ISPIN"]
 
-        if store_bandstructure:
-            bs = bandstructure
-        else:
-            bs = None
+        bs = bandstructure if store_bandstructure else None
 
         if defect_band is None:
             if procar is None:  # pragma: no cover
+                msg = "If defect_band_index is not provided, you must provide a Procar object."
                 raise ValueError(
-                    "If defect_band_index is not provided, you must provide a Procar object."
+                    msg,
                 )
             # Get the defect bands
             defect_band_2s = list(
                 get_localized_states(
-                    bandstructure=bandstructure, procar=procar, band_window=band_window
-                )
+                    bandstructure=bandstructure,
+                    procar=procar,
+                    band_window=band_window,
+                ),
             )
             defect_band_2s.sort(key=lambda x: (x[2], x[1]))
             # group by the spin index
             defect_band_grouped = {
                 spin: list(bands)
                 for spin, bands in groupby(defect_band_2s, lambda x: x[2])
             }
@@ -230,15 +235,15 @@
             # drop the val
             defect_band = [r_[:3] for r_ in defect_band_grouped[spin_index]]
 
         return cls(
             omega=omega,
             charge_state=charge_state,
             ispin=ispin,
-            structures=structures,
+            structures=list(structures),
             distortions=distortions,
             energies=energies,
             defect_band=defect_band,
             relaxed_index=relaxed_index,
             relaxed_bandstructure=bs,
             vrun=vaspruns[relaxed_index],
             **kwargs,
@@ -276,21 +281,25 @@
         min_idx = np.argmin([v.final_energy for v in vaspruns])
         min_dir = directories[min_idx]
         procar_file = get_zfile(min_dir, "PROCAR")
         procar = Procar(procar_file) if procar_file else None
 
         if charge_state is None:
             if vaspruns[min_idx].final_structure._charge is None:
-                raise ValueError(
+                msg = (
                     "Charge state is not provided and cannot be parsed from the POTCAR."
                 )
+                raise ValueError(
+                    msg,
+                )
             charge_state = vaspruns[0].final_structure.charge
 
         if any(v.final_structure.charge != charge_state for v in vaspruns):
-            raise ValueError("All vaspruns must have the same charge state.")
+            msg = "All vaspruns must have the same charge state."
+            raise ValueError(msg)
 
         return cls.from_vaspruns(
             vaspruns=vaspruns,
             charge_state=charge_state,
             relaxed_index=relaxed_index,
             defect_band=defect_band,
             procar=procar,
@@ -309,34 +318,37 @@
 
         Args:
             t: The temperature in Kelvin.
         """
         return 1.0 / (1 - np.exp(-self.omega_eV / KB * t))
 
     def read_wswqs(
-        self, directory: Path, distortions: list[float] | None = None
+        self,
+        directory: Path,
+        distortions: Sequence[float] | None = None,
     ) -> None:
         """Read the WSWQ files from a directory.
 
         Assuming that we have a directory containing the WSWQ files ordered in
         the same way as the `self.distortions`.
 
         Args:
             directory: The directory containing the WSWQ files formatted as WSWQ.0, WSWQ.1, ...
             distortions: The distortions used to generate the WSWQ files,
                 if different from self.distortions
         """
-        wswq_files = [f for f in directory.glob("WSWQ*")]
+        wswq_files = list(directory.glob("WSWQ*"))
         wswq_files.sort(key=lambda x: int(x.name.split(".")[1]))
         if distortions is None:
             distortions = self.distortions
 
         if len(wswq_files) != len(distortions):
+            msg = f"Number of WSWQ files ({len(wswq_files)}) does not match number of distortions ({len(distortions)})."
             raise ValueError(
-                f"Number of WSWQ files ({len(wswq_files)}) does not match number of distortions ({len(distortions)})."
+                msg,
             )
         self.wswqs = [
             {"Q": d, "wswq": WSWQ.from_file(f)} for d, f in zip(distortions, wswq_files)
         ]
 
     def get_elph_me(self, defect_state: tuple) -> npt.ArrayLike:
         """Calculate the electron phonon matrix elements.
@@ -355,27 +367,31 @@
                 k-point associated with the band-edge states.
 
         Returns:
             npt.ArrayLike: The electron phonon matrix elements from the defect band to all other bands.
                 The indices are [band_j,]
         """
         if self.wswqs is None:
-            raise RuntimeError("WSWQs have not been read. Use `read_wswqs` first.")
+            msg = "WSWQs have not been read. Use `read_wswqs` first."
+            raise RuntimeError(msg)
         distortions = [wswq["Q"] for wswq in self.wswqs]
         wswqs = [wswq["wswq"] for wswq in self.wswqs]
         band_index, kpoint_index, spin_index = defect_state
         # The second band index is associated with the defect state
         # since we are usually interested in capture
         slopes = _get_wswq_slope(distortions, wswqs)[
-            spin_index, kpoint_index, :, band_index
+            spin_index,
+            kpoint_index,
+            :,
+            band_index,
         ]
         ediffs = self._get_ediff(output_order="skb")[spin_index, kpoint_index, :]
         return np.multiply(slopes, ediffs)
 
-    def _get_ediff(self, output_order="skb") -> npt.NDArray:
+    def _get_ediff(self, output_order: str = "skb") -> npt.NDArray:
         """Compute the eigenvalue difference to the defect band.
 
         .. note::
             Since the different matrix element output files have different index orders,
             But most calculations require the energies, we should always perform the
             rearrangement here so that we have a single point of failure.
 
@@ -383,56 +399,62 @@
             output_order: The order of the output. Defaults to "skb" (spin, kpoint, band]).
                 You can also use "bks" (band, kpoint, spin).
 
         Returns:
             The eigenvalue difference to the defect band in the order specified by output_order.
 
         """
-        if self.relaxed_bandstructure is None:
-            raise ValueError(  # pragma: no cover
+        if self.relaxed_bandstructure is None:  # pragma: no cover
+            msg = (
                 "The ``relaxed_bandstructure`` must be set before ``ediff`` can be computed. "
                 "Try setting ``store_bandstructure=True`` when initializing."
             )
+            raise ValueError(
+                msg,
+            )
 
         ediffs_ = _get_ks_ediff(
             bandstructure=self.relaxed_bandstructure,
             defect_band=self.defect_band,
         )
         ediffs_stack = [
             ediffs_[Spin.up].T,
         ]
-        if Spin.down in ediffs_.keys():
+        if Spin.down in ediffs_:
             ediffs_stack.append(ediffs_[Spin.down].T)
         ediffs = np.stack(ediffs_stack)
 
         if output_order == "skb":
             return ediffs
-        elif output_order == "bks":
+        if output_order == "bks":
             return ediffs.transpose((2, 1, 0))
-        else:
-            raise ValueError(
-                "Invalid output_order, choose from 'skb' or 'bks'."
-            )  # pragma: no cover
+        msg = "Invalid output_order, choose from 'skb' or 'bks'."
+        raise ValueError(
+            msg,
+        )
 
     def get_dielectric_function(
-        self, idir: int, jdir: int
+        self,
+        idir: int,
+        jdir: int,
     ) -> tuple[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike]:
         """Calculate the dielectric function.
 
         Args:
             idir: The first direction of the dielectric tensor.
             jdir: The second direction of the dielectric tensor.
 
         Returns:
             energy: The energy grid representing the dielectric function.
             eps_vbm: The dielectric function from the VBM to the defect state.
             eps_cbm: The dielectric function from the defect state to the CBM.
         """
         dfc = DielectricFunctionCalculator.from_vasp_objects(
-            vrun=self.vrun, waveder=self.waveder
+            vrun=self.vrun,
+            waveder=self.waveder,
         )
 
         # two masks to select for VBM -> Defect and Defect -> CBM
         mask_vbm = np.zeros_like(dfc.cder_real)
         mask_cbm = np.zeros_like(dfc.cder_real)
         min_def_eig, max_def_eig = np.inf, -np.inf
         for ib, ik, ispin in self.defect_band:
@@ -515,15 +537,16 @@
     defect_band, _, _ = defect_state
 
     if initial_state.charge_state == final_state.charge_state + 1:
         band_slice = slice(defect_band + 1, defect_band + 1 + n_band_edge)
     elif initial_state.charge_state == final_state.charge_state - 1:
         band_slice = slice(defect_band - n_band_edge, defect_band)
     else:
-        raise ValueError("SRH capture event must involve a charge state change of 1.")
+        msg = "SRH capture event must involve a charge state change of 1."
+        raise ValueError(msg)
 
     me_band_edge = me_all[band_slice]
     dQ = get_dQ(initial_state.relaxed_structure, final_state.relaxed_structure)
     volume = initial_state.relaxed_structure.volume
     return get_SRH_coef(
         T,
         dQ=dQ,
@@ -533,164 +556,31 @@
         elph_me=np.average(me_band_edge),
         volume=volume,
         g=g,
         occ_tol=occ_tol,
     )
 
 
-# @dataclass
-# class RadiativeCatpture(MSONable):
-#     """Representation of a radiative capture event.
-
-#     Attributes:
-#         initial_state: The initial state of the radiative capture event.
-#         final_state: The final state of the radiative capture event.
-#         dQ: The configuration coordinate change between the relaxed initial state and the final state.
-#         waveder: The data from the WAVEDER file obtained with ``LOPTICS=.True.``.
-
-#     """
-
-#     initial_state: HarmonicDefect
-#     final_state: HarmonicDefect
-#     dQ: float
-#     waveder: Waveder
-
-#     def get_coeff(
-#         self,
-#         T: float | npt.ArrayLike,
-#         dE: float,
-#         omega_photon: float,
-#         volume: float | None = None,
-#         g: int = 1,
-#         occ_tol: float = 1e-3,
-#         n_band_edge: int = 1,
-#     ):
-#         """Calculate the SRH recombination coefficient."""
-#         if volume is None:
-#             volume = self.initial_state.relaxed_structure.volume
-
-#         me_all = self.get_dipoles()  # indices: [band, kpoint, spin, coord]
-
-#         istate = self.initial_state
-
-#         if self.initial_state.charge_state == self.final_state.charge_state + 1:
-#             band_slice = slice(
-#                 istate.defect_band_index + 1, istate.defect_band_index + 1 + n_band_edge
-#             )
-#         elif self.initial_state.charge_state == self.final_state.charge_state - 1:
-#             band_slice = slice(
-#                 istate.defect_band_index - n_band_edge, istate.defect_band_index
-#             )
-#         else:
-#             raise ValueError(
-#                 "SRH capture event must involve a charge state change of 1."
-#             )
-
-#         me_band_edge = me_all[band_slice, istate.kpt_index, istate.spin_index]
-
-#         return get_Rad_coef(
-#             T,
-#             dQ=self.dQ,
-#             dE=dE,
-#             omega_i=self.initial_state.omega_eV,
-#             omega_f=self.final_state.omega_eV,
-#             omega_photon=omega_photon,
-#             dipole_me=np.average(me_band_edge),
-#             volume=volume,
-#             g=g,
-#             occ_tol=occ_tol,
-#         )
-
-#     @classmethod
-#     def from_directories(
-#         cls,
-#         initial_dirs: list[Path],
-#         final_dirs: list[Path],
-#         waveder_dir: Path,
-#         kpt_index: int,
-#         initial_charge_state: int | None = None,
-#         final_charge_state: int | None = None,
-#         spin_index: int | None = None,
-#         defect_band_index: int | None = None,
-#         store_bandstructure: bool = False,
-#         get_band_structure_kwargs: dict | None = None,
-#         **kwargs,
-#     ) -> RadiativeCatpture:
-#         """Create a RadiativeCapture object from a list of directories.
-
-#         Args:
-#             initial_dirs: A list of directories for the initial state.
-#             final_dirs: A list of directories for the final state.
-#             waveder_dir: The directory containing the WAVEDER file.
-#             kpt_index: The index of the k-point to use.
-#             initial_charge_state: The charge state of the initial state.
-#                 If None, the charge state is determined from the vasprun.xml and POTCAR files.
-#             final_charge_state: The charge state of the final state.
-#                 If None, the charge state is determined from the vasprun.xml and POTCAR files.
-#             spin_index: The index of the spin channel to use.
-#                 If None, the spin channel is determined by the channel with the most localized state.
-#             defect_band_index: The index of the defect band (0-indexed).
-#                 If None, the defect band is determined by the band with the most localized state.
-#             store_bandstructure: Whether to store the band structure.
-#             get_band_structure_kwargs: Keyword arguments to pass to get_band_structure.
-#             **kwargs: Keyword arguments to pass to the HarmonicDefect constructor.
-
-#         Returns:
-#             A SRHCapture object.
-#         """
-#         initial_defect = HarmonicDefect.from_directories(
-#             directories=initial_dirs,
-#             charge_state=initial_charge_state,
-#             spin_index=spin_index,
-#             relaxed_index=None,
-#             defect_band_index=defect_band_index,
-#             store_bandstructure=store_bandstructure,
-#             get_band_structure_kwargs=get_band_structure_kwargs,
-#             **kwargs,
-#         )
-
-#         # the final state does not need the additional
-#         # information about the electronic states
-#         final_defect = HarmonicDefect.from_directories(
-#             directories=final_dirs,
-#             kpt_index=kpt_index,
-#             charge_state=final_charge_state,
-#             spin_index=spin_index,
-#             relaxed_index=None,
-#             defect_band_index=None,
-#             store_bandstructure=None,
-#             get_band_structure_kwargs=None,
-#             **kwargs,
-#         )
-
-#         waveder_file = get_zfile(waveder_dir, "WAVEDER")
-#         waveder = Waveder(waveder_file)
-#         dQ = get_dQ(initial_defect.relaxed_structure, final_defect.relaxed_structure)
-#         return cls(initial_defect, final_defect, dQ=dQ, waveder=waveder)
-
-
 def get_dQ(ground: Structure, excited: Structure) -> float:
     """Calculate configuration coordinate difference.
 
     Args:
         ground : pymatgen structure corresponding to the ground (final) state
         excited : pymatgen structure corresponding to the excited (initial) state
 
     Returns:
         (float):  the dQ value (amu^{1/2} Angstrom)
     """
     return np.sqrt(
         np.sum(
-            list(
-                map(
-                    lambda x: x[0].distance(x[1]) ** 2 * x[0].specie.atomic_mass,
-                    zip(ground, excited),
-                )
-            )
-        )
+            [
+                x[0].distance(x[1]) ** 2 * x[0].specie.atomic_mass
+                for x in zip(ground, excited)
+            ],
+        ),
     )
 
 
 def _get_omega(
     Q: npt.ArrayLike,
     E: npt.ArrayLike,
     Q0: float,
@@ -710,19 +600,22 @@
         omega: the harmonic phonon frequency in (eV)
     """
     popt = _fit_parabola(Q, E, Q0, E0)
     return popt[0]
 
 
 def _fit_parabola(
-    Q: npt.ArrayLike, energy: npt.ArrayLike, Q0: float, E0: float
-) -> Tuple[float, float, float]:
+    Q: npt.ArrayLike,
+    energy: npt.ArrayLike,
+    Q0: float,
+    E0: float,
+) -> tuple[float, float, float]:
     """Fit the parabola to the data."""
 
-    def f(Q, omega):
+    def f(Q: float, omega: float) -> float:
         """Get the parabola function."""
         return 0.5 * omega**2 * (Q - Q0) ** 2 + E0
 
     popt, _ = curve_fit(f, Q, energy)
     return popt
 
 
@@ -737,15 +630,15 @@
         npt.NDArray: slope matrix with the same shape as the ``WSWQ.data``.
             Since there is always ambiguity in the phase, we require that the output
             is always positive.
     """
     yy = np.stack([np.abs(ww.data) * np.sign(qq) for qq, ww in zip(distortions, wswqs)])
     _, *oldshape = yy.shape
     return np.polyfit(distortions, yy.reshape(yy.shape[0], -1), deg=1)[0].reshape(
-        *oldshape
+        *oldshape,
     )
 
 
 def _get_ks_ediff(
     bandstructure: BandStructure,
     defect_band: Sequence[tuple],
 ) -> dict[Spin, npt.NDArray]:
@@ -758,15 +651,15 @@
         bandstructure: A BandStructure object.
         defect_band: The defect band given as a list of tuples (band_index, kpoint_index, spin_index).
 
     Returns:
         npt.NDArray: The Kohn-Sham energy difference between the defect state and other states.
         Indexed the same way as ``bandstructure.bands``.
     """
-    res = dict()
+    res = {}
     b_at_kpt_and_spin = {(k, s): b for b, k, s in defect_band}
     for ispin, eigs in bandstructure.bands.items():
         spin_index = 0 if ispin == Spin.up else 1
         res[ispin] = np.zeros_like(eigs)
         for ikpt, _kpt in enumerate(bandstructure.kpoints):
             iband = b_at_kpt_and_spin.get((ikpt, spin_index), None)
             if iband is None:
@@ -774,15 +667,19 @@
             e_at_def_band = eigs[iband, ikpt]
             e_diff = eigs[:, ikpt] - e_at_def_band
             res[ispin][:, ikpt] = e_diff
     return res
 
 
 def plot_pes(
-    hd: HarmonicDefect, x_shift=0, y_shift=0, width: float = 1.0, ax: Axes = None
+    hd: HarmonicDefect,
+    x_shift: float = 0,
+    y_shift: float = 0,
+    width: float = 1.0,
+    ax: Axes = None,
 ) -> None:
     """Plot the Potential Energy Surface of a HarmonicDefect.
 
     Args:
         hd: HarmonicDefect object
         x_shift: shift the PES by this amount in the x-direction
         y_shift: shift the PES by this amount in the y-direction
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/constants.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Constants used in the Defects module."""
 
-
 import numpy as np
 from scipy import constants
 
 HBAR_EV = constants.physical_constants["Planck constant over 2 pi in eV s"][0]
 HBAR_J = constants.physical_constants["Planck constant over 2 pi"][0]
 EV2J = constants.e  # 1 eV in Joules
 AMU2KG = constants.physical_constants["atomic mass constant"][0]
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/core.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Classes representing defects."""
+
 from __future__ import annotations
 
 import collections
 import logging
 from abc import ABCMeta, abstractmethod, abstractproperty
 from enum import Enum
-from typing import TYPE_CHECKING, Dict
+from typing import TYPE_CHECKING
 
 import numpy as np
 from monty.json import MSONable
 from pymatgen.analysis.defects.supercells import get_sc_fromstruct
 from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
 from pymatgen.core import Element, PeriodicSite, Species
 from pymatgen.core.periodic_table import DummySpecies
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+from typing_extensions import Self
 
 from .utils import get_plane_spacing
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
     from pymatgen.core import Structure
     from pymatgen.symmetry.structure import SymmetrizedStructure
@@ -31,14 +33,16 @@
 __author__ = "Jimmy-Xuan Shen"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy-Xuan Shen @jmmshn"
 __date__ = "Mar 15, 2022"
 
 _logger = logging.getLogger(__name__)
 
+RNG = np.random.default_rng(42)
+
 
 class DefectType(Enum):
     """Defect type, for sorting purposes."""
 
     Vacancy = 0
     Substitution = 1
     Interstitial = 2
@@ -87,15 +91,15 @@
             # Try to use the reduced cell first since oxidation state assignment
             # scales poorly with systems size.
             try:
                 self.structure.add_oxidation_state_by_guess(max_sites=-1)
                 # check oxi_states assigned and not all zero
                 if all(specie.oxi_state == 0 for specie in self.structure.species):
                     self.structure.add_oxidation_state_by_guess()
-            except Exception:
+            except Exception:  # noqa: BLE001 # pragma: no cover
                 self.structure.add_oxidation_state_by_guess()
             self.oxi_state = self._guess_oxi_state()
         else:
             self.oxi_state = oxi_state
 
     @abstractmethod
     def get_multiplicity(self) -> int:
@@ -122,15 +126,15 @@
         """Name of the defect."""
 
     @abstractproperty
     def defect_structure(self) -> Structure:
         """Get the unit-cell structure representing the defect."""
 
     @abstractproperty
-    def element_changes(self) -> Dict[Element, int]:
+    def element_changes(self) -> dict[Element, int]:
         """Get the species changes of the defect.
 
         Returns:
             Dict[Element, int]: The species changes of the defect.
         """
 
     @property
@@ -159,15 +163,22 @@
         """
         if self.user_charges:
             return self.user_charges
 
         if isinstance(self.oxi_state, int) or self.oxi_state.is_integer():
             oxi_state = int(self.oxi_state)
         else:  # pragma: no cover
-            raise ValueError("Oxidation state must be an integer")
+            sign = -1 if self.oxi_state < 0 else 1
+            oxi_state = sign * int(np.ceil(abs(self.oxi_state)))
+            _logger.warning(
+                "Non-integer oxidation state detected."
+                "Round to integer with larger absolute value: %s -> %s",
+                self.oxi_state,
+                oxi_state,
+            )
 
         if oxi_state >= 0:
             charges = [*range(-padding, oxi_state + padding + 1)]
         else:
             charges = [*range(oxi_state - padding, padding + 1)]
 
         return charges
@@ -222,16 +233,16 @@
             return_site: If True, returns a tuple of the (defect supercell, defect site position).
 
         Returns:
             Structure: The supercell structure.
             PeriodicSite (optional): The position of the defect site in the supercell.
         """
 
-        def _has_oxi(struct):
-            return all([hasattr(site.specie, "oxi_state") for site in struct])
+        def _has_oxi(struct: Structure) -> bool:
+            return all(hasattr(site.specie, "oxi_state") for site in struct)
 
         if defect_structure is None:
             defect_structure = self.centered_defect_structure
         bulk_structure = center_structure(self.structure, self.site.frac_coords)
         keep_oxi = _has_oxi(bulk_structure) and _has_oxi(defect_structure)
 
         if sc_mat is None:
@@ -268,15 +279,15 @@
 
         # Set the species for the sites that are mapped
         for defect_site, bulk_site in defect_site_mapping.items():
             sc_defect_struct[bulk_site]._species = defect_structure[defect_site].species
 
         # interstitials
         int_uc_indices = set(range(len(defect_structure))) - set(
-            defect_site_mapping.keys()
+            defect_site_mapping.keys(),
         )
         for i in int_uc_indices:
             int_sc_pos = np.dot(defect_structure[i].frac_coords, sc_mat_inv)
             sc_defect_struct.insert(
                 0,
                 defect_structure[i].specie,
                 int_sc_pos,
@@ -311,27 +322,30 @@
             return sc_defect_struct, sc_site
         return sc_defect_struct
 
     @property
     def symmetrized_structure(self) -> SymmetrizedStructure:
         """Get the symmetrized version of the bulk structure."""
         sga = SpacegroupAnalyzer(
-            self.structure, symprec=self.symprec, angle_tolerance=self.angle_tolerance
+            self.structure,
+            symprec=self.symprec,
+            angle_tolerance=self.angle_tolerance,
         )
         return sga.get_symmetrized_structure()
 
     def __eq__(self, __o: object) -> bool:
         """Equality operator."""
         if not isinstance(__o, Defect):  # pragma: no cover
-            raise TypeError("Can only compare Defects to Defects")
+            msg = "Can only compare Defects to Defects"
+            raise TypeError(msg)
         sm = StructureMatcher(comparator=ElementComparator())
         return sm.fit(self.defect_structure, __o.defect_structure)
 
     @property
-    def defect_type(self) -> int:
+    def defect_type(self) -> DefectType:
         """Get the defect type.
 
         Returns:
             int: The defect type.
         """
         return getattr(DefectType, self.__class__.__name__)
 
@@ -370,15 +384,17 @@
             element_changes: The species changes of the defect.
         """
         self.name = name
         self.bulk_formula = bulk_formula
         self.element_changes = element_changes
 
     @classmethod
-    def from_structures(cls, defect_structure: Structure, bulk_structure: Structure):
+    def from_structures(
+        cls, defect_structure: Structure, bulk_structure: Structure
+    ) -> Self:
         """Initialize a NameDefect object from structures.
 
         Args:
             defect_structure: The structure of the defect.
             bulk_structure: The structure of the bulk.
 
         Returns:
@@ -402,15 +418,16 @@
             root, suffix = n.split("_")
             l_names.append(rf"{root}$_{{\rm {suffix}}}$")
         return " + ".join(l_names)
 
     def __eq__(self, __value: object) -> bool:
         """Only need to compare names."""
         if not isinstance(__value, NamedDefect):  # pragma: no cover
-            raise TypeError("Can only compare NamedDefects to NamedDefects")
+            msg = "Can only compare NamedDefects to NamedDefects"
+            raise TypeError(msg)
         return self.__repr__() == __value.__repr__()
 
     def __repr__(self) -> str:
         """String representation of the NamedDefect."""
         return f'{self.bulk_formula}:{"+".join(sorted(self.name.split("+")))}'
 
 
@@ -433,38 +450,39 @@
 
     @property
     def name(self) -> str:
         """Name of the defect."""
         return f"v_{get_element(self.defect_site.specie)}"
 
     @property
-    def defect_site(self):
+    def defect_site(self) -> PeriodicSite:
         """Returns the site in the structure that corresponds to the defect site."""
-        res = min(
+        return min(
             self.structure.get_sites_in_sphere(
-                self.site.coords, 0.1, include_index=True
+                self.site.coords,
+                0.1,
+                include_index=True,
             ),
             key=lambda x: x[1],
         )
-        return res
 
     @property
     def defect_site_index(self) -> int:
         """Get the index of the defect in the structure."""
         return self.defect_site.index
 
     @property
-    def defect_structure(self):
+    def defect_structure(self) -> Structure:
         """Returns the defect structure with the proper oxidation state."""
         struct = self.structure.copy()
         struct.remove_sites([self.defect_site_index])
         return struct
 
     @property
-    def element_changes(self) -> Dict[Element, int]:
+    def element_changes(self) -> dict[Element, int]:
         """Get the species changes of the vacancy defect.
 
         Returns:
             Dict[Element, int]: The species changes of the defect.
         """
         return {get_element(self.structure.sites[self.defect_site_index].specie): -1}
 
@@ -537,30 +555,32 @@
             self.defect_site_index,
             species=insert_el,
             coords=np.mod(self.site.frac_coords, 1),
         )
         return struct
 
     @property
-    def defect_site(self):
+    def defect_site(self) -> PeriodicSite:
         """Returns the site in the structure that corresponds to the defect site."""
         return min(
             self.structure.get_sites_in_sphere(
-                self.site.coords, 0.1, include_index=True
+                self.site.coords,
+                0.1,
+                include_index=True,
             ),
             key=lambda x: x[1],
         )
 
     @property
     def defect_site_index(self) -> int:
         """Get the index of the defect in the structure."""
         return self.defect_site.index
 
     @property
-    def element_changes(self) -> Dict[Element, int]:
+    def element_changes(self) -> dict[Element, int]:
         """Get the species changes of the substitution defect.
 
         Returns:
             Dict[Element, int]: The species changes of the defect.
         """
         return {
             get_element(self.structure.sites[self.defect_site_index].specie): -1,
@@ -583,23 +603,26 @@
             site
             for site in self.structure
             if site.specie.symbol
             == self.site.specie.symbol  # gives Element symbol (without oxi state)
         ]
         if len(sub_elt_sites_in_struct) == 0:
             sub_states = self.site.specie.common_oxidation_states
-            if len(sub_states) == 0:
-                raise ValueError(
+            if len(sub_states) == 0:  # pragma: no cover
+                msg = (
                     f"No common oxidation states found for {self.site.specie}."
                     "Please specify the oxidation state manually."
                 )
+                raise ValueError(
+                    msg,
+                )
             sub_oxi = min(sub_states, key=lambda x: abs(x - rm_oxi))
         else:
             sub_oxi = int(
-                np.mean([site.specie.oxi_state for site in sub_elt_sites_in_struct])
+                np.mean([site.specie.oxi_state for site in sub_elt_sites_in_struct]),
             )
 
         return sub_oxi - rm_oxi
 
     def __repr__(self) -> str:
         """Representation of a substitutional defect."""
         rm_species = get_element(self.defect_site.specie)
@@ -632,21 +655,27 @@
             multiplicity: The multiplicity of the defect.
             oxi_state: The oxidation state of the defect, if not specified,
                 this will be determined automatically.
             equivalent_sites: A list of equivalent sites for the defect in the structure.
             **kwargs: Additional kwargs to pass to the Defect constructor.
         """
         super().__init__(
-            structure, site, multiplicity, oxi_state, equivalent_sites, **kwargs
+            structure,
+            site,
+            multiplicity,
+            oxi_state,
+            equivalent_sites,
+            **kwargs,
         )
 
     def get_multiplicity(self) -> int:
         """Determine the multiplicity of the defect site within the structure."""
+        msg = "Interstitial multiplicity should be determined by the generator."
         raise NotImplementedError(
-            "Interstitial multiplicity should be determined by the generator."
+            msg,
         )
 
     @property
     def name(self) -> str:
         """Name of the defect."""
         return f"{get_element(self.site.specie)}_i"
 
@@ -655,16 +684,17 @@
         """Returns the defect structure."""
         struct: Structure = self.structure.copy()
         # use the highest value oxidation state among the two most popular ones
         # found in the ICSD
         inter_states = self.site.specie.icsd_oxidation_states[:2]
         if len(inter_states) == 0:
             _logger.warning(
-                f"No oxidation states found for {self.site.specie.symbol}. "
-                "in ICSD using `oxidation_states` without frequency ranking."
+                "No oxidation states found for %s. "
+                "in ICSD using `oxidation_states` without frequency ranking.",
+                self.site.specie.symbol,
             )
             inter_states = self.site.specie.oxidation_states
         inter_oxi = max(inter_states, key=abs)
         int_specie = Species(self.site.specie.symbol, inter_oxi)
         struct.insert(
             0,
             species=int_specie,
@@ -674,15 +704,15 @@
 
     @property
     def defect_site_index(self) -> int:
         """Get the index of the defect in the structure."""
         return 0
 
     @property
-    def element_changes(self) -> Dict[Element, int]:
+    def element_changes(self) -> dict[Element, int]:
         """Get the species changes of the intersitial defect.
 
         Returns:
             Dict[Element, int]: The species changes of the defect.
         """
         return {
             get_element(self.site.specie): +1,
@@ -738,15 +768,16 @@
     def __repr__(self) -> str:
         """Representation of a complex defect."""
         return f"Complex defect containing: {[d.name for d in self.defects]}"
 
     def __eq__(self, __o: object) -> bool:
         """Check if  are equal."""
         if not isinstance(__o, Defect):
-            raise TypeError("Can only compare Defects to Defects")
+            msg = "Can only compare Defects to Defects"
+            raise TypeError(msg)
         sm = StructureMatcher(comparator=ElementComparator())
         this_structure = self.defect_structure_with_com
         if isinstance(__o, DefectComplex):
             that_structure = __o.defect_structure_with_com
         else:
             that_structure = __o.defect_structure
         return sm.fit(this_structure, that_structure)
@@ -756,20 +787,21 @@
         """Returns the defect structure with the center of mass as dummy site."""
         struct = self.defect_structure.copy()
         struct.insert(0, self.site.specie, self.site.frac_coords)
         return struct
 
     def get_multiplicity(self) -> int:
         """Determine the multiplicity of the defect site within the structure."""
+        msg = "Not implemented for defect complexes"
         raise NotImplementedError(
-            "Not implemented for defect complexes"
+            msg,
         )  # pragma: no cover
 
     @property
-    def element_changes(self) -> Dict[Element, int]:
+    def element_changes(self) -> dict[Element, int]:
         """Determine the species changes of the complex defect."""
         cnt: dict[Element, int] = collections.defaultdict(int)
         for defect in self.defects:
             for el, change in defect.element_changes.items():
                 cnt[el] += change
         return dict(cnt)
 
@@ -786,26 +818,30 @@
 
     @property
     def defect_structure(self) -> Structure:
         """Returns the defect structure."""
         defect_structure = self.structure.copy()
         for defect in self.defects:
             update_structure(
-                defect_structure, defect.site, defect_type=defect.defect_type
+                defect_structure,
+                defect.site,
+                defect_type=defect.defect_type,
             )
         return defect_structure
 
     @property
     def latex_name(self) -> str:
         """Get the latex name of the defect."""
         single_names = [d.latex_name for d in self.defects]
         return "$+$".join(single_names)
 
 
-def update_structure(structure, site, defect_type):
+def update_structure(
+    structure: Structure, site: PeriodicSite, defect_type: DefectType
+) -> None:
     """Update the structure with the defect site.
 
     Types of operations:
         1. Vacancy: remove the site.
         2. Substitution: replace the site with the defect species.
         3. Interstitial: insert the defect species at the site.
 
@@ -814,19 +850,22 @@
         site: The defect site.
         defect_type: The type of the defect.
 
     Returns:
         Structure: The updated structure.
     """
 
-    def _update(structure, site, rm: bool, replace: bool):
+    def _update(
+        structure: Structure, site: PeriodicSite, rm: bool, replace: bool
+    ) -> None:
         in_sphere = structure.get_sites_in_sphere(site.coords, 0.1, include_index=True)
 
         if len(in_sphere) == 0 and rm:  # pragma: no cover
-            raise ValueError("No site found to remove.")
+            msg = "No site found to remove."
+            raise ValueError(msg)
 
         if rm or replace:
             rm_site = min(
                 in_sphere,
                 key=lambda x: x[1],
             )
             rm_index = rm_site.index
@@ -845,15 +884,16 @@
     if defect_type == DefectType.Vacancy:
         _update(structure, site, rm=True, replace=False)
     elif defect_type == DefectType.Substitution:
         _update(structure, site, rm=False, replace=True)
     elif defect_type == DefectType.Interstitial:
         _update(structure, site, rm=False, replace=False)
     else:
-        raise ValueError("Unknown point defect type.")  # pragma: no cover
+        msg = "Unknown point defect type."
+        raise ValueError(msg)  # pragma: no cover
 
 
 class Adsorbate(Interstitial):
     """Subclass of Interstitial with a different name.
 
     Used for keeping track of adsorbate, which are treated the same
     algorithmically as interstitials, but are conceptually separate.
@@ -889,16 +929,18 @@
         **kwargs: Keyword arguments to pass to Vacancy constructor.
     """
     site = structure[isite]
     return Vacancy(structure=structure, site=site, **kwargs)
 
 
 def _set_selective_dynamics(
-    structure: Structure, site_pos: ArrayLike, relax_radius: float | str | None
-):
+    structure: Structure,
+    site_pos: ArrayLike,
+    relax_radius: float | str | None,
+) -> None:
     """Set the selective dynamics behavior.
 
     Allow atoms to move for sites within a given radius of a given site,
     all other atoms are fixed.  Modify the structure in place.
 
     Args:
         structure: The structure to set the selective dynamics.
@@ -906,28 +948,31 @@
         relax_radius: The radius of the relaxation sphere.
     """
     if relax_radius is None:
         return
     if relax_radius == "auto":
         relax_radius = min(get_plane_spacing(structure.lattice.matrix)) / 2.0
     if not isinstance(relax_radius, float):
-        raise ValueError("relax_radius must be a float or 'auto' or None")
+        msg = "relax_radius must be a float or 'auto' or None"
+        raise ValueError(msg)
     structure.get_sites_in_sphere(site_pos, relax_radius)
     relax_sites = structure.get_sites_in_sphere(
-        site_pos, relax_radius, include_index=True
+        site_pos,
+        relax_radius,
+        include_index=True,
     )
     relax_indices = [site.index for site in relax_sites]
     relax_mask = [[False, False, False]] * len(structure)
     for i in relax_indices:
         relax_mask[i] = [True, True, True]
     structure.add_site_property("selective_dynamics", relax_mask)
 
 
 def perturb_sites(
-    structure,
+    structure: Structure,
     distance: float,
     min_distance: float | None = None,
     site_indices: list | None = None,
 ) -> None:
     """Performs a random perturbation.
 
     Perturb the sites in a structure to break symmetry.  This is useful for
@@ -942,42 +987,44 @@
             distance drawn from the uniform distribution between
             'min_distance' and 'distance'.
         site_indices (list): List of site indices on which to perform the
             perturbation. If None, all sites will be perturbed.
 
     """
 
-    def get_rand_vec():
+    def get_rand_vec() -> ArrayLike:
         # deals with zero vectors.
-        vector = np.random.randn(3)
+        vector = RNG.normal(size=3)
         vnorm = np.linalg.norm(vector)
         dist = distance
         if isinstance(min_distance, (float, int)):
-            dist = np.random.uniform(min_distance, dist)
+            dist = RNG.uniform(min_distance, dist)
         return vector / vnorm * dist if vnorm != 0 else get_rand_vec()
 
     if site_indices is None:
         site_indices_ = list(range(len(structure._sites)))
     else:
         site_indices_ = site_indices
 
     for i in site_indices_:
         structure.translate_sites([i], get_rand_vec(), frac_coords=False)
 
 
-def _perturb_dynamic_sites(structure, distance):
+def _perturb_dynamic_sites(structure: Structure, distance: float) -> None:
     free_indices = [
         i
         for i, site in enumerate(structure)
         if site.properties["selective_dynamics"][0]
     ]
     perturb_sites(structure=structure, distance=distance, site_indices=free_indices)
 
 
-def _get_mapped_sites(uc_structure: Structure, sc_structure: Structure, r=0.001):
+def _get_mapped_sites(
+    uc_structure: Structure, sc_structure: Structure, r: float = 0.001
+) -> dict:
     """Get the list of sites indices in the supercell corresponding to the unit cell."""
     mapped_site_indices = {}
     for isite, uc_site in enumerate(uc_structure):
         sc_sites = sc_structure.get_sites_in_sphere(uc_site.coords, r)
         if len(sc_sites) == 1:
             mapped_site_indices[isite] = sc_sites[0].index
     return mapped_site_indices
@@ -1009,27 +1056,28 @@
         defect_sc: The defect structure.
         bulk_sc: The bulk structure.
 
     Returns:
         dict: A dictionary representing the species changes in creating the defect.
     """
 
-    def _check_int(n):
+    def _check_int(n: float) -> bool:
         return isinstance(n, int) or n.is_integer()
 
     comp_defect = defect_sc.composition.element_composition
     comp_bulk = bulk_sc.composition.element_composition
 
     # get the element changes
     el_diff = {}
     for el, cnt in comp_defect.items():
         # has to be integer
         if not (_check_int(comp_bulk[el]) and _check_int(cnt)):
+            msg = "Defect structure and bulk structure must have integer compositions."
             raise ValueError(
-                "Defect structure and bulk structure must have integer compositions."
+                msg,
             )
         tmp_ = int(cnt) - int(comp_bulk[el])
         if tmp_ != 0:
             el_diff[el] = tmp_
     return el_diff
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Freysoldt defect corrections module."""
 
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 from pymatgen.analysis.defects.finder import DefectSiteFinder
 from pymatgen.analysis.defects.utils import (
     CorrectionResult,
     QModel,
     ang_to_bohr,
     converge,
     eV_to_k,
     generate_reciprocal_vectors_squared,
     hart_to_ev,
 )
-from pymatgen.io.vasp.outputs import Locpot
+from pymatgen.io.vasp.outputs import Locpot, VolumetricData
 from scipy import stats
 
 if TYPE_CHECKING:
+    from matplotlib.axes import Axes
     from numpy.typing import ArrayLike
     from pymatgen.core import Lattice
 
 __author__ = "Jimmy-Xuan Shen, Danny Broberg, Shyam Dwaraknath"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy-Xuan Shen"
 __email__ = "jmmshn@gmail.com"
@@ -40,19 +41,19 @@
 
 
 def get_freysoldt_correction(
     q: int,
     dielectric: float,
     defect_locpot: Locpot,
     bulk_locpot: Locpot,
-    defect_frac_coords: Optional[ArrayLike] = None,
-    lattice: Optional[Lattice] = None,
+    defect_frac_coords: ArrayLike | None = None,
+    lattice: Lattice | None = None,
     energy_cutoff: float = 520,
     mad_tol: float = 1e-4,
-    q_model: Optional[QModel] = None,
+    q_model: QModel | None = None,
     step: float = 1e-4,
 ) -> CorrectionResult:
     """Gets the Freysoldt correction for a defect entry.
 
     Args:
         q:
             Charge state of defect
@@ -93,70 +94,76 @@
     # dielectric has to be a float
     if isinstance(dielectric, (int, float)):
         dielectric = float(dielectric)
     elif np.ndim(dielectric) == 1:  # pragma: no cover
         dielectric = float(np.mean(dielectric))
     elif np.ndim(dielectric) == 2:  # pragma: no cover
         dielectric = float(np.mean(dielectric.diagonal()))
-    else:
+    else:  # pragma: no cover
+        msg = f"Dielectric constant cannot be converted into a scalar. Currently of type {type(dielectric)}"
         raise ValueError(
-            f"Dielectric constant is cannot be converted into a scalar. Currently of type {type(dielectric)}"
+            msg,
         )
 
     q_model = QModel() if q_model is None else q_model
 
-    if isinstance(defect_locpot, Locpot):
+    if isinstance(defect_locpot, VolumetricData):
         list_axis_grid = [*map(defect_locpot.get_axis_grid, [0, 1, 2])]
         list_defect_plnr_avg_esp = [
-            *map(defect_locpot.get_average_along_axis, [0, 1, 2])
+            *map(defect_locpot.get_average_along_axis, [0, 1, 2]),
         ]
         lattice_ = defect_locpot.structure.lattice.copy()
         if lattice is not None and lattice != lattice_:
+            msg = "Lattice of defect_locpot and user provided lattice do not match."
             raise ValueError(
-                "Lattice of defect_locpot and user provided lattice do not match."
+                msg,
             )
         lattice = lattice_
     elif isinstance(defect_locpot, dict):
         defect_locpot_ = {int(k): v for k, v in defect_locpot.items()}
         list_defect_plnr_avg_esp = [defect_locpot_[i] for i in range(3)]
         list_axis_grid = [
             *map(
                 np.linspace,
                 [0, 0, 0],
                 lattice.abc,
                 [len(i) for i in list_defect_plnr_avg_esp],
-            )
+            ),
         ]
     else:
-        raise ValueError("defect_locpot must be of type Locpot or dict")
+        msg = "defect_locpot must be of type Locpot or dict"
+        raise ValueError(msg)
 
-    # TODO this can be done with regridding later
-    if isinstance(bulk_locpot, Locpot):
+    if isinstance(bulk_locpot, VolumetricData):
         list_bulk_plnr_avg_esp = [*map(bulk_locpot.get_average_along_axis, [0, 1, 2])]
     elif isinstance(bulk_locpot, dict):
         bulk_locpot_ = {int(k): v for k, v in bulk_locpot.items()}
         list_bulk_plnr_avg_esp = [bulk_locpot_[i] for i in range(3)]
-    else:
-        raise ValueError("bulk_locpot must be of type Locpot or dict")
+    else:  # pragma: no cover
+        msg = "bulk_locpot must be of type Locpot or dict"
+        raise ValueError(msg)
 
     es_corr = perform_es_corr(
         lattice=lattice,
         q=q,
         dielectric=dielectric,
         q_model=q_model,
         energy_cutoff=energy_cutoff,
         mad_tol=mad_tol,
         step=step,
     )
 
-    alignment_corrs = dict()
-    plot_data = dict()
+    alignment_corrs = {}
+    plot_data = {}
 
     for x, pureavg, defavg, axis in zip(
-        list_axis_grid, list_bulk_plnr_avg_esp, list_defect_plnr_avg_esp, [0, 1, 2]
+        list_axis_grid,
+        list_bulk_plnr_avg_esp,
+        list_defect_plnr_avg_esp,
+        [0, 1, 2],
     ):
         alignment_corr, md = perform_pot_corr(
             axis_grid=x,
             pureavg=pureavg,
             defavg=defavg,
             lattice=lattice,
             q=q,
@@ -182,15 +189,21 @@
             "mean_alignments": mean_alignment,
             "potential": pot_corr,
         },
     )
 
 
 def perform_es_corr(
-    lattice, q, dielectric, q_model, energy_cutoff=520, mad_tol=1e-4, step=1e-4
+    lattice: Lattice,
+    q: float,
+    dielectric: float,
+    q_model: QModel,
+    energy_cutoff: float = 520,
+    mad_tol: float = 1e-4,
+    step: float = 1e-4,
 ) -> float:
     """Perform Electrostatic Freysoldt Correction.
 
     Perform the electrostatic Freysoldt correction for a defect.
 
     Args:
         lattice: Pymatgen lattice object
@@ -202,32 +215,32 @@
         step: Step size for numerical integration
 
     Return:
         float:
             Electrostatic Point Charge contribution to Freysoldt Correction (float)
     """
     _logger.info(
-        "Running Freysoldt 2011 PC calculation (should be equivalent to sxdefectalign)"
+        "Running Freysoldt 2011 PC calculation (should be equivalent to sxdefectalign)",
     )
-    _logger.debug("defect lattice constants are (in angstroms)" + str(lattice.abc))
+    _logger.debug("defect lattice constants are (in angstroms) %s", str(lattice.abc))
 
     [a1, a2, a3] = ang_to_bohr * np.array(lattice.get_cartesian_coords(1))
-    logging.debug("In atomic units, lat consts are (in bohr):" + str([a1, a2, a3]))
+    logging.debug("In atomic units, lat consts are (in bohr): %s", str([a1, a2, a3]))
     vol = np.dot(a1, np.cross(a2, a3))  # vol in bohr^3
 
-    def e_iso(encut):
+    def e_iso(encut: float) -> float:
         gcut = eV_to_k(encut)  # gcut is in units of 1/A
         return (
             scipy.integrate.quad(lambda g: q_model.rho_rec(g * g) ** 2, step, gcut)[0]
             * (q**2)
             / np.pi
         )
 
-    def e_per(encut):
-        eper = 0
+    def e_per(encut: float) -> float:
+        eper = 0.0
         for g2 in generate_reciprocal_vectors_squared(a1, a2, a3, encut):
             eper += (q_model.rho_rec(g2) ** 2) / g2
         eper *= (q**2) * 2 * round(np.pi, 6) / vol
         eper += (q**2) * 4 * round(np.pi, 6) * q_model.rho_rec_limit0 / vol
         return eper
 
     eiso = converge(e_iso, 5, mad_tol, energy_cutoff)
@@ -241,26 +254,26 @@
 
     es_corr = round((eiso - eper) / dielectric * hart_to_ev, 6)
     _logger.info("Defect Correction without alignment %f (eV): ", es_corr)
     return es_corr
 
 
 def perform_pot_corr(
-    axis_grid,
-    pureavg,
-    defavg,
-    lattice,
-    q,
-    defect_frac_coords,
-    axis,
-    dielectric,
-    q_model,
-    mad_tol=1e-4,
-    widthsample=1.0,
-):
+    axis_grid: ArrayLike,
+    pureavg: ArrayLike,
+    defavg: ArrayLike,
+    lattice: Lattice,
+    q: float,
+    defect_frac_coords: ArrayLike,
+    axis: Axes,
+    dielectric: float,
+    q_model: QModel,
+    mad_tol: float = 1e-4,
+    widthsample: float = 1.0,
+) -> tuple[float, dict]:
     """For performing planar averaging potential alignment.
 
     Args:
         axis_grid:
             (1 x NGX where NGX is the length of the NGX grid
             in the axis direction. Same length as pureavg list)
             A numpy array which contain the Cartesian axis
@@ -286,15 +299,15 @@
         widthsample (float): width (in Angstroms) of the region in between defects
             where the potential alignment correction is averaged. Default is 1 Angstrom.
 
     Returns:
         (float) Potential Alignment shift required to make the short range potential
         zero far from the defect.  (-C) in the Freysoldt paper.
     """
-    logging.debug("run Freysoldt potential alignment method for axis " + str(axis))
+    logging.debug("run Freysoldt potential alignment method for axis %s", str(axis))
     nx = len(axis_grid)
 
     # shift these planar averages to have defect at origin
     axfracval = defect_frac_coords[axis]
     axbulkval = axfracval * lattice.abc[axis]
     if axbulkval < 0:
         axbulkval += lattice.abc[axis]
@@ -323,15 +336,16 @@
     v_G[1:] = 4 * np.pi / (dielectric * g2) * -q * q_model.rho_rec(g2)
     v_G[nx // 2] = 0 if not (nx % 2) else v_G[nx // 2]
 
     # Get the real space potential via fft and grabbing the imaginary portion
     v_R = np.fft.fft(v_G)
 
     if abs(np.imag(v_R).max()) > mad_tol:
-        raise Exception("imaginary part found to be %s", repr(np.imag(v_R).max()))
+        msg = "imaginary part found to be %s"
+        raise Exception(msg, repr(np.imag(v_R).max()))
     v_R /= lattice.volume * ang_to_bohr**3
     v_R = np.real(v_R) * hart_to_ev
 
     # get correction
     short = (
         np.array(defavg, dtype=float)
         - np.array(pureavg, dtype=float)
@@ -347,21 +361,21 @@
         axis_grid[mid - checkdis],
         axis_grid[mid + checkdis],
     )
 
     C = np.mean(tmppot)
     _logger.debug("C = %f", C)
     short_range = short
-    v_R = [elmnt for elmnt in v_R]
+    v_R = list(v_R)
 
     _logger.info("C value is averaged to be %f eV ", C)
     _logger.info("Potentital alignment energy correction (q * Delta):  %f (eV)", q * C)
 
     # log plotting data:
-    metadata = dict()
+    metadata = {}
     metadata["pot_plot_data"] = {
         "Vr": v_R,
         "x": axis_grid,
         "dft_diff": np.array(defavg) - np.array(pureavg),
         "short_range": short_range,
         "shift": C,
         "check": [mid - checkdis, mid + checkdis + 1],
@@ -370,30 +384,33 @@
     metadata["pot_corr_uncertainty_md"] = {
         "stats": stats.describe(tmppot)._asdict(),
         "potcorr": C,
     }
     return C, metadata
 
 
-def plot_plnr_avg(plot_data, title=None, saved=False, ax=None):
+def plot_plnr_avg(
+    plot_data: dict, title: str | None = None, saved: bool = False, ax: Axes = None
+) -> Axes:
     """Plot the planar average electrostatic potential.
 
     Plot the planar average electrostatic potential against the Long range and
     short range models from Freysoldt. Must run perform_pot_corr or get_correction
     (to load metadata) before this can be used.
 
     Args:
         plot_data (dict): Dictionary of FreysoldtCorrection metadata.
         title (str): Title to be given to plot. Default is no title.
         saved (bool): Whether to save file or not. If False then returns plot object.
             If True then saves plot as   str(title) + "FreyplnravgPlot.pdf"
         ax (matplotlib.axes.Axes): Axes object to plot on. If None, makes new figure.
     """
-    if not plot_data["pot_plot_data"]:
-        raise ValueError("Cannot plot potential alignment before running correction!")
+    if not plot_data["pot_plot_data"]:  # pragma: no cover
+        msg = "Cannot plot potential alignment before running correction!"
+        raise ValueError(msg)
 
     x = plot_data["pot_plot_data"]["x"]
     v_R = plot_data["pot_plot_data"]["Vr"]
     dft_diff = plot_data["pot_plot_data"]["dft_diff"]
     short_range = plot_data["pot_plot_data"]["short_range"]
     check = plot_data["pot_plot_data"]["check"]
     C = plot_data["pot_plot_data"]["shift"]
@@ -404,24 +421,29 @@
     ax.plot(x, dft_diff, c="red", label="DFT locpot diff")
     ax.plot(x, short_range, c="green", label="short range (not aligned)")
     ax.axhline(C, color="k", linestyle="--")
     ax.text(4, C, f"C={C:0.3f}", va="bottom")
 
     tmpx = [x[i] for i in range(check[0], check[1])]
     ax.fill_between(
-        tmpx, -100, 100, facecolor="red", alpha=0.15, label="sampling region"
+        tmpx,
+        -100,
+        100,
+        facecolor="red",
+        alpha=0.15,
+        label="sampling region",
     )
 
     ax.set_xlim(round(x[0]), round(x[-1]))
-    ymin = min(min(v_R), min(dft_diff), min(short_range))
-    ymax = max(max(v_R), max(dft_diff), max(short_range))
+    ymin = min(v_R + dft_diff + short_range)
+    ymax = max(v_R + dft_diff + short_range)
     ax.set_ylim(-0.2 + ymin, 0.2 + ymax)
     ax.set_xlabel(r"distance along axis ($\AA$)", fontsize=15)
     ax.set_ylabel("Potential (V)", fontsize=15)
     ax.legend(loc=9)
     ax.axhline(y=0, linewidth=0.2, color="black")
-    if title is not None:
+    if title is not None:  # pragma: no cover
         ax.set_title(str(title), fontsize=18)
     ax.set_xlim(0, max(x))
-    if saved:
+    if saved:  # pragma: no cover
         fig.savefig(str(title) + "FreyplnravgPlot.pdf")
     return ax
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,19 +34,20 @@
 __maintainer__ = "Jimmy-Xuan Shen"
 __email__ = "jmmshn@gmail.com"
 _logger = logging.getLogger(__name__)
 # suppress pydefect INFO messages
 logging.getLogger("pydefect").setLevel(logging.WARNING)
 
 
-def _check_import_pydefect():
+def _check_import_pydefect() -> None:
     """Import pydefect if it is installed."""
     if __has_pydefect__:
+        msg = "vise/pydefect is not installed. Please install it first."
         raise ModuleNotFoundError(
-            "vise/pydefect is not installed. Please install it first."
+            msg,
         )
 
 
 def get_structure_with_pot(directory: Path) -> Structure:
     """Reads vasprun.xml and OUTCAR files in a directory.
 
     Args:
@@ -67,16 +68,15 @@
         energy=outcar.final_energy,
         magnetization=outcar.total_mag or 0.0,
         potentials=[-p for p in outcar.electrostatic_potential],
         electronic_conv=vasprun.converged_electronic,
         ionic_conv=vasprun.converged_ionic,
     )
 
-    struct = calc.structure.copy(site_properties={"potential": calc.potentials})
-    return struct
+    return calc.structure.copy(site_properties={"potential": calc.potentials})
 
 
 def get_efnv_correction(
     charge: int,
     defect_structure: Structure,
     bulk_structure: Structure,
     dielectric_tensor: list[list[float]],
@@ -114,9 +114,10 @@
         calc_results=defect_calc_results,
         perfect_calc_results=bulk_calc_results,
         dielectric_tensor=dielectric_tensor,
         **kwargs,
     )
 
     return CorrectionResult(
-        correction_energy=efnv_corr.correction_energy, metadata={"efnv_corr": efnv_corr}
+        correction_energy=efnv_corr.correction_energy,
+        metadata={"efnv_corr": efnv_corr},
     )
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/finder.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Defect position identification without prior knowledge."""
+
 from __future__ import annotations
 
 import logging
-import warnings
-from collections import namedtuple
-from typing import TYPE_CHECKING, List, Tuple
+from typing import TYPE_CHECKING, NamedTuple
 
 import numpy as np
 from monty.json import MSONable
 from pymatgen.io.ase import AseAtomsAdaptor
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
 if TYPE_CHECKING:
@@ -26,41 +25,55 @@
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy Shen @jmmshn"
 __date__ = "Jan 24, 2022"
 
 _logger = logging.getLogger(__name__)
 DUMMY_SPECIES = "Si"
 
-SiteVec = namedtuple("SiteVec", ["species", "site", "vec"])
-SiteGroup = namedtuple("SiteGroup", ["species", "similar_sites", "vec"])
+
+class SiteVec(NamedTuple):
+    """NamedTuple representing a site in the defect structure."""
+
+    species: str
+    site: Structure
+    vec: NDArray
+
+
+class SiteGroup(NamedTuple):
+    """NamedTuple representing a group of symmetrically equivalent sites."""
+
+    species: str
+    similar_sites: list[int]
+    vec: NDArray
 
 
 class DefectSiteFinder(MSONable):
     """Find the location of a defect with no pior knowledge."""
 
-    def __init__(self, symprec: float = 0.01, angle_tolerance: float = 5.0):
+    def __init__(self, symprec: float = 0.01, angle_tolerance: float = 5.0) -> None:
         """Configure the behavior of the defect site finder.
 
         Args:
             symprec (float): Symmetry tolerance parameter for SpacegroupAnalyzer
             angle_tolerance (float): Angle tolerance parameter for SpacegroupAnalyzer
         """
         if SOAP is None:
+            msg = "dscribe is required to use DefectSiteFinder. Install with ``pip install dscribe``."
             raise ImportError(
-                "dscribe is required to use DefectSiteFinder. Install with ``pip install dscribe``."
+                msg,
             )
         self.symprec = symprec
         self.angle_tolerance = angle_tolerance
 
     def get_defect_fpos(
         self,
-        defect_structure: "Structure",
-        base_structure: "Structure",
+        defect_structure: Structure,
+        base_structure: Structure,
         remove_oxi: bool = True,
-    ) -> "ArrayLike":
+    ) -> ArrayLike:
         """Get the position of a defect in the pristine structure.
 
         Args:
             defect_structure: Relaxed structure containing the defect
             base_structure: Structure for the pristine cell
             remove_oxi: Whether to remove oxidation states from the structures
 
@@ -70,19 +83,20 @@
         """
         if remove_oxi:
             defect_structure.remove_oxidation_states()
             base_structure.remove_oxidation_states()
 
         if self._is_impurity(defect_structure, base_structure):
             return self.get_impurity_position(defect_structure, base_structure)
-        else:
-            return self.get_native_defect_position(defect_structure, base_structure)
+        return self.get_native_defect_position(defect_structure, base_structure)
 
     def _is_impurity(
-        self, defect_structure: "Structure", base_structure: "Structure"
+        self,
+        defect_structure: Structure,
+        base_structure: Structure,
     ) -> bool:
         """Check if the defect structure is an impurity.
 
         Args:
             defect_structure: Structure containing the defect
             base_structure: Structure for the pristine cell
 
@@ -91,37 +105,43 @@
         """
         # check if the defect structure is an impurity
         base_species = {site.species_string for site in base_structure}
         defect_species = {site.species_string for site in defect_structure}
         return len(defect_species - base_species) > 0
 
     def get_native_defect_position(
-        self, defect_structure: "Structure", base_structure: "Structure"
-    ) -> "ArrayLike":
+        self,
+        defect_structure: Structure,
+        base_structure: Structure,
+    ) -> ArrayLike:
         """Get the position of a native defect in the defect structure.
 
         Args:
             defect_structure: Relaxed structure containing the defect
             base_structure: Pristine structure without the defect
 
         Returns:
             ArrayLike: Position of the defect in the defect structure
             (in fractional coordinates)
         """
         distored_sites, distortions = list(
-            zip(*self.get_most_distorted_sites(defect_structure, base_structure))
+            zip(*self.get_most_distorted_sites(defect_structure, base_structure)),
         )
         positions = [defect_structure[isite].frac_coords for isite in distored_sites]
         return get_weighted_average_position(
-            defect_structure.lattice, positions, distortions
+            defect_structure.lattice,
+            positions,
+            distortions,
         )
 
     def get_impurity_position(
-        self, defect_structure: "Structure", base_structure: "Structure"
-    ):
+        self,
+        defect_structure: Structure,
+        base_structure: Structure,
+    ) -> ArrayLike:
         """Get the position of an impurity defect.
 
         Look at all sites with impurity atoms, and take the average of the positions of
         the sites.
 
         Args:
             defect_structure: Relaxed structure containing the defect
@@ -129,23 +149,26 @@
 
         Returns:
             ArrayLike: Position of the defect in the defect structure
         """
         # get the pbc average position of all sites not in the base structure
         base_species = {site.species_string for site in base_structure}
         impurity_sites = [
-            *filter(lambda x: x.species_string not in base_species, defect_structure)
+            *filter(lambda x: x.species_string not in base_species, defect_structure),
         ]
         return get_weighted_average_position(
-            defect_structure.lattice, [s.frac_coords for s in impurity_sites]
+            defect_structure.lattice,
+            [s.frac_coords for s in impurity_sites],
         )
 
     def get_most_distorted_sites(
-        self, defect_structure: "Structure", base_structure: "Structure"
-    ) -> List[Tuple[int, float]]:
+        self,
+        defect_structure: Structure,
+        base_structure: Structure,
+    ) -> list[tuple[int, float]]:
         """Identify the set of sites with the most deviation from the pristine.
 
         Performs the following steps:
 
         1. For each site in the defect structure, find the closest site in the
             pristine structure.
         2. Then, compute a distortion field based on SOAP vectors.
@@ -170,29 +193,31 @@
         res = []
         for i, v in enumerate(defect_vecs):
             (
                 best_m,
                 best_s,
             ) = best_match(v, pristine_groups)
             if v.species != best_m.species:
-                warnings.warn(
+                _logger.warning(
                     "The species of a site in the distorted structure is different "
-                    "from the species of the closest pristine site."
+                    "from the species of the closest pristine site.",
                 )
 
             res.append((i, np.abs(best_s - 1)))
 
         res.sort(key=lambda x: x[1], reverse=True)
         deviations = [r[1] for r in res]
         bound = _get_broundary(deviations)
         return res[:bound]
 
 
 # %%
-def get_site_groups(struct, symprec=0.01, angle_tolerance=5.0) -> List[SiteGroup]:
+def get_site_groups(
+    struct: Structure, symprec: float = 0.01, angle_tolerance: float = 5.0
+) -> list[SiteGroup]:
     """Group the sites in the structure by symmetry.
 
     Group the sites in the structure by symmetry and return a
     list of ``SiteGroup`` namedtuples.
 
     Args:
         struct: Structure object to be analyzed
@@ -207,21 +232,23 @@
     sa = SpacegroupAnalyzer(struct, symprec=symprec, angle_tolerance=angle_tolerance)
     sstruct = sa.get_symmetrized_structure()
     site_groups = []
     groups = sstruct.equivalent_indices
     soap_vec = get_soap_vec(struct)
     for g in groups:
         sg = SiteGroup(
-            species=sstruct[g[0]].species_string, similar_sites=g, vec=soap_vec[g[0]]
+            species=sstruct[g[0]].species_string,
+            similar_sites=g,
+            vec=soap_vec[g[0]],
         )
         site_groups.append(sg)
     return site_groups
 
 
-def get_soap_vec(struct: "Structure") -> NDArray:
+def get_soap_vec(struct: Structure) -> NDArray:
     """Get the SOAP vector for each site in the structure.
 
     Args:
         struct: Structure object to compute the SOAP vector for
 
     Returns:
         NDArray: SOAP vector for each site in the structure,
@@ -229,19 +256,18 @@
     """
     adaptor = AseAtomsAdaptor()
     species_ = [str(el) for el in struct.composition.elements]
     dummy_structure = struct.copy()
     for el in species_:
         dummy_structure.replace_species({str(el): DUMMY_SPECIES})
     soap_desc = SOAP(species=[DUMMY_SPECIES], r_cut=5, n_max=8, l_max=6, periodic=True)
-    vecs = soap_desc.create(adaptor.get_atoms(dummy_structure))
-    return vecs
+    return soap_desc.create(adaptor.get_atoms(dummy_structure))
 
 
-def get_site_vecs(struct: Structure) -> List[SiteVec]:
+def get_site_vecs(struct: Structure) -> list[SiteVec]:
     """Get the SiteVec representation of each site in the structure.
 
     Args:
         struct: Structure object to compute the site vectors (SOAP).
 
     Returns:
         List[SiteVec]: List of SiteVec representing each site in the structure.
@@ -249,28 +275,28 @@
     vecs = get_soap_vec(struct)
     return [
         SiteVec(species=site.species_string, site=site, vec=vecs[i])
         for i, site in enumerate(struct)
     ]
 
 
-def cosine_similarity(vec1, vec2) -> float:
+def cosine_similarity(vec1: ArrayLike, vec2: ArrayLike) -> float:
     """Cosine similarity between two vectors.
 
     Args:
         vec1: First vector
         vec2: Second vector
 
     Returns:
         float: Cosine similarity between the two vectors
     """
     return np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2))
 
 
-def best_match(sv: SiteVec, sgs: List[SiteGroup]) -> Tuple[SiteGroup, float]:
+def best_match(sv: SiteVec, sgs: list[SiteGroup]) -> tuple[SiteGroup, float]:
     """Find the best match for a site in the defect structure.
 
     Args:
         sv: SiteVec namedtuples representing a site in the defect structure
         sgs: List of SiteGroup namedtuples representing groups of
         symmetrically equivalent sites in the pristine structure
 
@@ -285,19 +311,20 @@
         if sv.species != sg.species:
             continue
         csim = cosine_similarity(sv.vec, sg.vec)
         if csim > best_similarity:
             best_similarity = csim
             best_match = sg
     if best_match is None:
-        raise ValueError("No matching species found.")
+        msg = "No matching species found."
+        raise ValueError(msg)
     return best_match, best_similarity
 
 
-def _get_broundary(arr, n_max=16, n_skip=3) -> int:
+def _get_broundary(arr: list, n_max: int = 16, n_skip: int = 3) -> int:
     """Get the boundary index for the high-distortion indices.
 
     Assuming arr is sorted in reverse order,
     find the biggest value drop in arr[n_skip:n_max].
 
     Args:
         arr: List of numbers
@@ -309,15 +336,17 @@
     """
     sub_arr = np.array(arr[n_skip:n_max])
     diffs = sub_arr[1:] - sub_arr[:-1]
     return np.argmin(diffs) + n_skip + 1
 
 
 def get_weighted_average_position(
-    lattice: Lattice, frac_positions: ArrayLike, weights: ArrayLike | None = None
+    lattice: Lattice,
+    frac_positions: ArrayLike,
+    weights: ArrayLike | None = None,
 ) -> NDArray:
     """Get the weighted average position of a set of positions in frac coordinates.
 
     The algorithm starts at position with the highest weight, and gradually moves
     the average point by finding the closest image of each additional position to the
     average point. This can be used to find the center of mass of a group of sites in a
     molecule in CH3NH3PbI3 (Note: Since the average positions in periodic system is not
@@ -333,15 +362,16 @@
     Returns:
     -------
         NDArray: (3x1 array): The weighted average position in fractional coordinates.
     """
     if weights is None:
         weights = [1.0] * len(frac_positions)
     if len(frac_positions) != len(weights):
-        raise ValueError("The number of positions and weights must be the same.")
+        msg = "The number of positions and weights must be the same."
+        raise ValueError(msg)
 
     # TODO: can be replaced with the zip(..., strict=True) syntax in Python 3.10
     pos_weights = list(zip(frac_positions, weights))
     pos_weights.sort(key=lambda x: x[1], reverse=True)
 
     # initial guess at the center with zero weight
     p_guess = np.ones(3) * 0.5
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/generators.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 from __future__ import annotations
 
 import collections
 import itertools
 import logging
 from abc import ABCMeta
 from itertools import combinations
-from typing import TYPE_CHECKING, Generator
+from typing import TYPE_CHECKING
 
 from monty.json import MSONable
 from pymatgen.analysis.defects.core import Interstitial, Substitution, Vacancy
 from pymatgen.analysis.defects.utils import (
     ChargeInsertionAnalyzer,
     TopographyAnalyzer,
     remove_collisions,
 )
 from pymatgen.core import Element, PeriodicSite, Species, Structure
 from pymatgen.io.vasp import Chgcar
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
 if TYPE_CHECKING:
+    from collections.abc import Generator, Sequence
+
     from pymatgen.analysis.defects.core import Defect
     from pymatgen.io.vasp import VolumetricData
 
 __author__ = "Jimmy-Xuan Shen"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy-Xuan Shen @jmmshn"
 __date__ = "Mar 15, 2022"
@@ -40,32 +42,32 @@
         struct = _remove_oxidation_states(structure)
         if hasattr(self, "symprec") and hasattr(self, "angle_tolerance"):
             return SpacegroupAnalyzer(
                 struct,
                 symprec=self.symprec,
                 angle_tolerance=self.angle_tolerance,
             )
-        else:  # pragma: no cover
-            raise ValueError(
-                "This generator is using the `SpaceGroupAnalyzer` and requires `symprec` and `angle_tolerance` to be set."
-            )
+        msg = "This generator is using the `SpaceGroupAnalyzer` and requires `symprec` and `angle_tolerance` to be set."
+        raise ValueError(
+            msg,
+        )
 
-    def generate(self, *args, **kwargs) -> Generator[Defect, None, None]:
+    def generate(self, *args, **kwargs) -> Generator[Defect, None, None]:  # noqa: ANN002
         """Generate a defect.
 
         Args:
             *args: Additional positional arguments.
             **kwargs: Additional keyword arguments.
 
         Returns:
             Generator[Defect, None, None]: Generator that yields a list of ``Defect`` objects.
         """
         raise NotImplementedError
 
-    def get_defects(self, *args, **kwargs) -> list[Defect]:
+    def get_defects(self, *args, **kwargs) -> list[Defect]:  # noqa: ANN002
         """Alias for self.generate."""
         return list(self.generate(*args, **kwargs))
 
 
 class VacancyGenerator(DefectGenerator):
     """Generator for vacancy defects.
 
@@ -76,41 +78,42 @@
             (parameter for ``SpacegroupAnalyzer``).
     """
 
     def __init__(
         self,
         symprec: float = 0.01,
         angle_tolerance: float = 5,
-    ):
+    ) -> None:
         """Initialize the vacancy generator."""
         self.symprec = symprec
         self.angle_tolerance = angle_tolerance
 
     def generate(
-        self, structure: Structure, rm_species: list[str | Species] = None, **kwargs
+        self,
+        structure: Structure,
+        rm_species: list[str | Species] | None = None,
+        **kwargs,
     ) -> Generator[Vacancy, None, None]:
         """Generate a vacancy defects.
 
         Args:
             structure: The bulk structure the vacancies are generated from.
             rm_species: List of species to be removed. If None considered all species.
             **kwargs: Additional keyword arguments for the ``Vacancy`` constructor.
 
         Returns:
             Generator[Vacancy, None, None]: Generator that yields a list of ``Vacancy`` objects.
         """
         all_species = [*map(_element_str, structure.composition.elements)]
-        if rm_species is None:
-            rm_species = all_species
-        else:
-            rm_species = [*map(str, rm_species)]
+        rm_species = all_species if rm_species is None else [*map(str, rm_species)]
 
         if not set(rm_species).issubset(all_species):
+            msg = f"rm_species({rm_species}) must be a subset of the structure's species ({all_species})."
             raise ValueError(
-                f"rm_species({rm_species}) must be a subset of the structure's species ({all_species})."
+                msg,
             )
 
         sga = self._space_group_analyzer(structure)
         sym_struct = sga.get_symmetrized_structure()
         for site_group in sym_struct.equivalent_sites:
             site = site_group[0]
             if _element_str(site.specie) in rm_species:
@@ -127,21 +130,24 @@
 
     Attributes:
         symprec:  Tolerance for symmetry finding (parameter for ``SpacegroupAnalyzer``).
         angle_tolerance: Angle tolerance for symmetry finding (parameter for ``SpacegroupAnalyzer``).
 
     """
 
-    def __init__(self, symprec: float = 0.01, angle_tolerance: float = 5):
+    def __init__(self, symprec: float = 0.01, angle_tolerance: float = 5) -> None:
         """Initialize the substitution generator."""
         self.symprec = symprec
         self.angle_tolerance = angle_tolerance
 
     def generate(
-        self, structure: Structure, substitution: dict[str, str | list], **kwargs
+        self,
+        structure: Structure,
+        substitution: dict[str, str | list],
+        **kwargs,
     ) -> Generator[Substitution, None, None]:
         """Generate subsitutional defects.
 
         Args:
             structure: The bulk structure the vacancies are generated from.
             substitution: The substitutions to be made given as a dictionary.
                 e.g. {"Ga": "Ca"} means that Ga is substituted with Ca. You
@@ -152,15 +158,15 @@
             Generator[Substitution, None, None]: Generator that yields a list of ``Substitution`` objects
         """
         sga = self._space_group_analyzer(structure)
         sym_struct = sga.get_symmetrized_structure()
         for site_group in sym_struct.equivalent_sites:
             site = site_group[0]
             el_str = _element_str(site.specie)
-            if el_str not in substitution.keys():
+            if el_str not in substitution:
                 continue
             sub_el = substitution[el_str]
             if isinstance(sub_el, str):
                 sub_site = PeriodicSite(
                     Species(sub_el),
                     site.frac_coords,
                     structure.lattice,
@@ -208,15 +214,15 @@
     """Generator of all anti-site defects.
 
     Attributes:
         symprec:  Tolerance for symmetry finding (parameter for ``SpacegroupAnalyzer``).
         angle_tolerance: Angle tolerance for symmetry finding (parameter for ``SpacegroupAnalyzer``).
     """
 
-    def __init__(self, symprec: float = 0.01, angle_tolerance: float = 5):
+    def __init__(self, symprec: float = 0.01, angle_tolerance: float = 5) -> None:
         """Initialize the anti-site generator."""
         self.symprec = symprec
         self.angle_tolerance = angle_tolerance
         self._sub_gen = SubstitutionGenerator(symprec, angle_tolerance)
 
     def generate(
         self,
@@ -230,15 +236,15 @@
             **kwargs: Additional keyword arguments for the ``Substitution.generate`` function.
         """
         all_species = [*map(_element_str, structure.composition.elements)]
         subs = collections.defaultdict(list)
         for u, v in combinations(all_species, 2):
             subs[u].append(v)
             subs[v].append(u)
-        _logger.debug(f"All anti-site pairings: {subs}")
+        _logger.debug("All anti-site pairings: %s", subs)
         for site, species in subs.items():
             for sub in species:
                 yield from self._sub_gen.generate(structure, {site: sub}, **kwargs)
 
 
 class InterstitialGenerator(DefectGenerator):
     """Generator of interstitiald defects.
@@ -250,17 +256,18 @@
     def __init__(self, min_dist: float = 0.5) -> None:
         """Initialize the interstitial generator."""
         self.min_dist = min_dist
 
     def generate(
         self,
         structure: Structure,
-        insertions: dict[str, list[list[float]]],
-        multiplicities: dict[str, list[int]] | None = None,
-        equivalent_positions: dict[str, list[list[list[float]]]] | None = None,
+        insertions: dict[str, Sequence[Sequence[float]]],
+        multiplicities: dict[str, Sequence[int]] | None = None,
+        equivalent_positions: dict[str, Sequence[Sequence[Sequence[float]]]]
+        | None = None,
         **kwargs,
     ) -> Generator[Interstitial, None, None]:
         """Generate interstitials.
 
         Args:
             structure: The bulk structure the interstitials are generated from.
             insertions: The insertions to be made given as a dictionary {"Mg": [[0.0, 0.0, 0.0], [0.5, 0.5, 0.5]]}.
@@ -277,52 +284,60 @@
                 el_str: [1] * len(coords) for el_str, coords in insertions.items()
             }
         if equivalent_positions is None:
             equivalent_positions = {
                 el_str: [
                     [insertions[el_str][i]] for i in range(len(insertions[el_str]))
                 ]
-                for el_str in insertions.keys()
+                for el_str in insertions
             }
 
         for el_str, coords in insertions.items():
             for i, coord in self._filter_colliding(coords, structure=structure):
                 mul = multiplicities[el_str][i]
                 equiv_positions = equivalent_positions[el_str][i]
                 isite = PeriodicSite(
-                    species=Species(el_str), coords=coord, lattice=structure.lattice
+                    species=Species(el_str),
+                    coords=coord,
+                    lattice=structure.lattice,
                 )
                 equiv_sites = [
                     PeriodicSite(
-                        species=Species(el_str), coords=coord, lattice=structure.lattice
+                        species=Species(el_str),
+                        coords=coord,
+                        lattice=structure.lattice,
                     )
                     for coord in equiv_positions
                 ]
                 yield Interstitial(
                     structure,
                     isite,
                     multiplicity=mul,
                     equivalent_sites=equiv_sites,
                     **kwargs,
                 )
 
     def _filter_colliding(
-        self, fcoords: list[list[float]], structure: Structure
-    ) -> Generator[tuple[int, list[float]], None, None]:
+        self,
+        fcoords: Sequence[Sequence[float]],
+        structure: Structure,
+    ) -> Generator[tuple[int, Sequence[float]], None, None]:
         """Check the sites for collisions.
 
         Args:
             fcoords: List of fractional coordinates of the sites.
             structure: The bulk structure the interstitials placed in.
         """
-        unique_fcoords = set(tuple(f) for f in fcoords)
+        unique_fcoords = {tuple(f) for f in fcoords}
         cleaned_fcoords = remove_collisions(
-            fcoords=list(unique_fcoords), structure=structure, min_dist=self.min_dist
+            fcoords=list(unique_fcoords),
+            structure=structure,
+            min_dist=self.min_dist,
         )
-        cleaned_fcoords = set(tuple(f) for f in cleaned_fcoords)
+        cleaned_fcoords = {tuple(f) for f in cleaned_fcoords}
         for i, fc in enumerate(fcoords):
             if tuple(fc) not in cleaned_fcoords:
                 continue
             yield i, fc
 
 
 class VoronoiInterstitialGenerator(InterstitialGenerator):
@@ -365,29 +380,31 @@
 
         Args:
             structure: The bulk structure the interstitials inserted in.
             insert_species: The species to be inserted.
             **kwargs: Additional keyword arguments for the ``Interstitial`` constructor.
         """
         if len(set(insert_species)) != len(insert_species):  # pragma: no cover
-            raise ValueError("Insert species must be unique.")
+            msg = "Insert species must be unique."
+            raise ValueError(msg)
         cand_sites_mul_and_equiv_fpos = [*self._get_candidate_sites(structure)]
         for species in insert_species:
             cand_sites, multiplicity, equiv_fpos = zip(*cand_sites_mul_and_equiv_fpos)
 
             yield from super().generate(
                 structure,
                 insertions={species: list(cand_sites)},
                 multiplicities={species: list(multiplicity)},
                 equivalent_positions={species: list(equiv_fpos)},
                 **kwargs,
             )
 
     def _get_candidate_sites(
-        self, structure: Structure
+        self,
+        structure: Structure,
     ) -> Generator[tuple[list[float], int, list[list[float]]], None, None]:
         """Get the candidate sites for interstitials.
 
         Args:
             structure: The bulk structure the interstitials inserted in.
         """
         framework = list(structure.symbol_set)
@@ -399,27 +416,27 @@
             clustering_tol=self.clustering_tol,
             min_dist=self.min_dist,
             ltol=self.ltol,
             stol=self.stol,
             angle_tol=self.angle_tol,
             **self.top_kwargs,
         )
-        insert_sites = dict()
-        multiplicity: dict[int, int] = dict()
-        equiv_fpos: dict[int, list[list[float]]] = dict()
+        insert_sites = {}
+        multiplicity: dict[int, int] = {}
+        equiv_fpos: dict[int, list[list[float]]] = {}
         for fpos, lab in top.labeled_sites:
             if lab in insert_sites:
                 multiplicity[lab] += 1
                 equiv_fpos[lab].append(fpos)
                 continue
             insert_sites[lab] = fpos
             multiplicity[lab] = 1
             equiv_fpos[lab] = [fpos]
 
-        for key in insert_sites.keys():
+        for key in insert_sites:
             yield insert_sites[key], multiplicity[key], equiv_fpos[key]
 
 
 class ChargeInterstitialGenerator(InterstitialGenerator):
     """Generator of interstitiald defects.
 
     Attributes:
@@ -452,25 +469,29 @@
         self.angle_tol = angle_tol
         self.avg_radius = avg_radius
         self.max_avg_charge = max_avg_charge
         self.max_insertions = max_insertions
         super().__init__(min_dist=min_dist)
 
     def generate(  # type: ignore[override]
-        self, chgcar: VolumetricData, insert_species: set[str] | list[str], **kwargs
+        self,
+        chgcar: VolumetricData,
+        insert_species: set[str] | list[str],
+        **kwargs,
     ) -> Generator[Interstitial, None, None]:
         """Generate interstitials.
 
         Args:
             chgcar: The chgcar object to be used for the charge density.
             insert_species: The species to be inserted.
             **kwargs: Additional keyword arguments for the ``Interstitial`` constructor.
         """
         if len(set(insert_species)) != len(insert_species):  # pragma: no cover
-            raise ValueError("Insert species must be unique.")
+            msg = "Insert species must be unique."
+            raise ValueError(msg)
         cand_sites_mul_and_equiv_fpos = [*self._get_candidate_sites(chgcar)]
         for species in insert_species:
             cand_sites, multiplicity, equiv_fpos = zip(*cand_sites_mul_and_equiv_fpos)
             if self.max_insertions is not None:
                 cand_sites = cand_sites[: self.max_insertions]
                 multiplicity = multiplicity[: self.max_insertions]
                 equiv_fpos = equiv_fpos[: self.max_insertions]
@@ -479,37 +500,38 @@
                 chgcar.structure,
                 insertions={species: cand_sites},
                 multiplicities={species: multiplicity},
                 equivalent_positions={species: equiv_fpos},
                 **kwargs,
             )
 
-    def _get_candidate_sites(self, chgcar: Chgcar):
+    def _get_candidate_sites(self, chgcar: Chgcar) -> Generator[tuple, None, None]:
         cia = ChargeInsertionAnalyzer(
             chgcar,
             clustering_tol=self.clustering_tol,
             ltol=self.ltol,
             stol=self.stol,
             angle_tol=self.angle_tol,
             min_dist=self.min_dist,
         )
         avg_chg_groups = cia.filter_and_group(
-            avg_radius=self.avg_radius, max_avg_charge=self.max_avg_charge
+            avg_radius=self.avg_radius,
+            max_avg_charge=self.max_avg_charge,
         )
         for _, g in avg_chg_groups:
             yield min(g), len(g), g
 
 
 def generate_all_native_defects(
     host: Structure | Chgcar,
     sub_generator: SubstitutionGenerator | None = None,
     vac_generator: VacancyGenerator | None = None,
     int_generator: ChargeInterstitialGenerator | None = None,
     max_insertions: int | None = None,
-):
+) -> Generator[Defect, None, None]:
     """Generate all native defects.
 
     Convenience function to generate all native defects for a host structure or chgcar object.
 
     Args:
         host: The host structure or chgcar object.
         sub_generator: The substitution generator, if None, a default generator is used.
@@ -521,41 +543,42 @@
     if isinstance(host, Chgcar):
         struct = host.structure
         chgcar = host
     elif isinstance(host, Structure):
         struct = host
         chgcar = None
     else:
-        raise ValueError("Host must be a Structure or Chgcar object.")
+        msg = "Host must be a Structure or Chgcar object."
+        raise ValueError(msg)
 
     species = set(map(_element_str, struct.species))
     sub_generator = sub_generator or SubstitutionGenerator()
     vac_generator = vac_generator or VacancyGenerator()
     # generate all vacancies
     yield from vac_generator.generate(struct)
     # generate substitutions for all pairs of species
     for sp1, sp2 in itertools.combinations(species, 2):
         yield from sub_generator.generate(struct, {sp1: sp2})
         yield from sub_generator.generate(struct, {sp2: sp1})
     # generate interstitials if a chgcar is provided
     if chgcar is not None:
         int_generator = int_generator or ChargeInterstitialGenerator(
-            max_insertions=max_insertions
+            max_insertions=max_insertions,
         )
         yield from int_generator.generate(chgcar, insert_species=species)
 
 
 def _element_str(sp_or_el: Species | Element) -> str:
     """Convert a species or element to a string."""
     if isinstance(sp_or_el, Species):
         return str(sp_or_el.element)
-    elif isinstance(sp_or_el, Element):
+    if isinstance(sp_or_el, Element):
         return str(sp_or_el)
-    else:
-        raise ValueError(f"{sp_or_el} is not a species or element")  # pragma: no cover
+    msg = f"{sp_or_el} is not a species or element"
+    raise ValueError(msg)
 
 
 def _remove_oxidation_states(structure: Structure) -> Structure:
     """Get a structure with oxidation states removed."""
     struct = structure.copy()
     struct.remove_oxidation_states()
     return struct
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/plotting/optics.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/plotting/optics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """Plotting functions."""
+
 from __future__ import annotations
 
 import collections
 import logging
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
-from matplotlib.colors import Normalize
+from matplotlib.colors import Colormap, Normalize
 from pymatgen.electronic_structure.core import Spin
 
 if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+    from matplotlib.axes import Axes
     from pymatgen.analysis.defects.ccd import HarmonicDefect
 
 __author__ = "Jimmy Shen"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy Shen @jmmshn"
 __date__ = "July 2023"
 
 logger = logging.getLogger(__name__)
 
 
 def plot_optical_transitions(
     defect: HarmonicDefect,
     kpt_index: int = 0,
     band_window: int = 5,
-    user_defect_band: tuple = tuple(),
-    other_defect_bands: list[int] = None,
-    ijdirs: list[tuple] = None,
-    shift_eig: dict[tuple, float] = None,
+    user_defect_band: tuple = (),
+    other_defect_bands: list[int] | None = None,
+    ijdirs: Sequence[tuple] | None = None,
+    shift_eig: dict[tuple, float] | None = None,
     x0: float = 0,
     x_width: float = 2,
-    ax=None,
-    cmap=None,
-    norm=None,
-):
+    ax: Axes = None,
+    cmap: Colormap = None,
+    norm: Normalize = None,
+) -> tuple[pd.DataFrame, Colormap, Normalize]:
     """Plot the optical transitions from the defect state to all other states.
 
     Only plot the transitions for a specific kpoint index. The arrows present the transitions
     between the defect state of interest and all other states. The color of the arrows
     indicate the magnitude of the matrix element (derivative of the wavefunction) for the
     transition.
 
@@ -73,37 +77,50 @@
         ax:
             The matplotlib axis object to plot on.
         cmap:
             The matplotlib color map to use for the color of the arrorws.
         norm:
             The matplotlib normalization to use for the color map of the arrows.
 
+    Returns:
+        A pandas dataframe with the following columns:
+            ib: The band index of the state the arrow is pointing to.
+            jb: The band index of the defect state.
+            kpt: The kpoint index of the state the arrow is pointing to.
+            spin: The spin index of the state the arrow is pointing to.
+            eig: The eigenvalue of the state the arrow is pointing to.
+            M.E.: The matrix element of the transition.
+        cmap:
+            The matplotlib color map used.
+        norm:
+            The matplotlib normalization used.
     """
     d_eigs = get_bs_eigenvalues(
         defect=defect,
         kpt_index=kpt_index,
         band_window=band_window,
         user_defect_band=user_defect_band,
         other_defect_bands=other_defect_bands,
         shift_eig=shift_eig,
     )
     if user_defect_band:
         defect_band_index = user_defect_band[0]
     else:
         defect_band_index = next(
-            filter(lambda x: x[1] == kpt_index, defect.defect_band)
+            filter(lambda x: x[1] == kpt_index, defect.defect_band),
         )[0]
-    if ax is None:
-        ax_ = plt.gca()
-    else:  # pragma: no cover
-        ax_ = ax
+    ax_ = plt.gca() if ax is None else ax
     _plot_eigs(
-        d_eigs, defect.relaxed_bandstructure.efermi, ax=ax_, x0=x0, x_width=x_width
+        d_eigs,
+        defect.relaxed_bandstructure.efermi,
+        ax=ax_,
+        x0=x0,
+        x_width=x_width,
     )
-    ijdirs = ijdirs or [(0, 0), (1, 1), (2, 2)]
+    ijdirs = ijdirs or ((0, 0), (1, 1), (2, 2))
     me_plot_data, cmap, norm = _plot_matrix_elements(
         defect.waveder.cder,
         d_eigs,
         defect_band_index=defect_band_index,
         ijdirs=ijdirs,
         ax=ax_,
         x0=x0,
@@ -114,17 +131,17 @@
     return _get_dataframe(d_eigs=d_eigs, me_plot_data=me_plot_data), cmap, norm
 
 
 def get_bs_eigenvalues(
     defect: HarmonicDefect,
     kpt_index: int = 0,
     band_window: int = 5,
-    user_defect_band: tuple = None,
-    other_defect_bands: list[int] = None,
-    shift_eig: dict[tuple, float] = None,
+    user_defect_band: tuple | None = None,
+    other_defect_bands: list[int] | None = None,
+    shift_eig: dict[tuple, float] | None = None,
 ) -> dict[tuple, float]:
     """Read the eigenvalues from `HarmonicDefect.relaxed_bandstructure`.
 
     Args:
         defect:
             The HarmonicDefect object, the `relaxed_bandstructure` attribute
             must be set since this contains the eigenvalues.
@@ -146,26 +163,27 @@
             valence or conduction band for plotting and schematic purposes.
 
 
     Returns:
         Dictionary of the format: (iband, ikpt, ispin) -> eigenvalue
     """
     if defect.relaxed_bandstructure is None:  # pragma: no cover
-        raise ValueError("The defect object does not have a band structure.")
+        msg = "The defect object does not have a band structure."
+        raise ValueError(msg)
 
     other_defect_bands = other_defect_bands or []
 
     if user_defect_band:
         def_indices = user_defect_band
     else:
         def_indices = next(filter(lambda x: x[1] == kpt_index, defect.defect_band))
 
     band_index, kpt_index, spin_index = def_indices
     spin_key = Spin.up if spin_index == 0 else Spin.down
-    output: dict[tuple, float] = dict()
+    output: dict[tuple, float] = {}
     shift_dict: dict = collections.defaultdict(lambda: 0.0)
     if shift_eig is not None:
         shift_dict.update(shift_eig)
     for ib in range(band_index - band_window, band_index + band_window + 1):
         if ib in other_defect_bands:
             continue
         output[(ib, kpt_index, spin_index)] = (
@@ -173,16 +191,16 @@
             + shift_dict[(ib, kpt_index, spin_index)]
         )
     return output
 
 
 def _plot_eigs(
     d_eigs: dict[tuple, float],
-    e_fermi=None,
-    ax=None,
+    e_fermi: float | None = None,
+    ax: Axes = None,
     x0: float = 0.0,
     x_width: float = 0.3,
     **kwargs,
 ) -> None:
     """Plot the eigenvalues.
 
     Args:
@@ -210,34 +228,42 @@
     collections.defaultdict(list)
     eigenvalues = np.array(list(d_eigs.values()))
     if e_fermi is None:  # pragma: no cover
         e_fermi = -np.inf
 
     eigs_ = eigenvalues[eigenvalues <= e_fermi]
     ax.hlines(
-        eigs_, x0 - (x_width / 2.0), x0 + (x_width / 2.0), color=colors[0], **kwargs
+        eigs_,
+        x0 - (x_width / 2.0),
+        x0 + (x_width / 2.0),
+        color=colors[0],
+        **kwargs,
     )
     eigs_ = eigenvalues[eigenvalues > e_fermi]
     ax.hlines(
-        eigs_, x0 - (x_width / 2.0), x0 + (x_width / 2.0), color=colors[1], **kwargs
+        eigs_,
+        x0 - (x_width / 2.0),
+        x0 + (x_width / 2.0),
+        color=colors[1],
+        **kwargs,
     )
 
 
 def _plot_matrix_elements(
-    cder,
-    d_eig,
-    defect_band_index,
-    ijdirs=((0, 0), (1, 1), (2, 2)),
-    ax=None,
-    x0=0,
-    x_width=0.6,
-    arrow_width=0.1,
-    cmap=None,
-    norm=None,
-) -> tuple[list[tuple], plt.cm, plt.Normalize]:
+    cder: dict[tuple, float],
+    d_eig: dict[tuple, float],
+    defect_band_index: int,
+    ijdirs: Sequence[tuple] = ((0, 0), (1, 1), (2, 2)),
+    ax: Axes = None,
+    x0: float = 0.0,
+    x_width: float = 0.6,
+    arrow_width: float = 0.1,
+    cmap: Colormap = None,
+    norm: Normalize = None,
+) -> tuple[list[tuple], Colormap, Normalize]:
     """Plot arrow for the transition from the defect state to all other states.
 
     Args:
         cder:
             The matrix element (derivative of the wavefunction) for the defect state.
         d_eig:
             The dictionary of eigenvalues for the defect state. In the format of
@@ -276,15 +302,15 @@
     y0 = d_eig[jb, jkpt, jspin]
     plot_data: list[tuple] = []
     for (ib, ik, ispin), eig in d_eig.items():
         A = 0
         for idir, jdir in ijdirs:
             A += np.abs(
                 cder[ib, jb, ik, ispin, idir]
-                * np.conjugate(cder[ib, jb, ik, ispin, jdir])
+                * np.conjugate(cder[ib, jb, ik, ispin, jdir]),
             )
         plot_data.append((jb, ib, eig, A))
 
     if cmap is None:
         cmap = plt.get_cmap("viridis")
 
     # get the range of A values
@@ -294,15 +320,15 @@
             max(plot_data, key=lambda x: x[3])[3],
         )
         norm = Normalize(vmin=A_min, vmax=A_max)
 
     n_arrows = len(plot_data)
     x_step = x_width / n_arrows
     x = x0 - x_width / 2 + x_step / 2
-    for ib, jb, eig, A in plot_data:
+    for _ib, _jb, eig, A in plot_data:
         ax.arrow(
             x=x,
             y=y0,
             dx=0,
             dy=eig - y0,
             width=arrow_width,
             length_includes_head=True,
@@ -331,14 +357,14 @@
             jb: The band index of the defect state.
             kpt: The kpoint index of the state the arrow is pointing to.
             spin: The spin index of the state the arrow is pointing to.
             eig: The eigenvalue of the state the arrow is pointing to.
             M.E.: The matrix element of the transition.
     """
     _, ikpt, ispin = next(iter(d_eigs.keys()))
-    df = pd.DataFrame(
+    output_dataframe = pd.DataFrame(
         me_plot_data,
         columns=["ib", "jb", "eig", "M.E."],
     )
-    df["kpt"] = ikpt
-    df["spin"] = ispin
-    return df
+    output_dataframe["kpt"] = ikpt
+    output_dataframe["spin"] = ispin
+    return output_dataframe
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/plotting/phases.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/plotting/phases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Plotting functions for competing phases."""
+
 # %%
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from matplotlib import pyplot as plt
@@ -16,17 +17,16 @@
     from pymatgen.core import Element
 
 # check if labellines is installed
 try:
     from labellines import labelLines
 except ImportError:
 
-    def labelLines(*args, **kwargs):
+    def labelLines(*args, **kwargs) -> None:  # noqa: ARG001, ANN002
         """Dummy function if labellines is not installed."""
-        pass
 
 
 __author__ = "Jimmy Shen"
 __copyright__ = "Copyright 2022, The Materials Project"
 __maintainer__ = "Jimmy Shen @jmmshn"
 __date__ = "July 2023"
 
@@ -38,15 +38,15 @@
     x_element: Element,
     y_element: Element,
     ax: Axes | None = None,
     min_mu: float = -5.0,
     label_lines: bool = False,
     x_vals: list[float] | None = None,
     label_fontsize: int = 12,
-):
+) -> None:
     """Plot the chemical potential diagram for two elements.
 
     Args:
         fed:
             The formation energy diagram.
         x_element:
             The element to use for the x-axis.
@@ -86,28 +86,28 @@
 
     patch = Polygon(
         clip_path,
         closed=True,
     )
     ax.add_patch(patch)
 
-    ax.set_xlabel(f"$\Delta\mu_{{{x_element}}}$ (eV)")
-    ax.set_ylabel(f"$\Delta\mu_{{{y_element}}}$ (eV)")
+    ax.set_xlabel(rf"$\Delta\mu_{{{x_element}}}$ (eV)")
+    ax.set_ylabel(rf"$\Delta\mu_{{{y_element}}}$ (eV)")
     ax.set_xlim(x_min - PLOT_PADDING, 0 + PLOT_PADDING)
     ax.set_ylim(y_min - PLOT_PADDING, 0 + PLOT_PADDING)
     if label_lines:
         labelLines(ax.get_lines(), align=False, xvals=x_vals, fontsize=label_fontsize)
 
 
 def _convex_hull_2d(
     points: list[dict],
     x_element: Element,
     y_element: Element,
-    competing_phases: list = None,
-) -> list[dict]:
+    competing_phases: list | None = None,
+) -> list:
     """Compute the convex hull of a set of points in 2D.
 
     Args:
         points:
             A list of dictionaries with keys "x" and "y" and values as floats.
         x_element:
             The element to use for the x-axis.
@@ -123,21 +123,21 @@
         convex hull.
     """
     if competing_phases is None:
         competing_phases = [None] * len(points)
     xy_points = [(pt[x_element], pt[y_element]) for pt in points]
     hull = ConvexHull(xy_points)
     xy_hull = [xy_points[i] for i in hull.vertices]
-    pt_and_phase = []
 
-    def _get_line_data(i1, i2):
+    def _get_line_data(i1: int, i2: int) -> tuple:
         cp1 = competing_phases[hull.vertices[i1]]
         cp2 = competing_phases[hull.vertices[i2]]
         shared_keys = cp1.keys() & cp2.keys()
         shared_phase = {k: cp1[k] for k in shared_keys}
         return xy_hull[i1], xy_hull[i2], shared_phase
 
     # return all pairs of points:
-    for itr in range(1, len(hull.vertices)):
-        pt_and_phase.append(_get_line_data(itr - 1, itr))
+    pt_and_phase = [
+        _get_line_data(itr - 1, itr) for itr in range(1, len(hull.vertices))
+    ]
     pt_and_phase.append(_get_line_data(len(hull.vertices) - 1, 0))
     return pt_and_phase
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/recombination.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/recombination.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 The the SRH recombination code is taken from the NonRad code (www.github.com/mturiansky/nonrad)
 """
 
 from __future__ import annotations
 
 import itertools
 import logging
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 from scipy.interpolate import PchipInterpolator
 
 from .constants import AMU2KG, ANGS2M, EV2J, HBAR_EV, HBAR_J, KB, LOOKUP_TABLE
 
 _logger = logging.getLogger(__name__)
 
 try:
     from numba import njit
 except ImportError:
     _logger.warning("Numba not installed. Install Numba for better performance.")
 
-    def njit(*args, **kwargs):
+    def njit(*args, **kwargs) -> Callable:  # noqa: ARG001, ANN002
         """Dummy decorator for njit."""
         return lambda func: func
 
 
 if TYPE_CHECKING:
     from numpy import typing as npt
 
@@ -48,15 +48,15 @@
         n: The number to compute the factorial of.
 
     Returns:
         The factorial of n.
     """
     if n > 20:
         return LOOKUP_TABLE[-1] * np.prod(
-            np.array(list(range(21, n + 1)), dtype=np.double)
+            np.array(list(range(21, n + 1)), dtype=np.double),
         )
     return LOOKUP_TABLE[n]
 
 
 @njit(cache=True)
 def herm(x: float, n: int) -> float:  # pragma: no cover
     """Recursive definition of hermite polynomial.
@@ -81,15 +81,19 @@
         y1 = yn
         dy1 = dyn
     return yn
 
 
 @njit(cache=True)
 def analytic_overlap_NM(
-    dQ: float, omega1: float, omega2: float, n1: int, n2: int
+    dQ: float,
+    omega1: float,
+    omega2: float,
+    n1: int,
+    n2: int,
 ) -> float:  # pragma: no cover
     """Compute the overlap between two displaced harmonic oscillators.
 
     This function computes the overlap integral between two harmonic
     oscillators with frequencies w1, w2 that are displaced by DQ for the
     quantum numbers n1, n2. The integral is computed using an analytic formula
     for the overlap of two displaced harmonic oscillators. The method comes
@@ -161,15 +165,15 @@
 def get_mQn(
     dQ: float,
     omega_i: float,
     omega_f: float,
     m_init: int,
     Nf: int,
     ovl: npt.NDArray,
-):
+) -> tuple[npt.ArrayLike, npt.ArrayLike]:
     """Get the matrix element values for the position operator.
 
         <m_i|Q|n_f>
 
     Args:
         dQ: The displacement between the initial and final phonon states.
         omega_i: The initial phonon frequency in eV.
@@ -201,15 +205,15 @@
 def get_mn(
     dQ: float,
     omega_i: float,
     omega_f: float,
     m_init: int,
     en_final: float,
     en_pad: float = 0.5,
-):
+) -> tuple[npt.ArrayLike, npt.ArrayLike]:
     """Get the matrix element values for the position operator.
 
         <m_i|n_f>
     Starting in state m_init and ending and ending on final states between
     ``en_final - en_pad`` and ``en_final + en_pad`` reference to the bottom of the final state parabola.
 
     Args:
@@ -228,26 +232,30 @@
     """
     n_min = max(int((en_final - en_pad) // omega_f), 0)
     n_max = int((en_final + en_pad) // omega_f) + 2
     E = np.arange(n_min, n_max) * omega_f
     matels = np.zeros_like(E)
     for n in range(n_min, n_max):
         matels[n - n_min] = analytic_overlap_NM(
-            dQ=dQ, omega1=omega_i, omega2=omega_f, n1=m_init, n2=n
+            dQ=dQ,
+            omega1=omega_i,
+            omega2=omega_f,
+            n1=m_init,
+            n2=n,
         )
     return E, matels
 
 
 def pchip_eval(
     x: npt.ArrayLike | float,
     x_coarse: npt.ArrayLike,
     y_coarse: npt.ArrayLike,
     pad_frac: float = 0.2,
     n_points: int = 5000,
-):
+) -> npt.ArrayLike:
     """Evaluate a piecewise cubic Hermite interpolant.
 
     Assuming a function is evenly sampleded on (``x_coarse``, ``y_coarse``),
     Then we know the final shape of the function has to satisfy match the coarsely sampled data.
     Thus, we can just interpolate the function on a finer grid and ensure that the interpolated function
     Integrates to the same value as the sum of the coarsely sampled data.
 
@@ -314,18 +322,27 @@
     ovl = np.zeros((Ni + 1, Nf), dtype=np.longdouble)
     for m, n in itertools.product(range(Ni + 1), range(Nf)):
         ovl[m, n] = analytic_overlap_NM(dQ, omega_i, omega_f, m, n)
     weights = boltzmann_filling(omega_i, T, Ni)
     rate = np.zeros_like(T, dtype=np.longdouble)
     for m in range(Ni):
         E, me = get_mQn(
-            dQ=dQ, omega_i=omega_i, omega_f=omega_f, m_init=m, Nf=Nf, ovl=ovl
+            dQ=dQ,
+            omega_i=omega_i,
+            omega_f=omega_f,
+            m_init=m,
+            Nf=Nf,
+            ovl=ovl,
         )
         interp_me = pchip_eval(
-            dE, E, np.abs(np.conj(me) * me), pad_frac=0.2, n_points=5000
+            dE,
+            E,
+            np.abs(np.conj(me) * me),
+            pad_frac=0.2,
+            n_points=5000,
         )
         rate += weights[m, :] * interp_me
     return 2 * np.pi * g * elph_me**2 * volume * rate
 
 
 def get_Rad_coef(
     T: float | npt.ArrayLike,
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/thermo.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/thermo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Classes and methods related to thermodynamics and energy."""
+
 from __future__ import annotations
 
 import collections
 import logging
 from dataclasses import dataclass, field
 from itertools import chain, groupby
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Callable
 
 import numpy as np
 from matplotlib import pyplot as plt
 from monty.json import MSONable
 from pymatgen.analysis.chempot_diagram import ChemicalPotentialDiagram
 from pymatgen.analysis.defects.core import Defect, NamedDefect
 from pymatgen.analysis.defects.corrections.freysoldt import get_freysoldt_correction
 from pymatgen.analysis.defects.finder import DefectSiteFinder
+from pymatgen.analysis.defects.supercells import get_closest_sc_mat
 from pymatgen.analysis.defects.utils import get_zfile, group_docs
 from pymatgen.analysis.phase_diagram import PhaseDiagram
 from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
 from pymatgen.core import Composition, Element
 from pymatgen.electronic_structure.dos import FermiDos
 from pymatgen.entries.computed_entries import ComputedEntry
-from pymatgen.io.vasp import Locpot, Vasprun
+from pymatgen.io.vasp import Locpot, Vasprun, VolumetricData
+from pyrho.charge_density import get_volumetric_like_sc
 from scipy.constants import value as _cd
 from scipy.optimize import bisect
 from scipy.spatial import ConvexHull
 
 if TYPE_CHECKING:
+    from collections.abc import Generator, Sequence
+
+    from matplotlib.axes import Axes
     from numpy.typing import ArrayLike, NDArray
+    from pandas import DataFrame
     from pymatgen.analysis.defects.utils import CorrectionResult
     from pymatgen.core import Structure
     from pymatgen.electronic_structure.dos import Dos
     from pymatgen.entries.computed_entries import ComputedStructureEntry
 
 __author__ = "Jimmy-Xuan Shen, Danny Broberg, Shyam Dwaraknath"
 __copyright__ = "Copyright 2022, The Materials Project"
@@ -89,16 +96,16 @@
         self.entry_id = self.entry_id or self.sc_entry.entry_id
 
     def get_freysoldt_correction(
         self,
         defect_locpot: Locpot | dict,
         bulk_locpot: Locpot | dict,
         dielectric: float | NDArray,
-        defect_struct: Optional[Structure] = None,
-        bulk_struct: Optional[Structure] = None,
+        defect_struct: Structure | None = None,
+        bulk_struct: Structure | None = None,
         **kwargs,
     ) -> CorrectionResult:
         """Calculate the Freysoldt correction.
 
         Updates the corrections dictionary with the Freysoldt correction
         and returns the planar averaged potential data for plotting.
 
@@ -113,70 +120,88 @@
                 The dielectric tensor or constant for the bulk material.
             defect_struct:
                 The defect structure. If None, the structure of the defect_locpot
                 will be used.
             bulk_struct:
                 The bulk structure. If None, the structure of the bulk_locpot
                 will be used.
-            kwargs:
+            **kwargs:
                 Additional keyword arguments for the get_correction method.
 
         Returns:
             dict:
                 The plotting data to analyze the planar averaged electrostatic potential
                 in the three periodic lattice directions.
         """
         if defect_struct is None:
             defect_struct = getattr(defect_locpot, "structure", None)
         if bulk_struct is None:
             bulk_struct = getattr(bulk_locpot, "structure", None)
 
         if defect_struct is None or bulk_struct is None:  # pragma: no cover
+            msg = "defect_struct and/or bulk_struct is missing either provide the structure or provide the complete locpot."
             raise ValueError(
-                "defect_struct and/or bulk_struct is missing either provide the structure or provide the complete locpot."
+                msg,
             )
 
         if self.sc_defect_frac_coords is None:
             finder = DefectSiteFinder()
             defect_fpos = finder.get_defect_fpos(
                 defect_structure=defect_struct,
                 base_structure=bulk_struct,
             )
             self.sc_defect_frac_coords = defect_fpos
         else:  # pragma: no cover
             defect_fpos = self.sc_defect_frac_coords
 
+        if isinstance(defect_locpot, VolumetricData):
+            defect_gn = defect_locpot.dim
+        elif isinstance(defect_locpot, dict):
+            defect_gn = tuple(map(len, (defect_locpot for k in ["0", "1", "2"])))
+
+        if isinstance(bulk_locpot, VolumetricData):
+            bulk_sc_locpot = get_sc_locpot(
+                uc_locpot=bulk_locpot,
+                defect_struct=defect_struct,
+                grid_out=defect_gn,
+                up_sample=2,
+            )
+            bulk_locpot = bulk_sc_locpot
+
         frey_corr = get_freysoldt_correction(
             q=self.charge_state,
             dielectric=dielectric,
             defect_locpot=defect_locpot,
-            bulk_locpot=bulk_locpot,
+            bulk_locpot=bulk_sc_locpot,
             defect_frac_coords=defect_fpos,
             lattice=defect_struct.lattice,
             **kwargs,
         )
         self.corrections.update(
             {
                 "freysoldt": frey_corr.correction_energy,
-            }
+            },
         )
         self.corrections_metadata.update({"freysoldt": frey_corr.metadata.copy()})
         return frey_corr
 
     @property
     def corrected_energy(self) -> float:
         """The energy of the defect entry with all corrections applied."""
         return self.sc_entry.energy + sum(self.corrections.values())
 
     def get_ediff(self) -> float | None:
         """Get the energy difference between the defect and the bulk (including finite-size correction)."""
         if self.bulk_entry is None:
-            raise RuntimeError(
+            msg = (
                 "Attempting to compute the energy difference without a bulk entry data."
             )
+            raise RuntimeError(
+                msg,
+            )
         return self.corrected_energy - self.bulk_entry.energy
 
     def get_summary_dict(self) -> dict:
         """Get a summary dictionary for the defect entry."""
         corrections_d = {f"correction_{k}": v for k, v in self.corrections.items()}
         res = {
             "name": self.defect.name,
@@ -221,66 +246,76 @@
             This can be justified since these tend to be the substitutional elements
             which should not have very negative chemical potential.
         bulk_stability:
             If the bulk energy is above the convex hull, lower it to this value below
             the convex hull.
     """
 
-    defect_entries: List[DefectEntry]
+    defect_entries: list[DefectEntry]
     pd_entries: list[ComputedEntry]
     vbm: float
-    band_gap: Optional[float] = None
-    bulk_entry: Optional[ComputedStructureEntry] = None
+    band_gap: float | None = None
+    bulk_entry: ComputedStructureEntry | None = None
     inc_inf_values: bool = False
     bulk_stability: float = 0.001
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """Post-initialization.
 
         - Reconstruct the phase diagram with the bulk entry
         - Make sure that the bulk entry is stable
         - create the chemical potential diagram using only the formation energies
         """
         g = group_defect_entries(self.defect_entries)
         if next(g, True) and next(g, False):
-            raise ValueError(
+            msg = (
                 "Defects are not of same type! "
                 "Use MultiFormationEnergyDiagram for multiple defect types"
             )
+            raise ValueError(
+                msg,
+            )
         # if all of the `DefectEntry` objects have the same `bulk_entry` then `self.bulk_entry` is not needed
-        if any(d.bulk_entry is None for d in self.defect_entries):
-            if self.bulk_entry is None:
-                raise RuntimeError(
-                    "Not all of the `DefectEntry` objects have a `bulk_entry` attribute, you need to provide `bulk_entry` to `FormationEnergyDiagram`"
-                )
+        if self.bulk_entry is None and any(
+            x.bulk_entry is None for x in self.defect_entries
+        ):
+            msg = "The bulk entry must be provided."
+            raise RuntimeError(
+                msg,
+            )
 
-        bulk_entry = self.bulk_entry or self.defect_entries[0].bulk_entry
-        self.bulk_entry = bulk_entry
+        bulk_entry = self.bulk_entry or min(
+            [x.bulk_entry for x in self.defect_entries],
+            key=lambda x: x.energy_per_atom,
+        )
         pd_ = PhaseDiagram(self.pd_entries)
         entries = pd_.stable_entries | {bulk_entry}
         pd_ = PhaseDiagram(entries)
         self.phase_diagram = ensure_stable_bulk(pd_, bulk_entry, self.bulk_stability)
         entries = []
         for entry in self.phase_diagram.stable_entries:
-            d_ = dict(
-                energy=self.phase_diagram.get_form_energy(entry),
-                composition=entry.composition,
-                entry_id=entry.entry_id,
-                correction=0.0,
-            )
+            d_ = {
+                "energy": self.phase_diagram.get_form_energy(entry),
+                "composition": entry.composition,
+                "entry_id": entry.entry_id,
+                "correction": 0.0,
+            }
             entries.append(ComputedEntry.from_dict(d_))
             entries.append(ComputedEntry.from_dict(d_))
         self.chempot_diagram = ChemicalPotentialDiagram(entries)
         if (
             bulk_entry.composition.reduced_formula not in self.chempot_diagram.domains
         ):  # pragma: no cover
-            raise ValueError(
+            msg = (
                 "Bulk entry is not stable in the chemical potential diagram."
                 "Consider increasing the `bulk_stability` to make it more stable."
             )
+            raise ValueError(
+                msg,
+            )
         chempot_limits = self.chempot_diagram.domains[
             bulk_entry.composition.reduced_formula
         ]
 
         if self.inc_inf_values:
             self._chempot_limits_arr = chempot_limits
         else:
@@ -299,15 +334,15 @@
         cls,
         defect_entries: list[DefectEntry],
         atomic_entries: list[ComputedEntry],
         phase_diagram: PhaseDiagram,
         vbm: float,
         bulk_entry: ComputedEntry | None = None,
         **kwargs,
-    ):
+    ) -> FormationEnergyDiagram:
         """Create a FormationEnergyDiagram object using an existing phase diagram.
 
         Since the Formation energy usually looks like:
 
         E[Defect] - (E[Bulk] + ∑ E[Atom_i] + ∑ Chempot[Atom_i])
 
         The most convenient, and likely most accurate way to obtain the chemical potentials
@@ -342,71 +377,76 @@
                 Additional keyword arguments for the FormationEnergyDiagram class.
 
         Returns:
             FormationEnergyDiagram:
                 The FormationEnergyDiagram object.
         """
         adjusted_entries = _get_adjusted_pd_entries(
-            phase_diagram=phase_diagram, atomic_entries=atomic_entries
+            phase_diagram=phase_diagram,
+            atomic_entries=atomic_entries,
         )
         return cls(
             bulk_entry=bulk_entry,
             defect_entries=defect_entries,
             pd_entries=adjusted_entries,
             vbm=vbm,
             **kwargs,
         )
 
     @classmethod
     def with_directories(
         cls,
-        directory_map: Dict[str, str],
+        directory_map: dict[str, str | Path],
         defect: Defect,
         pd_entries: list[ComputedEntry],
         dielectric: float | NDArray,
         vbm: float | None = None,
         **kwargs,
-    ):
+    ) -> FormationEnergyDiagram:
         """Create a FormationEnergyDiagram from VASP directories.
 
         Args:
             directory_map: A dictionary mapping the defect name to the directory containing the
                 VASP calculation.
             defect: The defect used to create the defect entries.
             pd_entries: The list of entries used to construct the phase diagram and chemical
                 potential diagram. They will be used to determine the stability region
                 of the bulk crystal.
             dielectric: The dielectric constant of the bulk crystal.
             vbm: The VBM of the bulk crystal.
             **kwargs: Additional keyword arguments for the constructor.
         """
 
-        def _read_dir(directory):
+        def _read_dir(directory: str | Path) -> tuple[ComputedEntry, Locpot]:
+            directory = Path(directory)
             vr = Vasprun(get_zfile(Path(directory), "vasprun.xml"))
             ent = vr.get_computed_entry()
             locpot = Locpot.from_file(get_zfile(directory, "LOCPOT"))
             return ent, locpot
 
         if "bulk" not in directory_map:
-            raise ValueError("The bulk directory must be provided.")
+            msg = "The bulk directory must be provided."
+            raise ValueError(msg)
         bulk_entry, bulk_locpot = _read_dir(directory_map["bulk"])
 
         def_entries = []
         for qq, q_dir in directory_map.items():
             if qq == "bulk":
                 continue
             q_entry, q_locpot = _read_dir(q_dir)
             q_d_entry = DefectEntry(
                 defect=defect,
                 charge_state=int(qq),
                 sc_entry=q_entry,
             )
 
             q_d_entry.get_freysoldt_correction(
-                defect_locpot=q_locpot, bulk_locpot=bulk_locpot, dielectric=dielectric
+                defect_locpot=q_locpot,
+                bulk_locpot=bulk_locpot,
+                dielectric=dielectric,
             )
             def_entries.append(q_d_entry)
         if vbm is None:
             vr = Vasprun(get_zfile(Path(directory_map["bulk"]), "vasprun.xml"))
             vbm = vr.get_band_structure().get_vbm()["energy"]
 
         return cls(
@@ -457,63 +497,54 @@
                 The formation energy at the VBM.
         """
         chempots = self._parse_chempots(chempots)
         en_change = sum(
             [
                 (self.dft_energies[Element(el)] + chempots[Element(el)]) * fac
                 for el, fac in defect_entry.defect.element_changes.items()
-            ]
+            ],
         )
 
-        if self.bulk_entry is not None:
-            formation_en = (
-                defect_entry.corrected_energy
-                - self.bulk_entry.energy
-                - en_change
-                + self.vbm * defect_entry.charge_state
-            )
-        else:
-            formation_en = (
-                defect_entry.get_ediff()
-                - en_change
-                + self.vbm * defect_entry.charge_state
-            )
+        try:
+            ediff = defect_entry.get_ediff()
+        except RuntimeError:
+            ediff = defect_entry.corrected_energy - self.bulk_entry.energy
 
-        return formation_en
+        return ediff - en_change + self.vbm * defect_entry.charge_state
 
     @property
-    def chempot_limits(self):
+    def chempot_limits(self) -> list[dict[Element, float]]:
         """Return the chemical potential limits in dictionary format."""
-        res = []
-        for vertex in self._chempot_limits_arr:
-            res.append(dict(zip(self.chempot_diagram.elements, vertex)))
-        return res
+        return [
+            dict(zip(self.chempot_diagram.elements, vertex))
+            for vertex in self._chempot_limits_arr
+        ]
 
     @property
     def competing_phases(self) -> list[dict[str, ComputedEntry]]:
         """Return the competing phases."""
         bulk_formula = self.bulk_entry.composition.reduced_formula
         cd = self.chempot_diagram
         res = []
         for pt in self._chempot_limits_arr:
-            competing_phases = dict()
+            competing_phases = {}
             for hp_ent, hp in zip(cd._hyperplane_entries, cd._hyperplanes):
                 if hp_ent.composition.reduced_formula == bulk_formula:
                     continue
                 if _is_on_hyperplane(pt, hp):
                     competing_phases[hp_ent.composition.reduced_formula] = hp_ent
             res.append(competing_phases)
         return res
 
     @property
-    def defect(self):
+    def defect(self) -> Defect:
         """Get the defect that this FormationEnergyDiagram represents."""
         return self.defect_entries[0].defect
 
-    def _get_lines(self, chempots: Dict) -> list[tuple[float, float]]:
+    def _get_lines(self, chempots: dict) -> list[tuple[float, float]]:
         """Get the lines for the formation energy diagram.
 
         Args:
             chempots:
                 A dictionary of the chemical potentials (referenced to the elements)
                 representations a vertex of the stability region of the chemical
                 potential diagram.
@@ -528,15 +559,18 @@
         for def_ent in self.defect_entries:
             b = self._vbm_formation_energy(def_ent, chempots)
             m = float(def_ent.charge_state)
             lines.append((m, b))
         return lines
 
     def get_transitions(
-        self, chempots: dict, x_min: float = 0, x_max: float | None = None
+        self,
+        chempots: dict,
+        x_min: float = 0,
+        x_max: float | None = None,
     ) -> list[tuple[float, float]]:
         """Get the transition levels for the formation energy diagram.
 
         Get all of the kinks in the formation energy diagram.
         The points at the VBM and CBM are given by the first and last
         point respectively.
 
@@ -552,67 +586,70 @@
 
         Returns:
             Transition levels and the formation energy at each transition level.
             The first and last points are the intercepts with the
             VBM and CBM respectively.
         """
         chempots = self._parse_chempots(chempots)
-        if x_max is None:
+        if x_max is None:  # pragma: no cover
             x_max = self.band_gap
 
         lines = self._get_lines(chempots)
         lines = get_lower_envelope(lines)
         return get_transitions(lines, x_min, x_max)
 
-    def get_formation_energy(self, fermi_level: float, chempot_dict: dict):
+    def get_formation_energy(self, fermi_level: float, chempot_dict: dict) -> float:
         """Get the formation energy at a given Fermi level.
 
         Linearly interpolate between the transition levels.
 
         Args:
             fermi_level:
                 The Fermi level at which the formation energy is computed.
             chempot_dict:
                 A dictionary of the chemical potentials (referenced to the elemental energies).
 
         Returns:
             The formation energy at the given Fermi level.
         """
         transitions = np.array(
-            self.get_transitions(chempot_dict, x_min=-100, x_max=100)
+            self.get_transitions(chempot_dict, x_min=-100, x_max=100),
         )
         # linearly interpolate between the set of points
         return np.interp(fermi_level, transitions[:, 0], transitions[:, 1])
 
     def get_concentration(
-        self, fermi_level: float, chempots: dict, temperature: int | float
+        self,
+        fermi_level: float,
+        chempots: dict,
+        temperature: float,
     ) -> float:
         """Get equilibrium defect concentration assuming the dilute limit.
 
         Args:
             fermi_level: fermi level with respect to the VBM
             chempots: Chemical potentials
             temperature: in Kelvin
         """
         chempots = self._parse_chempots(chempots=chempots)
         fe = self.get_formation_energy(fermi_level, chempots)
         return self.defect_entries[0].defect.multiplicity * fermi_dirac(
-            energy=fe, temperature=temperature
+            energy=fe,
+            temperature=temperature,
         )
 
-    def as_dataframe(self):
+    def as_dataframe(self) -> DataFrame:
         """Return the formation energy diagram as a pandas dataframe."""
         from pandas import DataFrame
 
         defect_entries = self.defect_entries
-        l_ = map(lambda x: x.get_summary_dict(), defect_entries)
-        df = DataFrame(l_)
-        return df
+        l_ = (x.get_summary_dict() for x in defect_entries)
+        return DataFrame(l_)
 
-    def get_chempots(self, rich_element: Element | str, en_tol: float = 0.01):
+    def get_chempots(self, rich_element: Element | str, en_tol: float = 0.01) -> dict:
         """Get the chemical potential for a desired growth condition.
 
         Choose an element to be rich in, require the chemical potential of that element
         to be near the MAX energy among the points (MAX_EN - en_tol, MAX_EN), then sort
         the remaining elements by:
             1. Are they in the bulk structure:
                 elements in the bulk structure are prioritized.
@@ -632,60 +669,62 @@
         Returns:
             A dictionary of the chemical potentials for the growth condition.
         """
         rich_element = Element(rich_element)
         max_val = max(self.chempot_limits, key=lambda x: x[rich_element])[rich_element]
         rich_conditions = list(
             filter(
-                lambda cp: abs(cp[rich_element] - max_val) < en_tol, self.chempot_limits
-            )
+                lambda cp: abs(cp[rich_element] - max_val) < en_tol,
+                self.chempot_limits,
+            ),
         )
-        if len(rich_conditions) == 0:
+        if len(rich_conditions) == 0:  # pragma: no cover
+            msg = f"Cannot find a chemical potential condition with {rich_element} near zero."
             raise ValueError(
-                f"Cannot find a chemical potential condition with {rich_element} near zero."
+                msg,
             )
         # defect = self.defect_entries[0].defect
         in_bulk = self.defect_entries[0].sc_entry.composition.elements
         # make sure they are of type Element
-        in_bulk = list(map(lambda x: Element(x.symbol), in_bulk))
+        in_bulk = [Element(x.symbol) for x in in_bulk]
         not_in_bulk = list(set(self.chempot_limits[0].keys()) - set(in_bulk))
         in_bulk = list(filter(lambda x: x != rich_element, in_bulk))
 
-        def el_sorter(element):
+        def el_sorter(element: Element) -> float:
             return -abs(element.electron_affinity - rich_element.electron_affinity)
 
         el_list = sorted(in_bulk, key=el_sorter) + sorted(not_in_bulk, key=el_sorter)
 
-        def chempot_sorter(chempot_dict):
+        def chempot_sorter(chempot_dict: dict) -> tuple[float, ...]:
             return tuple(chempot_dict[el] for el in el_list)
 
         return min(rich_conditions, key=chempot_sorter)
 
     def __repr__(self) -> str:
         """Representation."""
-        defect_entry_summary = []
-        for dent in self.defect_entries:
-            defect_entry_summary.append(
-                f"\t{dent.defect.name} {dent.charge_state} {dent.corrected_energy}"
-            )
+        defect_entry_summary = [
+            f"\t{dent.defect.name} {dent.charge_state} {dent.corrected_energy}"
+            for dent in self.defect_entries
+        ]
+
         txt = (
             f"{self.__class__.__name__} for {self.defect.name}",
             "Defect Entries:",
             "\n".join(defect_entry_summary),
         )
         return "\n".join(txt)
 
 
 @dataclass
 class MultiFormationEnergyDiagram(MSONable):
     """Container for multiple formation energy diagrams."""
 
-    formation_energy_diagrams: List[FormationEnergyDiagram]
+    formation_energy_diagrams: list[FormationEnergyDiagram]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """Set some attributes after initialization."""
         self.band_gap = self.formation_energy_diagrams[0].band_gap
         self.vbm = self.formation_energy_diagrams[0].vbm
 
     @classmethod
     def with_atomic_entries(
         cls,
@@ -720,15 +759,18 @@
                 **kwargs,
             )
             single_form_en_diagrams.append(_fd)
 
         return cls(formation_energy_diagrams=single_form_en_diagrams)
 
     def solve_for_fermi_level(
-        self, chempots: dict, temperature: int | float, dos: Dos
+        self,
+        chempots: dict,
+        temperature: float,
+        dos: Dos,
     ) -> float:
         """Solves for the equilibrium fermi level at a given chempot, temperature, density of states.
 
         Args:
             chempots: dictionary of chemical potentials to use
             temperature: temperature at which to evaluate.
             dos: Density of states object. Must contain a structure attribute. If band_gap attribute
@@ -741,114 +783,116 @@
         bulk_factor = self.formation_energy_diagrams[
             0
         ].defect.structure.composition.get_reduced_formula_and_factor()[1]
         fdos_factor = fdos.structure.composition.get_reduced_formula_and_factor()[1]
         fdos_multiplicity = fdos_factor / bulk_factor
         fdos_cbm, fdos_vbm = fdos.get_cbm_vbm()
 
-        def _get_chg(fd: FormationEnergyDiagram, ef):
+        def _get_chg(fd: FormationEnergyDiagram, ef: float) -> float:
             lines = fd._get_lines(chempots=chempots)
             return sum(
                 fd.defect.multiplicity
                 * charge
                 * fermi_dirac(vbm_fe + charge * ef, temperature)
                 for charge, vbm_fe in lines
             )
 
-        def _get_total_q(ef):
+        def _get_total_q(ef: float) -> float:
             qd_tot = sum(
                 _get_chg(fd=fd, ef=ef) for fd in self.formation_energy_diagrams
             )
             qd_tot += fdos_multiplicity * fdos.get_doping(
-                fermi_level=ef + fdos_vbm, temperature=temperature
+                fermi_level=ef + fdos_vbm,
+                temperature=temperature,
             )
             return qd_tot
 
         return bisect(_get_total_q, -1.0, fdos_cbm - fdos_vbm + 1.0)
 
 
 def group_defect_entries(
-    defect_entries: list[DefectEntry], sm: StructureMatcher = None
-):
+    defect_entries: list[DefectEntry],
+    sm: StructureMatcher = None,
+) -> Generator[tuple[str, list[DefectEntry]], None, None]:
     """Group defect entries by their representation.
 
     First by name then by structure.
 
     Args:
         defect_entries: list of defect entries
         sm: StructureMatcher to use for grouping
 
     Returns:
         Generator of (name, list of defect entries) tuples
     """
     if sm is None:
         sm = StructureMatcher(comparator=ElementComparator())
 
-    def _get_structure(entry):
+    def _get_structure(entry: DefectEntry) -> Structure:
         return entry.defect.defect_structure
 
-    def _get_name(entry):
+    def _get_name(entry: DefectEntry) -> str:
         return entry.defect.name
 
-    def _get_hash_no_structure(entry):
+    def _get_hash_no_structure(entry: DefectEntry) -> tuple[str, str]:
         return entry.defect.bulk_formula, entry.defect.name
 
     if all(isinstance(entry.defect, Defect) for entry in defect_entries):
         ent_groups = group_docs(
-            defect_entries, sm=sm, get_structure=_get_structure, get_hash=_get_name
+            defect_entries,
+            sm=sm,
+            get_structure=_get_structure,
+            get_hash=_get_name,
         )
-        for g_name, g_entries in ent_groups:
-            yield g_name, g_entries
+        yield from ent_groups
     elif all(isinstance(entry.defect, NamedDefect) for entry in defect_entries):
         l_ = sorted(defect_entries, key=_get_hash_no_structure)
-        for _, g_entries in groupby(l_, key=_get_hash_no_structure):
-            similar_ents = list(g_entries)
+        for _, g_entries_no_struct in groupby(l_, key=_get_hash_no_structure):
+            similar_ents = list(g_entries_no_struct)
             yield similar_ents[0].defect.name, similar_ents
 
 
 def group_formation_energy_diagrams(
     feds: list[FormationEnergyDiagram],
     sm: StructureMatcher = None,
-    combine_diagrams: bool = True,
-):
+) -> Generator[tuple[str | None, FormationEnergyDiagram], None, None]:
     """Group formation energy diagrams by their representation.
 
     First by name then by structure.
 
     Args:
         feds: list of formation energy diagrams
         sm: StructureMatcher to use for grouping
-        combine_diagrams: whether to combine matching diagrams into a single diagram
 
     Returns:
         If combine_diagrams is True, generator of (name, combined formation energy diagram) tuples.
         If combine_diagrams is False, generator of (name, list of formation energy diagrams) tuples.
 
     """
     if sm is None:
         sm = StructureMatcher(comparator=ElementComparator())
 
-    def _get_structure(fed):
+    def _get_structure(fed: FormationEnergyDiagram) -> Structure:
         return fed.defect.defect_structure
 
-    def _get_name(fed):
+    def _get_name(fed: FormationEnergyDiagram) -> str:
         return fed.defect.name
 
     fed_groups = group_docs(
-        feds, sm=sm, get_structure=_get_structure, get_hash=_get_name
+        feds,
+        sm=sm,
+        get_structure=_get_structure,
+        get_hash=_get_name,
     )
     for g_name, f_group in fed_groups:
-        if combine_diagrams:
-            fed = f_group[0]
-            fed_d = fed.as_dict()
-            dents = [dfed.defect_entries for dfed in f_group]
-            fed_d["defect_entries"] = list(chain.from_iterable(dents))
-            yield g_name, FormationEnergyDiagram.from_dict(fed_d)
-        else:
-            yield g_name, f_group
+        fed = f_group[0]
+        fed_d = fed.as_dict()
+        dents = [dfed.defect_entries for dfed in f_group]
+        fed_d["defect_entries"] = list(chain.from_iterable(dents))
+        yield g_name, FormationEnergyDiagram.from_dict(fed_d)
 
 
 def ensure_stable_bulk(
     pd: PhaseDiagram,
     entry: ComputedEntry,
     threshold: float = 0.001,
 ) -> PhaseDiagram:
@@ -871,22 +915,59 @@
             the convex hull.
 
     Returns:
         PhaseDiagram:
             Modified Phase diagram.
     """
     stable_entry = ComputedEntry(
-        entry.composition, pd.get_hull_energy(entry.composition) - threshold
+        entry.composition,
+        pd.get_hull_energy(entry.composition) - threshold,
+    )
+    return PhaseDiagram([*pd.all_entries, stable_entry])
+
+
+def get_sc_locpot(
+    uc_locpot: Locpot,
+    defect_struct: Structure,
+    grid_out: tuple,
+    up_sample: int = 2,
+    sm: StructureMatcher = None,
+) -> Locpot:
+    """Transform a unit cell locpot to be like a supercell locpot.
+
+    This is useful in situations where the supercell bulk locpot is not available.
+    In these cases, we will have a bulk supercell structure that is most closely
+    related to the defect cell.
+
+    Args:
+        uc_locpot: Locpot object for the unit cell.
+        defect_struct: Defect structure to use for the transformation.
+        grid_out: grid dimensions for the supercell locpot
+        up_sample: upsample factor for the supercell locpot
+        sm: StructureMatcher to use for finding the transformation for UC to SC.
+
+    Returns:
+        Locpot: Locpot object for the unit cell transformed to be like the supercell.
+    """
+    sc_mat = get_closest_sc_mat(uc_locpot.structure, sc_struct=defect_struct, sm=sm)
+    bulk_sc = uc_locpot.structure * sc_mat
+    return get_volumetric_like_sc(
+        uc_locpot,
+        bulk_sc,
+        grid_out=grid_out,
+        up_sample=up_sample,
+        sm=sm,
+        normalization=None,
     )
-    pd = PhaseDiagram(pd.all_entries + [stable_entry])
-    return pd
 
 
 def get_transitions(
-    lines: list[tuple[float, float]], x_min: float, x_max: float
+    lines: list[tuple[float, float]],
+    x_min: float,
+    x_max: float,
 ) -> list[tuple[float, float]]:
     """Get the "transition" points in a list of lines.
 
     Given a list of lines represented as (m, b) pairs sorted in order of decreasing m.
     A "transition" point is a point where adjacent lines in the list intersect.
     i.e. intersection points (x_i, y_i) where line i intersects line i+1
 
@@ -902,31 +983,32 @@
     """
     # make sure the lines are sorted by decreasing slope
     lines = sorted(lines, key=lambda x: x[0], reverse=True)
     transitions = [(x_min, lines[0][0] * x_min + lines[0][1])]
     for i, (m1, b1) in enumerate(lines[:-1]):
         m2, b2 = lines[i + 1]
         if m1 == m2:
+            msg = "The slopes (charge states) of the set of lines should be distinct."
             raise ValueError(
-                "The slopes (charge states) of the set of lines should be distinct."
+                msg,
             )  # pragma: no cover
         nx, ny = ((b2 - b1) / (m1 - m2), (m1 * b2 - m2 * b1) / (m1 - m2))
         if nx < x_min:
             transitions = [(x_min, m2 * x_min + b2)]
         elif nx > x_max:
             transitions.append((x_max, m1 * x_max + b1))
             break
         else:
             transitions.append((nx, ny))
     else:
         transitions.append((x_max, lines[-1][0] * x_max + lines[-1][1]))
     return transitions
 
 
-def get_lower_envelope(lines):
+def get_lower_envelope(lines: list[tuple[float, float]]) -> list[tuple[float, float]]:
     """Get the lower envelope of the formation energy.
 
     Based on the fact that the lower envelope of the lines is
     given by the upper convex hull of the points (m, -b) as shown in:
     https://www.cs.umd.edu/class/spring2020/cmsc754/Lects/lect06-duality.pdf
     Note: The lines are returned with decreasing slope.
 
@@ -934,36 +1016,36 @@
         lines: (m, b) format for each line
 
     Returns:
         List[List[float]]:
             List lines that make up the lower envelope.
     """
 
-    def _hash_float(x):
+    def _hash_float(x: float) -> float:
         return round(x, 10)
 
-    lines_dd = collections.defaultdict(lambda: float("inf"))
+    lines_dd: dict = collections.defaultdict(lambda: float("inf"))
     for m, b in lines:
         lines_dd[_hash_float(m)] = min(lines_dd[_hash_float(m)], b)
-    lines = [(m, b) for m, b in lines_dd.items()]
+    lines = list(lines_dd.items())
 
-    if len(lines) < 1:
-        raise ValueError("Need at least one line to get lower envelope.")
-    elif len(lines) == 1:
+    if len(lines) < 1:  # pragma: no cover
+        msg = "Need at least one line to get lower envelope."
+        raise ValueError(msg)
+    if len(lines) == 1:
         return lines
-    elif len(lines) == 2:
+    if len(lines) == 2:
         return sorted(lines)
 
     dual_points = [(m, -b) for m, b in lines]
     upper_hull = get_upper_hull(dual_points)
-    lower_envelope = [(m, -b) for m, b in upper_hull]
-    return lower_envelope
+    return [(m, -b) for m, b in upper_hull]
 
 
-def get_upper_hull(points: ArrayLike) -> List[ArrayLike]:
+def get_upper_hull(points: ArrayLike) -> list[ArrayLike]:
     """Get the upper hull of a set of points in 2D.
 
     Args:
         points:
             List of points in 2D.
 
     Returns:
@@ -990,57 +1072,60 @@
             xi, yi = points[i]
             upper_hull.append((xi, yi))
         if seen_right_most and i == left_most_idx:
             break
     return upper_hull
 
 
-def _get_adjusted_pd_entries(phase_diagram, atomic_entries) -> list[ComputedEntry]:
+def _get_adjusted_pd_entries(
+    phase_diagram: PhaseDiagram, atomic_entries: Sequence[ComputedEntry]
+) -> list[ComputedEntry]:
     """Get the adjusted entries for the phase diagram.
 
     Combine the terminal energies from ``atomic_entries`` with the enthalpies of formation
     for the provided ``phase_diagram``.  To create the entries for a new phase diagram.
 
     Args:
         phase_diagram: Phase diagram where the enthalpies of formation are taken from.
         atomic_entries: Entries for the terminal energies.
 
     Returns:
         List[ComputedEntry]: Entries for the new phase diagram.
     """
 
-    def get_interp_en(entry: ComputedEntry):
+    def get_interp_en(entry: ComputedEntry) -> float:
         """Get the interpolated energy of an entry."""
-        e_dict = dict()
+        e_dict = {}
         for e in atomic_entries:
-            if len(e.composition.elements) != 1:
+            if len(e.composition.elements) != 1:  # pragma: no cover
+                msg = "Only single-element entries should be provided."
                 raise ValueError(
-                    "Only single-element entries should be provided."
-                )  # pragma: no cover
+                    msg,
+                )
             e_dict[e.composition.elements[0]] = e.energy_per_atom
 
         return sum(
             entry.composition[el] * e_dict[el] for el in entry.composition.elements
         )
 
     adjusted_entries = []
 
     for entry in phase_diagram.stable_entries:
-        d_ = dict(
-            energy=get_interp_en(entry) + phase_diagram.get_form_energy(entry),
-            composition=entry.composition,
-            entry_id=entry.entry_id,
-            correction=0,
-        )
+        d_ = {
+            "energy": get_interp_en(entry) + phase_diagram.get_form_energy(entry),
+            "composition": entry.composition,
+            "entry_id": entry.entry_id,
+            "correction": 0,
+        }
         adjusted_entries.append(ComputedEntry.from_dict(d_))
 
     return adjusted_entries
 
 
-def fermi_dirac(energy: float, temperature: int | float) -> float:
+def fermi_dirac(energy: float, temperature: float) -> float:
     """Get value of fermi dirac distribution.
 
     Gets the defects equilibrium concentration (up to the multiplicity factor)
     at a particular fermi level, chemical potential, and temperature (in Kelvin),
     assuming dilute limit thermodynamics (non-interacting defects) using FD statistics.
 
     Args:
@@ -1048,38 +1133,38 @@
         temperature: Temperature in Kelvin.
     """
     return 1.0 / (1.0 + np.exp((energy) / (boltzman_eV_K * temperature)))
 
 
 def plot_formation_energy_diagrams(
     formation_energy_diagrams: FormationEnergyDiagram
-    | List[FormationEnergyDiagram]
+    | list[FormationEnergyDiagram]
     | MultiFormationEnergyDiagram,
     rich_element: Element | None = None,
-    chempots: Dict | None = None,
+    chempots: dict | None = None,
     alignment: float = 0.0,
     xlim: list | None = None,
     ylim: list | None = None,
     only_lower_envelope: bool = True,
     show: bool = True,
     save: bool | str = False,
     colors: list | None = None,
     legend_prefix: str | None = None,
     transition_marker: str = "*",
     transition_markersize: int = 16,
     linestyle: str = "-",
     linewidth: int = 4,
     envelope_alpha: float = 0.8,
     line_alpha: float = 0.5,
-    band_edge_color="k",
+    band_edge_color: str = "k",
     filterfunction: Callable | None = None,
     legend_loc: str = "lower center",
     show_legend: bool = True,
-    axis=None,
-):
+    axis: Axes = None,
+) -> Axes:
     """Plot the formation energy diagram.
 
     Args:
         formation_energy_diagrams: Which formation energy lines to plot.
         rich_element: The abundant element used to set the limit of the chemical potential.
         chempots: Chemical potentials at which to plot the formation energy lines
             Should be bounded by the chempot_limits property
@@ -1115,20 +1200,21 @@
         Axis subplot
     """
     if isinstance(formation_energy_diagrams, MultiFormationEnergyDiagram):
         formation_energy_diagrams = formation_energy_diagrams.formation_energy_diagrams
     elif isinstance(formation_energy_diagrams, FormationEnergyDiagram):
         formation_energy_diagrams = [formation_energy_diagrams]
 
-    filterfunction = filterfunction if filterfunction else lambda x: True
+    filterfunction = filterfunction if filterfunction else lambda _x: True
     formation_energy_diagrams = list(filter(filterfunction, formation_energy_diagrams))
 
     band_gap = formation_energy_diagrams[0].band_gap
     if not xlim and band_gap is None:
-        raise ValueError("Must specify xlim or set band_gap attribute")
+        msg = "Must specify xlim or set band_gap attribute"
+        raise ValueError(msg)
 
     if axis is None:
         _, axis = plt.subplots()
     axis.axvline(band_gap, color=band_edge_color, linestyle="--", linewidth=1)
     axis.axvline(0, color=band_edge_color, linestyle="--", linewidth=1)
     if not xlim:
         xmin, xmax = (
@@ -1145,31 +1231,33 @@
     lg_fontsize = 10
 
     named_feds = []
     for name_, fed_ in group_formation_energy_diagrams(formation_energy_diagrams):
         named_feds.append((name_, fed_))
 
     color_line_gen = _get_line_color_and_style(colors, linestyle)
-    for fid, (fed_name, single_fed) in enumerate(named_feds):
+    for _fid, (fed_name, single_fed) in enumerate(named_feds):
         cur_color, cur_style = next(color_line_gen)
         chempots_ = (
             chempots
             if chempots
             else single_fed.get_chempots(rich_element=Element(rich_element))
         )
         lines = single_fed._get_lines(chempots=chempots_)
         lowerlines = get_lower_envelope(lines)
         trans = np.array(
             get_transitions(
-                lowerlines, np.add(xmin, alignment), np.add(xmax, alignment)
-            )
+                lowerlines,
+                np.add(xmin, alignment),
+                np.add(xmax, alignment),
+            ),
         )
         trans_y = trans[:, 1]
-        ymin = min(ymin, min(trans_y))
-        ymax = max(ymax, max(trans_y))
+        ymin = min(ymin, *trans_y)
+        ymax = max(ymax, *trans_y)
 
         dfct: Defect = single_fed.defect_entries[0].defect
         latexname = dfct.latex_name
         if legend_prefix is not None:
             latexname = f"{legend_prefix} {latexname}"
 
         if ":" in fed_name:
@@ -1188,15 +1276,18 @@
         )
         if not only_lower_envelope:
             cur_color = _l.get_color()
             for line in lines:
                 x = np.linspace(xmin, xmax)
                 y = line[0] * x + line[1]
                 axis.plot(
-                    np.subtract(x, alignment), y, color=cur_color, alpha=line_alpha
+                    np.subtract(x, alignment),
+                    y,
+                    color=cur_color,
+                    alpha=line_alpha,
                 )
 
     axis.set_xlim(xmin, xmax)
     axis.set_ylim(ylim[0] if ylim else ymin - 0.1, ylim[1] if ylim else ymax + 0.1)
     axis.set_xlabel("Fermi energy (eV)", size=ax_fontsize * fontwidth)
     axis.set_ylabel("Defect Formation\nEnergy (eV)", size=ax_fontsize * fontwidth)
     axis.minorticks_on()
@@ -1219,15 +1310,19 @@
         labelsize=fontwidth * ax_fontsize,
     )
     for _ax in axis.spines.values():
         _ax.set_linewidth(1.5)
 
     axis.axvline(0, ls="--", color="k", lw=2, alpha=0.2)
     axis.axvline(
-        np.subtract(0, alignment), ls="--", color=band_edge_color, lw=2, alpha=0.8
+        np.subtract(0, alignment),
+        ls="--",
+        color=band_edge_color,
+        lw=2,
+        alpha=0.8,
     )
     if band_gap:
         axis.axvline(
             np.subtract(band_gap, alignment),
             ls="--",
             color=band_edge_color,
             lw=2,
@@ -1254,15 +1349,17 @@
         plt.savefig(save)
     if show:
         plt.show()
 
     return axis
 
 
-def _get_line_color_and_style(colors=None, styles=None):
+def _get_line_color_and_style(
+    colors: Sequence | None = None, styles: Sequence | None = None
+) -> Generator[tuple[str, str], None, None]:
     """Get a generator for colors and styles.
 
     Create an iterator that will cycle through the colors and styles.
 
     Args:
         colors: List of colors to use, if None, use the default matplotlib colors.
         styles: List of styles to use, if None, will use ["-", "--", "-.", ":"]
@@ -1278,15 +1375,15 @@
         styles = [styles] if isinstance(styles, str) else styles
 
     for style in styles:
         for color in colors:
             yield color, style
 
 
-def _is_on_hyperplane(pt: np.array, hp: np.array, tol: float = 1e-8):
+def _is_on_hyperplane(pt: np.array, hp: np.array, tol: float = 1e-8) -> bool:
     """Check if a point lies on a hyperplane.
 
     Args:
         pt: point to check
         hp: hyperplane ((a, b, c, d) such that ax + by + cz + d = 0)
         tol: tolerance for checking if the point lies on the hyperplane
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen/analysis/defects/utils.py` & `pymatgen_analysis_defects-2024.4.22/pymatgen/analysis/defects/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Utilities for defects module."""
+
 from __future__ import annotations
 
 import bisect
 import collections
 import itertools
 import logging
 import math
 import operator
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Callable, Generator
+from typing import TYPE_CHECKING, Any, Callable
 
 import numpy as np
 from monty.dev import deprecated
 from monty.json import MSONable
 from numpy.linalg import norm
 from pymatgen.analysis.local_env import cn_opt_params
 from pymatgen.analysis.structure_matcher import StructureMatcher
@@ -25,14 +26,15 @@
 from pymatgen.io.vasp.sets import get_valid_magmom_struct
 from pymatgen.util.coord import pbc_diff
 from scipy.cluster.hierarchy import fcluster, linkage
 from scipy.spatial import ConvexHull, Voronoi
 from scipy.spatial.distance import squareform
 
 if TYPE_CHECKING:
+    from collections.abc import Generator
     from pathlib import Path
 
     from numpy import typing as npt
     from pymatgen.core import Lattice
     from pymatgen.io.vasp.outputs import BandStructure, Procar, VolumetricData
 
 try:
@@ -73,15 +75,17 @@
     q_model(r) = q [x exp(-r/gamma) + (1-x) exp(-r^2/beta^2)]
     without normalization constants
 
     By default, gaussian distribution with 1 Bohr width is assumed.
     If defect charge is more delocalized, exponential tail is suggested.
     """
 
-    def __init__(self, beta=1.0, expnorm=0.0, gamma=1.0):
+    def __init__(
+        self, beta: float = 1.0, expnorm: float = 0.0, gamma: float = 1.0
+    ) -> None:
         """Initialize the model.
 
         Args:
             beta: Gaussian decay constant. Default value is 1 Bohr.
                 When delocalized (eg. diamond), 2 Bohr is more appropriate.
             expnorm: Weight for the exponential tail in the range of [0-1].
                 Default is 0.0 indicating no tail. For delocalized charges ideal value
@@ -91,17 +95,18 @@
         self.beta = beta
         self.expnorm = expnorm
         self.gamma = gamma
 
         self.beta2 = beta * beta
         self.gamma2 = gamma * gamma
         if expnorm and not gamma:
-            raise ValueError("Please supply exponential decay constant.")
+            msg = "Please supply exponential decay constant."
+            raise ValueError(msg)
 
-    def rho_rec(self, g2):
+    def rho_rec(self, g2: float) -> float:
         """Reciprocal space model charge value.
 
         Reciprocal space model charge value, for input squared reciprocal vector.
 
         Args:
             g2: Square of reciprocal vector
 
@@ -109,36 +114,38 @@
             Charge density at the reciprocal vector magnitude
         """
         return self.expnorm / np.sqrt(1 + self.gamma2 * g2) + (
             1 - self.expnorm
         ) * np.exp(-0.25 * self.beta2 * g2)
 
     @property
-    def rho_rec_limit0(self):
+    def rho_rec_limit0(self) -> float:
         """Reciprocal space model charge value.
 
         Close to reciprocal vector 0 .
         rho_rec(g->0) -> 1 + rho_rec_limit0 * g^2
         """
         return -2 * self.gamma2 * self.expnorm - 0.25 * self.beta2 * (1 - self.expnorm)
 
 
-def eV_to_k(energy):
+def eV_to_k(energy: float) -> float:
     """Convert energy to reciprocal vector magnitude k via hbar*k^2/2m.
 
     Args:
         energy: Energy in eV.
 
     Returns:
         (double) Reciprocal vector magnitude (units of 1/Bohr).
     """
     return math.sqrt(energy / invang_to_ev) * ang_to_bohr
 
 
-def genrecip(a1, a2, a3, encut) -> Generator[npt.ArrayLike, None, None]:
+def genrecip(
+    a1: npt.ArrayLike, a2: npt.ArrayLike, a3: npt.ArrayLike, encut: float
+) -> Generator[npt.ArrayLike, None, None]:
     """Generate reciprocal lattice vectors within the energy cutoff.
 
     Args:
         a1: Lattice vector a (in Bohrs)
         a2: Lattice vector b (in Bohrs)
         a3: Lattice vector c (in Bohrs)
         encut: energy cut off in eV
@@ -172,15 +179,17 @@
 
     # Yield based on radii
     for vec, r in zip(vecs, radii):
         if r < G_cut and r != 0:
             yield vec
 
 
-def generate_reciprocal_vectors_squared(a1, a2, a3, encut):
+def generate_reciprocal_vectors_squared(
+    a1: npt.ArrayLike, a2: npt.ArrayLike, a3: npt.ArrayLike, encut: float
+) -> Generator[float, None, None]:
     """Generate Reciprocal vectors squared.
 
     Generate reciprocal vector magnitudes within the cutoff along the specified
     lattice vectors.
 
     Args:
         a1: Lattice vector a (in Bohrs)
@@ -192,15 +201,15 @@
         [[g1^2], [g2^2], ...] Square of reciprocal vectors (1/Bohr)^2
         determined by a1, a2, a3 and whose magntidue is less than gcut^2.
     """
     for vec in genrecip(a1, a2, a3, encut):
         yield np.dot(vec, vec)
 
 
-def converge(f, step, tol, max_h) -> float:
+def converge(f: Callable, step: float, tol: float, max_h: float) -> float:
     """Simple newton iteration based convergence function.
 
     Args:
         f: function to converge
         step: step size for newton iteration
         tol: tolerance for convergence
         max_h: maximum value of h to try before giving up
@@ -214,58 +223,62 @@
     while dx > tol:
         g2 = f(h)
         dx = abs(g - g2)
         g = g2
         h += step
 
         if h > max_h:
-            raise Exception(f"Did not converge before {h}")
+            msg = f"Did not converge before {h}"
+            raise Exception(msg)
     return g
 
 
 def get_zfile(
-    directory: Path, base_name: str, allow_missing: bool = False
+    directory: Path,
+    base_name: str,
+    allow_missing: bool = False,
 ) -> Path | None:
     """Find gzipped or non-gzipped versions of a file in a directory listing.
 
     Args:
         directory : A list of files in a directory.
         base_name : The base name of file file to find.
         allow_missing : Whether to error if no version of the file (gzipped or un-gzipped) can be found.
 
     Returns:
         Path | None: A path to the matched file. If ``allow_missing=True``
         and the file cannot be found, then ``None`` will be returned.
     """
     for file in directory.glob(f"{base_name}*"):
-        if base_name == file.name:
-            return file
-        elif base_name + ".gz" == file.name:
-            return file
-        elif base_name + ".GZ" == file.name:
+        if (
+            base_name == file.name
+            or base_name + ".gz" == file.name
+            or base_name + ".GZ" == file.name
+        ):
             return file
 
     if allow_missing:
         return None
 
-    raise FileNotFoundError(f"Could not find {base_name} or {base_name}.gz file.")
+    msg = f"Could not find {base_name} or {base_name}.gz file."
+    raise FileNotFoundError(msg)
 
 
-def generic_group_labels(list_in, comp=operator.eq):
+def generic_group_labels(list_in: list, comp: Callable = operator.eq) -> list[int]:
     """Group a list of unsortable objects.
 
     Args:
         list_in: A list of generic objects
         comp: (Default value = operator.eq) The comparator
 
     Returns:
         list[int]: list of labels for the input list
 
     """
-    list_out = [None] * len(list_in)
+    list_out: list[int | None] = [None] * len(list_in)
     label_num = 0
     for i1, ls1 in enumerate(list_out):
         if ls1 is not None:
             continue
         list_out[i1] = label_num
         for i2, ls2 in list(enumerate(list_out))[(i1 + 1) :]:
             if comp(list_in[i1], list_in[i2]):
@@ -289,18 +302,15 @@
         find_min (bool): True to find local minimum else maximum, otherwise
             find local maximum.
 
     Returns:
         extrema_coords (list): list of fractional coordinates corresponding
             to local extrema.
     """
-    if find_min:
-        sign = -1
-    else:
-        sign = 1
+    sign = -1 if find_min else 1
 
     # Make 3x3x3 supercell
     # This is a trick to resolve the periodical boundary issue.
     # TODO: Add code to pyrho for max and min filtering.
     total_chg = sign * chgcar.data["total"]
     total_chg = np.tile(total_chg, reps=(3, 3, 3))
     coordinates = peak_local_max(total_chg, min_distance=1)
@@ -311,15 +321,17 @@
         f - 1 for f in f_coords if all(np.array(f) < 2) and all(np.array(f) >= 1)
     ]
 
     return np.array(f_coords)
 
 
 def remove_collisions(
-    fcoords: npt.NDArray, structure: Structure, min_dist: float = 0.9
+    fcoords: npt.NDArray,
+    structure: Structure,
+    min_dist: float = 0.9,
 ) -> npt.NDArray:
     """Removed points that are too close to existing atoms in the structure.
 
     Args:
         fcoords (npt.ArrayLike): fractional coordinates of points to remove
         structure (Structure): The structure in which to check for collisions.
         min_dist(float): The minimum distance that a vertex needs to be
@@ -329,20 +341,22 @@
         fcoord (numpy.ndarray): The filtered coordinates.
     """
     s_fcoord = structure.frac_coords
     _logger.info(s_fcoord)
     dist_matrix = structure.lattice.get_all_distances(fcoords, s_fcoord)
     all_dist = np.min(dist_matrix, axis=1)
     return np.array(
-        [fcoords[i] for i in range(len(fcoords)) if all_dist[i] >= min_dist]
+        [fcoords[i] for i in range(len(fcoords)) if all_dist[i] >= min_dist],
     )
 
 
 def cluster_nodes(
-    fcoords: npt.ArrayLike, lattice: Lattice, tol: float = 0.2
+    fcoords: npt.ArrayLike,
+    lattice: Lattice,
+    tol: float = 0.2,
 ) -> npt.NDArray:
     """Cluster nodes that are too close together using hiercharcal clustering.
 
     Args:
         fcoords (npt.ArrayLike): fractional coordinates of points to cluster.
         lattice (Lattice): The lattice of the structure.
         tol (float): A distance tolerance. PBC is taken into account.
@@ -379,15 +393,17 @@
     # np.array([ 5.0000000e-01 -4.4408921e-17  5.0000000e-01])
     # where the shift to [0,1) does not work due to float precision
 
     return np.array(merged_fcoords)
 
 
 def get_avg_chg(
-    chgcar: VolumetricData, fcoord: npt.ArrayLike, radius: float = 0.4
+    chgcar: VolumetricData,
+    fcoord: npt.ArrayLike,
+    radius: float = 0.4,
 ) -> float:
     """Get the average charge in a sphere.
 
     Args:
         chgcar: The charge density.
         fcoord: The fractional coordinates of the center of the sphere.
         radius: The radius of the sphere in Angstroms.
@@ -396,32 +412,32 @@
         The average charge in the sphere.
 
 
     """
     # makesure fcoord is an array
     fcoord = np.array(fcoord)
 
-    def _dist_mat(pos_frac):
+    def _dist_mat(pos_frac: npt.ArrayLike) -> npt.NDArray:
         # return a matrix that contains the distances
         aa = np.linspace(0, 1, len(chgcar.get_axis_grid(0)), endpoint=False)
         bb = np.linspace(0, 1, len(chgcar.get_axis_grid(1)), endpoint=False)
         cc = np.linspace(0, 1, len(chgcar.get_axis_grid(2)), endpoint=False)
         AA, BB, CC = np.meshgrid(aa, bb, cc, indexing="ij")
         dist_from_pos = chgcar.structure.lattice.get_all_distances(
             fcoords1=np.vstack([AA.flatten(), BB.flatten(), CC.flatten()]).T,
             fcoords2=pos_frac,
         )
         return dist_from_pos.reshape(AA.shape)
 
     if np.any(fcoord < 0) or np.any(fcoord > 1):
-        raise ValueError("f_coords must be in [0,1)")
+        msg = "f_coords must be in [0,1)"
+        raise ValueError(msg)
     mask = _dist_mat(fcoord) < radius
     vol_sphere = chgcar.structure.volume * (mask.sum() / chgcar.ngridpts)
-    avg_chg = np.sum(chgcar.data["total"] * mask) / mask.size / vol_sphere
-    return avg_chg
+    return np.sum(chgcar.data["total"] * mask) / mask.size / vol_sphere
 
 
 class TopographyAnalyzer:
     """Topography Analyzer.
 
     This is a generalized module to perform topological analyses of a crystal
     structure using Voronoi tessellations. It can be used for finding potential
@@ -435,28 +451,28 @@
     typical use is something like::
 
         a = TopographyAnalyzer(structure, ["O", "P"])
     """
 
     def __init__(
         self,
-        structure,
-        framework_ions,
-        cations,
-        image_tol=0.0001,
-        max_cell_range=1,
-        check_volume=True,
-        constrained_c_frac=0.5,
-        thickness=0.5,
+        structure: Structure,
+        framework_ions: list[str],
+        cations: list[str],
+        image_tol: float = 0.0001,
+        max_cell_range: int = 1,
+        check_volume: bool = True,
+        constrained_c_frac: float = 0.5,
+        thickness: float = 0.5,
         clustering_tol: float = 0.5,
         min_dist: float = 0.9,
         ltol: float = 0.2,
         stol: float = 0.3,
         angle_tol: float = 5,
-    ):
+    ) -> None:
         """Initialize the TopographyAnalyzer.
 
         Args:
             structure (Structure): An initial structure.
             framework_ions ([str]): A list of ions to be considered as a
                 framework. Typically, this would be all anion species. E.g.,
                 ["O", "S"].
@@ -505,29 +521,30 @@
 
         # if input cell is very small (< 5 atoms) and max cell range is 1 (default), bump to 2 for
         # accurate Voronoi tessellation:
         if len(structure) < 5 and max_cell_range == 1:
             max_cell_range = 2
 
         # Let us first map all sites to the standard unit cell, i.e.,
+
         # 0 ≤ coordinates < 1.
         # structure = Structure.from_sites(structure, to_unit_cell=True)
         # lattice = structure.lattice
 
         # We could constrain the region where we want to dope/explore by setting
         # the value of constrained_c_frac and thickness. The default mode is
         # mapping all sites to the standard unit cell
 
         self.structure = structure.copy()
-        # TODO: Structure is still being mutated something weird is going on but the code works.
+        # NOTE: Structure is still being mutated something weird is going on but the code works.
         # remove oxidation state
         self.structure.remove_oxidation_states()
 
         constrained_sites = []
-        for i, site in enumerate(self.structure):
+        for _i, site in enumerate(self.structure):
             if (
                 site.frac_coords[2] >= constrained_c_frac - thickness
                 and site.frac_coords[2] <= constrained_c_frac + thickness
             ):
                 constrained_sites.append(site)
         constrained_struct = Structure.from_sites(sites=constrained_sites)
         lattice = constrained_struct.lattice
@@ -562,22 +579,22 @@
 
         # Store a mapping of each voronoi node to a set of points.
         node_points_map = defaultdict(set)
         for pts, vs in voro.ridge_dict.items():
             for v in vs:
                 node_points_map[v].update(pts)
 
-        _logger.debug(f"{len(voro.vertices)} total Voronoi vertices")
+        _logger.debug("Voronoi vertices in cell: %s", len(voro.vertices))
 
         # Vnodes store all the valid voronoi polyhedra. Cation vnodes store
         # the voronoi polyhedra that are already occupied by existing cations.
         vnodes: list[VoronoiPolyhedron] = []
         cation_vnodes = []
 
-        def get_mapping(poly):
+        def get_mapping(poly: VoronoiPolyhedron) -> VoronoiPolyhedron | None:
             """Helper function.
 
             Checks if a vornoi poly is a periodic image of
             one of the existing voronoi polys.
             """
             for v in vnodes:
                 if v.is_image(poly, image_tol):
@@ -595,15 +612,15 @@
                 if len(vnodes) == 0:
                     vnodes.append(poly)
                 else:
                     ref = get_mapping(poly)
                     if ref is None:
                         vnodes.append(poly)
 
-        _logger.debug(f"{len(vnodes)} voronoi vertices in cell.")
+        _logger.debug("%s - voronoi vertices in cell.", len(vnodes))
 
         # Eliminate all voronoi nodes which are closest to existing cations.
         if len(cations) > 0:
             cation_coords = [
                 site.frac_coords
                 for site in non_framework
                 if self.cations.intersection(site.species.keys())
@@ -611,15 +628,15 @@
 
             vertex_fcoords = [v.frac_coords for v in vnodes]
             dist_matrix = lattice.get_all_distances(cation_coords, vertex_fcoords)
             indices = np.where(dist_matrix == np.min(dist_matrix, axis=1)[:, None])[1]
             cation_vnodes = [v for i, v in enumerate(vnodes) if i in indices]
             vnodes = [v for i, v in enumerate(vnodes) if i not in indices]
 
-        _logger.debug(f"{len(vnodes)} vertices in cell not with cation.")
+        _logger.debug("%s - vertices in cell not with cation.", len(vnodes))
         self.coords = coords
         self.vnodes = vnodes
         self.cation_vnodes = cation_vnodes
         self.framework = framework
         self.non_framework = non_framework
         if check_volume:
             self.check_volume()
@@ -640,45 +657,55 @@
             host_structure=self.structure,
             working_ion="X",
             min_dist=self.min_dist,
             clustering_tol=self.clustering_tol,
             sm=self.sm,
         )
 
-    def check_volume(self):
+    def check_volume(self) -> None:
         """Basic check for volume of all voronoi poly sum to unit cell volume.
 
         Note that this does not apply after poly combination.
         """
         vol = sum(v.volume for v in self.vnodes) + sum(
             v.volume for v in self.cation_vnodes
         )
         if abs(vol - self.structure.volume) > 1e-8:  # pragma: no cover
-            raise ValueError(
+            msg = (
                 "Sum of voronoi volumes is not equal to original volume of "
                 "structure! This may lead to inaccurate results. You need to "
                 "tweak the tolerance and max_cell_range until you get a "
                 "correct mapping."
             )
+            raise ValueError(
+                msg,
+            )
 
-    def get_structure_with_nodes(self):
+    def get_structure_with_nodes(self) -> Structure:
         """Get the modified structure with the voronoi nodes inserted.
 
         The species is set as a DummySpecies X.
         """
         new_s = Structure.from_sites(self.structure)
         for v in self.vnodes:
             new_s.append("X", v.frac_coords)
         return new_s
 
 
 class VoronoiPolyhedron:
     """Convenience container for a voronoi point in PBC and its associated polyhedron."""
 
-    def __init__(self, lattice, frac_coords, polyhedron_indices, all_coords, name=None):
+    def __init__(
+        self,
+        lattice: Lattice,
+        frac_coords: npt.ArrayLike,
+        polyhedron_indices: list | set,
+        all_coords: list,
+        name: str | int | None = None,
+    ) -> None:
         """Initialize a VoronoiPolyhedron.
 
         Args:
             lattice (Lattice): Lattice of the structure.
             frac_coords (np.array): Fractional coordinates of the voronoi point.
             polyhedron_indices (list): Indices of the polyhedron vertices.
             all_coords (list): List of all polyhedron vertices.
@@ -712,24 +739,24 @@
                     found = True
                     break
             if not found:
                 return False
         return True
 
     @property
-    def coordination(self):
+    def coordination(self) -> int:
         """Coordination number."""
         return len(self.polyhedron_indices)
 
     @property
-    def volume(self):
+    def volume(self) -> float:
         """Volume of the polyhedron."""
         return calculate_vol(self.polyhedron_coords)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """String representation."""
         return f"Voronoi polyhedron {self.name}"
 
 
 class ChargeInsertionAnalyzer(MSONable):
     """Object for insertions sites from charge density.
 
@@ -764,15 +791,15 @@
         chgcar: VolumetricData,
         working_ion: str = "Li",
         clustering_tol: float = 0.5,
         ltol: float = 0.2,
         stol: float = 0.3,
         angle_tol: float = 5,
         min_dist: float = 0.9,
-    ):
+    ) -> None:
         """Initialize the ChargeInsertionAnalyzer."""
         self.chgcar = chgcar
         self.working_ion = working_ion
         self.sm = StructureMatcher(ltol=ltol, stol=stol, angle_tol=angle_tol)
         self.clustering_tol = clustering_tol
         self.min_dist = min_dist
 
@@ -798,15 +825,17 @@
 
     @cached_property
     def local_minima(self) -> list[npt.ArrayLike]:
         """Get the full list of local minima."""
         return [s for s, _ in self.labeled_sites]
 
     def filter_and_group(
-        self, avg_radius: float = 0.4, max_avg_charge: float = 1.0
+        self,
+        avg_radius: float = 0.4,
+        max_avg_charge: float = 1.0,
     ) -> list[tuple[float, list[list[float]]]]:
         """Filter and group the insertion sites by average charge.
 
         Args:
             avg_radius: The radius used to calculate average charge density.
             max_avg_charge: Do no consider local minmas with avg charge above this value.
 
@@ -818,27 +847,29 @@
         lab_groups = collections.defaultdict(list)
         for idx, (_, lab) in enumerate(self.labeled_sites):
             lab_groups[lab].append(idx)
 
         avg_chg_first_member = {}
         for lab, g in lab_groups.items():
             avg_chg_first_member[lab] = get_avg_chg(
-                self.chgcar, fcoord=self.local_minima[g[0]], radius=avg_radius
+                self.chgcar,
+                fcoord=self.local_minima[g[0]],
+                radius=avg_radius,
             )
 
         res = []
         for lab, avg_chg in sorted(avg_chg_first_member.items(), key=lambda x: x[1]):
             if avg_chg > max_avg_charge:
                 break
             res.append((avg_chg, [self.local_minima[idx] for idx in lab_groups[lab]]))
 
         return res
 
 
-def _get_ipr(spin, k_index, procar):
+def _get_ipr(spin: int, k_index: int, procar: Procar) -> npt.NDArray:
     states = procar.data[spin][k_index, ...]
     flat_states = states.reshape(states.shape[0], -1)
     return 1 / np.sum(flat_states**2, axis=1)
 
 
 def get_ipr_in_window(
     bandstructure: BandStructure,
@@ -854,27 +885,28 @@
             The band just below the fermi level is used as the center of band window.
         procar: The procar object.
         band_window: The number of bands above and blow the fermi level to include in the search window.
 
     Returns:
         dict[(int, int), npt.NDArray]: The IPR of the states in the band window keyed for each k-point and spin.
     """
-    res = dict()
-    for spin in bandstructure.bands.keys():
+    res = {}
+    for spin in bandstructure.bands:
         s_index = 0 if spin == Spin.up else 1
         # last band that is fully below the fermi level
         last_occ_idx = bisect.bisect_left(
-            bandstructure.bands[spin].max(1), bandstructure.efermi
+            bandstructure.bands[spin].max(1),
+            bandstructure.efermi,
         )
         lbound = max(last_occ_idx - band_window, 0)
         ubound = min(last_occ_idx + band_window, bandstructure.nb_bands)
         for k_idx, _ in enumerate(bandstructure.kpoints):
             ipr = _get_ipr(spin, k_idx, procar)
             res[(k_idx, s_index)] = np.stack(
-                (np.arange(lbound, ubound), ipr[lbound:ubound])
+                (np.arange(lbound, ubound), ipr[lbound:ubound]),
             ).T
     return res
 
 
 def get_localized_states(
     bandstructure: BandStructure,
     procar: Procar,
@@ -899,16 +931,19 @@
     for (k_index, ispin), ib_ipr in d_ib_ipr.items():
         # find the index of the minimum IPR
         min_idx, val = min(ib_ipr, key=lambda x: x[1])
         yield (int(min_idx), k_index, ispin, val)
 
 
 def sort_positive_definite(
-    list_in: list, ref1: Any, ref2: Any, dist: Callable
-) -> tuple[list, list[float]]:
+    list_in: list,
+    ref1: object,
+    ref2: object,
+    dist: Callable,
+) -> tuple[tuple, tuple[float]]:
     """Sort a list where we can only compute a positive-definite distance.
 
     Sometimes, we can only compute a positive-definite distance between two objects.
     (E.g., the displacement between two structures). In these cases, standard
     sorting algorithms will not work. Here, we accept two reference points to give
     some sense of direction. We then sort the list based on the distance between the
     reference points. Note: this only works if the list falls on a line of some sort.
@@ -934,30 +969,29 @@
             sign = -1
         d_vs_s.append((sign * q1, el))
     d_vs_s.sort()
     distances, sorted_list = list(zip(*d_vs_s))
     return sorted_list, distances
 
 
-def calculate_vol(coords: npt.NDArray):
+def calculate_vol(coords: npt.NDArray) -> float:
     """Calculate volume given a set of points in 3D space.
 
     Args:
         coords: The coordinates of the points in 3D space.
 
     Returns:
         The volume of the convex hull of the points.
     """
     return ConvexHull(coords).volume
 
 
-@deprecated("Name changed")
-def get_symmetry_labeled_structures():
+@deprecated("Name changed to get_labeled_inserted_structure.")
+def get_symmetry_labeled_structures() -> None:
     """Deprecated."""
-    pass
 
 
 def get_labeled_inserted_structure(
     sites: npt.NDArray,
     host_structure: Structure,
     working_ion: str,
     min_dist: float,
@@ -1014,15 +1048,17 @@
         metadata: A dictionary of metadata for plotting and intermediate analysis.
     """
 
     correction_energy: float
     metadata: dict[Any, Any]
 
 
-def _group_docs_by_structure(docs: list, sm: StructureMatcher, get_structure: Callable):
+def _group_docs_by_structure(
+    docs: list, sm: StructureMatcher, get_structure: Callable
+) -> Generator[list, None, None]:
     """Group docs by structure.
 
     Args:
         docs (list): list of generic documents/objects.
         sm (StructureMatcher): StructureMatcher object.
         get_structure (function): function to get the representative structure from the document.
 
@@ -1030,24 +1066,23 @@
         Generator of lists of grouped documents/objects.
     """
     labs = generic_group_labels(
         docs,
         comp=lambda x, y: sm.fit(get_structure(x), get_structure(y), symmetric=True),
     )
     for ilab in set(labs):
-        sub_g = [docs[itr] for itr, jlab in enumerate(labs) if jlab == ilab]
-        yield [el for el in sub_g]
+        yield [docs[itr] for itr, jlab in enumerate(labs) if jlab == ilab]
 
 
 def group_docs(
     docs: list,
     sm: StructureMatcher,
     get_structure: Callable,
     get_hash: Callable | None = None,
-):
+) -> Generator[tuple[str | None, list], None, None]:
     """Group docs by a simple hash followed by structure.
 
     Assuming that you have a basic representation of the defect, like `name`.
     Will first group the documents by name, then group them by the structure
     of their representation.
 
     Args:
@@ -1057,16 +1092,16 @@
             this should be some kind of simple string representation.
         get_structure (function): function to get the structure from the document
 
     Returns:
         Generator of (name, group)
     """
     if get_hash is None:
-        for g in _group_docs_by_structure(docs, sm, get_structure):
-            yield None, g
+        for g_ in _group_docs_by_structure(docs, sm, get_structure):
+            yield None, g_
     else:
         s_docs = sorted(docs, key=get_hash)
         for h, g in itertools.groupby(s_docs, key=get_hash):
             sgroups = list(_group_docs_by_structure(list(g), sm, get_structure))
             if len(sgroups) <= 1:
                 for group in sgroups:
                     yield h, group
@@ -1102,14 +1137,14 @@
         (i, j): np.dot(lattice[i], lattice[j]) / latt_len[i] / latt_len[j]
         for i, j in idx_pairs
     }
     # get the spacing in each direction:
     spacing = []
     for idir in range(ndim):
         idir_proj = [
-            np.array(lattice[j]) * pproj[tuple(sorted([idir, j]))]  # type: ignore
+            np.array(lattice[j]) * pproj[tuple(sorted([idir, j]))]  # type: ignore[index]
             for j in range(ndim)
             if j != idir
         ]
         v_perp_subspace = lattice[idir] - sum(idir_proj)
         spacing.append(np.linalg.norm(v_perp_subspace))
     return spacing
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen_analysis_defects-2024.4.22/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2024.2.9
+Version: 2024.4.22
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
@@ -14,151 +14,159 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymatgen
 Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: numpy
+Requires-Dist: mp-pyrho>=0.4.4
 Provides-Extra: finder
 Requires-Dist: dscribe>=2.0.0; extra == "finder"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: jupyter-book>=0.13.1; extra == "docs"
 Provides-Extra: optional
 Requires-Dist: pydefect>=0.6.2; extra == "optional"
 Requires-Dist: dscribe>=2.0.0; extra == "optional"
 Requires-Dist: numba; extra == "optional"
 Provides-Extra: strict
-Requires-Dist: pymatgen==2023.10.11; extra == "strict"
+Requires-Dist: pymatgen==2024.3.1; extra == "strict"
 Requires-Dist: dscribe==2.1.0; extra == "strict"
-Requires-Dist: scikit-image==0.21.0; extra == "strict"
+Requires-Dist: scikit-image==0.22.0; extra == "strict"
+Requires-Dist: mp-pyrho==0.4.4; extra == "strict"
 Provides-Extra: tests
-Requires-Dist: pytest==7.4.2; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0; extra == "tests"
-Requires-Dist: nbmake==1.4.6; extra == "tests"
+Requires-Dist: nbmake==1.5.3; extra == "tests"
 
-pymatgen-analysis-defects
-=========================
+# pymatgen-analysis-defects
 
-|testing| |codecov| |zenodo| |pypi|
+[![testing](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml)
+[![codecov](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects/branch/main/graph/badge.svg?token=FOKXRCZTXZ)](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects)
+[![zenodo](https://zenodo.org/badge/452872799.svg)](https://zenodo.org/badge/latestdoi/452872799)
+[![pypi](https://badge.fury.io/py/pymatgen-analysis-defects.svg)](https://badge.fury.io/py/pymatgen-analysis-defects)
+
+📄 [Full
+Documentation](https://materialsproject.github.io/pymatgen-analysis-defects/)
+[Paper](https://joss.theoj.org/papers/10.21105/joss.05941)
+
+This package is an extension to `pymatgen` for performing defect
+analysis. The package is designed to work with VASP inputs and output
+files and is meant to be used as a namespace package extension to the
+main `pymatgen` library. The new module has been redesigned to work
+closely with `atomate2`.
+
+While the `atomate2` automation framework is not required for this code
+to be useful, users are strongly encouraged to to adopt the `atomate2`
+framework as it contains codified \"best practices\" for running defect
+calculations as well as orchestrating the running of calculations and
+storing the results.
+
+The package serves as an object-oriented interface to defect physics and
+is capable of generating a list of non-equivalent defect objects
+directly from the Materials Project API.
+
+``` python
+from pymatgen.analysis.defects.generators import ChargeInterstitialGenerator, generate_all_native_defects
+from pymatgen.ext.matproj import MPRester
+with MPRester() as mpr:
+chgcar = mpr.get_charge_density_from_material_id("mp-804")
+for defect in generate_all_native_defects(chgcar):
+    print(defect)
+```
 
-📄 `Full Documentation <https://materialsproject.github.io/pymatgen-analysis-defects/>`_
+# Non-exhaustive list of features:
 
-
-This package is an extension to ``pymatgen`` for performing defect analysis.
-The package is designed to work with VASP inputs and output files and is meant
-to be used as a namespace package extension to the main ``pymatgen`` library.
-The new module has been redesigned to work closely with ``atomate2``.
-
-While the ``atomate2`` automation framework is not required for this code to be useful, users are strongly encouraged to
-to adopt the ``atomate2`` framework as it contains codified "best practices" for running defect calculations
-as well as orchestrating the running of calculations and storing the results.
-
-
-Non-exhaustive list of features:
---------------------------------
-
-Reproducible definition of defects
-++++++++++++++++++++++++++++++++++
+## Reproducible definition of defects
 
 Defects are defined based on the physical concept they represent,
-independent of the calculation details such as simulation cell size.
-As an example, a Vacancy defect is defined by the primitive cell of the
+independent of the calculation details such as simulation cell size. As
+an example, a Vacancy defect is defined by the primitive cell of the
 pristine material plus a single site that represents the vacancy site in
 the unit cell.
 
-
-Formation energy calculations
-+++++++++++++++++++++++++++++
+## Formation energy calculations
 
 The formation energy diagram is a powerful tool for understanding the
 thermodynamics of defects. This package provides a simple interface for
 calculating the formation energy diagram from first-principles results.
-This package handles the energy accounting of the chemical species for the chemical
-potential calculations, which determines the y-offset of the formation energy.
-This package also performs finite-size corrections for the formation energy which is required
-when studying charged defects in periodic simulation cells.
-
-Defect Position
-+++++++++++++++
-
-Identification of the defect positions in a simulation cell after atomic relaxation
-is not trivial since the many atoms can collectively shift in response to the creation of
-the defect.
-Yet the exact location of the defect is required for the calculation of finite-size corrections
-as well as other physical properties.
-We devised a method based on calculating a SOAP-based distortion field that can be used to
-identify the defect position in a simulation cell.
-Note, this method only requires the reference pristine supercell and does not need prior knowledge
-of how the defect was created.
-
-Defect Complexes
-++++++++++++++++
-
-Multiple defects can be composed into defect complexes.
-The complex is can be treated as a normal defect object for subsequent analysis.
-
-Defect Interactions
-+++++++++++++++++++
-
-Simulation of defect-photon and defect-phonon interactions under the independent particle approximation.
+This package handles the energy accounting of the chemical species for
+the chemical potential calculations, which determines the y-offset of
+the formation energy. This package also performs finite-size corrections
+for the formation energy which is required when studying charged defects
+in periodic simulation cells.
 
-Previous versions of the defects code
--------------------------------------
+## Defect Position
 
-This package replaces the older ``pymatgen.analysis.defects`` modules.
-The previous module was used by ``pyCDT`` code which will continue to work with version ``2022.7.8`` of ``pymatgen``.
+Identification of the defect positions in a simulation cell after atomic
+relaxation is not trivial since the many atoms can collectively shift in
+response to the creation of the defect. Yet the exact location of the
+defect is required for the calculation of finite-size corrections as
+well as other physical properties. We devised a method based on
+calculating a SOAP-based distortion field that can be used to identify
+the defect position in a simulation cell. Note, this method only
+requires the reference pristine supercell and does not need prior
+knowledge of how the defect was created.
 
-Contributing
-------------
+## Defect Complexes
 
-The source code can be downloaded from the GitHub repository at
+Multiple defects can be composed into defect complexes. The complex is
+can be treated as a normal defect object for subsequent analysis.
 
-.. code-block:: bash
+## Defect Interactions
 
-    $ git clone https://github.com/materialsproject/pymatgen-analysis-defects.git
+Simulation of defect-photon and defect-phonon interactions under the
+independent particle approximation.
 
-All code contributions are welcome. Please submit a pull request on GitHub.
-To make maintenance easier, please use a workflow similar to the automated CI
-`workflow <https://github.com/materialsproject/pymatgen-analysis-defects/blob/main/.github/workflows/testing.yml>`_.
+# Previous versions of the defects code
 
-Specifically, please make sure to run the following commands for linting:
+This package replaces the older `pymatgen.analysis.defects` modules. The
+previous module was used by `pyCDT` code which will continue to work
+with version `2022.7.8` of `pymatgen`.
 
-.. code-block:: bash
+# Contributing
 
-    $ pip install -e .[strict]
-    $ pip install -e .[dev]
-    $ pre-commit install
-    $ pre-commit run --all-files
+The source code can be downloaded from the GitHub repository at
 
-And run these commands for testing:
+``` bash
+$ git clone https://github.com/materialsproject/pymatgen-analysis-defects.git
+```
+
+All code contributions are welcome. Please submit a pull request on
+GitHub. To make maintenance easier, please use a workflow similar to the
+automated CI
+[workflow](https://github.com/materialsproject/pymatgen-analysis-defects/blob/main/.github/workflows/testing.yml).
+
+Specifically, please make sure to run the following commands for
+linting:
+
+``` bash
+$ pip install -e .[strict]
+$ pip install -e .[dev]
+$ pre-commit install
+$ pre-commit run --all-files
+```
 
-.. code-block:: bash
+And run these commands for testing:
 
-    $ pip install -e .[strict]
-    $ pip install -e .[tests]
-    $ pytest --cov=pymatgen
-    $ pytest --nbmake ./docs/source/content
-
-For more details about what is actually installed with each of the ``pip install .[arg]`` commands, please inspect the
-``pyproject.toml`` file.
-
-Contributors
-------------
-
-* Lead developer: Dr. Jimmy-Xuan Shen
-* This code contains contributions from the original defects analysis module of ``pymatgen`` from Dr. Danny Broberg and Dr. Shyam Dwaraknath.
-
-.. |testing| image:: https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml/badge.svg?branch=main
-   :target: https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml
-.. |codecov| image:: https://codecov.io/gh/materialsproject/pymatgen-analysis-defects/branch/main/graph/badge.svg?token=FOKXRCZTXZ
-   :target: https://codecov.io/gh/materialsproject/pymatgen-analysis-defects
-.. |zenodo| image:: https://zenodo.org/badge/452872799.svg
-   :target: https://zenodo.org/badge/latestdoi/452872799
-.. |pypi| image:: https://badge.fury.io/py/pymatgen-analysis-defects.svg
-    :target: https://badge.fury.io/py/pymatgen-analysis-defects
+``` bash
+$ pip install -e .[strict]
+$ pip install -e .[tests]
+$ pytest --cov=pymatgen
+$ pytest --nbmake ./docs/source/content
+```
+
+For more details about what is actually installed with each of the
+`pip install .[arg]` commands, please inspect the `pyproject.toml` file.
+
+# Contributors
+
+-   Lead developer: Dr. Jimmy-Xuan Shen
+-   This code contains contributions from the original defects analysis
+    module of `pymatgen` from Dr. Danny Broberg and Dr. Shyam
+    Dwaraknath.
```

### Comparing `pymatgen-analysis-defects-2024.2.9/pyproject.toml` & `pymatgen_analysis_defects-2024.4.22/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -14,43 +14,44 @@
   "Operating System :: OS Independent",
   "Topic :: Other/Nonlisted Topic",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
   "pymatgen",
   "scikit-image>=0.19.3",
-  "numpy"
+  "numpy",
+  "mp-pyrho>=0.4.4",
 ]
 description = "Pymatgen extension for defects analysis"
 dynamic = ["version"]
 keywords = ["high-throughput", "automated", "dft", "defects"]
 license = { text = "modified BSD" }
 name = "pymatgen-analysis-defects"
-readme = "README.rst"
+readme = "README.md"
 requires-python = '>=3.9'
 
 [project.optional-dependencies]
 finder = ["dscribe>=2.0.0"]
 dev = ["pre-commit>=2.12.1"]
 docs = [
   "jupyter-book>=0.13.1",
 ]
 optional = ["pydefect>=0.6.2", "dscribe>=2.0.0", "numba"]
 
 strict = [
-  "pymatgen==2023.10.11",
+  "pymatgen==2024.3.1",
   "dscribe==2.1.0",
-  "scikit-image==0.21.0",
+  "scikit-image==0.22.0",
+  "mp-pyrho==0.4.4",
 ]
 
-tests = ["pytest==7.4.2", "pytest-cov==4.1.0", "nbmake==1.4.6"]
-
+tests = ["pytest==8.1.1", "pytest-cov==4.1.0", "nbmake==1.5.3"]
 
 [tool.setuptools.dynamic]
-readme = { file = ["README.rst"] }
+readme = { file = ["README.md"] }
 
 [project.urls]
 documentation = "https://materialsproject.github.io/pymatgen-analysis-defects/"
 homepage = "https://materialsproject.github.io/pymatgen-analysis-defects/"
 repository = "https://github.com/materialsproject/pymatgen-analysis-defects"
 
 [tool.setuptools.packages.find]
@@ -98,65 +99,22 @@
 
 [tool.ruff]
 src = ["pymatgen", "tests"]
 
 line-length = 88
 indent-width = 4
 
-
-# By default, ruff only uses all "E" (pycodestyle) and "F" (pyflakes) rules.
-# Here we append to the defaults.
-select = [
-  # (flake8-builtins) detect shadowing of python builtin symbols by variables and arguments.
-  # Attributes are OK (which is why A003) is not included here.
-  "A001",
-  "A002",
-  # (useless expression): Expressions that aren't assigned to anything are typically bugs.
-  "B018",
-  # (pydocstyle) Docstring-related rules. A large subset of these are ignored by the
-  # "convention=google" setting, we set under tool.ruff.pydocstyle.
-  "D",
-  # (pycodestyle) pycodestyle rules
-  "E",
-  # (pyflakes) pyflakes rules
-  "F",
-  # (isort) detect improperly sorted imports
-  "I001",
-  # (pylint) use all pylint rules from categories "Convention", "Error", and "Warning" (ruff
-  # currently implements only a subset of pylint's rules)
-  "PLE",
-  "PLW",
-  # (no commented out code) keep commented out code blocks out of the codebase
-  # "ERA001",
-  # (ruff-specific) Enable all ruff-specific checks (i.e. not ports of
-  # functionality from an existing linter).
-  "RUF",
-  # (private member access) Flag access to `_`-prefixed symbols. By default the various special
-  # methods on `NamedTuple` are ignored (e.g. `_replace`).
-  "SLF001",
-  # (flake8-type-checking) Auto-sort imports into TYPE_CHECKING blocks depending on whether
-  # they are runtime or type-only imports.
-  "TCH",
-  # (banned-api) Flag use of banned APIs. See tool.ruff.flake8-tidy-imports.banned-api for details.
-  "TID251",
-  # (disallow print statements) keep debugging statements out of the codebase
-  "T20",
-  # (f-strings) use f-strings instead of .format()
-  "UP032",
-  # (invalid escape sequence) flag errant backslashes
-  "W605",
-]
-
 [tool.ruff.lint]
-# Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`).
-select = ["E4", "E7", "E9", "F", "D", "I001", "TCH"]
-ignore = ["E203", "E501", "F401"]
+select = ["ALL"]
+ignore = [
+  "E203", "E501", "N", "PLR", "SLF", "ANN101",  "ANN102",
+  "TRY", "COM812", "ISC001", "ERA001", "FBT", "C", "FIX", "TD", "ANN003"]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
-fixable = ["ALL", "TCH"]
+fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.format]
 # Like Black, use double quotes for strings.
```

