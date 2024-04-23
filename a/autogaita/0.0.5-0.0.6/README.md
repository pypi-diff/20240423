# Comparing `tmp/autogaita-0.0.5.tar.gz` & `tmp/autogaita-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogaita-0.0.5.tar", last modified: Tue Apr 16 13:07:14 2024, max compression
+gzip compressed data, was "autogaita-0.0.6.tar", last modified: Tue Apr 23 13:01:56 2024, max compression
```

## Comparing `autogaita-0.0.5.tar` & `autogaita-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-16 13:07:14.995471 autogaita-0.0.5/
--rw-r--r--   0 mahan      (501) staff       (20)    35129 2023-12-11 14:01:05.000000 autogaita-0.0.5/LICENSE
--rw-r--r--   0 mahan      (501) staff       (20)      212 2024-04-16 13:07:14.995348 autogaita-0.0.5/PKG-INFO
--rw-r--r--   0 mahan      (501) staff       (20)     4825 2024-04-16 12:51:52.000000 autogaita-0.0.5/README.md
-drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-16 13:07:14.992706 autogaita-0.0.5/autogaita/
--rw-r--r--   0 mahan      (501) staff       (20)      973 2024-03-28 08:56:08.000000 autogaita-0.0.5/autogaita/__init__.py
--rw-r--r--   0 mahan      (501) staff       (20)      147 2023-12-05 12:00:15.000000 autogaita-0.0.5/autogaita/__main__.py
--rw-r--r--   0 mahan      (501) staff       (20)     5643 2024-03-28 08:51:54.000000 autogaita-0.0.5/autogaita/autogaita.py
--rw-r--r--   0 mahan      (501) staff       (20)    78399 2024-04-16 12:02:36.000000 autogaita-0.0.5/autogaita/autogaita_dlc.py
--rw-r--r--   0 mahan      (501) staff       (20)    51250 2024-04-03 13:40:51.000000 autogaita-0.0.5/autogaita/autogaita_dlc_gui.py
--rw-r--r--   0 mahan      (501) staff       (20)    99483 2024-04-15 12:31:54.000000 autogaita-0.0.5/autogaita/autogaita_group.py
--rw-r--r--   0 mahan      (501) staff       (20)    38497 2024-03-28 08:51:38.000000 autogaita-0.0.5/autogaita/autogaita_group_gui.py
--rw-r--r--   0 mahan      (501) staff       (20)   101705 2023-12-04 13:54:23.000000 autogaita-0.0.5/autogaita/autogaita_icon.icns
--rw-r--r--   0 mahan      (501) staff       (20)     4286 2023-12-04 13:54:35.000000 autogaita-0.0.5/autogaita/autogaita_icon.ico
--rw-r--r--   0 mahan      (501) staff       (20)   585823 2023-11-02 13:05:18.000000 autogaita-0.0.5/autogaita/autogaita_logo.png
--rw-r--r--   0 mahan      (501) staff       (20)    89994 2024-04-16 11:56:16.000000 autogaita-0.0.5/autogaita/autogaita_simi.py
--rw-r--r--   0 mahan      (501) staff       (20)    34310 2024-03-28 08:51:46.000000 autogaita-0.0.5/autogaita/autogaita_simi_gui.py
--rw-r--r--   0 mahan      (501) staff       (20)     3092 2024-03-28 08:51:12.000000 autogaita-0.0.5/autogaita/autogaita_utils.py
-drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-16 13:07:14.995074 autogaita-0.0.5/autogaita/batchrun_scripts/
--rw-r--r--   0 mahan      (501) staff       (20)        0 2024-03-28 08:46:31.000000 autogaita-0.0.5/autogaita/batchrun_scripts/__init__.py
--rw-r--r--   0 mahan      (501) staff       (20)     6247 2024-04-16 08:43:44.000000 autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_dlc_multirun.py
--rw-r--r--   0 mahan      (501) staff       (20)     3900 2024-04-16 08:42:57.000000 autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_dlc_singlerun.py
--rw-r--r--   0 mahan      (501) staff       (20)     1281 2024-04-15 12:30:24.000000 autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_group_dlcrun.py
--rw-r--r--   0 mahan      (501) staff       (20)     1866 2024-03-28 09:09:25.000000 autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_group_simirun.py
--rw-r--r--   0 mahan      (501) staff       (20)     3482 2023-12-05 11:55:00.000000 autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_simi_multirun.py
--rw-r--r--   0 mahan      (501) staff       (20)     2282 2023-12-05 11:54:55.000000 autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_simi_singlerun.py
-drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-16 13:07:14.993445 autogaita-0.0.5/autogaita.egg-info/
--rw-r--r--   0 mahan      (501) staff       (20)      212 2024-04-16 13:07:14.000000 autogaita-0.0.5/autogaita.egg-info/PKG-INFO
--rw-r--r--   0 mahan      (501) staff       (20)      916 2024-04-16 13:07:14.000000 autogaita-0.0.5/autogaita.egg-info/SOURCES.txt
--rw-r--r--   0 mahan      (501) staff       (20)        1 2024-04-16 13:07:14.000000 autogaita-0.0.5/autogaita.egg-info/dependency_links.txt
--rw-r--r--   0 mahan      (501) staff       (20)      176 2024-04-16 13:07:14.000000 autogaita-0.0.5/autogaita.egg-info/requires.txt
--rw-r--r--   0 mahan      (501) staff       (20)       10 2024-04-16 13:07:14.000000 autogaita-0.0.5/autogaita.egg-info/top_level.txt
--rw-r--r--   0 mahan      (501) staff       (20)       38 2024-04-16 13:07:14.995507 autogaita-0.0.5/setup.cfg
--rw-r--r--   0 mahan      (501) staff       (20)      896 2024-04-16 13:06:40.000000 autogaita-0.0.5/setup.py
+drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-23 13:01:56.754200 autogaita-0.0.6/
+-rw-r--r--   0 mahan      (501) staff       (20)    35129 2023-12-11 14:01:05.000000 autogaita-0.0.6/LICENSE
+-rw-r--r--   0 mahan      (501) staff       (20)      256 2024-04-23 13:01:56.754027 autogaita-0.0.6/PKG-INFO
+-rw-r--r--   0 mahan      (501) staff       (20)     5666 2024-04-22 11:54:35.000000 autogaita-0.0.6/README.md
+drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-23 13:01:56.751127 autogaita-0.0.6/autogaita/
+-rw-r--r--   0 mahan      (501) staff       (20)      994 2024-04-19 09:02:31.000000 autogaita-0.0.6/autogaita/__init__.py
+-rw-r--r--   0 mahan      (501) staff       (20)      147 2024-04-19 08:50:15.000000 autogaita-0.0.6/autogaita/__main__.py
+-rw-r--r--   0 mahan      (501) staff       (20)     5643 2024-04-19 08:50:41.000000 autogaita-0.0.6/autogaita/autogaita.py
+-rw-r--r--   0 mahan      (501) staff       (20)    82027 2024-04-23 12:19:12.000000 autogaita-0.0.6/autogaita/autogaita_dlc.py
+-rw-r--r--   0 mahan      (501) staff       (20)    54962 2024-04-23 12:21:06.000000 autogaita-0.0.6/autogaita/autogaita_dlc_gui.py
+-rw-r--r--   0 mahan      (501) staff       (20)    99967 2024-04-19 09:08:26.000000 autogaita-0.0.6/autogaita/autogaita_group.py
+-rw-r--r--   0 mahan      (501) staff       (20)    38774 2024-04-19 09:06:44.000000 autogaita-0.0.6/autogaita/autogaita_group_gui.py
+-rw-r--r--   0 mahan      (501) staff       (20)   101705 2023-12-04 13:54:23.000000 autogaita-0.0.6/autogaita/autogaita_icon.icns
+-rw-r--r--   0 mahan      (501) staff       (20)     4286 2023-12-04 13:54:35.000000 autogaita-0.0.6/autogaita/autogaita_icon.ico
+-rw-r--r--   0 mahan      (501) staff       (20)   585823 2023-11-02 13:05:18.000000 autogaita-0.0.6/autogaita/autogaita_logo.png
+-rw-r--r--   0 mahan      (501) staff       (20)    90907 2024-04-19 15:37:27.000000 autogaita-0.0.6/autogaita/autogaita_simi.py
+-rw-r--r--   0 mahan      (501) staff       (20)    34287 2024-04-19 08:50:35.000000 autogaita-0.0.6/autogaita/autogaita_simi_gui.py
+-rw-r--r--   0 mahan      (501) staff       (20)     3077 2024-04-23 11:10:28.000000 autogaita-0.0.6/autogaita/autogaita_utils.py
+drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-23 13:01:56.753718 autogaita-0.0.6/autogaita/batchrun_scripts/
+-rw-r--r--   0 mahan      (501) staff       (20)        0 2024-03-28 08:46:31.000000 autogaita-0.0.6/autogaita/batchrun_scripts/__init__.py
+-rw-r--r--   0 mahan      (501) staff       (20)     6354 2024-04-23 12:22:24.000000 autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_dlc_multirun.py
+-rw-r--r--   0 mahan      (501) staff       (20)     4063 2024-04-19 15:38:37.000000 autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_dlc_singlerun.py
+-rw-r--r--   0 mahan      (501) staff       (20)     1287 2024-04-19 09:02:48.000000 autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_group_dlcrun.py
+-rw-r--r--   0 mahan      (501) staff       (20)     1873 2024-04-19 09:02:52.000000 autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_group_simirun.py
+-rw-r--r--   0 mahan      (501) staff       (20)     3391 2024-04-23 08:35:01.000000 autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_simi_multirun.py
+-rw-r--r--   0 mahan      (501) staff       (20)     2270 2024-04-19 09:07:57.000000 autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_simi_singlerun.py
+drwxr-xr-x   0 mahan      (501) staff       (20)        0 2024-04-23 13:01:56.751951 autogaita-0.0.6/autogaita.egg-info/
+-rw-r--r--   0 mahan      (501) staff       (20)      256 2024-04-23 13:01:56.000000 autogaita-0.0.6/autogaita.egg-info/PKG-INFO
+-rw-r--r--   0 mahan      (501) staff       (20)      916 2024-04-23 13:01:56.000000 autogaita-0.0.6/autogaita.egg-info/SOURCES.txt
+-rw-r--r--   0 mahan      (501) staff       (20)        1 2024-04-23 13:01:56.000000 autogaita-0.0.6/autogaita.egg-info/dependency_links.txt
+-rw-r--r--   0 mahan      (501) staff       (20)      170 2024-04-23 13:01:56.000000 autogaita-0.0.6/autogaita.egg-info/requires.txt
+-rw-r--r--   0 mahan      (501) staff       (20)       10 2024-04-23 13:01:56.000000 autogaita-0.0.6/autogaita.egg-info/top_level.txt
+-rw-r--r--   0 mahan      (501) staff       (20)       38 2024-04-23 13:01:56.754257 autogaita-0.0.6/setup.cfg
+-rw-r--r--   0 mahan      (501) staff       (20)     1005 2024-04-23 13:01:37.000000 autogaita-0.0.6/setup.py
```

### Comparing `autogaita-0.0.5/LICENSE` & `autogaita-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autogaita-0.0.5/README.md` & `autogaita-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 ![AutoGaitA](https://github.com/mahan-hosseini/AutoGaitA/blob/main/res/autogaita_logo.png?raw=true)
-![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
+[![PyPI version](https://badge.fury.io/py/autogaita.svg)](https://badge.fury.io/py/autogaita)
+[![Test AutoGaitA](https://github.com/mahan-hosseini/AutoGaitA/actions/workflows/auto_test_gaita.yml/badge.svg)](https://github.com/mahan-hosseini/AutoGaitA/actions/workflows/auto_test_gaita.yml)
+![Python](https://img.shields.io/badge/python-v3.10+-blue.svg)
 ![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)
 ![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 # Automated Gait Analysis in Python 🐸
 
 - AutoGaitA simplifies, accelerates, and standardises gait analyses after body posture tracking with [DeepLabCut](https://github.com/DeepLabCut/DeepLabCut) and [Simi Motion](http://www.simi.com/en/products/movement-analysis/simi-motion-2d3d.html?type=rss%2F). 
 - AutoGaitA's first-level tools provide a wide range of automated kinematic analyses for each input video and AutoGaitA Group allows the comparison of up to six groups. 
 - AutoGaitA enables comparisons to be made across experimental conditions, species, disease states or genotypes. 
 - Despite being developed with gait data, AutoGaitA can be utilised for the analysis of any motor behaviour.
 
 ## Getting Started
 
 ***Note!** Our documentation provides step-by-step walkthroughs of how to install autogaita for **[Windows](https://docs.google.com/document/d/1Y4wrrsjs0ybLDKPzE2LAatqPDq9jtwjIuk4M0jRZ3wE/edit#heading=h.28j6wu2vamre)** and **[Mac](https://docs.google.com/document/d/1Y4wrrsjs0ybLDKPzE2LAatqPDq9jtwjIuk4M0jRZ3wE/edit)***
 
-It is strongly recommended that a separate virtual environment for AutoGaitA is created via
+It is strongly recommended that a separate virtual environment for AutoGaitA is created (note that the approach below creates the virtual environment to your current directory):
 
-`python -m venv env_gaita`
+- Create the virtual environment
+    - `python -m venv env_gaita`
 
-After creating and activating the virtual environment, AutoGaitA can be installed via pip
+- After creation, activate the virtual environment via:
+    - *Windows:* `env_gaita\Scripts\activate`
+    - *Mac:* `source env_gaita/bin/activate`
 
-`pip install autogaita`
+- Once activated, install AutoGaitA in the virtual environment via pip: `pip install autogaita`.
 
-The main user interface can then be accessed via
-
-`python -m autogaita`
+- Access the main user interface via `python -m autogaita`.
 
 ## Tutorials and Examples
 
 ### Video Walkthrough Tutorials
 
 **[The AutoGaitA YouTube Channel](https://youtube.com/playlist?list=PLCn5T7K_H8K56NIcEsfDK664OP7cN_Bad&si=mV5p2--nYvbofkPh) provides tutorials for file preparation and instructions on how to use AutoGaitA**
 
@@ -50,13 +53,17 @@
 
 **Find out more about *AutoGaitA's custom joints and angles:***
 - [YouTube - AutoGaitA DLC Advanced Configuration](https://youtu.be/YABoQMOqChk?feature=shared) 
 - [YouTube - AutoGaitA Simi](https://youtu.be/fJhnjrJbA5c?feature=shared) 
 - [Documentation - AutoGaitA DLC](https://docs.google.com/document/d/1Y4wrrsjs0ybLDKPzE2LAatqPDq9jtwjIuk4M0jRZ3wE/edit#heading=h.20bg7b7ymt0b)
 - [Documentation - AutoGaitA Simi](https://docs.google.com/document/d/1Y4wrrsjs0ybLDKPzE2LAatqPDq9jtwjIuk4M0jRZ3wE/edit#heading=h.uz61bpmua7qz)
 
+## Reference
+If you use this code or data please [cite our preprint](https://www.biorxiv.org/content/10.1101/2024.04.14.589409v1).
+
 ## License
+AutoGaitA is licensed under [GPL v3.0](https://github.com/mahan-hosseini/AutoGaitA/blob/main/LICENSE) and Forschungszentrum Jülich GmbH holds all copyrights. 
 
-AutoGaitA is licensed under [GPL v3.0](https://github.com/mahan-hosseini/AutoGaitA/blob/main/LICENSE) and Forschungszentrum Jülich GmbH holds all copyrights.
+The AutoGaitA software is provided without warranty of any kind, express or implied, including, but not limited to, the implied warranty of fitness for a particular purpose.
 
 ## Authors
 Mahan Hosseini
```

### Comparing `autogaita-0.0.5/autogaita/autogaita.py` & `autogaita-0.0.6/autogaita/autogaita.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     """Configure the icon - in macos it changes the dock icon, in windows it changes
     all windows titlebar icons (taskbar cannot be changed without converting to exe)
     """
     if platform.system().startswith("Darwin"):
         try:
             from Cocoa import NSApplication, NSImage
         except ImportError:
-            print('Unable to import pyobjc modules')
+            print("Unable to import pyobjc modules")
         else:
             with resources.path("autogaita", "autogaita_icon.icns") as icon_path:
                 ns_application = NSApplication.sharedApplication()
                 logo_ns_image = NSImage.alloc().initWithContentsOfFile_(str(icon_path))
                 ns_application.setApplicationIconImage_(logo_ns_image)
     elif platform.system().startswith("win"):
         with resources.path("autogaita", "autogaita_icon.ico") as icon_path:
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_dlc.py` & `autogaita-0.0.6/autogaita/autogaita_dlc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # %% imports
 import os
 import sys
-import pdb
 import shutil
 import json
+import warnings
 import pandas as pd
 import numpy as np
 import math
 import matplotlib
 import matplotlib.pyplot as plt
 
 # %% constants
 plt.rcParams["figure.dpi"] = 300  # increase resolution of figures
 DIRECTION_DLC_THRESHOLD = 0.95  # DLC confidence used for direction-detection
 TIME_COL = "Time"
 ISSUES_TXT_FILENAME = "Issues.txt"  # filename to which we write issues-info
 CONFIG_JSON_FILENAME = "config.json"  # filename to which we write cfg-infos
 SCXLS_MOUSECOLS = [
-    "Mouse", "mouse", "Fly", "fly", "Animal", "animal", "Subject", "subject", "ID", "id"
-    ]  # SC XLS info
+    "Mouse",
+    "mouse",
+    "Fly",
+    "fly",
+    "Animal",
+    "animal",
+    "Subject",
+    "subject",
+    "ID",
+    "id",
+]  # SC XLS info
 SCXLS_RUNCOLS = ["Run", "run", "Runs", "runs", "Trial", "trial", "Trials", "trials"]
 SCXLS_SCCOLS = ["SC Number", "SC number", "sc number", "SC Num", "sc num", "SC num"]
 SWINGSTART_COL = "Swing (ti)"
 STANCEEND_COL = "Stance (te)"
 ORIGINAL_XLS_FILENAME = " - Original Stepcycles"  # filenames of sheet exports
 NORMALISED_XLS_FILENAME = " - Normalised Stepcycles"
 AVERAGE_XLS_FILENAME = " - Average Stepcycle"
@@ -231,15 +240,15 @@
     }
     # note - using "w" will overwrite/truncate file, thus no need to remove it if exists
     with open(config_json_path, "w") as config_json_file:
         json.dump(config_vars_to_json, config_json_file, indent=4)
     # if wanted: fix that deeplabcut inverses y
     if invert_y_axis:
         for col in data.columns:
-            if col.endswith("y"):
+            if col.endswith(" y"):
                 data[col] = data[col] * -1
     # if we don't have a beam to subtract, normalise y to global y minimum being 0
     if not subtract_beam:
         global_y_min = float("inf")
         y_cols = [col for col in data.columns if col.endswith("y")]
         global_y_min = min(data[y_cols].min())
         data[y_cols] -= global_y_min
@@ -255,24 +264,26 @@
     # subtract the beam from the joints to normalise y
     # => bc. we simulate that all mice run from left to right, we can write:
     #     (note that we also flip beam x columns, but never y-columns!)
     # => & bc. we multiply y values by *-1 earlier, it's a neg_num - - neg_num
     #    pushing it towards zero.
     # => using list(set()) to ensure that we don't have duplicate values (if users
     #    should have provided them in both cfg vars by misstake)
+    # => beam_col_left and right is provided by users
     if subtract_beam:
+        # note beam_col_left/right are always lists in cfg!
+        beam_col_left = cfg["beam_col_left"][0]
+        beam_col_right = cfg["beam_col_right"][0]
         for joint in list(set(hind_joints + beam_hind_jointadd)):
-            data[joint + "y"] = data[joint + "y"] - data["BeamLeft y"]
+            data[joint + "y"] = data[joint + "y"] - data[beam_col_left + "y"]
         for joint in list(set(fore_joints + beam_fore_jointadd)):
-            data[joint + "y"] = data[joint + "y"] - data["BeamRight y"]
-        dropcols = [c for c in data.columns if "Beam" in c]
-        data.drop(columns=dropcols, inplace=True)  # beamcols not needed anymore
+            data[joint + "y"] = data[joint + "y"] - data[beam_col_right + "y"]
+        data.drop(columns=list(beamdf.columns), inplace=True)  # beam not needed anymore
     # add Time and round based on sampling rate
     data[TIME_COL] = data.index * (1 / sampling_rate)
-    pdb.set_trace()
     if sampling_rate <= 100:
         data[TIME_COL] = round(data[TIME_COL], 2)
     elif 100 < sampling_rate <= 1000:
         data[TIME_COL] = round(data[TIME_COL], 3)
     else:
         data[TIME_COL] = round(data[TIME_COL], 4)
     # reorder the columns we added
@@ -339,21 +350,24 @@
     Procedure
     ---------
     Check that no strings are empty
     Check that all strings end with a space character
     Check that all features are present in the dataset
     Add plot_joints & direction_joint
     Make sure to set dont_show_plots to True if Python is not in interactive mode
+    If users subtract a beam, set normalise @ sc level to False
     """
 
-    # run the 3 tests first
+    # run the tests first
     for cfg_key in [
         "angles",
         "hind_joints",
         "fore_joints",
+        "beam_col_left",  # note beamcols are lists even though len=1 bc. of
+        "beam_col_right",  # check function's procedure
         "beam_hind_jointadd",
         "beam_fore_jointadd",
     ]:
         cfg[cfg_key] = check_and_fix_cfg_strings(data, cfg, cfg_key, info)
 
     # add plot_joints - used for average plots & stick diagram
     hind_joints = cfg["hind_joints"]
@@ -369,35 +383,62 @@
         )
         write_issues_to_textfile(fix_plot_joints_message, info)
         print(fix_plot_joints_message)
         cfg["plot_joints"] = hind_joints
     else:
         cfg["plot_joints"] = hind_joints[: cfg["plot_joint_number"]]
 
-    # add direction_joint - used to determine gait direction
+    # check hindlimb joints & add direction_joint - used to determine gait direction
     if not hind_joints:  # no valid string after above cleaning
         no_hind_joint_message = (
             "\n******************\n! CRITICAL ERROR !\n******************\n"
             + "After testing your hind limb joint names, no valid joint was left to "
             + "perform gait direction checks on.\nPlease make sure that at least one "
             + "hind limb joint is provided & try again!"
-            )
+        )
         write_issues_to_textfile(no_hind_joint_message, info)
         print(no_hind_joint_message)
         return
     cfg["direction_joint"] = hind_joints[0]
 
+    # if subtracting beam, check that its colnames were valid.
+    if cfg["subtract_beam"]:
+        beam_col_error_message = (
+            "\n******************\n! CRITICAL ERROR !\n******************\n"
+            + "It seems like you want to normalise heights to a baseline (beam)."
+            + "\nUnfortunately we were unable to find the y-columns you listed in "
+            + "your beam's csv-file.\nPlease try again.\nInvalid beam side(s) was/were:"
+        )
+        beam_error = False  # check 3 possible cases
+        if (cfg["beam_col_left"]) and (not cfg["beam_col_right"]):
+            beam_error = True
+            beam_col_error_message += "\n right beam!"
+        elif (not cfg["beam_col_left"]) and (cfg["beam_col_right"]):
+            beam_error = True
+            beam_col_error_message += "\n left beam!"
+        elif (not cfg["beam_col_left"]) and (not cfg["beam_col_right"]):
+            beam_error = True
+            beam_col_error_message += "\n both beams!"
+        if beam_error:  # if any case was True, stop everything
+            write_issues_to_textfile(beam_col_error_message, info)
+            print(beam_col_error_message)
+            return
+
     # dont show plots
     # !!! If users should complain that they dont get figures but they should, it might
     #     be because these lines wrongly determine user to be in non-interactive mode
     #     while they are not!
     if not hasattr(sys, "ps1") and not sys.flags.interactive:
         cfg["dont_show_plots"] = True
         matplotlib.use("agg")
 
+    # never normalise @ SC level if user subtracted a beam
+    if cfg["subtract_beam"]:
+        cfg["normalise_height_at_SC_level"] = False
+
     return cfg
 
 
 def check_and_fix_cfg_strings(data, cfg, cfg_key, info):
     """Check and fix strings in our joint & angle lists so that:
     1) They don't include empty strings
     2) All strings end with the space character (since we do string + "y")
@@ -434,37 +475,54 @@
             string_variable = clean_string_list
             # print & save info about remaining ("clean") strings
             clean_strings_message = "\nRemaining joints / key points are:"
             for string in clean_string_list:
                 clean_strings_message += "\n" + string
             clean_strings_message += (
                 "\n\nNote that capitalisation matters."
-                + "\nIf you are running a group analysis, we'll use this updated cfg "
+                + "\nIf you are running a batch analysis, we'll use this updated cfg "
                 + "throughout\nCheck out the config.json file for the full cfg used."
             )
             print(clean_strings_message)
             write_issues_to_textfile(clean_strings_message, info)
 
     # things are more involved for angle dicts
     elif type(string_variable) is dict:
+        # 1) test if the lists of all keys are equally long, if not throw out last idxs
+        key_lengths = [len(string_variable[key]) for key in string_variable.keys()]
+        if not all(key_length == key_lengths[0] for key_length in key_lengths):
+            min_length = min(key_lengths)
+            for key in string_variable:  # remove invalid idxs
+                string_variable[key] = string_variable[key][:min_length]
+            key_length_mismatch_message = (  # inform user
+                "\n***********\n! WARNING !\n***********\n"
+                + "\nLength-mismatch in angle configuration!"
+                + "\nCheck angles' name/upper/lower-joint entries."
+                + "\nOnly processing first "
+                + str(min_length)
+                + " entries."
+            )
+            print(key_length_mismatch_message)
+            write_issues_to_textfile(key_length_mismatch_message, info)
+        # 2) check if all strings in the angle dict are valid columns
         invalid_angletrio_message = ""
         invalid_idxs = []  # these idxs hold across the 3 keys of our angles-dict
         for key in string_variable:
             # important to do this first (else string + "y" is invalid)
             string_variable[key] = [
                 s if s.endswith(" ") else s + " " for s in string_variable[key]
             ]
             # remove any empty or invalid (i.e. not in data) strings from our angletrio
             this_keys_missing_strings = ""
             for idx, string in enumerate(string_variable[key]):
                 if string + "y" not in data.columns:  # checks for empty strings too
                     invalid_idxs.append(idx)
                     if not this_keys_missing_strings:  # first occurance
                         this_keys_missing_strings += "\nAngle's " + key + " key: "
-                    this_keys_missing_strings += (string + "(#" + str(idx+1) + ") / ")
+                    this_keys_missing_strings += string + "(#" + str(idx + 1) + ") / "
             # string concat outside of idx-forloop above please
             invalid_angletrio_message += this_keys_missing_strings
         # if we have to remove idxs from all keys of our angles dict
         if invalid_angletrio_message:
             # print and save
             angles_warning = (
                 "\n***********\n! WARNING !\n***********\n"
@@ -493,15 +551,15 @@
                     "\nLower Joint: " + string_variable["lower_joint"][i]
                 )
                 clean_angles_message += (
                     "\nUpper Joint: " + string_variable["upper_joint"][i]
                 )
             clean_angles_message += (
                 "\n\nNote that capitalisation matters."
-                + "\nIf you are running a group analysis, we'll use this updated cfg "
+                + "\nIf you are running a batch analysis, we'll use this updated cfg "
                 + "throughout\nCheck out the config.json file for the full cfg used."
             )
             print(clean_angles_message)
             write_issues_to_textfile(clean_angles_message, info)
 
     return string_variable
 
@@ -623,25 +681,25 @@
 
     # check if excel file is .xlsx or .xls, if none found try to fix it
     if (".xls" in sctable_filename) | (".xlsx" in sctable_filename):
         if os.path.exists(os.path.join(root_dir, sctable_filename)):
             SCdf = pd.read_excel(os.path.join(root_dir, sctable_filename))
         else:
             raise FileNotFoundError(
-                "No SC XLS table found! sctable_filename has to be @ root_dir"
+                "No Annotation Table found! sctable_filename has to be @ root_dir"
             )
     else:
         # in cases below use string-concat (+) - otherwise xls added as path
         if os.path.exists(os.path.join(root_dir, sctable_filename + ".xls")):
             SCdf = pd.read_excel(os.path.join(root_dir, sctable_filename + ".xls"))
         elif os.path.exists(os.path.join(root_dir, sctable_filename + ".xlsx")):
             SCdf = pd.read_excel(os.path.join(root_dir, sctable_filename + ".xlsx"))
         else:
             raise FileNotFoundError(
-                "No SC XLS table found! sctable_filename has to be @ root_dir"
+                "No Annotation Table found! sctable_filename has to be @ root_dir"
             )
     # see if table columns are labelled correctly (try a couple to allow user typos)
     valid_col_flags = [False, False, False]
     header_columns = ["", "", ""]
     for h, header in enumerate([SCXLS_MOUSECOLS, SCXLS_RUNCOLS, SCXLS_SCCOLS]):
         for header_col in header:
             if header_col in SCdf.columns:
@@ -766,14 +824,15 @@
     all_cycles = check_cycle_duplicates(all_cycles)
     # check if user input progressively later latencies
     all_cycles = check_cycle_order(all_cycles, info)
     # check if DLC tracking broke for any SCs - if so remove them
     all_cycles = check_DLC_tracking(data, info, all_cycles, cfg)
     return all_cycles
 
+
 # ..............................  helper functions  ....................................
 def check_cycle_out_of_bounds(all_cycles):
     """Check if user provided SC latencies that were not in video/data bounds"""
     clean_cycles = []
     for cycle in all_cycles:
         # below checks if values are any type of int (just in case this should
         # for some super random reason change...)
@@ -813,24 +872,24 @@
             if cycle[1] > cycle[0]:
                 clean_cycles.append(cycle)  # only append if both tests passed
                 current_max_time = cycle[1]
             else:
                 this_message = (
                     "\n***********\n! WARNING !\n***********\n"
                     + "SC #"
-                    + str(c+1)
+                    + str(c + 1)
                     + " has a later start than end latency - Skipping!"
                 )
                 print(this_message)
                 write_issues_to_textfile(this_message, info)
         else:
             this_message = (
                 "\n***********\n! WARNING !\n***********\n"
                 + "SC #"
-                + str(c+1)
+                + str(c + 1)
                 + " has an earlier start than previous SC's end latency - Skipping!"
             )
             print(this_message)
             write_issues_to_textfile(this_message, info)
     return clean_cycles
 
 
@@ -926,15 +985,15 @@
 
 
 # %% local functions 3 - normalise SCs & export (orig. & norm.) XLS files
 # Note
 # ----
 # There is quite a lot going on in this function. We:
 # 1) loop through all step cycles for one leg at a time and extract data
-# 2) for each step's data we normalise all y (height) values to the hind paw's minimum
+# 2) for each step's data we normalise all y (height) values to the body's minimum
 #    if wanted
 # 3) we compute and add features (angles, velocities, accelerations)
 #    ==> see norm_y_and_add_features_to_one_step & helper functions a
 # 4) immediately after adding features, we normalise a step to bin_num
 #    ==> see normalise_one_steps_data & helper functions b
 # 5) we add original and normalised steps to all_steps_data and normalised_steps_data
 # 6) once we are done with this we create average and std dataframes7
@@ -954,28 +1013,34 @@
     # exactly 1 step
     if len(all_cycles) == 1:
         this_step = data_copy.loc[all_cycles[0][0] : all_cycles[0][1]]
         all_steps_data = norm_y_and_add_features_to_one_step(this_step, cfg)
         normalised_steps_data = normalise_one_steps_data(all_steps_data, bin_num)
     # 2 or more steps - build dataframe
     elif len(all_cycles) > 1:
-        # first step is added manually
+        # first- step is added manually
         first_step = data_copy.loc[all_cycles[0][0] : all_cycles[0][1]]
         first_step = norm_y_and_add_features_to_one_step(first_step, cfg)
         all_steps_data = first_step
         normalised_steps_data = normalise_one_steps_data(first_step, bin_num)
         # some prep for addition of further steps
         sc_num = len(all_cycles)
         nanvector = data_copy.loc[[1]]
-        nanvector[:] = np.nan
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            nanvector[:] = np.nan
         # ..............................  step-loop  ...................................
         for s in range(1, sc_num, 1):
             # get step separators
             numvector = data_copy.loc[[1]]
-            numvector[:] = s + 1
+            # we are ignoring this because we wont work with the incompatible dtypes ourselves much anymore (just export as xlsx and plot) - so its fine
+            # https://docs.python.org/3/library/warnings.html#temporarily-suppressing-warnings
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                numvector[:] = s + 1
             all_steps_data = add_step_separators(all_steps_data, nanvector, numvector)
             # this_step
             this_step = data_copy.loc[all_cycles[s][0] : all_cycles[s][1]]
             this_step = norm_y_and_add_features_to_one_step(this_step, cfg)
             all_steps_data = pd.concat([all_steps_data, this_step], axis=0)
             # this_normalised_step
             this_normalised_step = normalise_one_steps_data(this_step, bin_num)
@@ -1269,15 +1334,15 @@
     all_steps_data = results["all_steps_data"]
     average_data = results["average_data"]
     std_data = results["std_data"]
     x_acceleration = cfg["x_acceleration"]
     angular_acceleration = cfg["angular_acceleration"]
     dont_show_plots = cfg["dont_show_plots"]
     if dont_show_plots:
-        plt.switch_backend('Agg')
+        plt.switch_backend("Agg")
 
     # ....................0 - extract SCs from all_steps_data...........................
     sc_idxs = extract_sc_idxs(all_steps_data)
     cfg["sc_num"] = len(sc_idxs)  # add number of scs for plotting SE if wanted
 
     # .........................1 - y coords by x coords.................................
     plot_joint_y_by_x(all_steps_data, sc_idxs, info, cfg)
@@ -1393,30 +1458,42 @@
             this_x = all_steps_data.iloc[sc_idxs[s], x_col_idx]
             this_y = all_steps_data.iloc[sc_idxs[s], y_col_idx]
             if sampling_rate <= 100:
                 float_precision = 2  # how many decimals we round to
             else:
                 float_precision = 4
             this_label = (
-                str(round(all_steps_data.iloc[sc_idxs[s][0], time_col_idx], float_precision))
+                str(
+                    round(
+                        all_steps_data.iloc[sc_idxs[s][0], time_col_idx],
+                        float_precision,
+                    )
+                )
                 + "-"
-                + str(round(all_steps_data.iloc[sc_idxs[s][-1], time_col_idx], float_precision))
+                + str(
+                    round(
+                        all_steps_data.iloc[sc_idxs[s][-1], time_col_idx],
+                        float_precision,
+                    )
+                )
                 + "s"
             )
             ax[j].plot(this_x, this_y, label=this_label)
         ax[j].set_xlabel("x (pixel)")  # will be overwritten if we convert
         ax[j].set_ylabel("y (pixel)")
         ax[j].legend(fontsize=SC_LAT_LEGEND_FONTSIZE)
         if convert_to_mm:
             tickconvert_mm_to_cm(ax[j], "both")
         if joint == "Hind paw tao ":
             figure_file_string = " - Foot y by x coordinates"
         else:
             figure_file_string = " - " + joint + "y by x coordinates"
-        f[j].savefig(results_dir + name + figure_file_string + ".png", bbox_inches="tight")
+        f[j].savefig(
+            results_dir + name + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f[j], results_dir, name, figure_file_string)
         if dont_show_plots:
             plt.close(f[j])
 
 
 def plot_angles_by_time(all_steps_data, sc_idxs, info, cfg):
     """2 - Plot joints' angles as a function of time for each SC"""
@@ -1444,15 +1521,17 @@
         x_col_idx = all_steps_data.columns.get_loc(TIME_COL)
         y_col_idx = all_steps_data.columns.get_loc(angle + "Angle")
         for s in range(sc_num):
             this_x = all_steps_data.iloc[sc_idxs[s], x_col_idx]
             this_y = all_steps_data.iloc[sc_idxs[s], y_col_idx]
             ax[a].plot(this_x, this_y)
         figure_file_string = " - " + angle + " Angle by Time"
-        f[a].savefig(results_dir + name + figure_file_string + ".png", bbox_inches="tight")
+        f[a].savefig(
+            results_dir + name + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f[a], results_dir, name, figure_file_string)
         if dont_show_plots:
             plt.close(f[a])
 
 
 def plot_hindlimb_stickdiagram(all_steps_data, sc_idxs, info, cfg):
     """3 - Plot a stick diagram of the hindlimb"""
@@ -1477,17 +1556,23 @@
     for s, this_color_dict in zip(range(sc_num), color_cycle):  # SC loop (colors)
         this_color = this_color_dict["color"][:3]
         if sampling_rate <= 100:
             float_precision = 2  # how many decimals we round to
         else:
             float_precision = 4
         this_label = (
-            str(round(all_steps_data.iloc[sc_idxs[s][0], time_col_idx], float_precision))
+            str(
+                round(all_steps_data.iloc[sc_idxs[s][0], time_col_idx], float_precision)
+            )
             + "-"
-            + str(round(all_steps_data.iloc[sc_idxs[s][-1], time_col_idx], float_precision))
+            + str(
+                round(
+                    all_steps_data.iloc[sc_idxs[s][-1], time_col_idx], float_precision
+                )
+            )
             + "s"
         )
         for i in sc_idxs[s]:  # loop over timepoints of current SC
             this_xs = list()  # for each timepoint, define joints' xy coord new
             this_ys = list()
             for joint in plot_joints:
                 x_col_idx = all_steps_data.columns.get_loc(joint + "x")
@@ -1533,17 +1618,23 @@
     for s, this_color in zip(range(sc_num), color_cycle):  # SC loop (colors)
         this_color = this_color["color"][:3]
         if sampling_rate <= 100:
             float_precision = 2  # how many decimals we round to
         else:
             float_precision = 4
         this_label = (
-            str(round(all_steps_data.iloc[sc_idxs[s][0], time_col_idx], float_precision))
+            str(
+                round(all_steps_data.iloc[sc_idxs[s][0], time_col_idx], float_precision)
+            )
             + "-"
-            + str(round(all_steps_data.iloc[sc_idxs[s][-1], time_col_idx], float_precision))
+            + str(
+                round(
+                    all_steps_data.iloc[sc_idxs[s][-1], time_col_idx], float_precision
+                )
+            )
             + "s"
         )
         for i in sc_idxs[s]:
             this_xs = list()
             this_ys = list()
             for joint in fore_joints:
                 x_col_idx = all_steps_data.columns.get_loc(joint + "x")
@@ -1823,15 +1914,17 @@
 
 
 def save_as_svg(figure, results_dir, name, figure_file_string):
     """Save figures as svgs to separate subfolder"""
     svg_dir = os.path.join(results_dir, "SVG Figures")
     if not os.path.exists(svg_dir):
         os.makedirs(svg_dir)
-    figure.savefig(svg_dir + "/" + name + figure_file_string + ".svg", bbox_inches="tight")
+    figure.savefig(
+        svg_dir + "/" + name + figure_file_string + ".svg", bbox_inches="tight"
+    )
 
 
 def tickconvert_mm_to_cm(axis, whichlabel):
     """Convert axis-ticks from mm (of data) to cm"""
     if whichlabel == "both":
         x_ticks = axis.get_xticks()
         x_ticklabels = []
@@ -1868,9 +1961,9 @@
 if __name__ == "__main__":
     dlc_info_message = (
         "\n*************\nnot like this\n*************\n"
         + "You are trying to execute autogaita.dlc as a script, but that is not "
         + "possible.\nIf you prefer a non-GUI approach, please either: "
         + "\n1. Call this as a function, i.e. autogaita.dlc(info, folderinfo, cfg)"
         + "\n2. Use the single or multirun scripts in the batchrun_scripts folder"
-        )
+    )
     print(dlc_info_message)
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_dlc_gui.py` & `autogaita-0.0.6/autogaita/autogaita_dlc_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     "x_sc_broken_threshold",
     "y_sc_broken_threshold",
     "bin_num",
     "mouse_num",
     "run_num",
     "plot_joint_number",
 ]
-LIST_VARS = ["hind_joints", "fore_joints", "beam_hind_jointadd", "beam_fore_jointadd"]
+LIST_VARS = ["hind_joints", "fore_joints", "beam_hind_jointadd", "beam_fore_jointadd",
+             "beam_col_left", "beam_col_right"]
 DICT_VARS = ["angles"]
 WINDOWS_TASKBAR_MAXHEIGHT = 72
 
 # %% An important Note
 # I am using a global variable called cfg because I need its info to be shared
 # between root and advanced_cfg windows. This is not the object-oriented way
 # that one would do this typically. However, it works as expected since:
@@ -114,15 +115,20 @@
         "Elbow ",
         "Lower Shoulder ",
         "Upper Shoulder ",
     ]
     cfg["fore_joints"] = []
     for joint in default_fore_joints:
         cfg["fore_joints"].append(tk.StringVar(root, joint))
-    # beam subtraction columns
+    # beam columns - append to empty list to have a list of len=1
+    # (required for test in _dlc)
+    cfg["beam_col_left"] = []
+    cfg["beam_col_left"].append(tk.StringVar(root, "BeamLeft"))
+    cfg["beam_col_right"] = []
+    cfg["beam_col_right"].append(tk.StringVar(root, "BeamRight"))
     default_beam_hind_jointadd = ["Tail base ", "Tail center ", "Tail tip "]
     cfg["beam_hind_jointadd"] = []
     for joint in default_beam_hind_jointadd:
         cfg["beam_hind_jointadd"].append(tk.StringVar(root, joint))
     default_beam_fore_jointadd = ["Nose ", "Ear base "]
     cfg["beam_fore_jointadd"] = []
     for joint in default_beam_fore_jointadd:
@@ -182,15 +188,15 @@
     )
     cfgheader_label.grid(row=3, column=0, columnspan=2, rowspan=1, sticky="nsew")
 
     # .........................  left section  .................................
     # sampling rate
     samprate_label = ctk.CTkLabel(
         root, text="Insert sampling rate of videos (frames/second)"
-        )
+    )
     samprate_label.grid(row=4, column=0)
     samprate_entry = ctk.CTkEntry(root, textvariable=cfg["sampling_rate"])
     samprate_entry.grid(row=5, column=0)
     # subtract beam
     subtract_beam_string = "Normalise y-coordinates to baseline height"
     subtract_beam_checkbox = ctk.CTkCheckBox(
         root,
@@ -468,32 +474,39 @@
     columnwindow = ctk.CTkToplevel(root)
     columnwindow.geometry("%dx%d+%d+%d" % root_dimensions)
     columnwindow.title("Custom column names & features")
     fix_window_after_its_creation(columnwindow)
 
     # .............  Nested Function: Add joint label & entry  .........................
     def add_joint(window, key):
-        """Add a joint if needed or a angle name/lower_joint/upper_joint if angle widget
-        """
+        """Add a joint if needed or a angle name/lower_joint/upper_joint if angle widget"""
         # append StringVar to cfg appropriately
         if key == "angles":
             for angle_key in cfg[key]:
                 cfg[key][angle_key].append(tk.StringVar(root, ""))
         else:
             cfg[key].append(tk.StringVar(root, ""))
         # find out the number of rows to append to it
         nrows = window.grid_size()[1]
         # add stuff based on to which case we are adding
-        if key == "hind_joints":
-            label = ctk.CTkLabel(window, text="Hindlimb Joint #" + str(len(cfg[key])))
-            label.grid(row=nrows + 1, column=0, sticky="ew")
-            entry = ctk.CTkEntry(window, textvariable=cfg[key][-1])
-            entry.grid(row=nrows + 2, column=0)
-        elif key == "fore_joints":
-            label = ctk.CTkLabel(window, text="Forelimb Joint #" + str(len(cfg[key])))
+        if key in [
+            "hind_joints",
+            "fore_joints",
+            "beam_hind_jointadd",
+            "beam_fore_jointadd",
+        ]:
+            if key == "hind_joints":
+                label_string = "Hindlimb Joint #" + str(len(cfg[key]))
+            elif key == "fore_joints":
+                label_string = "Forelimb Joint #" + str(len(cfg[key]))
+            elif key == "beam_hind_jointadd":
+                label_string = "Hindlimb Beamsubtraction Joint #" + str(len(cfg[key]))
+            elif key == "beam_fore_jointadd":
+                label_string = "Forelimb Beamsubtraction Joint #" + str(len(cfg[key]))
+            label = ctk.CTkLabel(window, text=label_string)
             label.grid(row=nrows + 1, column=0, sticky="ew")
             entry = ctk.CTkEntry(window, textvariable=cfg[key][-1])
             entry.grid(row=nrows + 2, column=0)
         elif key == "angles":
             for a, angle_key in enumerate(cfg[key]):
                 if angle_key == "name":
                     this_case = "Angle"
@@ -503,91 +516,167 @@
                     this_case = "Upper Joint"
                 label = ctk.CTkLabel(
                     window, text=this_case + " #" + str(len(cfg[key][angle_key]))
                 )
                 label.grid(row=nrows + 1, column=angle_column + a, sticky="ew")
                 entry = ctk.CTkEntry(window, textvariable=cfg[key][angle_key][-1])
                 entry.grid(row=nrows + 2, column=angle_column + a)
-        else:  # beamsubtract joints
-            label = ctk.CTkLabel(
-                window, text="Beamsubtract Joint #" + str(len(cfg[key]))
-            )
-            label.grid(row=nrows + 1, column=0, sticky="ew")
-            entry = ctk.CTkEntry(window, textvariable=cfg[key][-1])
-            entry.grid(row=nrows + 2, column=0)
         # maximise columns
         for c in range(window.grid_size()[0]):
             window.grid_columnconfigure(c, weight=1)
 
     # ...............  Nested Function: Beam jointadd window  ..........................
-    def build_beam_jointadd_window(limb):
-        """Build small windows for configuring joints to subtract the beam from if
-        users had one"""
-        # build window and make it pretty and nice
-        w = root_dimensions[0]
-        h = root_dimensions[1]
+    def build_beam_window():
+        """Build a window for configuring the beam, i.e.:
+        1. beam_col_left and right
+        ==> what were the col names of your beam in the beam file
+        2. beam_hind_jointadd and beam_fore_jointadd
+        ==> what additional joints (not included in hind/fore) do you want to include in beam standardisation?
+        """
+        # build window and fullscreen
         beamwindow = ctk.CTkToplevel(columnwindow)
-        beam_w = w * (1 / 3)
-        beam_h = h * (1 / 2)
-        beam_x = ((1 / 2) * w) - (1 / 2 * beam_w)
-        beam_y = ((1 / 2) * h) - (1 / 2 * beam_h)
-        beamwindow.geometry("%dx%d+%d+%d" % (beam_w, beam_h, beam_x, beam_y))
+        beamwindow.geometry("%dx%d+%d+%d" % (root_dimensions))
         beamwindow.title("Beam Configuration")
         fix_window_after_its_creation(beamwindow)
-        # prepare key based on limb input
-        if limb == "hind":
-            key = "beam_hind_jointadd"
-        elif limb == "fore":
-            key = "beam_fore_jointadd"
-        # header label
-        beam_label = ctk.CTkLabel(
+        beam_scrollable_rows = 1
+        total_padx = 20
+        left_padx = (total_padx, total_padx / 2)
+        right_padx = (total_padx / 2, total_padx)
+        # ................... left section - left beam / hind joints ...................
+        # left beam label
+        beam_left_label = ctk.CTkLabel(
             beamwindow,
-            text="Which " + limb + "limb joints to subtract beam from",
+            text="Left Beam Column",
             fg_color=FG_COLOR,
             text_color=HEADER_TXT_COLOR,
             font=("Britannic Bold", HEADER_FONT_SIZE),
         )
-        beam_label.grid(row=0, column=0, sticky="nsew")
+        beam_left_label.grid(row=0, column=0, sticky="nsew")
+        # left beam entry
+        beam_left_entry = ctk.CTkEntry(beamwindow, textvariable=cfg["beam_col_left"][0])
+        beam_left_entry.grid(row=1, column=0)
+        # important: cfg key for forelimb joint add
+        hindlimb_key = "beam_hind_jointadd"
+        # hindlimb jointadd label
+        hind_jointsubtract_label = ctk.CTkLabel(
+            beamwindow,
+            text="Hindlimb Joints subtracted from Left Beam",
+            fg_color=FG_COLOR,
+            text_color=HEADER_TXT_COLOR,
+            font=("Britannic Bold", HEADER_FONT_SIZE),
+        )
+        hind_jointsubtract_label.grid(row=2, column=0, sticky="nsew")
         # initialise scrollable frame for beamsubtract windows
-        beam_frame = ctk.CTkScrollableFrame(beamwindow)
-        beam_scrollable_rows = 1
-        beam_frame.grid(row=1, column=0, rowspan=beam_scrollable_rows, sticky="nsew")
+        hind_jointsubtract_frame = ctk.CTkScrollableFrame(beamwindow)
+        hind_jointsubtract_frame.grid(
+            row=3,
+            column=0,
+            rowspan=beam_scrollable_rows,
+            sticky="nsew",
+        )
         # initialise labels & entries
         initialise_labels_and_entries(
-            beam_frame,
-            key,
-            "Beamsubtract Joint",
+            hind_jointsubtract_frame,
+            hindlimb_key,
+            "Hindlimb Beamsubtraction Joint",
         )
         # add button
-        add_beamjoint_button = ctk.CTkButton(
+        add_hindjoint_button = ctk.CTkButton(
             beamwindow,
-            text="Add beam-subtraction joint",
+            text="Add Hindlimb Beamsubtraction Joint",
             fg_color=FG_COLOR,
             hover_color=HOVER_COLOR,
-            command=lambda: add_joint(beam_frame, key),  # input = cfg's key
+            command=lambda: add_joint(
+                hind_jointsubtract_frame, hindlimb_key
+            ),  # input = cfg's key
         )
-        add_beamjoint_button.grid(
-            row=2 + beam_scrollable_rows, column=0, sticky="nsew", padx=5, pady=(6, 3)
+        add_hindjoint_button.grid(
+            row=3 + beam_scrollable_rows,
+            column=0,
+            sticky="nsew",
+            padx=left_padx,
+            pady=20,
         )
+        # .................. right section - right beam / fore joints ..................
+        # right beam label
+        beam_right_label = ctk.CTkLabel(
+            beamwindow,
+            text="Right Beam Column",
+            fg_color=FG_COLOR,
+            text_color=HEADER_TXT_COLOR,
+            font=("Britannic Bold", HEADER_FONT_SIZE),
+        )
+        beam_right_label.grid(row=0, column=1, sticky="nsew")
+        # right beam entry
+        beam_right_entry = ctk.CTkEntry(beamwindow, textvariable=cfg["beam_col_right"][0])
+        beam_right_entry.grid(row=1, column=1)
+        # important: cfg key for forelimb joint add
+        forelimb_key = "beam_fore_jointadd"
+        # hindlimb jointadd label
+        fore_jointsubtract_label = ctk.CTkLabel(
+            beamwindow,
+            text="Forelimb Joints subtracted from Right Beam",
+            fg_color=FG_COLOR,
+            text_color=HEADER_TXT_COLOR,
+            font=("Britannic Bold", HEADER_FONT_SIZE),
+        )
+        fore_jointsubtract_label.grid(row=2, column=1, sticky="nsew")
+        # initialise scrollable frame for beamsubtract windows
+        fore_jointsubtract_frame = ctk.CTkScrollableFrame(beamwindow)
+        fore_jointsubtract_frame.grid(
+            row=3,
+            column=1,
+            rowspan=beam_scrollable_rows,
+            sticky="nsew",
+        )
+        # initialise labels & entries
+        initialise_labels_and_entries(
+            fore_jointsubtract_frame,
+            forelimb_key,
+            "Forelimb Beamsubtraction Joint",
+        )
+        # add button
+        add_forejoint_button = ctk.CTkButton(
+            beamwindow,
+            text="Add Forelimb Beamsubtraction Joint",
+            fg_color=FG_COLOR,
+            hover_color=HOVER_COLOR,
+            command=lambda: add_joint(
+                fore_jointsubtract_frame, forelimb_key
+            ),  # input = cfg's key
+        )
+        add_forejoint_button.grid(
+            row=3 + beam_scrollable_rows,
+            column=1,
+            sticky="nsew",
+            padx=right_padx,
+            pady=20,
+        )
+        # .................... bottom section - update & close  ........................
         # done button
         beam_done_button = ctk.CTkButton(
             beamwindow,
             text="I am done, update cfg!",
             fg_color=FG_COLOR,
             hover_color=HOVER_COLOR,
             command=lambda: beamwindow.destroy(),
         )
         beam_done_button.grid(
-            row=3 + beam_scrollable_rows, column=0, sticky="nsew", padx=5, pady=(6, 3)
+            row=4 + beam_scrollable_rows,
+            column=0,
+            columnspan=2,
+            sticky="nsew",
+            padx=20,
+            pady=20,
         )
         # maximise widgets
         maximise_widgets(beamwindow)
 
     # ...................  Scrollable Window Configuration  ............................
-    scrollable_rows = 8
+    scrollable_rows = 7
 
     # ...................  Column 0: hind limb joint names  ............................
     hind_column = 0
     # header label
     hind_joint_label = ctk.CTkLabel(
         columnwindow,
         text="Hindlimb Joints",
@@ -595,15 +684,15 @@
         text_color=HEADER_TXT_COLOR,
         font=("Britannic Bold", HEADER_FONT_SIZE),
     )
     hind_joint_label.grid(row=0, column=hind_column, sticky="nsew", pady=(0, 5))
     # initialise scrollable frame for hindlimb
     hindlimb_frame = ctk.CTkScrollableFrame(columnwindow)
     hindlimb_frame.grid(
-        row=1, column=hind_column, rowspan=scrollable_rows, sticky="nsew"
+        row=1, column=hind_column, rowspan=scrollable_rows, sticky="nsew",
     )
     # initialise labels & entries with hind limb defaults
     initialise_labels_and_entries(hindlimb_frame, "hind_joints", "Hindlimb Joint ")
     # add joint button
     add_hind_joint_button = ctk.CTkButton(
         columnwindow,
         text="Add hindlimb joint",
@@ -612,24 +701,45 @@
         command=lambda: add_joint(
             hindlimb_frame, "hind_joints"
         ),  # 2nd input = cfg's key
     )
     add_hind_joint_button.grid(
         row=2 + scrollable_rows, column=hind_column, sticky="nsew", padx=5, pady=(10, 5)
     )
-    # beam subtraction joints window
-    hind_beamsubtract_button = ctk.CTkButton(
+    # beam config window label
+    beam_window_label = ctk.CTkLabel(
+        columnwindow,
+        text="Baseline (Beam) Configuration",
+        fg_color=FG_COLOR,
+        text_color=HEADER_TXT_COLOR,
+        font=("Britannic Bold", HEADER_FONT_SIZE),
+    )
+    beam_window_label.grid(
+        row=4 + scrollable_rows,
+        column=hind_column,
+        columnspan=2,
+        sticky="nsew",
+        padx=1,
+        pady=(0, 5),
+    )
+    # beam config window button
+    beam_window_button = ctk.CTkButton(
         columnwindow,
-        text="Add hindlimb joints for beamsubtraction",
+        text="Configure Beam Columns and Beamsubtraction Joints",
         fg_color=FG_COLOR,
         hover_color=HOVER_COLOR,
-        command=lambda: build_beam_jointadd_window("hind"),
+        command=lambda: build_beam_window(),
     )
-    hind_beamsubtract_button.grid(
-        row=3 + scrollable_rows, column=hind_column, sticky="nsew", padx=5, pady=(10, 5)
+    beam_window_button.grid(
+        row=5 + scrollable_rows,
+        column=hind_column,
+        columnspan=2,
+        sticky="nsew",
+        padx=40,
+        pady=(10, 5),
     )
 
     # ...................  Column 1: fore limb joint names  ............................
     fore_column = 1
     # header label
     fore_joint_label = ctk.CTkLabel(
         columnwindow,
@@ -659,25 +769,14 @@
         command=lambda: add_joint(
             forelimb_frame, "fore_joints"
         ),  # 2nd input = cfg's key
     )
     add_fore_joint_button.grid(
         row=2 + scrollable_rows, column=fore_column, sticky="nsew", padx=5, pady=(10, 5)
     )
-    # beam subtraction joints window
-    fore_beamsubtract_button = ctk.CTkButton(
-        columnwindow,
-        text="Add forelimb joints for beamsubtraction",
-        fg_color=FG_COLOR,
-        hover_color=HOVER_COLOR,
-        command=lambda: build_beam_jointadd_window("fore"),
-    )
-    fore_beamsubtract_button.grid(
-        row=3 + +scrollable_rows, column=fore_column, sticky="nsew", padx=5, pady=5
-    )
 
     # .........  Column 2: angle names/joint-definitions & done button  ................
     angle_column = 2
     # header label
     angle_label = ctk.CTkLabel(
         columnwindow,
         text="Angle Configuration",
@@ -716,28 +815,44 @@
         row=2 + scrollable_rows,
         column=angle_column,
         columnspan=3,
         sticky="nsew",
         padx=5,
         pady=(10, 5),
     )
+    # done label
+    done_label = ctk.CTkLabel(
+        columnwindow,
+        text="Update Configuration",
+        fg_color=FG_COLOR,
+        text_color=HEADER_TXT_COLOR,
+        font=("Britannic Bold", HEADER_FONT_SIZE),
+    )
+    done_label.grid(
+        row=4 + scrollable_rows,
+        column=angle_column,
+        columnspan=3,
+        sticky="nsew",
+        padx=1,
+        pady=(0, 5),
+    )
     # done button
     columncfg_done_button = ctk.CTkButton(
         columnwindow,
         text="I am done, update cfg!",
         fg_color=FG_COLOR,
         hover_color=HOVER_COLOR,
         command=lambda: columnwindow.destroy(),
     )
     columncfg_done_button.grid(
-        row=3 + scrollable_rows,
+        row=5 + scrollable_rows,
         column=angle_column,
         columnspan=3,
         sticky="nsew",
-        padx=5,
+        padx=40,
         pady=(10, 5),
     )
     # maximise everything in columnwindow
     maximise_widgets(columnwindow)
 
 
 def initialise_labels_and_entries(window, key, which_case_string, *args):
@@ -918,62 +1033,56 @@
     # stepcycle latency XLS
     SCXLS_string = "Name of the Annotation Table Excel file"
     SCXLS_label = ctk.CTkLabel(runwindow, text=SCXLS_string, width=runwindow_w)
     SCXLS_label.grid(row=r + 2, column=0)
     SCXLS_entry = ctk.CTkEntry(runwindow, textvariable=results["sctable_filename"])
     SCXLS_entry.grid(row=r + 3, column=0)
     # file naming convention label
-    name_convention_string = ("According to [A]_[B]_[C]_[D]-[E][G] filename convention "
-                              + "(e.g. C57B6_Mouse10_25mm_Run1-6DLC-JointTracking):")
+    name_convention_string = (
+        "According to [A]_[B]_[C]_[D]-[E][G] filename convention "
+        + "(e.g. C57B6_Mouse10_25mm_Run1-6DLC-JointTracking):"
+    )
     name_convention_label = ctk.CTkLabel(
         runwindow, text=name_convention_string, width=runwindow_w
-        )
+    )
     name_convention_label.grid(row=r + 4, column=0)
     # data string
     data_string = "[G] What is the identifier of the DLC-tracked coordinate file?"
     data_label = ctk.CTkLabel(runwindow, text=data_string, width=runwindow_w)
     data_label.grid(row=r + 5, column=0)
     data_entry = ctk.CTkEntry(runwindow, textvariable=results["data_string"])
     data_entry.grid(row=r + 6, column=0)
     # beam string
     beam_string = (
         "[G] What is the identifier of the DLC-tracked baseline file? (optional)"
-        )
+    )
     beam_label = ctk.CTkLabel(runwindow, text=beam_string, width=runwindow_w)
     beam_label.grid(row=r + 7, column=0)
     beam_entry = ctk.CTkEntry(runwindow, textvariable=results["beam_string"])
     beam_entry.grid(row=r + 8, column=0)
     # premouse_num string
-    premouse_string = (
-        "[B] Define the 'unique subject identifier' preceding the number"
-    )
+    premouse_string = "[B] Define the 'unique subject identifier' preceding the number"
     premouse_label = ctk.CTkLabel(runwindow, text=premouse_string, width=runwindow_w)
     premouse_label.grid(row=r + 9, column=0)
     premouse_entry = ctk.CTkEntry(runwindow, textvariable=results["premouse_string"])
     premouse_entry.grid(row=r + 10, column=0)
     # postmouse_num string
-    postmouse_string = (
-        "[C] Define the 'unique task identifier"
-    )
+    postmouse_string = "[C] Define the 'unique task identifier"
     postmouse_label = ctk.CTkLabel(runwindow, text=postmouse_string, width=runwindow_w)
     postmouse_label.grid(row=r + 11, column=0)
     postmouse_entry = ctk.CTkEntry(runwindow, textvariable=results["postmouse_string"])
     postmouse_entry.grid(row=r + 12, column=0)
     # prerun string
-    prerun_string = (
-        "[D] Define the 'unique trial identifier"
-    )
+    prerun_string = "[D] Define the 'unique trial identifier"
     prerun_label = ctk.CTkLabel(runwindow, text=prerun_string, width=runwindow_w)
     prerun_label.grid(row=r + 13, column=0)
     prerun_entry = ctk.CTkEntry(runwindow, textvariable=results["prerun_string"])
     prerun_entry.grid(row=r + 14, column=0)
     # postrun string
-    postrun_string = (
-        "[E] Define the 'unique camera identifier"
-    )
+    postrun_string = "[E] Define the 'unique camera identifier"
     postrun_label = ctk.CTkLabel(runwindow, text=postrun_string, width=runwindow_w)
     postrun_label.grid(row=r + 15, column=0)
     postrun_entry = ctk.CTkEntry(runwindow, textvariable=results["postrun_string"])
     postrun_entry.grid(row=r + 16, column=0)
     # button confirming being done
     # => change value of user_ready in this call
     finishbutton = ctk.CTkButton(
@@ -1098,24 +1207,25 @@
     """Configure the icon - in macos it changes the dock icon, in windows it changes
     all windows titlebar icons (taskbar cannot be changed without converting to exe)
     """
     if platform.system().startswith("Darwin"):
         try:
             from Cocoa import NSApplication, NSImage
         except ImportError:
-            print('Unable to import pyobjc modules')
+            print("Unable to import pyobjc modules")
         else:
             with resources.path("autogaita", "autogaita_icon.icns") as icon_path:
                 ns_application = NSApplication.sharedApplication()
                 logo_ns_image = NSImage.alloc().initByReferencingFile_(str(icon_path))
                 ns_application.setApplicationIconImage_(logo_ns_image)
     elif platform.system().startswith("win"):
         with resources.path("autogaita", "autogaita_icon.ico") as icon_path:
             root.iconbitmap(str(icon_path))
 
+
 def get_results_and_cfg(results, cfg):
     """Before calling analysis, use .get() to extract values from tk-vars"""
     # 1) We make sure to return and use for all "run"-purposes (i.e. everything
     #    that follows this local function) "this_" dicts (stuff is dangerous
     #    otherwise!)
     # 2) I implemented the usage & transformation of FLOAT_&INT_VARS the way I
     #    do here (instead of initialising as (e.g.) tk.IntVar because otherwise
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_group.py` & `autogaita-0.0.6/autogaita/autogaita_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     if cfg["stats_variables"]:  # empty lists are falsey!
         if cfg["do_permtest"]:
             for stats_var in cfg["stats_variables"]:
                 cluster_extent_test(
                     stats_df, g_avg_dfs, g_std_dfs, stats_var, folderinfo, cfg
                 )
 
-    # ..................................  ANOVA  .......................................
+        # ..................................  ANOVA  ...................................
         if cfg["do_anova"]:  # indentation since we check for stats-vars here too!
             for stats_var in cfg["stats_variables"]:
                 twoway_RMANOVA(
                     stats_df, g_avg_dfs, g_std_dfs, stats_var, folderinfo, cfg
                 )
 
     # ..................................  plots  .......................................
@@ -167,15 +167,17 @@
         os.remove(stats_txt_path)
 
     # extracted_cfg_vars: save_to_xls, PCA tests & dont show plots
     cfg = extract_cfg_vars(folderinfo, cfg)
 
     # see if there's a config json file and add to cfg dict
     for g_idx, group_dir in enumerate(group_dirs):
-        with open(os.path.join(group_dir + CONFIG_JSON_FILENAME), "r") as config_json_file:
+        with open(
+            os.path.join(group_dir + CONFIG_JSON_FILENAME), "r"
+        ) as config_json_file:
             config_vars_from_json = json.load(config_json_file)
             for key in config_vars_from_json.keys():
                 # assigning like this ensure all keys are in all jsons across groups
                 if g_idx == 0:
                     cfg[key] = config_vars_from_json[key]
                 else:
                     # sanity check for group-differences in cfg variables!
@@ -276,49 +278,47 @@
         # test that at least 1 folder has valid results for all groups
         if not valid_results_folders:
             no_valid_results_error = (
                 "\n***********\n! ERROR !\n***********\n"
                 + "No valid results folder found for "
                 + group_names[g]
                 + "\nFix & re-run!"
-                )
+            )
             print(no_valid_results_error)
             write_issues_to_textfile(no_valid_results_error, results_dir)
     # assign to our cfg dict after group loop
     cfg["save_to_xls"] = save_to_xls
 
-
     # .........................  test if PCA config is valid  ..........................
     if cfg["PCA_variables"]:  # only test if user wants PCA (ie. selected any features)
         if len(cfg["PCA_variables"]) < cfg["number_of_PCs"]:
             PCA_variable_num = len(cfg["PCA_variables"])
-            PCA_variables_str = '\n'.join(cfg["PCA_variables"])
+            PCA_variables_str = "\n".join(cfg["PCA_variables"])
             PCA_error_message = (
-            "\n***********\n! ERROR !\n***********\n"
-            + "\nPCA Configuration invalid, number of input features cannot exceed "
-            + "number of principal components to compute!\n"
-            + str(PCA_variable_num)
-            + " PCA variables: \n"
-            + PCA_variables_str
-            + "\n & Number of wanted PCs: "
-            + str(cfg["number_of_PCs"])
-            + "\n Fix & re-run!"
+                "\n***********\n! ERROR !\n***********\n"
+                + "\nPCA Configuration invalid, number of input features cannot exceed "
+                + "number of principal components to compute!\n"
+                + str(PCA_variable_num)
+                + " PCA variables: \n"
+                + PCA_variables_str
+                + "\n & Number of wanted PCs: "
+                + str(cfg["number_of_PCs"])
+                + "\n Fix & re-run!"
             )
             write_issues_to_textfile(PCA_error_message, results_dir)
             raise ValueError(PCA_error_message)
         if cfg["number_of_PCs"] < 2:
             print(
                 "\n***********\n! WARNING !\n***********\n"
                 + "Number of principal components of PCA cannot be smaller than 2!"
                 + "\nRunning PCA on 2 components - if you do not want to perform PCA, "
                 + "just don't choose any variables for it."
-                )
+            )
             cfg["number_of_PCs"] = 2  # make sure to update in cfg dict
 
-
     # ..............................  dont show plots  .................................
     # => in group gaita is always dependent on user system
     # !!! THIS DOES NOT PLOT ANYTHING BUT I HAD TO DO IT LIKE THIS OTHERWISE IT CRASHES
     # !!! If users should complain that they dont get figures but they should, it might
     #     be because these lines wrongly determine user to be in non-interactive mode
     #     while they are not!
     # if not hasattr(sys, "ps1") and not sys.flags.interactive:
@@ -455,18 +455,22 @@
     for g, group_name in enumerate(group_names):
         sc_breaks = np.where(pd.isnull(dfs[g][ID_COL]))[0]
         if bin_num == 0:
             bin_num = sc_breaks[0]
         for b in range(1, len(sc_breaks)):
             this_bin_num = sc_breaks[b] - sc_breaks[b - 1] - 1
             if this_bin_num != bin_num:
-                bin_num_error_helper_function(dfs, g, group_names, sc_breaks, results_dir, b)
+                bin_num_error_helper_function(
+                    dfs, g, group_names, sc_breaks, results_dir, b
+                )
         # handle the last step-cycle of the df (it doesn't have a sc_break after it!)
         if (len(dfs[g]) - sc_breaks[-1] - 1) != this_bin_num:
-            bin_num_error_helper_function(dfs, g, group_names, sc_breaks, results_dir, b)
+            bin_num_error_helper_function(
+                dfs, g, group_names, sc_breaks, results_dir, b
+            )
     return bin_num
 
 
 def bin_num_error_helper_function(dfs, g, group_names, sc_breaks, results_dir, b):
     """Handle this error in a separate function for readability"""
     id_col_idx = dfs[g].columns.get_loc(ID_COL)
     message = (
@@ -488,15 +492,15 @@
     PCA_variables = cfg["PCA_variables"]
     stats_variables = cfg["stats_variables"]
     if PCA_variables:
         if not all(variable in df.columns for variable in PCA_variables):
             missing_PCA_variables = [
                 variable for variable in PCA_variables if variable not in df.columns
             ]
-            missing_PCA_variables_str = '\n'.join(missing_PCA_variables)
+            missing_PCA_variables_str = "\n".join(missing_PCA_variables)
             PCA_variable_mismatch_message = (
                 "\n***********\n! ERROR !\n***********\n"
                 + "\nNot all features you asked us to analyse WITH PCA were present in "
                 + "the dataset of:\n"
                 + group_name
                 + "'s "
                 + name
@@ -508,15 +512,15 @@
             write_issues_to_textfile(PCA_variable_mismatch_message, results_dir)
             raise ValueError(PCA_variable_mismatch_message)
     if stats_variables:
         if not all(variable in df.columns for variable in stats_variables):
             missing_stats_variables = [
                 variable for variable in stats_variables if variable not in df.columns
             ]
-            missing_stats_variables_str = '\n'.join(missing_stats_variables)
+            missing_stats_variables_str = "\n".join(missing_stats_variables)
             stats_variable_mismatch_message = (
                 "\n***********\n! ERROR !\n***********\n"
                 + "\nNot all features you asked us to analyse STATISTICALLY were "
                 + "present in the dataset of:\n"
                 + group_name
                 + "'s "
                 + name
@@ -526,15 +530,23 @@
             )
             print(stats_variable_mismatch_message)
             write_issues_to_textfile(stats_variable_mismatch_message, results_dir)
             raise ValueError(stats_variable_mismatch_message)
 
 
 def import_and_combine_dfs(
-    group_df, group_name, group_dir, tracking_software, name, which_df, which_leg, results_dir, cfg
+    group_df,
+    group_name,
+    group_dir,
+    tracking_software,
+    name,
+    which_df,
+    which_leg,
+    results_dir,
+    cfg,
 ):
     """Import one run's df at a time and combine to group-level df"""
     if which_df == "Normalised":
         this_sheet_name = NORM_SHEET_NAME
     elif which_df == "Original":
         this_sheet_name = ORIG_SHEET_NAME
     fullfilepath = os.path.join(group_dir, name, name + " - " + this_sheet_name)
@@ -741,24 +753,24 @@
             this_ID_avg_df[SC_NUM_COL] = SC_num
             this_ID_std_df[SC_NUM_COL] = SC_num
             # SC Percentage column
             this_ID_avg_df[SC_PERCENTAGE_COL] = 0
             sc_percentage_col_idx = this_ID_avg_df.columns.get_loc(SC_PERCENTAGE_COL)
             for i in range(len(this_ID_avg_df)):
                 this_index = this_ID_avg_df.index[i]
-                this_ID_avg_df.iloc[
-                    i, sc_percentage_col_idx
-                ] = one_bin_in_sc_percent + (this_index * one_bin_in_sc_percent)
+                this_ID_avg_df.iloc[i, sc_percentage_col_idx] = (
+                    one_bin_in_sc_percent + (this_index * one_bin_in_sc_percent)
+                )
             this_ID_std_df[SC_PERCENTAGE_COL] = 0
             sc_percentage_col_idx = this_ID_std_df.columns.get_loc(SC_PERCENTAGE_COL)
             for i in range(len(this_ID_std_df)):
                 this_index = this_ID_std_df.index[i]
-                this_ID_std_df.iloc[
-                    i, sc_percentage_col_idx
-                ] = one_bin_in_sc_percent + (this_index * one_bin_in_sc_percent)
+                this_ID_std_df.iloc[i, sc_percentage_col_idx] = (
+                    one_bin_in_sc_percent + (this_index * one_bin_in_sc_percent)
+                )
             # add ID-level avg & std dfs to group-level dfs
             if avg_dfs[g].empty:
                 avg_dfs[g] = this_ID_avg_df
                 std_dfs[g] = this_ID_std_df
             else:
                 avg_dfs[g] = pd.concat([avg_dfs[g], this_ID_avg_df], axis=0)
                 std_dfs[g] = pd.concat([std_dfs[g], this_ID_std_df], axis=0)
@@ -1259,26 +1271,22 @@
     for i in np.where(results_df[CONTRASTS_COL] == contrast)[0]:
         if results_df.iloc[i, ttest_mask_col_idx] == True:
             this_tmass += abs(results_df.iloc[i, ttest_tval_col_idx])  # tval
             this_cluster_size += 1  # cluster size
             this_cluster_indices.append(i)
             # handle the case of results_df ending with a sig. cluster
             if i == max(np.where(results_df[CONTRASTS_COL] == contrast)[0]):
-                results_df.iloc[
-                    this_cluster_indices, tmass_col_idx
-                    ] = this_tmass
+                results_df.iloc[this_cluster_indices, tmass_col_idx] = this_tmass
         else:
             # if p was not significant, assign the previous cluster & reset our vars
             # => note this else also occurs when we keep having nonsig ts but for those
             #    nothing happens... coding it like this might make it a bit slower than
             #    a more sophisticated conditional logic here but the difference should
             #    be minimal so I just keep it as is
-            results_df.iloc[
-                this_cluster_indices, tmass_col_idx
-            ] = this_tmass
+            results_df.iloc[this_cluster_indices, tmass_col_idx] = this_tmass
             this_tmass = 0.0
             this_cluster_size = 0
             this_cluster_indices = []
     # handle case of all ps being significant
     if this_cluster_size == len(np.where(results_df[CONTRASTS_COL] == contrast)[0]):
         results_df.iloc[this_cluster_indices, tmass_col_idx] = this_tmass
     return results_df
@@ -1482,15 +1490,15 @@
     ANOVA_result = run_ANOVA(stats_df, stats_var, cfg)
     # check if sphericity is given to see if p vals have to be GG corrected
     # => even though this is done automatically for mixed anovas, you always get the GG
     #    col in results of rm anovas so we have to test it ourselves and can not (as
     #    done in an earlier version of gaita, have "if GG-col is there")
     sphericity_flag = sphericity(
         stats_df, dv=stats_var, within=SC_PERCENTAGE_COL, subject=ID_COL
-        )[0]
+    )[0]
     if sphericity_flag:  # sphericity is given, no need to correct
         interaction_effect_pval = ANOVA_result["p-unc"][2]
     else:
         interaction_effect_pval = ANOVA_result["p-GG-corr"][2]
     if interaction_effect_pval < 0.05:  # if interaction effect is sig, do multcomps
         multcomp_df = multcompare_SC_Percentages(stats_df, stats_var, folderinfo, cfg)
         save_stats_results_to_text(
@@ -1502,15 +1510,14 @@
     else:  # if interaction effect not sig, inform user that we didn't perform Tukey's!
         nonsig_multcomp_df = pd.DataFrame()
         save_stats_results_to_text(
             nonsig_multcomp_df, stats_var, "non-significant ANOVA", folderinfo, cfg
         )
 
 
-
 def multcompare_SC_Percentages(stats_df, stats_var, folderinfo, cfg):
     """Perform multiple comparison test if the ANOVA's interaction was significant.
     Do a separate multcomp test for each SC % bin."""
 
     # unpack
     group_names = folderinfo["group_names"]
     contrasts = folderinfo["contrasts"]
@@ -1784,15 +1791,17 @@
             figure_file_string = " - Joint y-coord.s over average step cycle"
         elif tracking_software == "Simi":
             ax.set_title(
                 group_name + " - " + which_leg + " Joint Z over average step cycle"
             )
             ax.set_ylabel("Z")
             figure_file_string = " - Joint Z-coord.s over average step cycle"
-        f.savefig(results_dir + group_name + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + group_name + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, group_name + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
     # B - lines = groups & figures = joints
     for j, joint in enumerate(joints):
         f, ax = plt.subplots(1, 1)
@@ -1827,15 +1836,17 @@
             if joint + "Z" in g_avg_dfs[g].columns:
                 title_leg = ""
             else:
                 title_leg = which_leg
             ax.set_title(title_leg + " " + joint + " Z over average step cycle")
             ax.set_ylabel("Z")
             figure_file_string = "- Z-coord.s over average step cycle"
-        f.savefig(results_dir + joint + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + joint + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, joint + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
 
 def plot_angles_by_average_SC(g_avg_dfs, g_std_dfs, folderinfo, cfg):
     """2 - Plot Angles as a function of average SC's percentage"""
@@ -1877,15 +1888,17 @@
         if tracking_software == "DLC":
             ax.set_title(group_name + " - Joint angles over average step cycle")
         elif tracking_software == "Simi":
             ax.set_title(
                 group_name + " - " + which_leg + " joint angles over average step cycle"
             )
         figure_file_string = " - Joint angles over average step cycle"
-        f.savefig(results_dir + group_name + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + group_name + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, group_name + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
     # B - lines = groups & figures = angles
     for a, angle in enumerate(angles["name"]):
         f, ax = plt.subplots(1, 1)
@@ -1913,15 +1926,17 @@
         elif tracking_software == "Simi":
             if angle + "Angle" in g_avg_dfs[g].columns:
                 title_leg = ""
             else:
                 title_leg = which_leg
             ax.set_title(title_leg + " " + angle + " angle over average step cycle")
         figure_file_string = " - angle over average step cycle"
-        f.savefig(results_dir + angle + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + angle + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, angle + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
 
 def plot_x_velocities_by_average_SC(g_avg_dfs, g_std_dfs, folderinfo, cfg):
     """3 - Plot x velocities as a function of average SC's percentage"""
@@ -1973,24 +1988,28 @@
                     "Velocity (x in pixels / "
                     + str(int((1 / sampling_rate) * 1000))
                     + "ms)"
                 )
             ax.set_title(group_name + " - Joint velocities over average step cycle")
         elif tracking_software == "Simi":
             ax.set_ylabel(
-                "Velocity (Y in (your_units) / " + str(int((1 / sampling_rate) * 1000)) + "ms)"
+                "Velocity (Y in (your_units) / "
+                + str(int((1 / sampling_rate) * 1000))
+                + "ms)"
             )
             ax.set_title(
                 group_name
                 + " - "
                 + which_leg
                 + " joint velocities over average step cycle"
             )
         figure_file_string = " - Joint velocities over average step cycle"
-        f.savefig(results_dir + group_name + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + group_name + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, group_name + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
     # B - lines = groups & figures = joints
     for j, joint in enumerate(joints):
         f, ax = plt.subplots(1, 1)
@@ -2025,25 +2044,29 @@
                     "Velocity (x in pixels / "
                     + str(int((1 / sampling_rate) * 1000))
                     + "ms)"
                 )
             ax.set_title(joint + "velocities over average step cycle")
         elif tracking_software == "Simi":
             ax.set_ylabel(
-                "Velocity (Y in (your_units) / " + str(int((1 / sampling_rate) * 1000)) + "ms)"
+                "Velocity (Y in (your_units) / "
+                + str(int((1 / sampling_rate) * 1000))
+                + "ms)"
             )
             if joint + "Velocity" in g_avg_dfs[g].columns:
                 title_leg = ""
             else:
                 title_leg = which_leg
             ax.set_title(
                 title_leg + " " + joint + " velocities over average step cycle"
             )
         figure_file_string = "- Velocities over average step cycle"
-        f.savefig(results_dir + joint + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + joint + figure_file_string + ".png", bbox_inches="tight"
+        )
         if dont_show_plots:
             plt.close(f)
 
 
 def plot_angular_velocities_by_average_SC(g_avg_dfs, g_std_dfs, folderinfo, cfg):
     """4 - Plot angular velocities as a function of average SC's percentage"""
     # unpack
@@ -2089,15 +2112,17 @@
             ax.set_title(
                 group_name
                 + " - "
                 + which_leg
                 + " angular velocities over average step cycle"
             )
         figure_file_string = " - Angular velocities over average step cycle"
-        f.savefig(results_dir + group_name + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + group_name + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, group_name + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
     # B - lines = groups & figures = joints
     for a, angle in enumerate(angles["name"]):
         f, ax = plt.subplots(1, 1)
@@ -2125,17 +2150,24 @@
         if tracking_software == "DLC":
             ax.set_title(angle + " - Angular velocities over average step cycle")
         elif tracking_software == "Simi":
             if angle + "Angle" in g_avg_dfs[g].columns:
                 title_leg = ""
             else:
                 title_leg = which_leg
-            ax.set_title(title_leg + " " + angle + " - Angular velocities over average step cycle")
+            ax.set_title(
+                title_leg
+                + " "
+                + angle
+                + " - Angular velocities over average step cycle"
+            )
         figure_file_string = " - Angular Velocities over average step cycle"
-        f.savefig(results_dir + angle + figure_file_string + ".png", bbox_inches="tight")
+        f.savefig(
+            results_dir + angle + figure_file_string + ".png", bbox_inches="tight"
+        )
         save_as_svg(f, results_dir, angle + figure_file_string)
         if dont_show_plots:
             plt.close(f)
 
 
 def save_as_svg(figure, results_dir, figure_file_string):
     """Save figures as svgs to separate subfolder"""
@@ -2209,15 +2241,15 @@
         start_string += (
             "\nCluster-extent permutation test with "
             + str(cfg["permutation_number"])
             + " permutations"
         )
         start_string += (
             "\nAlpha Level of " + str(cfg["stats_threshold"] * 100) + "%\n\n"
-            )
+        )
     else:
         start_string += "\n\nNo stats wanted!\n\n"
 
     # done - print
     print(start_string)
 
 
@@ -2298,20 +2330,26 @@
                 )
         else:
             clusters = extract_all_clusters(results_df, contrast)
         # write message
         if len(clusters) == 0:  # no sig clusters were found!
             if "non-significant" in which_test:
                 message = (
-                    message + "\n\nContrast: " + contrast + " - interaction effect " +
-                    "not significant. Tukey's test was not performed!"
-                    )
+                    message
+                    + "\n\nContrast: "
+                    + contrast
+                    + " - interaction effect "
+                    + "not significant. Tukey's test was not performed!"
+                )
             else:
                 message = (
-                    message + "\n\nContrast: " + contrast + " - No significant clusters"
+                    message
+                    + "\n\nContrast: "
+                    + contrast
+                    + " - No significant clusters"
                     + "!"
                 )
         else:
             rounded_sc_percentages = np.linspace(0, 100, bin_num).round(2)
             message = (
                 message
                 + "\n\nContrast: "
@@ -2328,41 +2366,41 @@
                     + "%"
                     + ", p values:\n\n"
                 )
                 # add pvals to message
                 # => handle ANOVA and perm test differently since results_df different
                 if "ANOVA" in which_test:
                     # important to include cluster-end bin here thus cluster[1]+1!
-                    for i in range(cluster[0], cluster[1]+1):
+                    for i in range(cluster[0], cluster[1] + 1):
                         message = (
                             message
                             + "\n"
                             + str(rounded_sc_percentages[i])
                             + "% - p = "
                             + str(round(results_df.loc[i, contrast], 4))
-                            )
+                        )
                 else:
                     # extract subset df of only this contrast because cluster variables
                     # idxs values correspond to 0:bin_num and results_df of perm test
                     # (this is different for anovas) has 0:bin_num*contrast_number!
                     this_contrast_results_df = results_df[
                         results_df[CONTRASTS_COL] == contrast
-                        ]
+                    ]
                     cluster_p_colidx = this_contrast_results_df.columns.get_loc(
                         CLUSTER_P_COL
-                        )
+                    )
                     # also note that we only use cluster[0] to retrieve cluster's pval
                     # since the pval is constant across the whole cluster always
                     message = (
                         message
                         + "Cluster p value = "
                         + str(
                             this_contrast_results_df.iloc[cluster[0], cluster_p_colidx]
-                            )
                         )
+                    )
 
     # message end
     message = (
         message
         + "\n\n***********************************************************************"
         + "***\n\n"
     )
@@ -2378,9 +2416,9 @@
 if __name__ == "__main__":
     group_info_message = (
         "\n*************\nnot like this\n*************\n"
         + "You are trying to execute autogaita.group as a script, but that is not "
         + "possible.\nIf you prefer a non-GUI approach, please either: "
         + "\n1. Call this as a function, i.e. autogaita.group(folderinfo, cfg)"
         + "\n2. Use the dlc or simirun scripts in the batchrun_scripts folder"
-        )
+    )
     print(group_info_message)
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_group_gui.py` & `autogaita-0.0.6/autogaita/autogaita_group_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,20 @@
         font=("Britannic Bold", HEADER_FONT_SIZE),
         command=lambda: (
             mainwindow(root, group_number, root_dimensions),
             root.withdraw(),
         ),
     )
     continue_button.grid(
-        row=3, column=0, columnspan=MAX_GROUP_NUM - 1, pady=23, padx=30, sticky="nsew"
+        row=3,
+        column=0,
+        columnspan=MAX_GROUP_NUM - 1,
+        pady=23,
+        padx=30,
+        sticky="nsew",
     )
     root.grid_rowconfigure(3, weight=1)
     num_cols = root.grid_size()[0]  # maximise cols
     for c in range(num_cols):
         root.grid_columnconfigure(c, weight=1)
 
     root.mainloop()
@@ -216,15 +221,16 @@
         group_dirs_entries = []
         row_counter = 3  # track row idxs for loop-widget-creation
         for g in range(group_number):
             this_groups_number = g + 1
             # group names - labels
             group_names_labels.append(
                 ctk.CTkLabel(
-                    mainwindow, text="Group " + str(this_groups_number) + "'s Name"
+                    mainwindow,
+                    text="Group " + str(this_groups_number) + "'s Name",
                 )
             )
             group_names_labels[-1].grid(row=row_counter, column=0)
             # group names - entries
             group_names_entries.append(
                 ctk.CTkEntry(mainwindow, textvariable=group_names[g])
             )
@@ -334,15 +340,20 @@
         )
         definefeatures_button = ctk.CTkButton(
             mainwindow,
             text="I am ready - define features!",
             fg_color=FG_COLOR,
             hover_color=HOVER_COLOR,
             command=lambda: definefeatures_window(
-                mainwindow, group_names, group_dirs, results_dir, root, root_dimensions
+                mainwindow,
+                group_names,
+                group_dirs,
+                results_dir,
+                root,
+                root_dimensions,
             ),
         )
         definefeatures_button.grid(
             row=last_group_row + 6, column=1, sticky="nsew", pady=15, padx=30
         )
 
         # maximise widgets to fit fullscreen
@@ -428,21 +439,22 @@
 
 
 def definefeatures_window(
     mainwindow, group_names, group_dirs, results_dir, root, root_dimensions
 ):
     """Build define features window"""
 
-    # nested function (called by run-button): extract boolean checkbox vars and store in
-    # cfg dicts!
+    # nested function (called by run-button): extract boolean checkbox vars and store
+    # in cfg dicts!
     def get_selected_variables():
         for key in LIST_VARS:
             # this list comprehension extracts all strings (keys) of checkbox_vars'
             # given sub-dict (either stats_variables or PCA_variables) and stores it to
-            # the correct key of our cfg dict if it was checked (i.e., if var.get() is True!)
+            # the correct key of our cfg dict if it was checked (i.e., if var.get() is
+            # True!)
             cfg[key] = [
                 string for string, var in checkbox_vars[key].items() if var.get()
             ]
 
     # .................  EXTRACT FEATURES FROM A NORMALISED SC XLS  ....................
     # => First read the xls as df, extract columns that are meaningful after
     #    normalisation, or throw errors if we don't manage to do so
@@ -491,15 +503,15 @@
     else:
         error_string = "Unable to find any Normalised SC sheet at " + some_groups_dir
         tk.messagebox.showerror(title="Group Directory Error!", message=error_string)
         print(error_string)
         print("Analysis did not run due to above errors. Fix them & re-try!")
         return
 
-    # .......................  BUILD THE TOPLEVEL WINDOW  ..............................
+    # .......................  BUILD THE TOPLEVEL WINDOW  .............................
     # build window
     featureswindow = ctk.CTkToplevel(mainwindow)
     featureswindow.title("Add Features & Run!")
     featureswindow.geometry(f"{screen_width}x{screen_height}+0+0")
     fix_window_after_its_creation(featureswindow)
     # grid prep
     scrollbar_rows = 5  # scrollbar rowspan (in featureswindow)
@@ -554,15 +566,17 @@
                 fg_color=FG_COLOR,
                 hover_color=HOVER_COLOR,
                 font=("Britannic Bold", HEADER_FONT_SIZE - 5),
             )
             this_checkbox.grid(row=row_counter, column=col_counter, sticky="nsew")
             # if user doesn't want to do stats, dont have them choose features
             if frame == stats_frame:
-                if (cfg["do_permtest"].get() is False) & (cfg["do_anova"].get() is False):
+                if (cfg["do_permtest"].get() is False) & (
+                    cfg["do_anova"].get() is False
+                ):
                     this_checkbox.configure(state="disabled")
             row_counter += 1
             # # CARE - the -1 is important here since indexing starts at 0 and grid_nrows
             # # is like len() kinda
             if row_counter == scrollbar_grid_nrows:  # not nrows-1 because we start @ 1
                 row_counter = 1  # index rows at 1 for the top otherwise it breaks
                 col_counter += 1
@@ -607,15 +621,20 @@
     run_button = ctk.CTkButton(
         featureswindow,
         text="I am ready - run analysis!",
         fg_color=FG_COLOR,
         hover_color=HOVER_COLOR,
         command=lambda: (
             build_donewindow(
-                group_names, group_dirs, results_dir, root, mainwindow, featureswindow
+                group_names,
+                group_dirs,
+                results_dir,
+                root,
+                mainwindow,
+                featureswindow,
             ),
             get_selected_variables(),
         ),
     )
     run_button.grid(row=4 + scrollbar_rows, column=1, sticky="nsew", pady=40, padx=40)
 
     # maximise widgets to fit fullscreen
@@ -864,14 +883,15 @@
     #         done_message = (
     #             "Your run has finished execution! You can find your results in the "
     #             + "group directory you provided and are able to run further runs if "
     #             + "desired.")
     #         tk.messagebox(title="Finished :)", message=done_message)
     #         dummy_number = 0  # so we exit the while loop
 
+
 # %%...............  LOCAL FUNCTION(S) #6 - VARIOUS HELPER FUNCTIONS  ..................
 
 
 def change_ANOVA_buttons_state(ANOVA_buttons, cfg):
     """Change the state of ANOVA radio button widgets based on whether user wants
     to perform an ANOVA or not.
     """
@@ -905,20 +925,21 @@
     """Configure the icon - in macos it changes the dock icon, in windows it changes
     all windows titlebar icons (taskbar cannot be changed without converting to exe)
     """
     if platform.system().startswith("Darwin"):
         try:
             from Cocoa import NSApplication, NSImage
         except ImportError:
-            print('Unable to import pyobjc modules')
+            print("Unable to import pyobjc modules")
         else:
             with resources.path("autogaita", "autogaita_icon.icns") as icon_path:
                 ns_application = NSApplication.sharedApplication()
                 logo_ns_image = NSImage.alloc().initByReferencingFile_(str(icon_path))
                 ns_application.setApplicationIconImage_(logo_ns_image)
     elif platform.system().startswith("win"):
         with resources.path("autogaita", "autogaita_icon.ico") as icon_path:
             root.iconbitmap(str(icon_path))
 
+
 # %% what happens if we hit run
 if __name__ == "__main__":
     group_gui()
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_icon.icns` & `autogaita-0.0.6/autogaita/autogaita_icon.icns`

 * *Files identical despite different names*

### Comparing `autogaita-0.0.5/autogaita/autogaita_icon.ico` & `autogaita-0.0.6/autogaita/autogaita_icon.ico`

 * *Files identical despite different names*

### Comparing `autogaita-0.0.5/autogaita/autogaita_logo.png` & `autogaita-0.0.6/autogaita/autogaita_logo.png`

 * *Files identical despite different names*

### Comparing `autogaita-0.0.5/autogaita/autogaita_simi.py` & `autogaita-0.0.6/autogaita/autogaita_simi.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,24 @@
 # general
 LEGS = ["left", "right"]
 LEGS_COLFORMAT = [", left ", ", right "]
 OUTPUTS = LEGS + ["both"]
 ISSUES_TXT_FILENAME = "Issues.txt"  # filename to which we write issues-info
 CONFIG_JSON_FILENAME = "config.json"  # filename to which we write cfg-infos
 # sc extraction
-SCXLS_SUBJCOLS = ["Participant", "participant", "Animal", "animal", "Subject", "subject", "ID", "id"]  # SC XLS info
+SCXLS_SUBJCOLS = [
+    "Participant",
+    "participant",
+    "Animal",
+    "animal",
+    "Subject",
+    "subject",
+    "ID",
+    "id",
+]  # SC XLS info
 SCXLS_LEGCOLS = ["Leg", "leg", "Legs", "legs", "Side", "side"]
 SCXLS_RUNCOLS = ["Run", "run", "Runs", "runs", "Trial", "trial", "Trials", "trials"]
 SCXLS_SCCOLS = ["SC Number", "SC number", "sc number", "SC Num", "sc num", "SC num"]
 SWINGSTART_COL = "Swing (ti)"
 STANCEEND_COL = "Stance (te)"
 # simulate walking direction being left to right
 SEARCH_WIN_TURN_TIME = 500  # 5 seconds
@@ -47,38 +56,38 @@
 
 # %%
 # ......................................................................................
 # ........................  an important note for yourself  ............................
 # ......................................................................................
 # Please read this (& check_data_column_names!) when you are confused about col-names.
 # It's a bit tricky in this code, see comments & doc about this issue in:
-    # 1. check_and_fix_cfg_strings (why am I here, read the others)
-    # 2. check_data_column_names (read me first)
-    # 3. add_features (then me)
-    # 4. plot_results (me if you really have to)
+# 1. check_and_fix_cfg_strings (why am I here, read the others)
+# 2. check_data_column_names (read me first)
+# 3. add_features (then me)
+# 4. plot_results (me if you really have to)
 # => mainly (from 2.):
-    # Bodyside-specific colnames have to end WITHOUT a space (because we concat
-    # "name" + ", leg " + "Z" - so leg ends with a space)
-    # Bodyside-nonspecific colnames have to end WITH a space (because we concat "name "
-    # + "Z" so name has to end with a space)
+# Bodyside-specific colnames have to end WITHOUT a space (because we concat
+# "name" + ", leg " + "Z" - so leg ends with a space)
+# Bodyside-nonspecific colnames have to end WITH a space (because we concat "name "
+# + "Z" so name has to end with a space)
 # ......................................................................................
 
 
 # %% main program
 
 
 def simi(info, folderinfo, cfg):
     """Runs the main program for a given subject's run
 
     Procedure
     ---------
     1) import & preparation
     2) step cycle extraction
     3) z-normalisation, y-flipping & feature computation for individual step cycles
-    4) step cycle normalisation, dataframe creation & XLS-exportation
+    4) step cycle normalisaion, dataframe creation & XLS-exportation
     5) plots
     """
 
     # ...............................  preparation  ....................................
     data, global_Y_max = some_prep(info, folderinfo, cfg)
     if (data is None) & (global_Y_max is None):
         return
@@ -101,15 +110,14 @@
 
 # %% local functions 1 - preparation
 
 
 # ................................  main function  .....................................
 def some_prep(info, folderinfo, cfg):
     """Preparation of the data for later analyses"""
-
     # ............................  unpack stuff  ......................................
     name = info["name"]
     results_dir = info["results_dir"]
     postname_string = folderinfo["postname_string"]
     sampling_rate = cfg["sampling_rate"]
     normalise_height_at_SC_level = cfg["normalise_height_at_SC_level"]
 
@@ -132,17 +140,15 @@
                 + "!\n Results will only be updated if filenames match!"
             )
             print(unable_to_rm_resdir_error)
             write_issues_to_textfile(unable_to_rm_resdir_error, info)
     else:
         move_data_to_folders(info, folderinfo)
 
-
-
-     # .......  initialise Issues.txt & quick check for file existence  .................
+    # .......  initialise Issues.txt & quick check for file existence  .................
     issue_txt_path = os.path.join(results_dir, ISSUES_TXT_FILENAME)
     if os.path.exists(issue_txt_path):
         os.remove(issue_txt_path)
     # read data
     # => note that this catches xls and xlsx files. can do this since we previously
     #    handle cases of both being @ root_dir in move_data_to_folders function
     # => using empty data df & empty string for error handling
@@ -160,15 +166,15 @@
             else:
                 data_duplicate_error = (
                     "\n******************\n! CRITICAL ERROR !\n******************\n"
                     + "Two DATA xls-files found for "
                     + name
                     + "!\nPlease ensure your root directory only has one "
                     + "datafile per ID"
-                    )
+                )
 
     # ............................  import data  .......................................
     import_error_message = ""  # prep stuff for error handling
     if data_duplicate_error:
         import_error_message += data_duplicate_error
     if data.empty:
         import_error_message += (
@@ -372,15 +378,15 @@
     # add direction_joint - used to determine gait direction
     if not joints:  # no valid string after above cleaning
         no_joint_message = (
             "\n******************\n! CRITICAL ERROR !\n******************\n"
             + "After testing your joint names, no valid joint was left to "
             + "perform gait direction checks on.\nPlease make sure that at least one "
             + "joint is provided & try again!"
-            )
+        )
         write_issues_to_textfile(no_joint_message, info)
         print(no_joint_message)
         return (None, None)  # returning tuple bc. some_prep returns 2 variables
     if joints[0] + "Y" in data.columns:
         cfg["direction_joint"] = joints[0] + "Y"
     else:
         cfg["direction_joint"] = joints[0] + LEGS_COLFORMAT[0] + "Y"
@@ -416,61 +422,77 @@
     # easy checks: lists
     if type(string_variable) is list:
         string_variable = [string for string in string_variable if string]
         # note that below local func. DOES NOT CLEAN the list - it only corrects space
         # characters and returns invalid_idxs that we'll use next to clean the list
         string_variable, invalid_joint_idxs = check_data_column_names(
             data, string_variable
-            )
+        )
         # if user gave us joints we didnt find, write, print & save error message
         if invalid_joint_idxs:  # if none found, func returns an empty list (falsey!)
             # backup dirty variable
             dirty_string_variable = string_variable
             # now clean the list
             string_variable = [
-                item for i, item in enumerate(string_variable) if i not in invalid_joint_idxs
-                ]
+                item
+                for i, item in enumerate(string_variable)
+                if i not in invalid_joint_idxs
+            ]
             # now print & save erroneous & remaining joints
             joint_error = (
-            "\n***********\n! WARNING !\n***********\n"
-            + "\nYou entered joint-names that are not included in your dataset:"
+                "\n***********\n! WARNING !\n***********\n"
+                + "\nYou entered joint-names that are not included in your dataset:"
             )
             for idx in invalid_joint_idxs:
                 joint_error += "\n" + dirty_string_variable[idx]
             joint_error += "\n\nWe removed these and will analyse the remaining ones:"
             for string in string_variable:
                 joint_error += "\n" + string
             joint_error += (
                 "\n\nNote that capitalisation matters."
-                + "\nIf you are running a group analysis, we'll use this updated cfg "
+                + "\nIf you are running a batch analysis, we'll use this updated cfg "
                 + "throughout.\nCheck out the config.json file for the full cfg used."
-                )
+            )
             print(joint_error)
             write_issues_to_textfile(joint_error, info)
 
     # things are more involved for angle dicts
     elif type(string_variable) is dict:
+        # 1) test if the lists of all keys are equally long, if not throw out last idxs
+        key_lengths = [len(string_variable[key]) for key in string_variable.keys()]
+        if not all(key_length == key_lengths[0] for key_length in key_lengths):
+            min_length = min(key_lengths)
+            for key in string_variable:  # remove invalid idxs
+                string_variable[key] = string_variable[key][:min_length]
+            key_length_mismatch_message = (  # inform user
+                "\n***********\n! WARNING !\n***********\n"
+                + "\nLength-mismatch in angle configuration!"
+                + "\nCheck angles' name/upper/lower-joint entries."
+                + "\nOnly processing first "
+                + str(min_length)
+                + " entries."
+            )
+            print(key_length_mismatch_message)
+            write_issues_to_textfile(key_length_mismatch_message, info)
+        # 2) check if all strings in the angle dict are valid columns
         invalid_angletrio_message = ""
         invalid_idxs = []  # these idxs hold across the 3 keys of our angles-dict
         for key in string_variable:
             this_keys_missing_strings = ""
             string_variable[key], this_keys_invalid_idxs = check_data_column_names(
                 data, string_variable[key]
-                )
+            )
             if this_keys_invalid_idxs:  # if none found this is an empty list (falsey!)
                 invalid_idxs.append(this_keys_invalid_idxs)
                 if not this_keys_missing_strings:  # first occurance
                     this_keys_missing_strings += "\nAngle's " + key + " key: "
                 for idx in this_keys_invalid_idxs:
                     this_keys_missing_strings += (
-                        string_variable[key][idx]
-                        + " (#"
-                        + str(idx+1)
-                        + ") / "
-                        )
+                        string_variable[key][idx] + " (#" + str(idx + 1) + ") / "
+                    )
                 # string concat outside of idx-forloop above please
                 invalid_angletrio_message += this_keys_missing_strings
         # if we have to remove idxs from all keys of our angles dict
         if invalid_angletrio_message:
             # print and save
             angles_warning = (
                 "\n***********\n! WARNING !\n***********\n"
@@ -501,15 +523,15 @@
                     "\nLower Joint: " + string_variable["lower_joint"][i]
                 )
                 clean_angles_message += (
                     "\nUpper Joint: " + string_variable["upper_joint"][i]
                 )
             clean_angles_message += (
                 "\n\nNote that capitalisation matters."
-                + "\nIf you are running a group analysis, we'll use this updated cfg "
+                + "\nIf you are running a batch analysis, we'll use this updated cfg "
                 + "throughout\nCheck out the config.json file for the full cfg used."
             )
             print(clean_angles_message)
             write_issues_to_textfile(clean_angles_message, info)
 
     return string_variable
 
