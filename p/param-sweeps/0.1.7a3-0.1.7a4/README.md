# Comparing `tmp/param_sweeps-0.1.7a3.tar.gz` & `tmp/param_sweeps-0.1.7a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "param_sweeps-0.1.7a3.tar", max compression
+gzip compressed data, was "param_sweeps-0.1.7a4.tar", max compression
```

## Comparing `param_sweeps-0.1.7a3.tar` & `param_sweeps-0.1.7a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2022-10-12 15:56:34.681986 param_sweeps-0.1.7a3/LICENSE
--rw-r--r--   0        0        0      270 2024-03-18 16:36:55.677134 param_sweeps-0.1.7a3/param_sweeps/__init__.py
--rw-r--r--   0        0        0      572 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a3/param_sweeps/constants.py
--rw-r--r--   0        0        0     8454 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a3/param_sweeps/driver.py
--rw-r--r--   0        0        0     3230 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a3/param_sweeps/generate.py
--rw-r--r--   0        0        0      967 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a3/param_sweeps/sample_driver.py
--rw-r--r--   0        0        0     1648 2024-03-18 16:36:55.677134 param_sweeps-0.1.7a3/pyproject.toml
--rw-r--r--   0        0        0     1153 2022-11-10 19:09:10.043391 param_sweeps-0.1.7a3/README.md
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 param_sweeps-0.1.7a3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-10-12 15:56:34.681986 param_sweeps-0.1.7a4/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-23 17:22:53.644053 param_sweeps-0.1.7a4/param_sweeps/__init__.py
+-rw-r--r--   0        0        0      572 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a4/param_sweeps/constants.py
+-rw-r--r--   0        0        0     8151 2024-04-23 17:22:24.134054 param_sweeps-0.1.7a4/param_sweeps/driver.py
+-rw-r--r--   0        0        0     3230 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a4/param_sweeps/generate.py
+-rw-r--r--   0        0        0      967 2024-01-10 23:46:44.682317 param_sweeps-0.1.7a4/param_sweeps/sample_driver.py
+-rw-r--r--   0        0        0     1598 2024-04-23 17:22:53.644053 param_sweeps-0.1.7a4/pyproject.toml
+-rw-r--r--   0        0        0     1153 2022-11-10 19:09:10.043391 param_sweeps-0.1.7a4/README.md
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 param_sweeps-0.1.7a4/PKG-INFO
```

### Comparing `param_sweeps-0.1.7a3/LICENSE` & `param_sweeps-0.1.7a4/LICENSE`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a3/param_sweeps/constants.py` & `param_sweeps-0.1.7a4/param_sweeps/constants.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a3/param_sweeps/driver.py` & `param_sweeps-0.1.7a4/param_sweeps/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from __future__ import annotations
 
 import argparse
 import importlib
 import inspect
 import itertools
 import json
+import shutil
 import uuid
 from dataclasses import dataclass
 from inspect import signature
 from io import BytesIO
 from pathlib import Path
 from typing import Any
 
 import numpy as np
-from geoh5py.data import Data
 from geoh5py.shared.exceptions import BaseValidationError
 from geoh5py.ui_json import InputFile
 from geoh5py.workspace import Workspace
 
 
 @dataclass
 class SweepParams:
@@ -152,26 +152,23 @@
 
         ifile = InputFile.read_ui_json(self.params.worker_uijson)
         with ifile.data["geoh5"].open(mode="r") as workspace:
             for name, trial in lookup.items():
                 if trial["status"] != "pending":
                     continue
 
-                filepath = Path(workspace.h5file).parent / f"{name}.ui.geoh5"
-                with Workspace.create(filepath) as iter_workspace:
-                    ifile.data.update(
-                        dict(
-                            {key: val for key, val in trial.items() if key != "status"},
-                            **{"geoh5": iter_workspace},
-                        )
+                iter_h5file = str(Path(workspace.h5file).parent / f"{name}.ui.geoh5")
+                shutil.copy(workspace.h5file, iter_h5file)
+
+                ifile.data.update(
+                    dict(
+                        {key: val for key, val in trial.items() if key != "status"},
+                        **{"geoh5": iter_h5file},
                     )
-                    objects = [v for v in ifile.data.values() if hasattr(v, "uid")]
-                    for obj in objects:
-                        if not isinstance(obj, Data):
-                            obj.copy(parent=iter_workspace, copy_children=True)
+                )
 
                 ifile.name = f"{name}.ui.json"
                 ifile.path = str(Path(workspace.h5file).parent)
                 ifile.write_ui_json()
                 lookup[name]["status"] = "written"
 
         _ = self.update_lookup(lookup)
```

### Comparing `param_sweeps-0.1.7a3/param_sweeps/generate.py` & `param_sweeps-0.1.7a4/param_sweeps/generate.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a3/param_sweeps/sample_driver.py` & `param_sweeps-0.1.7a4/param_sweeps/sample_driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a3/pyproject.toml` & `param_sweeps-0.1.7a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "param-sweeps"
-version = "0.1.7-alpha.3"
+version = "0.1.7-alpha.4"
 
 description = "Parameter sweeper for ui.json powered applications"
 authors = ["Mira Geoscience <benjamink@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/param-sweeps"
 homepage = "https://mirageoscience.com"
 readme = "README.md"
 keywords = ["geology", "geophysics", "earth sciences"]
@@ -21,17 +21,16 @@
     "Operating System :: Unix",
 #    "Operating System :: MacOS",
     "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
-geoh5py = {version = "~0.9.0-alpha.1", allow-prereleases = true}
+geoh5py = {version = "~0.9.0-alpha.4", allow-prereleases = true}
 #geoh5py = {git = "https://github.com/MiraGeoscience/geoh5py.git", branch = "develop"}
-#geoh5py = {path = "../geoh5py", develop = true}
 
 numpy = "!=1.19.4, ~1.23.5"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `param_sweeps-0.1.7a3/README.md` & `param_sweeps-0.1.7a4/README.md`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7a3/PKG-INFO` & `param_sweeps-0.1.7a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: param-sweeps
-Version: 0.1.7a3
+Version: 0.1.7a4
 Summary: Parameter sweeper for ui.json powered applications
 Home-page: https://mirageoscience.com
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
 Author-email: benjamink@mirageoscience.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: geoh5py (>=0.9.0-alpha.1,<0.10.0)
+Requires-Dist: geoh5py (>=0.9.0-alpha.4,<0.10.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Project-URL: Repository, https://github.com/MiraGeoscience/param-sweeps
 Description-Content-Type: text/markdown
 
 # Param-sweeps
 
 A Parameter sweeper for applications driven by ui.json files
```

