# Comparing `tmp/biosppy-2.2.0.tar.gz` & `tmp/biosppy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosppy-2.2.0.tar", last modified: Tue Apr 16 14:31:27 2024, max compression
+gzip compressed data, was "biosppy-2.2.1.tar", last modified: Tue Apr 23 15:26:31 2024, max compression
```

## Comparing `biosppy-2.2.0.tar` & `biosppy-2.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-16 14:31:24.000000 biosppy-2.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 14:31:24.000000 biosppy-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 14:31:24.000000 biosppy-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 14:31:27.672315 biosppy-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-16 14:31:24.000000 biosppy-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.668315 biosppy-2.2.0/biosppy/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/biometrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    28599 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.668315 biosppy-2.2.0/biosppy/features/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/cepstral.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/phase_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/time_freq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.668315 biosppy-2.2.0/biosppy/inter_plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/inter_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/inter_plotting/acc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/inter_plotting/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    72253 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/biosppy/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/abp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/acc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/bvp.py
--rw-r--r--   0 runner    (1001) docker     (127)    65972 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/eda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/eeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    41783 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/emg.py
--rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/hrv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/pcg.py
--rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/ppg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/resp.py
--rw-r--r--   0 runner    (1001) docker     (127)    58646 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/biosppy/synthesizers/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/synthesizers/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)    29270 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/synthesizers/emg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/biosppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 14:31:27.672315 biosppy-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-16 14:31:24.000000 biosppy-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 15:26:27.000000 biosppy-2.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-23 15:26:27.000000 biosppy-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 15:26:27.000000 biosppy-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-23 15:26:31.157666 biosppy-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-23 15:26:27.000000 biosppy-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.153666 biosppy-2.2.1/biosppy/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/biometrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28599 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.153666 biosppy-2.2.1/biosppy/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/cepstral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/phase_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/time_freq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.153666 biosppy-2.2.1/biosppy/inter_plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/inter_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/inter_plotting/acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/inter_plotting/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72253 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/biosppy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/abp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/bvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65972 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/eda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41783 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/emg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/hrv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/pcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/ppg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58646 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/biosppy/synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/synthesizers/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29270 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/synthesizers/emg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/biosppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 15:26:31.157666 biosppy-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-23 15:26:27.000000 biosppy-2.2.1/setup.py
```

### Comparing `biosppy-2.2.0/LICENSE` & `biosppy-2.2.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿Copyright (c) 2015 Instituto de Telecomunicações. See AUTHORS for more details.
+﻿Copyright (c) 2024 Instituto de Telecomunicações. See AUTHORS for more details.
 
 All rights reserved.
 
 Redistribution and use in source and binary forms of the software as well
 as documentation, with or without modification, are permitted provided
 that the following conditions are met:
```

### Comparing `biosppy-2.2.0/PKG-INFO` & `biosppy-2.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosppy
-Version: 2.2.0
+Version: 2.2.1
 Summary: A toolbox for biosignal processing written in Python.
 Home-page: https://github.com/scientisst/BioSPPy
 Author: Instituto de Telecomunicacoes
 Author-email: developer@scientisst.com
 License: BSD 3-clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -34,48 +34,55 @@
 Requires-Dist: opencv-python
 Requires-Dist: pywavelets
 Requires-Dist: mock
 Provides-Extra: eda
 Requires-Dist: cvxopt; extra == "eda"
 
 