@@ -573,16 +595,15 @@
         SCdf = pd.read_excel(os.path.join(root_dir, sctable_filename))
     elif os.path.exists(os.path.join(root_dir, sctable_filename) + ".xlsx"):
         SCdf = pd.read_excel(os.path.join(root_dir, sctable_filename) + ".xlsx")
     elif os.path.exists(os.path.join(root_dir, sctable_filename) + ".xls"):
         SCdf = pd.read_excel(os.path.join(root_dir, sctable_filename) + ".xls")
     else:
         no_sc_table_message = (
-            "I did not find a step-cycle latency table. "
-            + "sctable_filename has to be @ root_dir"
+            "No Annotation Table found! sctable_filename has to be @ root_dir"
         )
         raise Exception(no_sc_table_message)
 
     # extract & return all_cycles
     all_cycles = {"left": [], "right": []}
     for legname in LEGS:
         all_cycles[legname] = read_SC_info(data, SCdf, info, legname, cfg)
@@ -594,27 +615,34 @@
     """Read table, and create a list of start/end indices of a leg's SCs"""
     # ...............................  preparation  ....................................
     # unpack
     name = info["name"]
     sampling_rate = cfg["sampling_rate"]
 
     # very first sanity check - see if table columns are labelled correctly
-    valid_col_flags = [False, False, False, False]  # add some flexibility to allow user typos
+    valid_col_flags = [
+        False,
+        False,
+        False,
+        False,
+    ]  # for user typos
     header_columns = ["", "", "", ""]
-    for h, header in enumerate([SCXLS_SUBJCOLS, SCXLS_LEGCOLS, SCXLS_RUNCOLS, SCXLS_SCCOLS]):
+    for h, header in enumerate(
+        [SCXLS_SUBJCOLS, SCXLS_LEGCOLS, SCXLS_RUNCOLS, SCXLS_SCCOLS]
+    ):
         for header_col in header:
             if header_col in SCdf.columns:
                 valid_col_flags[h] = True
                 header_columns[h] = header_col
                 break
     if not all(valid_col_flags):
         this_message = (
             "\n******************\n! CRITICAL ERROR !"
             + "\n******************\n"
-            + "Latency XLS Column names are wrong!\n"
+            + "Annotation Table Column names are wrong!\n"
             + "Check Instructions!"
         )
         print(this_message)
         write_issues_to_textfile(this_message, info)
         return
     # some prep
     leg_col = SCdf.columns.get_loc(header_columns[1])  # INDEXING! (see list above)
@@ -622,29 +650,29 @@
     sc_col = SCdf.columns.get_loc(header_columns[3])
     # first find the rows of this leg
     # a. find overall start row of this subject
     start_row = SCdf.index[SCdf[header_columns[0]] == name]
     if start_row.empty:
         this_message = (
             "\n******************\n! CRITICAL ERROR !\n******************\n"
-            + "\nNo SC latency information found for ID: "
+            + "\nNo timestamp information found for ID: "
             + name
-            + "\nCheck your SC Latency Table & try again!"
+            + "\nCheck your Annotation Table & try again!"
         )
         print(this_message)
         write_issues_to_textfile(this_message, info)
         return
     # b. check if this subjects ID was found more than once, if so - stop!
     if len(start_row) > 1:
         this_message = (
             "\n******************\n! CRITICAL ERROR !\n******************\n"
             + "\nID "
             + name
             + " was found more than once in ID column!"
-            + "\nCheck your SC Latency Table & try again!"
+            + "\nCheck your Annotation Table & try again!"
         )
         print(this_message)
         write_issues_to_textfile(this_message, info)
         return
     # c. find start row of current leg (whileloop works for both legs)
     while SCdf.iloc[start_row, leg_col].values[0] != legname:
         start_row += 1