+<a href="https://biosppy.readthedocs.org/">
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
+  <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
+  <img alt="Image" title="I know you're listening! - xkcd.com/525">
+</picture>
+</a>
+
+*A toolbox for biosignal processing written in Python.*
+
+[![PyPI version](https://badgen.net/pypi/v/biosppy)](https://pypi.org/project/biosppy/)
+[![PyPI downloads](https://badgen.net/pypi/dm/biosppy/?color=blue)](https://pypi.org/project/biosppy/)
+[![License](https://badgen.net/pypi/license/biosppy?color=grey)](https://github.com/scientisst/BioSPPy/blob/main/LICENSE)
+
+[![GitHub stars](https://badgen.net/github/stars/scientisst/BioSPPy?color=yellow)]()
+[![GitHub issues](https://badgen.net/github/open-issues/scientisst/BioSPPy?color=cyan)](https://github.com/scientisst/BioSPPy/issues)
+
+
 ### 🎙️ Announcements
-#### Latest
 ```
 🌀 New module for signal quality assessment 🌀
 With the biosppy.quality module you can now evaluate the quality of your signals!
 So far, the EDA and ECG quality are available, but more could be added soon. 
 ```
-#### New features
 ```
-🌀 New module for signal quality assessment (biosppy.quality)
 🫀 New module for heart rate variability (biosppy.signals.hrv)
 🎊 New module for feature extraction (biosppy.features)
 ```
 
 
 # BioSPPy - Biosignal Processing in Python
-
-*A toolbox for biosignal processing written in Python.*
-
-<a href="https://biosppy.readthedocs.org/">
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
-  <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
-  <img alt="Image" title="I know you're listening! - xkcd.com/525">
-</picture>
-</a>
-
 The toolbox bundles together various signal processing and pattern recognition
 methods geared towards the analysis of biosignals.
 
 Highlights:
 
-- Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration
+- Support for various biosignals: ECG, EDA, EEG, EMG, PCG, PPG, Respiration, HRV
 - Signal analysis primitives: filtering, frequency analysis
+- Feature extraction: time, frequency, and non-linear domain
+- Signal quality assessment
+- Signal synthesizers
 - Clustering
 - Biometrics
 
 Documentation can be found at: <https://biosppy.readthedocs.org/>
 
 ## Installation
 
@@ -122,30 +129,33 @@
 - shortuuid
 - six
 - joblib
 
 ## Citing
 Please use the following if you need to cite BioSPPy:
 
-- Carreiras C, Alves AP, Lourenço A, Canento F, Silva H, Fred A, *et al.*
-  **BioSPPy - Biosignal Processing in Python**, 2015-,
-  https://github.com/PIA-Group/BioSPPy/ [Online; accessed ```<year>-<month>-<day>```].
+P. Bota, R. Silva, C. Carreiras, A. Fred, and H. P. da Silva, "BioSPPy: A Python toolbox for physiological signal processing," SoftwareX, vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712.
 
 ```latex
-@Misc{,
-  author = {Carlos Carreiras and Ana Priscila Alves and Andr\'{e} Louren\c{c}o and Filipe Canento and Hugo Silva and Ana Fred and others},
-  title = {{BioSPPy}: Biosignal Processing in {Python}},
-  year = {2015--},
-  url = "https://github.com/PIA-Group/BioSPPy/",
-  note = {[Online; accessed <today>]}
+@article{biosppy,
+    title = {BioSPPy: A Python toolbox for physiological signal processing},
+    author = {Patrícia Bota and Rafael Silva and Carlos Carreiras and Ana Fred and Hugo Plácido {da Silva}},
+    journal = {SoftwareX},
+    volume = {26},
+    pages = {101712},
+    year = {2024},
+    issn = {2352-7110},
+    doi = {https://doi.org/10.1016/j.softx.2024.101712},
+    url = {https://www.sciencedirect.com/science/article/pii/S2352711024000839},
 }
 ```
 
-## License
+However, if you want to cite a specific version of BioSPPy, you can use Zenodo's DOI:
 
+## License
 BioSPPy is released under the BSD 3-clause license. See LICENSE for more details.
 
 ## Disclaimer
 
 This program is distributed in the hope it will be useful and provided
 to you "as is", but WITHOUT ANY WARRANTY, without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biosppy Version: 2.2.0 Summary: A toolbox for
+Metadata-Version: 2.1 Name: biosppy Version: 2.2.1 Summary: A toolbox for
 biosignal processing written in Python. Home-page: https://github.com/
 scientisst/BioSPPy Author: Instituto de Telecomunicacoes Author-email:
 developer@scientisst.com License: BSD 3-clause Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -11,46 +11,56 @@
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent Requires-Python: >3.5.2
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.md Requires-Dist: bidict Requires-Dist: h5py Requires-Dist: matplotlib
 Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scipy Requires-
 Dist: shortuuid Requires-Dist: six Requires-Dist: joblib Requires-Dist: opencv-
 python Requires-Dist: pywavelets Requires-Dist: mock Provides-Extra: eda
-Requires-Dist: cvxopt; extra == "eda" ### ðï¸ Announcements #### Latest ```
-ð New module for signal quality assessment ð With the biosppy.quality
-module you can now evaluate the quality of your signals! So far, the EDA and
-ECG quality are available, but more could be added soon. ``` #### New features
-``` ð New module for signal quality assessment (biosppy.quality) ð« New
-module for heart rate variability (biosppy.signals.hrv) ð New module for
-feature extraction (biosppy.features) ``` # BioSPPy - Biosignal Processing in
-Python *A toolbox for biosignal processing written in Python.* _[_I_m_a_g_e_]The
-toolbox bundles together various signal processing and pattern recognition
-methods geared towards the analysis of biosignals. Highlights: - Support for
-various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration - Signal
-analysis primitives: filtering, frequency analysis - Clustering - Biometrics
-Documentation can be found at:
+Requires-Dist: cvxopt; extra == "eda" _[_I_m_a_g_e_]*A toolbox for biosignal
+processing written in Python.* [![PyPI version](https://badgen.net/pypi/v/
+biosppy)](https://pypi.org/project/biosppy/) [![PyPI downloads](https://
+badgen.net/pypi/dm/biosppy/?color=blue)](https://pypi.org/project/biosppy/) [!
+[License](https://badgen.net/pypi/license/biosppy?color=grey)](https://
+github.com/scientisst/BioSPPy/blob/main/LICENSE) [![GitHub stars](https://
+badgen.net/github/stars/scientisst/BioSPPy?color=yellow)]() [![GitHub issues]
+(https://badgen.net/github/open-issues/scientisst/BioSPPy?color=cyan)](https://
+github.com/scientisst/BioSPPy/issues) ### ðï¸ Announcements ``` ð New
+module for signal quality assessment ð With the biosppy.quality module you
+can now evaluate the quality of your signals! So far, the EDA and ECG quality
+are available, but more could be added soon. ``` ``` ð« New module for heart
+rate variability (biosppy.signals.hrv) ð New module for feature extraction
+(biosppy.features) ``` # BioSPPy - Biosignal Processing in Python The toolbox
+bundles together various signal processing and pattern recognition methods
+geared towards the analysis of biosignals. Highlights: - Support for various
+biosignals: ECG, EDA, EEG, EMG, PCG, PPG, Respiration, HRV - Signal analysis
+primitives: filtering, frequency analysis - Feature extraction: time,
+frequency, and non-linear domain - Signal quality assessment - Signal
+synthesizers - Clustering - Biometrics Documentation can be found at:
 biosppy.readthedocs.org/> ## Installation Installation can be easily done with
 `pip`: ```bash $ pip install biosppy ``` Alternatively, you can install the
 latest version from the GitHub repository: ```bash $ pip install git+https://
 github.com/scientisst/BioSPPy.git ``` ## Simple Example The code below loads an
 ECG signal from the `examples` folder, filters it, performs R-peak detection,
 and computes the instantaneous heart rate. ```python from biosppy import
 storage from biosppy.signals import ecg # load raw ECG signal signal, mdata =
 storage.load_txt('./examples/ecg.txt') # process it and plot out = ecg.ecg
 (signal=signal, sampling_rate=1000., show=True) ``` This should produce a plot
 similar to the one below. ![ECG summary example](docs/images/ECG_summary.png)
 ## Dependencies - bidict - h5py - matplotlib - numpy - scikit-learn - scipy -
 shortuuid - six - joblib ## Citing Please use the following if you need to cite
-BioSPPy: - Carreiras C, Alves AP, LourenÃ§o A, Canento F, Silva H, Fred A, *et
-al.* **BioSPPy - Biosignal Processing in Python**, 2015-, https://github.com/
-PIA-Group/BioSPPy/ [Online; accessed ```--```]. ```latex @Misc{, author =
-{Carlos Carreiras and Ana Priscila Alves and Andr\'{e} Louren\c{c}o and Filipe
-Canento and Hugo Silva and Ana Fred and others}, title = {{BioSPPy}: Biosignal
-Processing in {Python}}, year = {2015--}, url = "https://github.com/PIA-Group/
-BioSPPy/", note = {[Online; accessed ]} } ``` ## License BioSPPy is released
+BioSPPy: P. Bota, R. Silva, C. Carreiras, A. Fred, and H. P. da Silva,
+"BioSPPy: A Python toolbox for physiological signal processing," SoftwareX,
+vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712. ```latex @article
+{biosppy, title = {BioSPPy: A Python toolbox for physiological signal
+processing}, author = {PatrÃ­cia Bota and Rafael Silva and Carlos Carreiras and
+Ana Fred and Hugo PlÃ¡cido {da Silva}}, journal = {SoftwareX}, volume = {26},
+pages = {101712}, year = {2024}, issn = {2352-7110}, doi = {https://doi.org/
+10.1016/j.softx.2024.101712}, url = {https://www.sciencedirect.com/science/
+article/pii/S2352711024000839}, } ``` However, if you want to cite a specific
+version of BioSPPy, you can use Zenodo's DOI: ## License BioSPPy is released
 under the BSD 3-clause license. See LICENSE for more details. ## Disclaimer
 This program is distributed in the hope it will be useful and provided to you
 "as is", but WITHOUT ANY WARRANTY, without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is NOT
 intended for medical diagnosis. We expressly disclaim any liability whatsoever
 for any direct, indirect, consequential, incidental or special damages,
 including, without limitation, lost revenues, lost profits, losses resulting
```

### Comparing `biosppy-2.2.0/README.md` & `biosppy-2.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,48 @@
+<a href="https://biosppy.readthedocs.org/">
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
+  <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
+  <img alt="Image" title="I know you're listening! - xkcd.com/525">
+</picture>
+</a>
+
+*A toolbox for biosignal processing written in Python.*
+
+[![PyPI version](https://badgen.net/pypi/v/biosppy)](https://pypi.org/project/biosppy/)
+[![PyPI downloads](https://badgen.net/pypi/dm/biosppy/?color=blue)](https://pypi.org/project/biosppy/)
+[![License](https://badgen.net/pypi/license/biosppy?color=grey)](https://github.com/scientisst/BioSPPy/blob/main/LICENSE)
+
+[![GitHub stars](https://badgen.net/github/stars/scientisst/BioSPPy?color=yellow)]()
+[![GitHub issues](https://badgen.net/github/open-issues/scientisst/BioSPPy?color=cyan)](https://github.com/scientisst/BioSPPy/issues)
+
+
 ### 🎙️ Announcements
-#### Latest
 ```
 🌀 New module for signal quality assessment 🌀
 With the biosppy.quality module you can now evaluate the quality of your signals!
 So far, the EDA and ECG quality are available, but more could be added soon. 
 ```
-#### New features
 ```
-🌀 New module for signal quality assessment (biosppy.quality)
 🫀 New module for heart rate variability (biosppy.signals.hrv)
 🎊 New module for feature extraction (biosppy.features)
 ```
 
 
 # BioSPPy - Biosignal Processing in Python
-
-*A toolbox for biosignal processing written in Python.*
-
-<a href="https://biosppy.readthedocs.org/">
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
-  <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
-  <img alt="Image" title="I know you're listening! - xkcd.com/525">
-</picture>
-</a>
-
 The toolbox bundles together various signal processing and pattern recognition
 methods geared towards the analysis of biosignals.
 
 Highlights:
 
-- Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration
+- Support for various biosignals: ECG, EDA, EEG, EMG, PCG, PPG, Respiration, HRV
 - Signal analysis primitives: filtering, frequency analysis
+- Feature extraction: time, frequency, and non-linear domain
+- Signal quality assessment
+- Signal synthesizers
 - Clustering
 - Biometrics
 
 Documentation can be found at: <https://biosppy.readthedocs.org/>
 
 ## Installation
 
@@ -82,30 +89,33 @@
 - shortuuid
 - six
 - joblib
 
 ## Citing
 Please use the following if you need to cite BioSPPy:
 
-- Carreiras C, Alves AP, Lourenço A, Canento F, Silva H, Fred A, *et al.*
-  **BioSPPy - Biosignal Processing in Python**, 2015-,
-  https://github.com/PIA-Group/BioSPPy/ [Online; accessed ```<year>-<month>-<day>```].
+P. Bota, R. Silva, C. Carreiras, A. Fred, and H. P. da Silva, "BioSPPy: A Python toolbox for physiological signal processing," SoftwareX, vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712.
 
 ```latex
-@Misc{,
-  author = {Carlos Carreiras and Ana Priscila Alves and Andr\'{e} Louren\c{c}o and Filipe Canento and Hugo Silva and Ana Fred and others},
-  title = {{BioSPPy}: Biosignal Processing in {Python}},
-  year = {2015--},
-  url = "https://github.com/PIA-Group/BioSPPy/",
-  note = {[Online; accessed <today>]}
+@article{biosppy,
+    title = {BioSPPy: A Python toolbox for physiological signal processing},
+    author = {Patrícia Bota and Rafael Silva and Carlos Carreiras and Ana Fred and Hugo Plácido {da Silva}},
+    journal = {SoftwareX},
+    volume = {26},
+    pages = {101712},
+    year = {2024},
+    issn = {2352-7110},
+    doi = {https://doi.org/10.1016/j.softx.2024.101712},
+    url = {https://www.sciencedirect.com/science/article/pii/S2352711024000839},
 }
 ```
 
-## License
+However, if you want to cite a specific version of BioSPPy, you can use Zenodo's DOI:
 
+## License
 BioSPPy is released under the BSD 3-clause license. See LICENSE for more details.
 
 ## Disclaimer
 
 This program is distributed in the hope it will be useful and provided
 to you "as is", but WITHOUT ANY WARRANTY, without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This
```

#### html2text {}

```diff
@@ -1,38 +1,49 @@
-### ðï¸ Announcements #### Latest ``` ð New module for signal quality
+_[_I_m_a_g_e_]*A toolbox for biosignal processing written in Python.* [![PyPI version]
+(https://badgen.net/pypi/v/biosppy)](https://pypi.org/project/biosppy/) [![PyPI
+downloads](https://badgen.net/pypi/dm/biosppy/?color=blue)](https://pypi.org/
+project/biosppy/) [![License](https://badgen.net/pypi/license/
+biosppy?color=grey)](https://github.com/scientisst/BioSPPy/blob/main/LICENSE)
+[![GitHub stars](https://badgen.net/github/stars/scientisst/
+BioSPPy?color=yellow)]() [![GitHub issues](https://badgen.net/github/open-
+issues/scientisst/BioSPPy?color=cyan)](https://github.com/scientisst/BioSPPy/
+issues) ### ðï¸ Announcements ``` ð New module for signal quality
 assessment ð With the biosppy.quality module you can now evaluate the
 quality of your signals! So far, the EDA and ECG quality are available, but
-more could be added soon. ``` #### New features ``` ð New module for signal
-quality assessment (biosppy.quality) ð« New module for heart rate variability
+more could be added soon. ``` ``` ð« New module for heart rate variability
 (biosppy.signals.hrv) ð New module for feature extraction (biosppy.features)
-``` # BioSPPy - Biosignal Processing in Python *A toolbox for biosignal
-processing written in Python.* _[_I_m_a_g_e_]The toolbox bundles together various
-signal processing and pattern recognition methods geared towards the analysis
-of biosignals. Highlights: - Support for various biosignals: BVP, ECG, EDA,
-EEG, EMG, PCG, PPG, Respiration - Signal analysis primitives: filtering,
-frequency analysis - Clustering - Biometrics Documentation can be found at:
+``` # BioSPPy - Biosignal Processing in Python The toolbox bundles together
+various signal processing and pattern recognition methods geared towards the
+analysis of biosignals. Highlights: - Support for various biosignals: ECG, EDA,
+EEG, EMG, PCG, PPG, Respiration, HRV - Signal analysis primitives: filtering,
+frequency analysis - Feature extraction: time, frequency, and non-linear domain
+- Signal quality assessment - Signal synthesizers - Clustering - Biometrics
+Documentation can be found at:
 biosppy.readthedocs.org/> ## Installation Installation can be easily done with
 `pip`: ```bash $ pip install biosppy ``` Alternatively, you can install the
 latest version from the GitHub repository: ```bash $ pip install git+https://
 github.com/scientisst/BioSPPy.git ``` ## Simple Example The code below loads an
 ECG signal from the `examples` folder, filters it, performs R-peak detection,
 and computes the instantaneous heart rate. ```python from biosppy import
 storage from biosppy.signals import ecg # load raw ECG signal signal, mdata =
 storage.load_txt('./examples/ecg.txt') # process it and plot out = ecg.ecg
 (signal=signal, sampling_rate=1000., show=True) ``` This should produce a plot
 similar to the one below. ![ECG summary example](docs/images/ECG_summary.png)
 ## Dependencies - bidict - h5py - matplotlib - numpy - scikit-learn - scipy -
 shortuuid - six - joblib ## Citing Please use the following if you need to cite
-BioSPPy: - Carreiras C, Alves AP, LourenÃ§o A, Canento F, Silva H, Fred A, *et
-al.* **BioSPPy - Biosignal Processing in Python**, 2015-, https://github.com/
-PIA-Group/BioSPPy/ [Online; accessed ```--```]. ```latex @Misc{, author =
-{Carlos Carreiras and Ana Priscila Alves and Andr\'{e} Louren\c{c}o and Filipe
-Canento and Hugo Silva and Ana Fred and others}, title = {{BioSPPy}: Biosignal
-Processing in {Python}}, year = {2015--}, url = "https://github.com/PIA-Group/
-BioSPPy/", note = {[Online; accessed ]} } ``` ## License BioSPPy is released
+BioSPPy: P. Bota, R. Silva, C. Carreiras, A. Fred, and H. P. da Silva,
+"BioSPPy: A Python toolbox for physiological signal processing," SoftwareX,
+vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712. ```latex @article
+{biosppy, title = {BioSPPy: A Python toolbox for physiological signal
+processing}, author = {PatrÃ­cia Bota and Rafael Silva and Carlos Carreiras and
+Ana Fred and Hugo PlÃ¡cido {da Silva}}, journal = {SoftwareX}, volume = {26},
+pages = {101712}, year = {2024}, issn = {2352-7110}, doi = {https://doi.org/
+10.1016/j.softx.2024.101712}, url = {https://www.sciencedirect.com/science/
+article/pii/S2352711024000839}, } ``` However, if you want to cite a specific
+version of BioSPPy, you can use Zenodo's DOI: ## License BioSPPy is released
 under the BSD 3-clause license. See LICENSE for more details. ## Disclaimer
 This program is distributed in the hope it will be useful and provided to you
 "as is", but WITHOUT ANY WARRANTY, without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is NOT
 intended for medical diagnosis. We expressly disclaim any liability whatsoever
 for any direct, indirect, consequential, incidental or special damages,
 including, without limitation, lost revenues, lost profits, losses resulting
```

### Comparing `biosppy-2.2.0/biosppy/__init__.py` & `biosppy-2.2.1/biosppy/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/biometrics.py` & `biosppy-2.2.1/biosppy/biometrics.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/clustering.py` & `biosppy-2.2.1/biosppy/clustering.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/features/__init__.py` & `biosppy-2.2.1/biosppy/features/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/features/cepstral.py` & `biosppy-2.2.1/biosppy/features/cepstral.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/features/frequency.py` & `biosppy-2.2.1/biosppy/features/frequency.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/features/phase_space.py` & `biosppy-2.2.1/biosppy/features/phase_space.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/features/time.py` & `biosppy-2.2.1/biosppy/features/time.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/features/time_freq.py` & `biosppy-2.2.1/biosppy/features/time_freq.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/inter_plotting/acc.py` & `biosppy-2.2.1/biosppy/inter_plotting/acc.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/inter_plotting/ecg.py` & `biosppy-2.2.1/biosppy/inter_plotting/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/metrics.py` & `biosppy-2.2.1/biosppy/metrics.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/plotting.py` & `biosppy-2.2.1/biosppy/plotting.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/quality.py` & `biosppy-2.2.1/biosppy/quality.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/__init__.py` & `biosppy-2.2.1/biosppy/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/abp.py` & `biosppy-2.2.1/biosppy/signals/abp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/acc.py` & `biosppy-2.2.1/biosppy/signals/acc.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/bvp.py` & `biosppy-2.2.1/biosppy/signals/bvp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/ecg.py` & `biosppy-2.2.1/biosppy/signals/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/eda.py` & `biosppy-2.2.1/biosppy/signals/eda.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/eeg.py` & `biosppy-2.2.1/biosppy/signals/eeg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/emg.py` & `biosppy-2.2.1/biosppy/signals/emg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/hrv.py` & `biosppy-2.2.1/biosppy/signals/hrv.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/pcg.py` & `biosppy-2.2.1/biosppy/signals/pcg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/ppg.py` & `biosppy-2.2.1/biosppy/signals/ppg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/resp.py` & `biosppy-2.2.1/biosppy/signals/resp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/signals/tools.py` & `biosppy-2.2.1/biosppy/signals/tools.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/stats.py` & `biosppy-2.2.1/biosppy/stats.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/storage.py` & `biosppy-2.2.1/biosppy/storage.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/synthesizers/ecg.py` & `biosppy-2.2.1/biosppy/synthesizers/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/synthesizers/emg.py` & `biosppy-2.2.1/biosppy/synthesizers/emg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/timing.py` & `biosppy-2.2.1/biosppy/timing.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy/utils.py` & `biosppy-2.2.1/biosppy/utils.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/biosppy.egg-info/PKG-INFO` & `biosppy-2.2.1/biosppy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosppy
-Version: 2.2.0
+Version: 2.2.1
 Summary: A toolbox for biosignal processing written in Python.
 Home-page: https://github.com/scientisst/BioSPPy
 Author: Instituto de Telecomunicacoes
 Author-email: developer@scientisst.com
 License: BSD 3-clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -34,48 +34,55 @@
 Requires-Dist: opencv-python
 Requires-Dist: pywavelets
 Requires-Dist: mock
 Provides-Extra: eda
 Requires-Dist: cvxopt; extra == "eda"
 
 
+<a href="https://biosppy.readthedocs.org/">
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
+  <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
+  <img alt="Image" title="I know you're listening! - xkcd.com/525">
+</picture>
+</a>
+
+*A toolbox for biosignal processing written in Python.*
+
+[![PyPI version](https://badgen.net/pypi/v/biosppy)](https://pypi.org/project/biosppy/)
+[![PyPI downloads](https://badgen.net/pypi/dm/biosppy/?color=blue)](https://pypi.org/project/biosppy/)
+[![License](https://badgen.net/pypi/license/biosppy?color=grey)](https://github.com/scientisst/BioSPPy/blob/main/LICENSE)
+
+[![GitHub stars](https://badgen.net/github/stars/scientisst/BioSPPy?color=yellow)]()
+[![GitHub issues](https://badgen.net/github/open-issues/scientisst/BioSPPy?color=cyan)](https://github.com/scientisst/BioSPPy/issues)
+
+
 ### 🎙️ Announcements
-#### Latest
 ```
 🌀 New module for signal quality assessment 🌀
 With the biosppy.quality module you can now evaluate the quality of your signals!
 So far, the EDA and ECG quality are available, but more could be added soon. 
 ```
-#### New features
 ```
-🌀 New module for signal quality assessment (biosppy.quality)
 🫀 New module for heart rate variability (biosppy.signals.hrv)
 🎊 New module for feature extraction (biosppy.features)
 ```
 
 
 # BioSPPy - Biosignal Processing in Python
-
-*A toolbox for biosignal processing written in Python.*
-
-<a href="https://biosppy.readthedocs.org/">
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
-  <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
-  <img alt="Image" title="I know you're listening! - xkcd.com/525">
-</picture>
-</a>
-
 The toolbox bundles together various signal processing and pattern recognition
 methods geared towards the analysis of biosignals.
 
 Highlights:
 
-- Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration
+- Support for various biosignals: ECG, EDA, EEG, EMG, PCG, PPG, Respiration, HRV
 - Signal analysis primitives: filtering, frequency analysis
+- Feature extraction: time, frequency, and non-linear domain
+- Signal quality assessment
+- Signal synthesizers
 - Clustering
 - Biometrics
 
 Documentation can be found at: <https://biosppy.readthedocs.org/>
 
 ## Installation
 
@@ -122,30 +129,33 @@
 - shortuuid
 - six
 - joblib
 
 ## Citing
 Please use the following if you need to cite BioSPPy:
 
-- Carreiras C, Alves AP, Lourenço A, Canento F, Silva H, Fred A, *et al.*
-  **BioSPPy - Biosignal Processing in Python**, 2015-,
-  https://github.com/PIA-Group/BioSPPy/ [Online; accessed ```<year>-<month>-<day>```].
+P. Bota, R. Silva, C. Carreiras, A. Fred, and H. P. da Silva, "BioSPPy: A Python toolbox for physiological signal processing," SoftwareX, vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712.
 
 ```latex
-@Misc{,
-  author = {Carlos Carreiras and Ana Priscila Alves and Andr\'{e} Louren\c{c}o and Filipe Canento and Hugo Silva and Ana Fred and others},
-  title = {{BioSPPy}: Biosignal Processing in {Python}},
-  year = {2015--},
-  url = "https://github.com/PIA-Group/BioSPPy/",
-  note = {[Online; accessed <today>]}
+@article{biosppy,
+    title = {BioSPPy: A Python toolbox for physiological signal processing},
+    author = {Patrícia Bota and Rafael Silva and Carlos Carreiras and Ana Fred and Hugo Plácido {da Silva}},
+    journal = {SoftwareX},
+    volume = {26},
+    pages = {101712},
+    year = {2024},
+    issn = {2352-7110},
+    doi = {https://doi.org/10.1016/j.softx.2024.101712},
+    url = {https://www.sciencedirect.com/science/article/pii/S2352711024000839},
 }
 ```
 
-## License
+However, if you want to cite a specific version of BioSPPy, you can use Zenodo's DOI:
 
+## License
 BioSPPy is released under the BSD 3-clause license. See LICENSE for more details.
 
 ## Disclaimer
 
 This program is distributed in the hope it will be useful and provided
 to you "as is", but WITHOUT ANY WARRANTY, without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biosppy Version: 2.2.0 Summary: A toolbox for
+Metadata-Version: 2.1 Name: biosppy Version: 2.2.1 Summary: A toolbox for
 biosignal processing written in Python. Home-page: https://github.com/
 scientisst/BioSPPy Author: Instituto de Telecomunicacoes Author-email:
 developer@scientisst.com License: BSD 3-clause Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -11,46 +11,56 @@
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent Requires-Python: >3.5.2
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.md Requires-Dist: bidict Requires-Dist: h5py Requires-Dist: matplotlib
 Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scipy Requires-
 Dist: shortuuid Requires-Dist: six Requires-Dist: joblib Requires-Dist: opencv-
 python Requires-Dist: pywavelets Requires-Dist: mock Provides-Extra: eda
-Requires-Dist: cvxopt; extra == "eda" ### ðï¸ Announcements #### Latest ```
-ð New module for signal quality assessment ð With the biosppy.quality
-module you can now evaluate the quality of your signals! So far, the EDA and
-ECG quality are available, but more could be added soon. ``` #### New features
-``` ð New module for signal quality assessment (biosppy.quality) ð« New
-module for heart rate variability (biosppy.signals.hrv) ð New module for
-feature extraction (biosppy.features) ``` # BioSPPy - Biosignal Processing in
-Python *A toolbox for biosignal processing written in Python.* _[_I_m_a_g_e_]The
-toolbox bundles together various signal processing and pattern recognition
-methods geared towards the analysis of biosignals. Highlights: - Support for
-various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration - Signal
-analysis primitives: filtering, frequency analysis - Clustering - Biometrics
-Documentation can be found at:
+Requires-Dist: cvxopt; extra == "eda" _[_I_m_a_g_e_]*A toolbox for biosignal
+processing written in Python.* [![PyPI version](https://badgen.net/pypi/v/
+biosppy)](https://pypi.org/project/biosppy/) [![PyPI downloads](https://
+badgen.net/pypi/dm/biosppy/?color=blue)](https://pypi.org/project/biosppy/) [!
+[License](https://badgen.net/pypi/license/biosppy?color=grey)](https://
+github.com/scientisst/BioSPPy/blob/main/LICENSE) [![GitHub stars](https://
+badgen.net/github/stars/scientisst/BioSPPy?color=yellow)]() [![GitHub issues]
+(https://badgen.net/github/open-issues/scientisst/BioSPPy?color=cyan)](https://
+github.com/scientisst/BioSPPy/issues) ### ðï¸ Announcements ``` ð New
+module for signal quality assessment ð With the biosppy.quality module you
+can now evaluate the quality of your signals! So far, the EDA and ECG quality
+are available, but more could be added soon. ``` ``` ð« New module for heart
+rate variability (biosppy.signals.hrv) ð New module for feature extraction
+(biosppy.features) ``` # BioSPPy - Biosignal Processing in Python The toolbox
+bundles together various signal processing and pattern recognition methods
+geared towards the analysis of biosignals. Highlights: - Support for various
+biosignals: ECG, EDA, EEG, EMG, PCG, PPG, Respiration, HRV - Signal analysis
+primitives: filtering, frequency analysis - Feature extraction: time,
+frequency, and non-linear domain - Signal quality assessment - Signal
+synthesizers - Clustering - Biometrics Documentation can be found at:
 biosppy.readthedocs.org/> ## Installation Installation can be easily done with
 `pip`: ```bash $ pip install biosppy ``` Alternatively, you can install the
 latest version from the GitHub repository: ```bash $ pip install git+https://
 github.com/scientisst/BioSPPy.git ``` ## Simple Example The code below loads an
 ECG signal from the `examples` folder, filters it, performs R-peak detection,
 and computes the instantaneous heart rate. ```python from biosppy import
 storage from biosppy.signals import ecg # load raw ECG signal signal, mdata =
 storage.load_txt('./examples/ecg.txt') # process it and plot out = ecg.ecg
 (signal=signal, sampling_rate=1000., show=True) ``` This should produce a plot
 similar to the one below. ![ECG summary example](docs/images/ECG_summary.png)
 ## Dependencies - bidict - h5py - matplotlib - numpy - scikit-learn - scipy -
 shortuuid - six - joblib ## Citing Please use the following if you need to cite
-BioSPPy: - Carreiras C, Alves AP, LourenÃ§o A, Canento F, Silva H, Fred A, *et
-al.* **BioSPPy - Biosignal Processing in Python**, 2015-, https://github.com/
-PIA-Group/BioSPPy/ [Online; accessed ```--```]. ```latex @Misc{, author =
-{Carlos Carreiras and Ana Priscila Alves and Andr\'{e} Louren\c{c}o and Filipe
-Canento and Hugo Silva and Ana Fred and others}, title = {{BioSPPy}: Biosignal
-Processing in {Python}}, year = {2015--}, url = "https://github.com/PIA-Group/
-BioSPPy/", note = {[Online; accessed ]} } ``` ## License BioSPPy is released
+BioSPPy: P. Bota, R. Silva, C. Carreiras, A. Fred, and H. P. da Silva,
+"BioSPPy: A Python toolbox for physiological signal processing," SoftwareX,
+vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712. ```latex @article
+{biosppy, title = {BioSPPy: A Python toolbox for physiological signal
+processing}, author = {PatrÃ­cia Bota and Rafael Silva and Carlos Carreiras and
+Ana Fred and Hugo PlÃ¡cido {da Silva}}, journal = {SoftwareX}, volume = {26},
+pages = {101712}, year = {2024}, issn = {2352-7110}, doi = {https://doi.org/
+10.1016/j.softx.2024.101712}, url = {https://www.sciencedirect.com/science/
+article/pii/S2352711024000839}, } ``` However, if you want to cite a specific
+version of BioSPPy, you can use Zenodo's DOI: ## License BioSPPy is released
 under the BSD 3-clause license. See LICENSE for more details. ## Disclaimer
 This program is distributed in the hope it will be useful and provided to you
 "as is", but WITHOUT ANY WARRANTY, without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is NOT
 intended for medical diagnosis. We expressly disclaim any liability whatsoever
 for any direct, indirect, consequential, incidental or special damages,
 including, without limitation, lost revenues, lost profits, losses resulting
```

### Comparing `biosppy-2.2.0/biosppy.egg-info/SOURCES.txt` & `biosppy-2.2.1/biosppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.0/setup.py` & `biosppy-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 BioSPPy
 -------
 
 A toolbox for biosignal processing written in Python.
 
-:copyright: (c) 2015-2018 by Instituto de Telecomunicacoes
+:copyright: (c) 2015-2024 by Instituto de Telecomunicacoes
 :license: BSD 3-clause, see LICENSE for more details.
 """
 
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pip install twine
 
 import io
@@ -23,15 +23,15 @@
 # Package meta-data.
 NAME = 'biosppy'
 DESCRIPTION = 'A toolbox for biosignal processing written in Python.'
 URL = 'https://github.com/scientisst/BioSPPy'
 EMAIL = 'developer@scientisst.com'
 AUTHOR = 'Instituto de Telecomunicacoes'
 REQUIRES_PYTHON = '>3.5.2'
-VERSION = '2.2.0'
+VERSION = '2.2.1'
 LICENSE = 'BSD 3-clause'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'bidict',
     'h5py',
     'matplotlib',
```