@@ -658,15 +686,15 @@
         if not np.isnan(SCdf.iloc[end_row, leg_col].values[0]):
             this_message = (
                 "\n******************\n! CRITICAL ERROR !\n******************\n"
                 + "\nID: "
                 + name
                 + ", Leg: "
                 + legname
-                + "\nRun & Leg columns of SC "
+                + "\nRun & Leg columns of Annotation "
                 + "Table seem wrong! \nYou need to have an "
                 + "empty row before each new leg or subject!"
                 + "\nCheck your table & make sure that it "
                 + "matches our template."
             )
             print(this_message)
             write_issues_to_textfile(this_message, info)
@@ -1183,15 +1211,14 @@
         elif angle + legname + "Y" in step.columns:
             this_colname = angle + legname + "Angle"
         step[this_colname] = this_angle
     return step
 
 
 def compute_angle(joint_angle, joint2, joint3):
-
     """Compute a given angle at a joint & a given timepoint"""
     # Get vectors between the joints
     v1 = (joint_angle[0] - joint2[0], joint_angle[1] - joint2[1])
     v2 = (joint_angle[0] - joint3[0], joint_angle[1] - joint3[1])
     # dot product, magnitude of vectors, angle in radians & convert 2 degrees
     dot_product = v1[0] * v2[0] + v1[1] * v2[1]
     mag_v1 = math.sqrt(v1[0] ** 2 + v1[1] ** 2)
@@ -1234,15 +1261,15 @@
             legname = ""
         else:
             legname = original_legname
         angle_colname = angle + legname + "Angle"
         step[angle_colname + " Velocity"] = 0.0  # spaces in colnames here!
         step.loc[:, angle_colname + " Velocity"] = np.gradient(
             step.loc[:, angle_colname]
-            )
+        )
         if angular_acceleration:
             step[angle_colname + " Acceleration"] = 0.0
             step.loc[:, angle_colname + " Acceleration"] = np.gradient(
                 step.loc[:, angle_colname + " Velocity"]
             )
     return step
 
@@ -1469,14 +1496,15 @@
 #    might not be bodyside-specific, the data dfs (e.g. all_steps_data) contain
 #    different values based on the leg that performed the step-cycles
 #
 # Only use extract_feature_column when you index using .iloc afterwards (don't be
 # surprised that we don't use this local func everywhere, since the first couple of
 # plotting functions extract values using .loc!)
 
+
 # ................................  master function  ...................................
 def plot_results(results, all_cycles, info, cfg):
     """Plot various results"""
 
     # unpack
     angles = cfg["angles"]
     y_acceleration = cfg["y_acceleration"]
@@ -1503,15 +1531,15 @@
         # .................  4 - average 5-joints' y over SC percentage  ...............
         plot_joint_z_by_average_SC(legname, average_data, std_data, sc_num, info, cfg)
 
         # ...................  5 - average angles over SC percentage  ..................
         if angles["name"]:
             plot_angles_by_average_SC(
                 legname, average_data, std_data, sc_num, info, cfg
-                )
+            )
 
         # .............  6 - average y velocities over SC percentage   .................
         plot_y_velocities_by_average_SC(
             legname, average_data, std_data, sc_num, info, cfg
         )
 
         # ..........  7 - average angular velocities over SC percentage  ...............
@@ -1656,15 +1684,15 @@
             )
             # check for bodyside-specificity
             if angle + "Angle" in all_steps_data.columns:
                 angle_col_string = angle + "Angle"
             else:
                 angle_col_string = transform_joint_and_leg_to_colname(
                     angle, legname, "Angle"
-                    )
+                )
             for s in range(sc_num):
                 this_time = all_steps_data.loc[
                     run_cycles[s][0] : run_cycles[s][1], DF_TIME_COL
                 ]
                 this_angle = all_steps_data.loc[
                     run_cycles[s][0] : run_cycles[s][1], angle_col_string
                 ]
@@ -1742,18 +1770,18 @@
                     # check for bodyside-specificity
                     if joint + "Y" in all_steps_data.columns:
                         y_col_string = joint + "Y"
                         z_col_string = joint + "Z"
                     else:
                         y_col_string = transform_joint_and_leg_to_colname(
                             joint, legname, "Y"
-                            )
+                        )
                         z_col_string = transform_joint_and_leg_to_colname(
                             joint, legname, "Z"
-                            )
+                        )
                     this_ys.append(all_steps_data.loc[i, y_col_string])
                     this_zs.append(all_steps_data.loc[i, z_col_string])
                 if i == range(cycle[0], cycle[1] + 1)[0]:
                     try:
                         ax[r].plot(
                             this_ys,
                             this_zs,
@@ -2108,9 +2136,9 @@
 if __name__ == "__main__":
     simi_info_message = (
         "\n*************\nnot like this\n*************\n"
         + "You are trying to execute autogaita.simi as a script, but that is not "
         + "possible.\nIf you prefer a non-GUI approach, please either: "
         + "\n1. Call this as a function, i.e. autogaita.simi(info, folderinfo, cfg)"
         + "\n2. Use the single or multirun scripts in the batchrun_scripts folder"
-        )
+    )
     print(simi_info_message)
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_simi_gui.py` & `autogaita-0.0.6/autogaita/autogaita_simi_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,15 @@
     cfg["angular_acceleration"] = tk.BooleanVar(root, True)
     cfg["bin_num"] = tk.StringVar(root, "25")
     cfg["plot_joint_number"] = tk.StringVar(root, "3")
     cfg["plot_SE"] = tk.BooleanVar(root, False)
     cfg["normalise_height_at_SC_level"] = tk.BooleanVar(root, True)
     results = {}  # local results variable
     results["name"] = tk.StringVar(root, "")
-    results["root_dir"] = tk.StringVar(
-        root, ""
-    )
+    results["root_dir"] = tk.StringVar(root, "")
     results["sctable_filename"] = tk.StringVar(root, "")
     results["postname_flag"] = tk.BooleanVar(root, False)
     results["postname_string"] = tk.StringVar(root, "")
     # joint columns
     default_joints = ["Midfoot", "Ankle ", "Knee ", "Hip ", "Pelvis "]
     cfg["joints"] = []
     for joint in default_joints:
@@ -195,15 +193,15 @@
     SCXLS_label = ctk.CTkLabel(root, text=SCXLS_string)
     SCXLS_label.grid(row=3, column=1)
     SCXLS_entry = ctk.CTkEntry(root, textvariable=results["sctable_filename"])
     SCXLS_entry.grid(row=4, column=1)
     # sampling rate
     samprate_label = ctk.CTkLabel(
         root, text="Insert sampling rate of videos (frames/second)"
-        )
+    )
     samprate_label.grid(row=5, column=1)
     samprate_entry = ctk.CTkEntry(root, textvariable=cfg["sampling_rate"])
     samprate_entry.grid(row=6, column=1)
     # single video checkbox
     singlevideo_string = "Do you want to only analyse one dataset?"
     singlevideo_checkbox = ctk.CTkCheckBox(
         root,
@@ -318,15 +316,17 @@
     column_info_button = ctk.CTkButton(
         root,
         text=column_info_string,
         fg_color=FG_COLOR,
         hover_color=HOVER_COLOR,
         command=lambda: build_column_info_window(root, cfg, root_dimensions),
     )
-    column_info_button.grid(row=15, column=1, sticky="nsew", rowspan=2, padx=10, pady=10)
+    column_info_button.grid(
+        row=15, column=1, sticky="nsew", rowspan=2, padx=10, pady=10
+    )
     # .........................  run and done section  .................................
     # run button
     runheader_label = ctk.CTkLabel(
         root,
         text="Run Analysis",
         width=w,
         fg_color=FG_COLOR,
@@ -354,14 +354,15 @@
 
     # maximise widgets
     maximise_widgets(root)
 
     # main loop
     root.mainloop()
 
+
 # %%..............  LOCAL FUNCTION(S) #1 - BUILD COLUMN INFO WINDOW  ...................
 def build_column_info_window(root, cfg, root_dimensions):
     """Build a window allowing users to configure custom column names if required"""
     columnwindow = ctk.CTkToplevel(root)
     columnwindow.geometry("%dx%d+%d+%d" % root_dimensions)
     columnwindow.title("Custom column names & features")
     fix_window_after_its_creation(columnwindow)
@@ -413,31 +414,31 @@
         fg_color=FG_COLOR,
         text_color=HEADER_TXT_COLOR,
         font=("Britannic Bold", HEADER_FONT_SIZE),
     )
     joint_label.grid(row=0, column=joint_column, sticky="nsew", pady=(0, 5))
     # initialise scrollable frame for hindlimb
     joint_frame = ctk.CTkScrollableFrame(columnwindow)
-    joint_frame.grid(
-        row=1, column=joint_column, rowspan=scrollable_rows, sticky="nsew"
-    )
+    joint_frame.grid(row=1, column=joint_column, rowspan=scrollable_rows, sticky="nsew")
     # initialise labels & entries with hind limb defaults
     initialise_labels_and_entries(joint_frame, "joints", "Joint ")
     # add joint button
     add_joint_button = ctk.CTkButton(
         columnwindow,
         text="Add joint",
         fg_color=FG_COLOR,
         hover_color=HOVER_COLOR,
-        command=lambda: add_joint(
-            joint_frame, "joints"
-        ),  # 2nd input = cfg's key
+        command=lambda: add_joint(joint_frame, "joints"),  # 2nd input = cfg's key
     )
     add_joint_button.grid(
-        row=2 + scrollable_rows, column=joint_column, sticky="nsew", padx=5, pady=(10, 5)
+        row=2 + scrollable_rows,
+        column=joint_column,
+        sticky="nsew",
+        padx=5,
+        pady=(10, 5),
     )
 
     # .........  Column 1: angle names/joint-definitions & done button  ................
     angle_column = 1
     # header label
     angle_label = ctk.CTkLabel(
         columnwindow,
@@ -531,19 +532,17 @@
         joint_entries[j].grid(row=row_counter, column=column_number)
         row_counter += 1
     # maximise columns
     for c in range(window.grid_size()[0]):
         window.grid_columnconfigure(c, weight=1)
 
 
-
-
 # %%..................  LOCAL FUNCTION(S) #2 - BUILD DONE WINDOW  ......................
 def build_donewindow(results, root, root_dimensions):
-    """Build done window informing people that they shouldn't touch the program"""
+    """Build done window informing people"""
 
     # .........................................................................
     # .............. IMPORTANT - GET VARS & CHECK USER-INPUT ..................
     # .........................................................................
     # ==> Extract "this" results & cfg info IMMEDIATELY BEFORE running analysis
     #     (i.e., before providing donewindow)
     # ==> get_results_and_cfg checks whether the numerical vars (see
@@ -631,36 +630,38 @@
 def analyse_single_run(this_runs_results, this_runs_cfg):
     """Prepare for one execution of autogaita_simi & execute"""
     # prepare
     this_info = {}  # info dict: run-specific info
     this_info["name"] = this_runs_results["name"]
     this_folderinfo = prepare_folderinfo(this_runs_results)
     if this_folderinfo is None:
-        error_msg = ("No directory found at: " + this_runs_results["root_dir"] + " - try again!")
+        error_msg = (
+            "No directory found at: " + this_runs_results["root_dir"] + " - try again!"
+        )
         tk.messagebox.showerror(title="Try again", message=error_msg)
         print(error_msg)
         return
     this_info["results_dir"] = os.path.join(
         this_runs_results["root_dir"] + "Results/" + this_info["name"] + "/"
     )
     # execute
-    autogaita_utils.try_to_run_gaita("Simi", this_info, this_folderinfo, this_runs_cfg, False)
+    autogaita_utils.try_to_run_gaita(
+        "Simi", this_info, this_folderinfo, this_runs_cfg, False
+    )
 
 
 def analyse_multi_run(this_runs_results, this_runs_cfg):
     """Analyse multiple runs at once - extracts folderinfo and then loops over all names
     of multirun_info
     """
     this_folderinfo = prepare_folderinfo(this_runs_results)
     if this_folderinfo is None:
         error_msg = (
-            "No directory found at: "
-            + this_runs_results["root_dir"]
-            + " - try again!"
-            )
+            "No directory found at: " + this_runs_results["root_dir"] + " - try again!"
+        )
         tk.messagebox.showerror(title="Try again", message=error_msg)
         print(error_msg)
         return
     multirun_info = multirun_extract_info(this_folderinfo)
     for idx, name in enumerate(multirun_info["name"]):
         multirun_run_a_single_dataset(
             idx, multirun_info, this_folderinfo, this_runs_cfg
@@ -672,15 +673,17 @@
     based on current cfg"""
     # extract and pass info of this mouse/run (also update resdir)
     this_info = {}
     keynames = multirun_info.keys()
     for keyname in keynames:
         this_info[keyname] = multirun_info[keyname][idx]
     # important to only pass this_info here (1 run at a time - prints error if needed)
-    autogaita_utils.try_to_run_gaita("Simi", this_info, this_folderinfo, this_runs_cfg, True)
+    autogaita_utils.try_to_run_gaita(
+        "Simi", this_info, this_folderinfo, this_runs_cfg, True
+    )
 
 
 # %%..............  LOCAL FUNCTION(S) #4 - VARIOUS HELPER FUNCTIONS  ...................
 
 
 def change_ID_entry_state(ID_entry, results):
     """Change the state of ID entry widget based on whether user wants to only analyse
@@ -703,24 +706,25 @@
     """Configure the icon - in macos it changes the dock icon, in windows it changes
     all windows titlebar icons (taskbar cannot be changed without converting to exe)
     """
     if platform.system().startswith("Darwin"):
         try:
             from Cocoa import NSApplication, NSImage
         except ImportError:
-            print('Unable to import pyobjc modules')
+            print("Unable to import pyobjc modules")
         else:
             with resources.path("autogaita", "autogaita_icon.icns") as icon_path:
                 ns_application = NSApplication.sharedApplication()
                 logo_ns_image = NSImage.alloc().initByReferencingFile_(str(icon_path))
                 ns_application.setApplicationIconImage_(logo_ns_image)
     elif platform.system().startswith("win"):
         with resources.path("autogaita", "autogaita_icon.ico") as icon_path:
             root.iconbitmap(str(icon_path))
 
+
 def change_postname_entry_state(postname_entry, results):
     """Change the state of ID entry widget based on whether user wants to only analyse
     a single dataset.
     """
     if results["postname_flag"].get() == True:
         postname_entry.configure(state="normal")
     elif results["postname_flag"].get() == False:
```

### Comparing `autogaita-0.0.5/autogaita/autogaita_utils.py` & `autogaita-0.0.6/autogaita/autogaita_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,29 @@
 
 
 # ...............................  global constants  ...................................
 ISSUES_TXT_FILENAME = "Issues.txt"
 
 
 # ...............................  error handling  .....................................
-def try_to_run_gaita(
-    which_gaita, info, folderinfo, cfg, multirun_flag
-):
+def try_to_run_gaita(which_gaita, info, folderinfo, cfg, multirun_flag):
     """Try to run AutoGaitA for a single dataset - print and log error if there was any
     error that prevented completion of the main code
 
     Note
     ----
     Needs to know "which gaita" (DLC or Simi) should be run and if "this run" is part
     of a call to one of our multiruns!
     """
     # print info
     message = (
         "\n\n\n*********************************************"
-        + "\n*                  "
+        + "\n*              "
         + info["name"]
-        + "                     *"
+        + "                *"
         + "\n*********************************************"
     )
     print(message)
     try:
         if which_gaita == "DLC":
             autogaita_dlc.dlc(info, folderinfo, cfg)
         elif which_gaita == "Simi":
```

### Comparing `autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_dlc_multirun.py` & `autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_dlc_multirun.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,52 +3,58 @@
 # imports
 from autogaita import autogaita_utils
 import os
 import pdb
 
 # constants
 # folderinfo
-ROOT_DIR = "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Error Mouse 2 Ines/"
-SCTABLE_FILENAME = "CB_5mm_SC.xlsx"  # has to be an excel file
-DATA_STRING = "SalkData"
-BEAM_STRING = "SalkBeam"
+ROOT_DIR = "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Testing/"
+SCTABLE_FILENAME = "25mm.xlsx"  # has to be an excel file
+DATA_STRING = "SIMINewOct"
+BEAM_STRING = "BeamTraining"
 PREMOUSE_STRING = "Mouse"
-POSTMOUSE_STRING = "_5mm"
-PRERUN_STRING = "Run"
-POSTRUN_STRING = "-2DLC_resnet50"
+POSTMOUSE_STRING = "_25mm"
+PRERUN_STRING = "run"
+POSTRUN_STRING = "-6DLC"
 # base cfg
-SAMPLING_RATE = 180
+SAMPLING_RATE = 100
 SUBTRACT_BEAM = True
 DONT_SHOW_PLOTS = False
-CONVERT_TO_MM = False
+CONVERT_TO_MM = True
 PIXEL_TO_MM_RATIO = 3.76  # used for converting x & y data to millimeters
 # advanced cfg
 X_SC_BROKEN_THRESHOLD = 200  # reject SC if x/y goes +-value @ neighbouring tps
 Y_SC_BROKEN_THRESHOLD = 50
 X_ACCELERATION = True
 ANGULAR_ACCELERATION = True
 SAVE_TO_XLS = True
 BIN_NUM = 25
 PLOT_SE = True
-NORMALISE_HEIGHT_AT_SC_LEVEL = True
+NORMALISE_HEIGHT_AT_SC_LEVEL = False
 INVERT_Y_AXIS = True
 FLIP_GAIT_DIRECTION = True
 PLOT_JOINT_NUMBER = 3
 # column cfg
 HIND_JOINTS = ["Hind paw tao", "Ankle", "Knee", "Hip", "Iliac Crest"]
 FORE_JOINTS = [
-        "Front paw tao ",
-        "Wrist ",
-        "Elbow ",
-        "Lower Shoulder ",
-        "Upper Shoulder ",
-    ]
+    "Front paw tao ",
+    "Wrist ",
+    "Elbow ",
+    "Lower Shoulder ",
+    "Upper Shoulder ",
+]
+BEAM_COL_LEFT = ["BeamLeft"]  # BEAM_COL_LEFT & _RIGHT must be lists of len=1
+BEAM_COL_RIGHT = ["BeamRight"]
 BEAM_HIND_JOINTADD = ["Tail base ", "Tail center ", "Tail tip "]
 BEAM_FORE_JOINTADD = ["Nose ", "Ear base "]
-ANGLES = {"name": ["Ankle", "Elbow"], "lower_joint": ["Hind paw tao", "Wrist"], "upper_joint": ["Knee", "Lower Shoulder"]}
+ANGLES = {
+    "name": ["Ankle", "Elbow"],
+    "lower_joint": ["Hind paw tao", "Wrist"],
+    "upper_joint": ["Knee", "Lower Shoulder"],
+}
 
 
 # .....................  User note - please configure  ........................
 # 1) ROOT_DIR: where are the files
 # 2) SCTABLE_FILENAME: excel filename with manual step cycle annotations
 # 3) DATA_STRING: what is the string that defines files to contain data
 # 4) BEAM_STRING: what is the string that defines files to contain beam-coords
@@ -67,28 +73,29 @@
         run_singlerun(idx, info, folderinfo, cfg)
 
 
 # %% local functions
 
 
 def run_singlerun(idx, info, folderinfo, cfg):
-    """ Run the main code of individual run-analyses based on current cfg """
+    """Run the main code of individual run-analyses based on current cfg"""
     # extract and pass info of this mouse/run (also update resdir)
     this_info = {}
     keynames = info.keys()
     for keyname in keynames:
         this_info[keyname] = info[keyname][idx]
-    this_info["results_dir"] = os.path.join(folderinfo["root_dir"] + "Results/"
-                                        + this_info["name"] + "/")
+    this_info["results_dir"] = os.path.join(
+        folderinfo["root_dir"] + "Results/" + this_info["name"] + "/"
+    )
     # important to only pass this_info to main script here (1 run at a time!)
     autogaita_utils.try_to_run_gaita("DLC", this_info, folderinfo, cfg, True)
 
 
 def prepare_folderinfo():
-    """ Dump all infos about this given folder into a dict """
+    """Dump all infos about this given folder into a dict"""
     folderinfo = {}
     folderinfo["root_dir"] = ROOT_DIR
     # to make sure root_dir works under windows
     # (windows is okay with all dir-separators being "/", so make sure it is!)
     folderinfo["root_dir"] = folderinfo["root_dir"].replace(os.sep, "/")
     if folderinfo["root_dir"][-1] != "/":
         folderinfo["root_dir"] = folderinfo["root_dir"] + "/"
@@ -99,15 +106,15 @@
     folderinfo["postmouse_string"] = POSTMOUSE_STRING
     folderinfo["prerun_string"] = PRERUN_STRING
     folderinfo["postrun_string"] = POSTRUN_STRING
     return folderinfo
 
 
 def prepare_cfg():
-    """ Dump all configuration information into a dict """
+    """Dump all configuration information into a dict"""
     cfg = {}
     cfg["sampling_rate"] = SAMPLING_RATE  # base cfg
     cfg["subtract_beam"] = SUBTRACT_BEAM
     cfg["dont_show_plots"] = DONT_SHOW_PLOTS
     cfg["convert_to_mm"] = CONVERT_TO_MM
     cfg["pixel_to_mm_ratio"] = PIXEL_TO_MM_RATIO
     cfg["x_sc_broken_threshold"] = X_SC_BROKEN_THRESHOLD  # optional cfg
@@ -119,45 +126,47 @@
     cfg["plot_SE"] = PLOT_SE
     cfg["normalise_height_at_SC_level"] = NORMALISE_HEIGHT_AT_SC_LEVEL
     cfg["plot_joint_number"] = PLOT_JOINT_NUMBER
     cfg["invert_y_axis"] = INVERT_Y_AXIS
     cfg["flip_gait_direction"] = FLIP_GAIT_DIRECTION
     cfg["hind_joints"] = HIND_JOINTS
     cfg["fore_joints"] = FORE_JOINTS
+    cfg["beam_col_left"] = BEAM_COL_LEFT
+    cfg["beam_col_right"] = BEAM_COL_RIGHT
     cfg["beam_hind_jointadd"] = BEAM_HIND_JOINTADD
     cfg["beam_fore_jointadd"] = BEAM_FORE_JOINTADD
     cfg["angles"] = ANGLES
     return cfg
 
 
 def extract_info():
-    """ Prepare a dict of lists that include unique name/mouse/run infos"""
-    info = {"name": [], "mouse_num":[], "run_num":[]}
+    """Prepare a dict of lists that include unique name/mouse/run infos"""
+    info = {"name": [], "mouse_num": [], "run_num": []}
     for filename in os.listdir(ROOT_DIR):
-        if ((PREMOUSE_STRING in filename)  # make sure we don't get wrong files
-        & (PRERUN_STRING in filename)
-        & (filename.endswith(".csv"))):
+        if (
+            (PREMOUSE_STRING in filename)  # make sure we don't get wrong files
+            & (PRERUN_STRING in filename)
+            & (filename.endswith(".csv"))
+        ):
             # we can use COUNT vars as we do here, since we start @ 0 and do
             # not include the last index (so if counts=2, idx=[0:2]=include
             # 0&1 only!)
-            this_mouse_num = find_number(filename, PREMOUSE_STRING,
-                                        POSTMOUSE_STRING)
+            this_mouse_num = find_number(filename, PREMOUSE_STRING, POSTMOUSE_STRING)
             this_run_num = find_number(filename, PRERUN_STRING, POSTRUN_STRING)
-            this_name = "ID " + str(
-                this_mouse_num) + " - Run " + str(this_run_num)
+            this_name = "ID " + str(this_mouse_num) + " - Run " + str(this_run_num)
             if this_name not in info["name"]:  # no data/beam duplicates here
                 info["name"].append(this_name)
                 info["mouse_num"].append(this_mouse_num)
                 info["run_num"].append(this_run_num)
     return info
 
 
 def find_number(fullstring, prestring, poststring):
-    """ Find (mouse/run) number based on user-defined strings in filenames """
+    """Find (mouse/run) number based on user-defined strings in filenames"""
     start_idx = fullstring.find(prestring) + len(prestring)
     end_idx = fullstring.find(poststring)
     return int(fullstring[start_idx:end_idx])
 
 
 # %% what happens if we just hit run
 if __name__ == "__main__":
-    dlc_multirun()
+    dlc_multirun()
```

### Comparing `autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_dlc_singlerun.py` & `autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_dlc_singlerun.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 # %% If we just want to analyse one run...
 from autogaita import autogaita_utils
 import os
 
 # ...............  1) folderinfo & cfg-dicts: constants  ......................
 # folderinfo
-ROOT_DIR = "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Error Mouse 1 Ines"
-SCTABLE_FILENAME = "AnnotationTable"  # has to be an excel file
-DATA_STRING = "BalanceJun"
+ROOT_DIR = "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Testing/"
+SCTABLE_FILENAME = "25mm.xlsx"  # has to be an excel file
+DATA_STRING = "SIMINewOct"
 BEAM_STRING = "BeamTraining"
 PREMOUSE_STRING = "Mouse"
-POSTMOUSE_STRING = "_4mm"
-PRERUN_STRING = "Run"
-POSTRUN_STRING = "_DLC"
+POSTMOUSE_STRING = "_25mm"
+PRERUN_STRING = "run"
+POSTRUN_STRING = "-6DLC"
 # base cfg
 SAMPLING_RATE = 100
-SUBTRACT_BEAM = False
+SUBTRACT_BEAM = True
 DONT_SHOW_PLOTS = False
 CONVERT_TO_MM = True
 PIXEL_TO_MM_RATIO = 3.76  # used for converting x & y data to millimeters
 # advanced cfg
 X_SC_BROKEN_THRESHOLD = 200  # reject SC if x/y goes +-value @ neighbouring tps
 Y_SC_BROKEN_THRESHOLD = 50
 X_ACCELERATION = True
 ANGULAR_ACCELERATION = True
 SAVE_TO_XLS = True
 BIN_NUM = 25
 PLOT_SE = True
-NORMALISE_HEIGHT_AT_SC_LEVEL = True
+NORMALISE_HEIGHT_AT_SC_LEVEL = False
 INVERT_Y_AXIS = True
 FLIP_GAIT_DIRECTION = True
 PLOT_JOINT_NUMBER = 3
+# column cfg
 HIND_JOINTS = ["Hind paw tao", "Ankle", "Knee", "Hip", "Iliac Crest"]
 FORE_JOINTS = [
-        "Front paw tao ",
-        "Wrist ",
-        "Elbow ",
-        "Lower Shoulder ",
-        "Upper Shoulder ",
-    ]
+    "Front paw tao ",
+    "Wrist ",
+    "Elbow ",
+    "Lower Shoulder ",
+    "Upper Shoulder ",
+]
+BEAM_COL_LEFT = ["BeamLeft"]  # BEAM_COL_LEFT & _RIGHT must be lists of len=1
+BEAM_COL_RIGHT = ["BeamRight"]
 BEAM_HIND_JOINTADD = ["Tail base ", "Tail center ", "Tail tip "]
 BEAM_FORE_JOINTADD = ["Nose ", "Ear base "]
-ANGLES = {"name": ["Ankle", "Elbow"], "lower_joint": ["Hind paw tao", "Wrist"], "upper_joint": ["Knee", "Lower Shoulder"]}
+ANGLES = {
+    "name": ["Ankle", "Elbow"],
+    "lower_joint": ["Hind paw tao", "Wrist"],
+    "upper_joint": ["Knee", "Lower Shoulder"],
+}
 
 
 # ......................  info-dict: mouse/run-constants  ..............................
 info = {}
-info["mouse_num"] = 174
+info["mouse_num"] = 14
 info["run_num"] = 1
-info["name"] = ("ID " + str(info["mouse_num"])
-                + " - Run " + str(info["run_num"]))
+info["name"] = "ID " + str(info["mouse_num"]) + " - Run " + str(info["run_num"])
 info["results_dir"] = os.path.join(ROOT_DIR + "Results/" + info["name"] + "/")
 
+
 # %% code
 def dlc_singlerun():
     folderinfo = prepare_folderinfo()
     cfg = prepare_cfg()
     # run
     autogaita_utils.try_to_run_gaita("DLC", info, folderinfo, cfg, False)
 
 
 def prepare_folderinfo():
-    """ Dump all infos about this given folder into a dict """
+    """Dump all infos about this given folder into a dict"""
     folderinfo = {}
     folderinfo["root_dir"] = ROOT_DIR
     # to make sure root_dir works under windows
     # (windows is okay with all dir-separators being "/", so make sure it is!)
     folderinfo["root_dir"] = folderinfo["root_dir"].replace(os.sep, "/")
     if folderinfo["root_dir"][-1] != "/":
         folderinfo["root_dir"] = folderinfo["root_dir"] + "/"
@@ -75,15 +82,15 @@
     folderinfo["postmouse_string"] = POSTMOUSE_STRING
     folderinfo["prerun_string"] = PRERUN_STRING
     folderinfo["postrun_string"] = POSTRUN_STRING
     return folderinfo
 
 
 def prepare_cfg():
-    """ Dump all configuration information into a dict """
+    """Dump all configuration information into a dict"""
     cfg = {}
     cfg["sampling_rate"] = SAMPLING_RATE  # base cfg
     cfg["subtract_beam"] = SUBTRACT_BEAM
     cfg["dont_show_plots"] = DONT_SHOW_PLOTS
     cfg["convert_to_mm"] = CONVERT_TO_MM
     cfg["pixel_to_mm_ratio"] = PIXEL_TO_MM_RATIO
     cfg["x_sc_broken_threshold"] = X_SC_BROKEN_THRESHOLD  # optional cfg
@@ -95,15 +102,18 @@
     cfg["plot_SE"] = PLOT_SE
     cfg["normalise_height_at_SC_level"] = NORMALISE_HEIGHT_AT_SC_LEVEL
     cfg["plot_joint_number"] = PLOT_JOINT_NUMBER
     cfg["invert_y_axis"] = INVERT_Y_AXIS
     cfg["flip_gait_direction"] = FLIP_GAIT_DIRECTION
     cfg["hind_joints"] = HIND_JOINTS
     cfg["fore_joints"] = FORE_JOINTS
+    cfg["beam_col_left"] = BEAM_COL_LEFT
+    cfg["beam_col_right"] = BEAM_COL_RIGHT
     cfg["beam_hind_jointadd"] = BEAM_HIND_JOINTADD
     cfg["beam_fore_jointadd"] = BEAM_FORE_JOINTADD
     cfg["angles"] = ANGLES
     return cfg
 
+
 # %% what happens if we just hit run
 if __name__ == "__main__":
-    dlc_singlerun()
+    dlc_singlerun()
```

### Comparing `autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_group_dlcrun.py` & `autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_group_dlcrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Contrast autogaita_dlc results using autogaita_group
 from autogaita import autogaita_group
 
+
 def group_dlcrun():
     """Batch run group level analyses for results obtained with _dlc"""
     folderinfo = {}
     cfg = {}
     cfg["do_permtest"] = True
     cfg["do_anova"] = True
     cfg["permutation_number"] = 100
@@ -34,12 +35,12 @@
         "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Testing/Group 1/",
         "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Testing/Group 2/",
     ]
 
     # results dir
     folderinfo[
         "results_dir"
-    # mouse
+        # mouse
     ] = "/Users/mahan/sciebo/Research/AutoGaitA/Mouse/Testing/GroupResults/"
 
     # run
-    autogaita_group.group(folderinfo, cfg)
+    autogaita_group.group(folderinfo, cfg)
```

### Comparing `autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_group_simirun.py` & `autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_group_simirun.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Contrast autogaita_simi results using autogaita_group
 from autogaita import autogaita_group
 
+
 def group_simirun():
     """Batch run group level analyses for results obtained with _simi"""
     # constant folderinfo & cfg vars
     folderinfo = {}
     cfg = {}
     cfg["do_permtest"] = True
     cfg["do_anova"] = True
@@ -31,25 +32,26 @@
         cfg["stats_variables"] = [
             "Midfoot, " + cfg["which_leg"] + " Z",
             "Ankle, " + cfg["which_leg"] + " Z",
             # "Knee, " + cfg["which_leg"] + " Z",
             # "Shoulder, " + cfg["which_leg"] + " Angle",
             "Skullbase Angle",
             "Elbow, " + cfg["which_leg"] + " Angle",
-            ]
+        ]
 
         # 2 groups - human
-        folderinfo["group_names"] = [
-            "Young",
-            "Old"
-            ]
+        folderinfo["group_names"] = ["Young", "Old"]
         folderinfo["group_dirs"] = [
             "/Users/mahan/sciebo/Research/AutoGaitA/Human/Testing2/Young/",
             "/Users/mahan/sciebo/Research/AutoGaitA/Human/Testing2/Old/",
         ]
 
         folderinfo[
             "results_dir"
             # human
-        ] = "/Users/mahan/sciebo/Research/AutoGaitA/Human/Testing2/Group/" + cfg["which_leg"] + " leg/"
+        ] = (
+            "/Users/mahan/sciebo/Research/AutoGaitA/Human/Testing2/Group/"
+            + cfg["which_leg"]
+            + " leg/"
+        )
 
         autogaita_group.group(folderinfo, cfg)
```

### Comparing `autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_simi_multirun.py` & `autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_simi_multirun.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 Y_ACCELERATION = True
 ANGULAR_ACCELERATION = True
 BIN_NUM = 25
 PLOT_SE = False
 NORMALISE_HEIGHT_AT_SC_LEVEL = True
 PLOT_JOINT_NUMBER = 7
 JOINTS = ["Midfoot", "Ankle", "Knee", "Hip", "Pelvis", "Shoulder", "Neck"]
-ANGLES = {"name": ["WHO", "Ankle", "Knee", "Elbow", "Skullbase"],
-          "lower_joint": ["Midfoot", "IS", "Ankle", "Wrist", "Neck"],
-          "upper_joint": ["Knee", "Hip", "Shoulder", "Skull"]}
+ANGLES = {
+    "name": ["Ankle", "Knee"],
+    "lower_joint": ["Midfoot", "Ankle"],
+    "upper_joint": ["Knee", "Hip"],
+}
 
 
 # %% main program
 
 
 def simi_multirun():
     info = extract_info()
@@ -46,63 +48,64 @@
         run_singlerun(idx, info, folderinfo, cfg)
 
 
 # %% local functions
 
 
 def run_singlerun(idx, info, folderinfo, cfg):
-    """ Run the main code of individual run-analyses based on current cfg """
+    """Run the main code of individual run-analyses based on current cfg"""
     # extract and pass info of this mouse/run (also update resdir)
     this_info = {}
     keynames = info.keys()
     for keyname in keynames:
         this_info[keyname] = info[keyname][idx]
     # important to only pass this_info to main script here (1 run at a time!)
     autogaita_utils.try_to_run_gaita("Simi", this_info, folderinfo, cfg, True)
 
 
 def extract_info():
-    """ Prepare a dict of lists that include unique name infos"""
-    info = {"name": [], "results_dir":[]}
+    """Prepare a dict of lists that include unique name infos"""
+    info = {"name": [], "results_dir": []}
     for filename in os.listdir(ROOT_DIR):
         if not POSTNAME_STRING:
             if (".xls" in filename) & (SCTABLE_FILENAME not in filename):
                 info["name"].append(filename.split(".xls")[0])
                 info["results_dir"].append(
                     os.path.join(ROOT_DIR + "Results/" + info["name"][-1] + "/")
-                    )
+                )
         else:
             if POSTNAME_STRING in filename:
                 info["name"].append(filename.split(POSTNAME_STRING)[0])
                 info["results_dir"].append(
                     os.path.join(ROOT_DIR + "Results/" + info["name"][-1] + "/")
-                    )
+                )
     return info
 
 
 def prepare_folderinfo():
-    """ Dump all infos about constants in this given folder into a dict """
+    """Dump all infos about constants in this given folder into a dict"""
     folderinfo = {}
     folderinfo["root_dir"] = ROOT_DIR
     folderinfo["sctable_filename"] = SCTABLE_FILENAME
     folderinfo["postname_string"] = POSTNAME_STRING
     return folderinfo
 
 
 def prepare_cfg():
-    """ Dump all configuration information into a dict """
+    """Dump all configuration information into a dict"""
     cfg = {}
     cfg["sampling_rate"] = SAMPLING_RATE  # base cfg
     cfg["dont_show_plots"] = DONT_SHOW_PLOTS
     cfg["y_acceleration"] = Y_ACCELERATION
     cfg["angular_acceleration"] = ANGULAR_ACCELERATION
     cfg["bin_num"] = BIN_NUM
     cfg["plot_SE"] = PLOT_SE
     cfg["normalise_height_at_SC_level"] = NORMALISE_HEIGHT_AT_SC_LEVEL
     cfg["plot_joint_number"] = PLOT_JOINT_NUMBER
     cfg["joints"] = JOINTS
     cfg["angles"] = ANGLES
     return cfg
 
+
 # %% what happens if we just hit run
 if __name__ == "__main__":
     simi_multirun()
```

### Comparing `autogaita-0.0.5/autogaita/batchrun_scripts/autogaita_simi_singlerun.py` & `autogaita-0.0.6/autogaita/batchrun_scripts/autogaita_simi_singlerun.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # %% If we just want to analyse one run...
 from autogaita import autogaita_utils
 import os
 import traceback
 
-# .............  1) folderinfo-dict: the folder-constants  ....................
+# .............  1) folderinfo-dict: the folder-constants  ...............
 # constants
 ROOT_DIR = "/Users/mahan/sciebo/Research/AutoGaitA/Human/Testing2/"
 SCTABLE_FILENAME = "SC Latency Table"  # has to be an xlsxfile
 POSTNAME_FLAG = False
 if POSTNAME_FLAG is False:
     POSTNAME_STRING = ""
 else:
@@ -21,17 +21,19 @@
 Y_ACCELERATION = True
 ANGULAR_ACCELERATION = True
 BIN_NUM = 25
 PLOT_SE = True
 NORMALISE_HEIGHT_AT_SC_LEVEL = True
 PLOT_JOINT_NUMBER = 7
 JOINTS = ["Ankle", "Knee", "Hip", "Pelvis", "Shoulder", "Neck"]
-ANGLES = {"name": ["Ankle", "Knee", "Elbow", "Skullbase"],
-          "lower_joint": ["Midfoot", "Ankle", "Wrist", "Neck"],
-          "upper_joint": ["Knee", "Hip", "Shoulder", "Skull"]}
+ANGLES = {
+    "name": ["Ankle", "Knee", "Elbow", "Skullbase"],
+    "lower_joint": ["Midfoot", "Ankle", "Wrist", "Neck"],
+    "upper_joint": ["Knee", "Hip", "Shoulder", "Skull"],
+}
 
 # .................  3) info-dict: ID-constants  .......................
 info = {}
 info["name"] = "SK"  # analyse this dataset
 info["results_dir"] = os.path.join(ROOT_DIR + "Results/" + info["name"] + "/")
 
 
@@ -40,33 +42,34 @@
     folderinfo = prepare_folderinfo()
     cfg = prepare_cfg()
     # run
     autogaita_utils.try_to_run_gaita("Simi", info, folderinfo, cfg, False)
 
 
 def prepare_folderinfo():
-    """ Dump all infos about constants in this given folder into a dict """
+    """Dump all infos about constants in this given folder into a dict"""
     folderinfo = {}
     folderinfo["root_dir"] = ROOT_DIR
     folderinfo["sctable_filename"] = SCTABLE_FILENAME
     folderinfo["postname_string"] = POSTNAME_STRING
     return folderinfo
 
 
 def prepare_cfg():
-    """ Dump all configuration information into a dict """
+    """Dump all configuration information into a dict"""
     cfg = {}
     cfg["sampling_rate"] = SAMPLING_RATE  # base cfg
     cfg["dont_show_plots"] = DONT_SHOW_PLOTS
     cfg["y_acceleration"] = Y_ACCELERATION
     cfg["angular_acceleration"] = ANGULAR_ACCELERATION
     cfg["bin_num"] = BIN_NUM
     cfg["plot_SE"] = PLOT_SE
     cfg["normalise_height_at_SC_level"] = NORMALISE_HEIGHT_AT_SC_LEVEL
     cfg["plot_joint_number"] = PLOT_JOINT_NUMBER
     cfg["joints"] = JOINTS
     cfg["angles"] = ANGLES
     return cfg
 
+
 # %% what happens if we just hit run
 if __name__ == "__main__":
-    simi_singlerun()
+    simi_singlerun()
```

### Comparing `autogaita-0.0.5/autogaita.egg-info/SOURCES.txt` & `autogaita-0.0.6/autogaita.egg-info/SOURCES.txt`

 * *Files identical despite different names*

