# Comparing `tmp/las_geoh5-0.1.0.tar.gz` & `tmp/las_geoh5-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "las_geoh5-0.1.0.tar", max compression
+gzip compressed data, was "las_geoh5-0.2.0a1.tar", max compression
```

## Comparing `las_geoh5-0.1.0.tar` & `las_geoh5-0.2.0a1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      283 2023-11-07 18:05:48.491460 las_geoh5-0.1.0/las_geoh5/__init__.py
--rw-r--r--   0        0        0      240 2023-11-07 18:05:48.491460 las_geoh5-0.1.0/las_geoh5/export_directories/__init__.py
--rw-r--r--   0        0        0     1753 2023-11-07 18:05:48.492519 las_geoh5-0.1.0/las_geoh5/export_directories/driver.py
--rw-r--r--   0        0        0     1086 2023-11-07 18:05:48.492519 las_geoh5-0.1.0/las_geoh5/export_directories/uijson.py
--rw-r--r--   0        0        0     6799 2023-11-07 18:05:48.493514 las_geoh5-0.1.0/las_geoh5/export_las.py
--rw-r--r--   0        0        0      240 2023-11-07 18:05:48.493514 las_geoh5-0.1.0/las_geoh5/import_directories/__init__.py
--rw-r--r--   0        0        0     2242 2023-11-07 18:05:48.493514 las_geoh5-0.1.0/las_geoh5/import_directories/driver.py
--rw-r--r--   0        0        0      514 2023-11-07 18:05:48.494513 las_geoh5-0.1.0/las_geoh5/import_directories/uijson.py
--rw-r--r--   0        0        0      240 2023-11-07 18:05:48.494513 las_geoh5-0.1.0/las_geoh5/import_files/__init__.py
--rw-r--r--   0        0        0     3779 2023-11-07 18:05:48.494513 las_geoh5-0.1.0/las_geoh5/import_files/driver.py
--rw-r--r--   0        0        0     2013 2023-11-07 18:05:48.495513 las_geoh5-0.1.0/las_geoh5/import_files/uijson.py
--rw-r--r--   0        0        0    12257 2023-11-07 18:05:48.495513 las_geoh5-0.1.0/las_geoh5/import_las.py
--rw-r--r--   0        0        0      122 2023-11-07 18:05:48.495513 las_geoh5-0.1.0/las_geoh5/uijson/__init__.py
--rw-r--r--   0        0        0      842 2023-10-24 15:49:31.448818 las_geoh5-0.1.0/las_geoh5/uijson/export_las_directories.ui.json
--rw-r--r--   0        0        0      842 2023-10-24 15:49:31.448818 las_geoh5-0.1.0/las_geoh5/uijson/import_las_directories.ui.json
--rw-r--r--   0        0        0     1940 2023-11-07 18:04:19.484024 las_geoh5-0.1.0/las_geoh5/uijson/import_las_files.ui.json
--rw-r--r--   0        0        0     2149 2023-11-07 18:05:48.496513 las_geoh5-0.1.0/las_geoh5/uijson/write_uijson.py
--rw-r--r--   0        0        0     1093 2023-11-07 18:05:48.490464 las_geoh5-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2222 2023-11-07 18:05:48.497513 las_geoh5-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2356 2023-11-07 18:05:48.490464 las_geoh5-0.1.0/README.rst
--rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 las_geoh5-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      291 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/export_files/__init__.py
+-rw-r--r--   0        0        0     1734 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/export_files/driver.py
+-rw-r--r--   0        0        0     1264 2024-04-23 17:07:21.289948 las_geoh5-0.2.0a1/las_geoh5/export_files/uijson.py
+-rw-r--r--   0        0        0     6748 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/export_las.py
+-rw-r--r--   0        0        0      240 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_directories/__init__.py
+-rw-r--r--   0        0        0     2104 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_directories/driver.py
+-rw-r--r--   0        0        0     1057 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_directories/uijson.py
+-rw-r--r--   0        0        0      240 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/__init__.py
+-rw-r--r--   0        0        0     4632 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/driver.py
+-rw-r--r--   0        0        0     1468 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/params.py
+-rw-r--r--   0        0        0     3080 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_files/uijson.py
+-rw-r--r--   0        0        0    13319 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/import_las.py
+-rw-r--r--   0        0        0      122 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/uijson/__init__.py
+-rw-r--r--   0        0        0     2119 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5/uijson/write_uijson.py
+-rw-r--r--   0        0        0      122 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/uijson/export_las_files.ui.json
+-rw-r--r--   0        0        0      974 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_directories.ui.json
+-rw-r--r--   0        0        0     2656 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_files.ui.json
+-rw-r--r--   0        0        0     1093 2024-04-23 17:07:21.274278 las_geoh5-0.2.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     2262 2024-04-23 17:07:21.305658 las_geoh5-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4962 2024-04-23 17:07:21.274278 las_geoh5-0.2.0a1/README.rst
+-rw-r--r--   0        0        0     5980 1970-01-01 00:00:00.000000 las_geoh5-0.2.0a1/PKG-INFO
```

### Comparing `las_geoh5-0.1.0/las_geoh5/export_directories/driver.py` & `las_geoh5-0.2.0a1/las_geoh5/import_directories/driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,71 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
 #  las-geoh5 is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 #
 
 from __future__ import annotations
 
 import sys
 from pathlib import Path
 
+import lasio
 from geoh5py.groups import DrillholeGroup
-from geoh5py.objects import Drillhole
 from geoh5py.shared.utils import fetch_active_workspace
 from geoh5py.ui_json import InputFile
-from tqdm import tqdm
 
-from las_geoh5.export_las import drillhole_to_las
+from las_geoh5.import_files.params import ImportOptions
+from las_geoh5.import_las import las_to_drillhole
 
 
-def run(file: str | Path):
+def run(file: str):
     ifile = InputFile.read_ui_json(file)
     dh_group = ifile.data["drillhole_group"]
-    name = ifile.data["name"]
-    with fetch_active_workspace(ifile.data["geoh5"]):
-        export_las_directory(dh_group, Path(ifile.path), name)
+    parent_folder = ifile.data["parent_folder"]
+    with fetch_active_workspace(ifile.data["geoh5"], mode="a"):
+        import_las_directory(dh_group, parent_folder)
 
 
-def export_las_directory(
-    group: DrillholeGroup, basepath: str | Path, name: str | None = None
-):
+def import_las_directory(dh_group: DrillholeGroup, basepath: str | Path):
     """
-    Export contents of drillhole group to las files organized by directories.
+    Import directory/files from previous export.
 
-    :param group: Drillhole group container.
-    :param basepath: Base path where directories/files will be created.
-    :param name: Alternate name of root directory to be created.
+    :param workspace: Project workspace.
+    :param basepath: Root directory for las data.
+
+    :return: New drillhole group containing imported items.
     """
 
     if isinstance(basepath, str):
         basepath = Path(basepath)
 
-    drillholes = [k for k in group.children if isinstance(k, Drillhole)]
+    if not basepath.exists():
+        raise OSError(f"Path {str(basepath)} does not exist.")
+
+    surveys_path = basepath / "Surveys"
+    surveys = list(surveys_path.iterdir()) if surveys_path.exists() else None
+
+    property_group_folders = [
+        p for p in basepath.iterdir() if p.is_dir() and p.name != "Surveys"
+    ]
+
+    for prop in property_group_folders:
+        lasfiles = []
+        for file in [k for k in prop.iterdir() if k.suffix == ".las"]:
+            lasfiles.append(lasio.read(file, mnemonic_case="preserve"))
+        print(f"Importing property group data from to {prop.name}")
+        las_to_drillhole(
+            lasfiles,
+            dh_group,
+            prop.name,
+            surveys,
+            options=ImportOptions(),
+        )
 
-    name = name if name is not None else group.name
-    subpath = basepath / name
-    if not subpath.exists():
-        subpath.mkdir()
-
-    print(f"Exporting drillhole surveys and property group data to {str(subpath)}")
-    for drillhole in tqdm(drillholes):
-        drillhole_to_las(drillhole, subpath)
+    return dh_group
 
 
 if __name__ == "__main__":
     run(sys.argv[1])
```

### Comparing `las_geoh5-0.1.0/las_geoh5/export_directories/uijson.py` & `las_geoh5-0.2.0a1/las_geoh5/export_files/uijson.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
 #  las-geoh5 is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 #
 
+from copy import deepcopy
 
-ui_json = {
-    "title": "Drillhole group to LAS file directories",
-    "geoh5": None,
-    "run_command": "las_geoh5.export_directories.driver",
-    "run_command_boolean": {
-        "value": False,
-        "label": "Run python module",
-        "main": True,
-        "tooltip": "Warning: launches process to run python model on save",
-    },
-    "monitoring_directory": None,
-    "conda_environment": "las-geoh5",
-    "conda_environment_boolean": False,
-    "workspace": None,
-    "drillhole_group": {
-        "main": True,
-        "label": "Drillhole group",
-        "value": None,
-        "groupType": ["{825424fb-c2c6-4fea-9f2b-6cd00023d393}"],
-    },
-    "name": {
-        "main": True,
-        "label": "Property group name",
-        "value": None,
-        "optional": True,
-        "enabled": False,
+from geoh5py.ui_json.constants import default_ui_json
+
+# pylint: disable=duplicate-code
+
+ui_json = dict(
+    deepcopy(default_ui_json),
+    **{
+        "title": "Drillhole group to LAS file directories",
+        "run_command": "las_geoh5.export_files.driver",
+        "conda_environment": "las-geoh5",
+        "drillhole_group": {
+            "main": True,
+            "label": "Drillhole group",
+            "value": None,
+            "groupType": ["{825424fb-c2c6-4fea-9f2b-6cd00023d393}"],
+        },
+        "rootpath": {
+            "main": True,
+            "label": "Directory",
+            "fileDescription": ["Directory"],
+            "fileType": ["directory"],
+            "value": None,
+            "directoryOnly": True,
+        },
+        "use_directories": {
+            "main": True,
+            "label": "Use directories",
+            "tooltip": "Organize las files by property group directories",
+            "value": True,
+        },
     },
-}
+)
```

### Comparing `las_geoh5-0.1.0/las_geoh5/export_las.py` & `las_geoh5-0.2.0a1/las_geoh5/export_las.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
 #  las-geoh5 is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 #
 
@@ -117,23 +117,23 @@
 
     return file
 
 
 def write_curves(
     drillhole: Drillhole,
     basepath: str | Path,
-    directory: bool = True,
+    use_directories: bool = True,
 ):
     """
     Write a formatted .las file for each property group in 'drillhole'.
 
     :param drillhole: geoh5py drillhole object containing property
         groups for collocated data.
     :param basepath: Path to working directory.
-    :param directory: True if data is stored in sub-directories
+    :param use_directories: True if data is stored in sub-directories
     """
 
     if isinstance(basepath, str):
         basepath = Path(basepath)
 
     if not drillhole.property_groups:
         raise AttributeError("Drillhole doesn't have any associated property groups.")
@@ -150,73 +150,70 @@
         file = add_curve_data(file, drillhole, group)
 
         if not [
             k for k in file.curves if k.mnemonic not in ["FROM", "TO", "DEPTH", "DEPT"]
         ]:
             continue
 
-        if directory:
+        if use_directories:
             subpath = basepath / group.name
             if not subpath.exists():
                 subpath.mkdir()
-            filename = f"{drillhole.name}.las"
         else:
             subpath = basepath
-            filename = f"{drillhole.name}_{group.name}.las"
 
+        filename = f"{drillhole.name}_{group.name}.las"
         with open(
             subpath / filename, "a", encoding="utf8"
         ) as io:  # pylint: disable=invalid-name
             file.write(io)
 
 
 def write_survey(
     drillhole: Drillhole,
     basepath: str | Path,
-    directory: bool = True,
+    use_directories: bool = True,
 ):
     """
     Write a formatted .las file with survey data from 'drillhole'.
 
     :param drillhole: geoh5py drillhole object containing property
         groups for collocated data.
     :param basepath: Path to working directory.
-    :param directory: True if data is stored in sub-directories
+    :param use_directories: True if data is stored in sub-directories
     """
 
     if isinstance(basepath, str):
         basepath = Path(basepath)
 
     file = LASFile()
     file = add_well_data(file, drillhole)
     file = add_survey_data(file, drillhole)
 
-    if directory:
+    if use_directories:
         basepath = basepath / "Surveys"
         if not basepath.exists():
             basepath.mkdir()
-        filename = f"{drillhole.name}.las"
-    else:
-        filename = f"{drillhole.name}_survey.las"
 
+    filename = f"{drillhole.name}_survey.las"
     with open(
         basepath / filename, "a", encoding="utf8"
     ) as io:  # pylint: disable=invalid-name
         file.write(io)
 
 
 def drillhole_to_las(
     drillhole: Drillhole,
     basepath: str | Path,
-    directory: bool = True,
+    use_directories: bool = True,
 ):
     """
     Write a formatted .las file with data from 'drillhole'.
 
     :param drillhole: geoh5py drillhole object containing property
         groups for collocated data.
     :param basepath: Path to working directory.
-    :param directory: True if data is stored in sub-directories
+    :param use_directories: True if data is stored in sub-directories
     """
 
-    write_survey(drillhole, basepath, directory)
-    write_curves(drillhole, basepath, directory)
+    write_survey(drillhole, basepath, use_directories)
+    write_curves(drillhole, basepath, use_directories)
```

### Comparing `las_geoh5-0.1.0/las_geoh5/import_directories/driver.py` & `las_geoh5-0.2.0a1/las_geoh5/uijson/write_uijson.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
-#  las-geoh5 is distributed under the terms and conditions of the MIT License
-#  (see LICENSE file at the root of this source code package).
+#  All rights reserved.
+#
+#
+#  This file is part of las-geoh5 project.
+#
+#  All rights reserved.
 #
 
 from __future__ import annotations
 
+import argparse
+import importlib
 import sys
 from pathlib import Path
 
-import lasio
-from geoh5py import Workspace
-from geoh5py.groups import DrillholeGroup
-from geoh5py.shared.utils import fetch_active_workspace
 from geoh5py.ui_json import InputFile
 
-from las_geoh5.import_las import las_to_drillhole
-
-
-def run(file: str):
-    ifile = InputFile.read_ui_json(file)
-    dh_group = ifile.data["drillhole_group"]
-    name = ifile.data["name"]
-    with fetch_active_workspace(ifile.data["geoh5"], mode="a") as workspace:
-        basepath = Path(ifile.path) / dh_group
-        import_las_directory(workspace, basepath, name)
 
-
-def import_las_directory(
-    workspace: Workspace, basepath: str | Path, name: str | None = None
-):
+def write_uijson(basepath: str | Path, mode: str = "import_files"):
     """
-    Import directory/files from previous export.
+    Write a ui.json file for either import or export or las files.
 
-    :param workspace: Project workspace.
     :param basepath: Root directory for las data.
-    :param name: Alternate name for property group to create.
+    :param mode: Switch for 'import' or 'export' behaviour.
 
-    :return: New drillhole group containing imported items.
+    :return: Input file for the written data.
     """
 
-    if isinstance(basepath, str):
-        basepath = Path(basepath)
-
-    if not basepath.exists():
-        raise OSError(f"Path {str(basepath)} does not exist.")
-
-    name = name if name is not None else basepath.name
-    dh_group = DrillholeGroup.create(workspace, name=name)
-
-    surveys_path = basepath / "Surveys"
-    surveys = list(surveys_path.iterdir()) if surveys_path.exists() else None
-
-    property_group_folders = [
-        p for p in basepath.iterdir() if p.is_dir() and p.name != "Surveys"
-    ]
-
-    for prop in property_group_folders:
-        lasfiles = []
-        for file in [k for k in prop.iterdir() if k.suffix == ".las"]:
-            lasfiles.append(lasio.read(file, mnemonic_case="preserve"))
-        print(f"Importing property group data from to {prop.name}")
-        las_to_drillhole(workspace, lasfiles, dh_group, prop.name, surveys)
-
-    return dh_group
+    if mode not in ["import_files", "import_directories", "export_files"]:
+        msg = "Mode argument must be 'import_files', 'import_directories', or 'export_files'."
+        raise ValueError(msg)
+
+    module = importlib.import_module(f"las_geoh5.{mode}.uijson")
+    ui_json = getattr(module, "ui_json")
+    filename = "_".join([mode.split("_")[0], "las", mode.split("_")[1]])
+
+    ifile = InputFile(ui_json=ui_json, validate=False)
+    ifile.path = str(basepath)
+    ifile.write_ui_json(filename, basepath)
+
+    return ifile
+
+
+def main(args):
+    parser = argparse.ArgumentParser(description="Write ui.json files.")
+    parser.add_argument(
+        "path", type=Path, help="Path to folder where ui.json files will be written."
+    )
+    parser.add_argument(
+        "mode",
+        type=str,
+        choices={"import_files", "import_directories", "export_files", "all"},
+        help=(
+            "Mode switching between 'import_files', 'import_directories',"
+            " 'export_files', and 'all' behaviour."
+        ),
+    )
+    args = parser.parse_args(args)
+    if args.mode == "all":
+        for mode in [
+            "import_files",
+            "import_directories",
+            "export_files",
+        ]:  # pylint: disable=invalid-name
+            write_uijson(args.path, mode)
+    else:
+        write_uijson(args.path, args.mode)
 
 
 if __name__ == "__main__":
-    run(sys.argv[1])
+    main(sys.argv[1:])
```

### Comparing `las_geoh5-0.1.0/las_geoh5/import_files/driver.py` & `las_geoh5-0.2.0a1/las_geoh5/import_files/driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
 #  las-geoh5 is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 #
 
@@ -17,23 +17,51 @@
 
 import lasio
 from geoh5py import Workspace
 from geoh5py.shared.utils import fetch_active_workspace
 from geoh5py.ui_json import InputFile
 from tqdm import tqdm
 
-from las_geoh5.import_las import LASTranslator, las_to_drillhole
+from las_geoh5.import_files.params import ImportOptions, NameOptions
+from las_geoh5.import_las import las_to_drillhole
 
-logger = logging.getLogger("Import Files")
-logger.setLevel(logging.INFO)
-stream_handler = logging.StreamHandler()
-stream_handler.setLevel(logging.INFO)
-formatter = logging.Formatter("%(asctime)s : %(name)s : %(levelname)s : %(message)s")
-stream_handler.setFormatter(formatter)
-logger.addHandler(stream_handler)
+
+def get_logger(
+    name: str, level: int = logging.INFO, path: str | Path | None = None
+) -> logging.Logger:
+    """
+    Create a looger with stream and optional file handlers.
+
+    :param name: Logger name.
+    :param level: logging level.
+    :param path: Creates a file handler at the specified path if not None.
+    :return: Logger object.
+    """
+    if isinstance(path, str):
+        path = Path(path)
+
+    logger = logging.getLogger(name)
+    logger.setLevel(level)
+    formatter = logging.Formatter(
+        "%(asctime)s : %(name)s : %(levelname)s : %(message)s"
+    )
+
+    stream_handler = logging.StreamHandler()
+    stream_handler.setFormatter(formatter)
+    stream_handler.setLevel(level)
+    logger.addHandler(stream_handler)
+
+    if path is not None:
+        filename = f"{'_'.join([k.lower() for k in name.split(' ')])}.log"
+        file_handler = logging.FileHandler(path / filename)
+        file_handler.setFormatter(formatter)
+        file_handler.setLevel(level)
+        logger.addHandler(file_handler)
+
+    return logger
 
 
 def elapsed_time_logger(start, end, message):
     if message[-1] != ".":
         message += "."
 
     elapsed = end - start
@@ -44,30 +72,24 @@
         out = f"{message} Time elapsed: {minutes}m {seconds}s."
     else:
         out = f"{message} Time elapsed: {seconds:.2f}s."
 
     return out
 
 
-def run(filepath: str):  # pylint: disable=too-many-locals
+def run(filepath: Path):  # pylint: disable=too-many-locals
     start = time()
     ifile = InputFile.read_ui_json(filepath)
 
+    logger = get_logger("Import Files", path=filepath.parent)
     logger.info(
         "Importing las file data to workspace %s.geoh5.",
         ifile.data["geoh5"].h5file.stem,
     )
 
-    translator = LASTranslator(
-        depth=ifile.data["depths_name"],
-        collar_x=ifile.data["collar_x_name"],
-        collar_y=ifile.data["collar_y_name"],
-        collar_z=ifile.data["collar_z_name"],
-    )
-
     workspace = Workspace()
     begin_reading = time()
 
     with Pool() as pool:
         futures = []
         for file in tqdm(ifile.data["files"].split(";"), desc="Reading las files"):
             futures.append(
@@ -87,28 +109,33 @@
 
     logger.info(
         "Saving drillhole data into drillhole group %s under property group %s",
         dh_group.name,
         ifile.data["name"],
     )
     begin_saving = time()
+
+    name_options = NameOptions(**ifile.data)
+    import_options = ImportOptions(names=name_options, **ifile.data)
     las_to_drillhole(
-        workspace,
         lasfiles,
         dh_group,
         ifile.data["name"],
-        translator=translator,
-        skip_empty_header=ifile.data["skip_empty_header"],
+        options=import_options,
     )
     end_saving = time()
     logger.info(
         elapsed_time_logger(begin_saving, end_saving, "Finished saving drillhole data")
     )
     end = time()
     logger.info(elapsed_time_logger(start, end, "All done."))
+    logpath = Path(logger.handlers[1].baseFilename)  # type: ignore
+    dh_group.add_file(logpath)
+    logger.handlers[1].close()
+    logpath.unlink()
 
     if ifile.data["monitoring_directory"]:
         working_path = Path(ifile.data["monitoring_directory"]) / ".working"
         working_path.mkdir(exist_ok=True)
         temp_geoh5 = f"temp{time():.3f}.geoh5"
         workspace.save_as(working_path / temp_geoh5)
         workspace.close()
@@ -122,8 +149,8 @@
         geoh5.h5file.unlink()
         workspace.save_as(geoh5_path)
 
     workspace.close()
 
 
 if __name__ == "__main__":
-    run(sys.argv[1])
+    run(Path(sys.argv[1]))
```

### Comparing `las_geoh5-0.1.0/las_geoh5/import_files/uijson.py` & `las_geoh5-0.2.0a1/las_geoh5/import_files/uijson.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,96 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
 #  las-geoh5 is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 #
 
 from copy import deepcopy
 
-from las_geoh5.export_directories.uijson import ui_json
+from geoh5py.ui_json.constants import default_ui_json
+
+# pylint: disable=duplicate-code
 
 ui_json = dict(
-    deepcopy(ui_json),
+    deepcopy(default_ui_json),
     **{
         "title": "LAS files to Drillhole group",
         "run_command": "las_geoh5.import_files.driver",
-        "name": {
+        "conda_environment": "las-geoh5",
+        "drillhole_group": {
             "main": True,
-            "label": "Name",
-            "value": "",
+            "label": "Drillhole group",
+            "value": None,
+            "groupType": ["{825424fb-c2c6-4fea-9f2b-6cd00023d393}"],
         },
         "files": {
             "main": True,
             "label": "Files",
             "value": None,
             "fileDescription": ["LAS files"],
             "fileType": ["las"],
             "fileMulti": True,
         },
-        "depths_name": {
-            "label": "Depths",
-            "value": "DEPTH",
-            "group": "Import fields",
-            "optional": True,
-            "enabled": False,
+        "name": {
+            "main": True,
+            "label": "Property group name",
+            "group": "Property group",
+            "value": "",
+        },
+        "collocation_tolerance": {
+            "main": True,
+            "label": "Collocation tolerance",
+            "group": "Property group",
+            "value": 0.01,
+            "tooltip": (
+                "Tolerance for determining collocation of data locations "
+                "and ultimately deciding if incoming data should belong to "
+                "an existing property group.",
+            ),
         },
         "collar_x_name": {
-            "label": "Collar x",
+            "main": True,
+            "label": "Easting",
+            "tooltip": "Name of header field containing the collar easting.",
             "value": "X",
-            "group": "Import fields",
+            "group": "Collar",
             "optional": True,
             "enabled": False,
         },
         "collar_y_name": {
-            "label": "Collar y",
+            "main": True,
+            "label": "Northing",
+            "tooltip": "Name of header field containing the collar northing.",
             "value": "Y",
-            "group": "Import fields",
+            "group": "Collar",
             "optional": True,
             "enabled": False,
         },
         "collar_z_name": {
-            "label": "Collar z",
+            "main": True,
+            "tooltip": "Name of header field containing the collar elevation.",
+            "label": "Elevation",
             "value": "ELEV",
-            "group": "Import fields",
+            "group": "Collar",
             "optional": True,
             "enabled": False,
         },
         "skip_empty_header": {
+            "main": True,
             "label": "Skip empty header",
             "value": False,
             "tooltip": (
                 "Importing files without collar information "
                 "results in drillholes placed at the origin. "
                 "Check this box to skip these files."
-                ""
             ),
         },
+        "warnings": {
+            "main": True,
+            "label": "Warnings",
+            "value": True,
+            "tooltip": "Show warnings during import.",
+        },
     }
 )
```

### Comparing `las_geoh5-0.1.0/las_geoh5/import_las.py` & `las_geoh5-0.2.0a1/las_geoh5/import_las.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,69 @@
-#  Copyright (c) 2023 Mira Geoscience Ltd.
+#  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of las-geoh5 project.
 #
 #  las-geoh5 is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 #
 
 from __future__ import annotations
 
-import warnings
+import logging
 from pathlib import Path
 from typing import Any
 
 import lasio
 import numpy as np
 from geoh5py import Workspace
 from geoh5py.groups import DrillholeGroup
-from geoh5py.objects import Drillhole
+from geoh5py.objects import Drillhole, ObjectBase
 from geoh5py.shared import Entity
+from geoh5py.shared.concatenation import ConcatenatedDrillhole
 from tqdm import tqdm
 
+from las_geoh5.import_files.params import ImportOptions, NameOptions
+
 
 class LASTranslator:
     """Translator for the weakly standardized LAS file standard."""
 
-    las_geoh5_standard = {
-        "well": "WELL",
-        "depth": "DEPTH",
-        "collar_x": "X",
-        "collar_y": "Y",
-        "collar_z": "ELEV",
-    }
-
-    def __init__(
-        self,
-        well: str = las_geoh5_standard["well"],
-        depth: str = las_geoh5_standard["depth"],
-        collar_x: str = las_geoh5_standard["collar_x"],
-        collar_y: str = las_geoh5_standard["collar_y"],
-        collar_z: str = las_geoh5_standard["collar_z"],
-    ):
-        self.well = well
-        self.depth = depth
-        self.collar_x = collar_x
-        self.collar_y = collar_y
-        self.collar_z = collar_z
+    def __init__(self, names: NameOptions):
+        self.names = names
 
     def translate(self, field: str):
         """
         Return translated field name or rais KeyError if field not recognized.
 
         :param field: Standardized field name.
+
         :return: Name of corresponding field in las file.
         """
-        if field not in self.las_geoh5_standard:
+        if field not in dict(self.names):
             raise KeyError(f"'{field}' is not a recognized field.")
 
-        return getattr(self, field)
+        return getattr(self.names, field)
 
-    def retrieve(self, field, lasfile):
+    def retrieve(self, field: str, lasfile: lasio.LASFile):
         """
         Access las data using translation.
 
         :param field: Name of field to retrieve.
         :param lasfile: lasio file object.
+
         :return: data stored in las file under translated field name.
         """
-        if getattr(self, field) in lasfile.well:
-            out = lasfile.well[getattr(self, field)].value
-        elif getattr(self, field) in lasfile.curves:
-            out = lasfile.curves[getattr(self, field)].data
-        elif getattr(self, field) in lasfile.params:
-            out = lasfile.params[getattr(self, field)].value
+        if getattr(self.names, field) in lasfile.well:
+            out = lasfile.well[getattr(self.names, field)].value
+        elif getattr(self.names, field) in lasfile.curves:
+            out = lasfile.curves[getattr(self.names, field)].data
+        elif getattr(self.names, field) in lasfile.params:
+            out = lasfile.params[getattr(self.names, field)].value
         else:
-            msg = f"'{field}' field: '{getattr(self, field)}' not found in las file."
+            msg = f"'{field}' field: '{getattr(self.names, field)}' not found in las file."
             raise KeyError(msg)
 
         return out
 
 
 def get_depths(lasfile: lasio.LASFile) -> dict[str, np.ndarray]:
     """
@@ -106,167 +92,165 @@
         out["from-to"] = np.c_[depths, tos]
     else:
         out["depth"] = depths
 
     return out
 
 
-def get_collar(lasfile: lasio.LASFile, translator: LASTranslator | None = None) -> list:
+def get_collar(
+    lasfile: lasio.LASFile,
+    translator: LASTranslator | None = None,
+    logger: logging.Logger | None = None,
+) -> list:
     """
     Returns collar data from las file or None if data missing.
 
     :param lasfile: Las file object.
+    :param translator: Translator for las file.
+    :param logger: Logger object if warnings are enabled.
 
     :return: Collar data.
     """
 
     if translator is None:
-        translator = LASTranslator()
+        translator = LASTranslator(names=NameOptions())
 
     collar = []
-    for field in ["collar_x", "collar_y", "collar_z"]:
+    for field in ["collar_x_name", "collar_y_name", "collar_z_name"]:
         collar_coord = 0.0
         try:
             collar_coord = translator.retrieve(field, lasfile)
         except KeyError:
             exclusions = ["STRT", "STOP", "STEP", "NULL"]
             options = [
                 k.mnemonic
                 for k in lasfile.well
                 if k.value and k.mnemonic not in exclusions
             ]
-            warnings.warn(
-                f"{field.replace('_', ' ').capitalize()} field "
-                f"'{getattr(translator, field)}' not found in las file."
-                f" Setting coordinate to 0.0. Non-null header fields include: "
-                f"{options}."
-            )
+            if logger is not None:
+                logger.warning(
+                    f"{field.replace('_', ' ').capitalize()} field "
+                    f"'{getattr(translator.names, field)}' not found in las file."
+                    f" Setting coordinate to 0.0. Non-null header fields include: "
+                    f"{options}."
+                )
 
             collar_coord = 0.0
 
         try:
             collar.append(float(collar_coord))
         except ValueError:
             collar.append(0.0)
 
     return collar
 
 
-def find_copy_name(workspace: Workspace, basename: str, start: int = 1):
+def find_copy_name(obj: Workspace | ObjectBase, basename: str, start: int = 0):
     """
     Augment name with increasing integer value until no entities found.
 
-    :param workspace: A geoh5py.Workspace object.
+    :param obj: A geoh5py object or workspace.
     :param basename: Existing name of entity in workspace.
-    :param start: Integer name augmenter to test for existence.
+    :param start: Integer name augmenter to test for existence.  Default is
+        0 and does not add a suffix
 
-    :returns: Augmented name of the earliest non-existent copy in workspace.
+    :returns: Suffix name of the earliest non-existent copy in workspace.
     """
 
-    name = f"{basename} ({start})"
-    obj = workspace.get_entity(name)
-    if obj and obj[0] is not None:
-        find_copy_name(workspace, basename, start=start + 1)
+    name = basename if start == 0 else f"{basename} ({start})"
+    child = obj.get_entity(name)
+    if child and child[0] is not None:
+        name = find_copy_name(obj, basename, start=start + 1)
     return name
 
 
-def add_survey(survey: str | Path, drillhole: Drillhole) -> Drillhole:
+def add_survey(
+    survey: str | Path,
+    drillhole: ConcatenatedDrillhole,
+    logger: logging.Logger | None = None,
+) -> ConcatenatedDrillhole:
     """
     Import survey data from csv or las format and add to drillhole.
 
     :param survey: Path to a survey file stored as .csv or .las format.
     :param drillhole: Drillhole object to append data to.
+    :param logger: logger object if warning are enabled.
 
     :return: Updated drillhole object.
     """
 
     if isinstance(survey, str):
         survey = Path(survey)
 
     if survey.suffix == ".las":
         file = lasio.read(survey, mnemonic_case="preserve")
         try:
             surveys = np.c_[get_depths(file)["depth"], file["DIP"], file["AZIM"]]
             if len(drillhole.surveys) == 1:
                 drillhole.surveys = surveys
         except KeyError:
-            warnings.warn(
-                "Attempted survey import failed because data read from "
-                ".las file did not contain the expected 3 curves 'DEPTH'"
-                ", 'DIP', 'AZIM'."
-            )
+            if logger is not None:
+                logger.warning(
+                    "Attempted survey import failed because data read from "
+                    ".las file did not contain the expected 3 curves 'DEPTH'"
+                    ", 'DIP', 'AZIM'."
+                )
     else:
         surveys = np.genfromtxt(survey, delimiter=",", skip_header=0)
         if surveys.shape[1] == 3:
             drillhole.surveys = surveys
         else:
-            warnings.warn(
-                "Attempted survey import failed because data read from "
-                "comma separated file did not contain the expected 3 "
-                "columns of depth/dip/azimuth."
-            )
+            if logger is not None:
+                logger.warning(
+                    "Attempted survey import failed because data read from "
+                    "comma separated file did not contain the expected 3 "
+                    "columns of depth/dip/azimuth."
+                )
 
     return drillhole
 
 
 def add_data(
-    drillhole: Drillhole,
+    drillhole: ConcatenatedDrillhole,
     lasfile: lasio.LASFile,
     group_name: str,
-) -> Drillhole:
+    collocation_tolerance: float = 0.01,
+) -> ConcatenatedDrillhole:
     """
     Add data from las file curves to drillhole.
 
     :param drillhole: Drillhole object to append data to.
     :param lasfile: Las file object.
-    :param property_group: Property group.
+    :param group_name: Property group name.
+    :param collocation_tolerance: Tolerance for determining collocation of data.
 
     :return: Updated drillhole object.
     """
 
     depths = get_depths(lasfile)
+    property_group_kwargs = {}
     if "depth" in depths:
-        method_name = "validate_depth_data"
         locations = depths["depth"]
+        property_group_kwargs["property_group_type"] = "Depth table"
+        property_group_kwargs["association"] = "DEPTH"
     else:
-        method_name = "validate_interval_data"
         locations = depths["from-to"]
-
-    try:
-        property_group = getattr(drillhole, method_name)(
-            "noname",
-            locations,
-            np.zeros_like(locations),
-            property_group=group_name,
-            collocation_distance=1e-4,
-        )
-    except ValueError as err:
-        msg = (
-            f"validate_depth_data call failed with message:\n{err.args[0]}. "
-            f"Skipping import for drillhole {drillhole.name}."
-        )
-        warnings.warn(msg)
-
-        # TODO: Increment property group name if it already exists and the depth
-        # Sampling is different.  Could try removing the try/except block once
-        # done and see if error start to appear.
-
-        return drillhole
+        property_group_kwargs["property_group_type"] = "Interval table"
+        property_group_kwargs["association"] = "FROM-TO"
 
     kwargs: dict[str, Any] = {}
-    for curve in tqdm(
-        [k for k in lasfile.curves if k.mnemonic not in ["DEPT", "DEPTH", "TO"]]
-    ):
+    for curve in [
+        k for k in lasfile.curves if k.mnemonic not in ["DEPT", "DEPTH", "TO"]
+    ]:
         name = curve.mnemonic
         if drillhole.get_data(name):
-            msg = f"Drillhole '{drillhole.name}' already contains '{name}' data"
-            warnings.warn(msg)
-            continue
+            name = find_copy_name(drillhole, name)
 
         kwargs[name] = {"values": curve.data, "association": "DEPTH"}
+        kwargs[name].update(depths)
 
         is_referenced = any(name in k.mnemonic for k in lasfile.params)
         is_referenced &= any(k.descr == "REFERENCE" for k in lasfile.params)
         if is_referenced:
             kwargs[name]["values"] = kwargs[name]["values"].astype(int)
             value_map = {
                 k.mnemonic: k.value for k in lasfile.params if name in k.mnemonic
@@ -275,104 +259,137 @@
             kwargs[name]["value_map"] = value_map
             kwargs[name]["type"] = "referenced"
 
         existing_data = drillhole.workspace.get_entity(name)[0]
         if existing_data and isinstance(existing_data, Entity):
             kwargs[name]["entity_type"] = existing_data.entity_type
 
-    drillhole.add_data(kwargs, property_group=property_group)
+    if kwargs:
+        if drillhole.property_groups is not None:
+            root_name_matches = [
+                g for g in drillhole.property_groups if group_name in g.name
+            ]
+            if root_name_matches:
+                group = [
+                    g
+                    for g in root_name_matches
+                    if g.is_collocated(locations, collocation_tolerance)
+                ]
+                if group:
+                    group_name = group[0].name
+                else:
+                    group_name = find_copy_name(drillhole.workspace, group_name)
+
+        drillhole.add_data(kwargs, property_group=group_name)
 
     return drillhole
 
 
 def create_or_append_drillhole(
-    workspace: Workspace,
     lasfile: lasio.LASFile,
     drillhole_group: DrillholeGroup,
     group_name: str,
     translator: LASTranslator | None = None,
-) -> Drillhole:
+    collocation_tolerance: float = 0.01,
+    logger: logging.Logger | None = None,
+) -> ConcatenatedDrillhole:
     """
     Create a drillhole or append data to drillhole if it exists in workspace.
 
-    :param workspace: Project workspace opened with read/write access.
     :param lasfile: Las file object.
     :param drillhole_group: Drillhole group container.
     :param group_name: Property group name.
     :param translator: Translator for las file.
+    :param collocation_tolerance: Tolerance for determining collocation of data.
+    :param logger: Logger object if warnings are enabled.
 
     :return: Created or augmented drillhole.
     """
 
     if translator is None:
-        translator = LASTranslator()
+        translator = LASTranslator(NameOptions())
+
+    name = translator.retrieve("well_name", lasfile)
+    if not name and logger is not None:
+        logger.warning(
+            "No well name provided for las file. "
+            "Saving drillhole with name 'Unknown'."
+        )
 
-    name = translator.retrieve("well", lasfile)
-    collar = get_collar(lasfile, translator)
+    collar = get_collar(lasfile, translator, logger)
     drillhole = drillhole_group.get_entity(name)[0]  # type: ignore
 
     if not isinstance(drillhole, Drillhole) or (
         isinstance(drillhole, Drillhole)
         and not np.allclose(collar, drillhole.collar.tolist())
     ):
-        name = name if drillhole is None else find_copy_name(workspace, name)
+        name = find_copy_name(drillhole_group.workspace, name)
         kwargs = {
             "name": name,
             "parent": drillhole_group,
         }
         if collar:
             kwargs["collar"] = collar
 
-        drillhole = Drillhole.create(workspace, **kwargs)
+        drillhole = Drillhole.create(drillhole_group.workspace, **kwargs)
 
-    if not isinstance(drillhole, Drillhole):
+    if not isinstance(drillhole, ConcatenatedDrillhole):
         raise TypeError(
             f"Drillhole {name} exists in workspace but is not a Drillhole object."
         )
 
-    drillhole = add_data(drillhole, lasfile, group_name)
+    drillhole = add_data(
+        drillhole, lasfile, group_name, collocation_tolerance=collocation_tolerance
+    )
 
     return drillhole
 
 
-def las_to_drillhole(  # pylint: disable=too-many-arguments
-    workspace: Workspace,
+def las_to_drillhole(
     data: lasio.LASFile | list[lasio.LASFile],
     drillhole_group: DrillholeGroup,
     property_group: str,
     survey: Path | list[Path] | None = None,
-    translator: LASTranslator | None = None,
-    skip_empty_header: bool = False,
+    logger: logging.Logger | None = None,
+    options: ImportOptions | None = None,
 ):
     """
     Import a las file containing collocated datasets for a single drillhole.
 
-    :param workspace: Project workspace.
     :param data: Las file(s) containing drillhole data.
     :param drillhole_group: Drillhole group container.
     :param property_group: Property group name.
     :param survey: Path to a survey file stored as .csv or .las format.
-    :param translator: Translator for las file.
-    :param skip_empty_header: Skip empty header data.
+    :param logger: Logger object if warnings are enabled.
+    :param options: Import options covering name translations, collocation
+        tolerance, and warnings control.
 
     :return: A :obj:`geoh5py.objects.Drillhole` object
     """
 
+    if options is None:
+        options = ImportOptions()
+
+    translator = LASTranslator(names=options.names)
+
     if not isinstance(data, list):
         data = [data]
     if not isinstance(survey, list):
         survey = [survey] if survey else []
-    if translator is None:
-        translator = LASTranslator()
 
-    for datum in data:
-        collar = get_collar(datum, translator)
-        if all(k == 0 for k in collar) and skip_empty_header:
+    for datum in tqdm(data, desc="Adding drillholes and data to workspace"):
+        collar = get_collar(datum, translator, logger)
+        if all(k == 0 for k in collar) and options.skip_empty_header:
             continue
 
         drillhole = create_or_append_drillhole(
-            workspace, datum, drillhole_group, property_group, translator=translator
+            datum,
+            drillhole_group,
+            property_group,
+            translator=translator,
+            logger=logger,
+            collocation_tolerance=options.collocation_tolerance,
         )
         ind = [drillhole.name == s.name.rstrip(".las") for s in survey]
         if any(ind):
             survey_path = survey[np.where(ind)[0][0]]
-            _ = add_survey(survey_path, drillhole)
+            _ = add_survey(survey_path, drillhole, logger)
```

### Comparing `las_geoh5-0.1.0/las_geoh5/uijson/export_las_directories.ui.json` & `las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_directories.ui.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7215909090909091%*

 * *Differences: {"'parent_folder'": "OrderedDict([('main', True), ('label', 'Directory'), ('value', ''), "*

 * *                    "('fileDescription', ['Directory']), ('fileType', ['directory']), "*

 * *                    "('directoryOnly', True), ('fileMulti', False)])",*

 * * "'run_command'": "'las_geoh5.import_directories.driver'",*

 * * "'run_command_boolean'": "{'label': 'Run python module '}",*

 * * "'title'": "'LAS file directories to Drillhole group'",*

 * * 'delete': "['name']"}*

```diff
@@ -7,24 +7,30 @@
         ],
         "label": "Drillhole group",
         "main": true,
         "value": ""
     },
     "geoh5": "",
     "monitoring_directory": "",
-    "name": {
-        "enabled": false,
-        "label": "Property group name",
+    "parent_folder": {
+        "directoryOnly": true,
+        "fileDescription": [
+            "Directory"
+        ],
+        "fileMulti": false,
+        "fileType": [
+            "directory"
+        ],
+        "label": "Directory",
         "main": true,
-        "optional": true,
         "value": ""
     },
-    "run_command": "las_geoh5.export_directories.driver",
+    "run_command": "las_geoh5.import_directories.driver",
     "run_command_boolean": {
-        "label": "Run python module",
+        "label": "Run python module ",
         "main": true,
         "tooltip": "Warning: launches process to run python model on save",
         "value": false
     },
-    "title": "Drillhole group to LAS file directories",
+    "title": "LAS file directories to Drillhole group",
     "workspace": ""
 }
```

### Comparing `las_geoh5-0.1.0/las_geoh5/uijson/import_las_directories.ui.json` & `las_geoh5-0.2.0a1/las_geoh5/import_directories/uijson.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,67 @@
-00000000: 7b0d 0a20 2020 2022 7469 746c 6522 3a20  {..    "title": 
-00000010: 224c 4153 2066 696c 6520 6469 7265 6374  "LAS file direct
-00000020: 6f72 6965 7320 746f 2044 7269 6c6c 686f  ories to Drillho
-00000030: 6c65 2067 726f 7570 222c 0d0a 2020 2020  le group",..    
-00000040: 2267 656f 6835 223a 2022 222c 0d0a 2020  "geoh5": "",..  
-00000050: 2020 2272 756e 5f63 6f6d 6d61 6e64 223a    "run_command":
-00000060: 2022 6c61 735f 6765 6f68 352e 696d 706f   "las_geoh5.impo
-00000070: 7274 5f64 6972 6563 746f 7269 6573 2e64  rt_directories.d
-00000080: 7269 7665 7222 2c0d 0a20 2020 2022 7275  river",..    "ru
-00000090: 6e5f 636f 6d6d 616e 645f 626f 6f6c 6561  n_command_boolea
-000000a0: 6e22 3a20 7b0d 0a20 2020 2020 2020 2022  n": {..        "
-000000b0: 7661 6c75 6522 3a20 6661 6c73 652c 0d0a  value": false,..
-000000c0: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-000000d0: 2022 5275 6e20 7079 7468 6f6e 206d 6f64   "Run python mod
-000000e0: 756c 6522 2c0d 0a20 2020 2020 2020 2022  ule",..        "
-000000f0: 6d61 696e 223a 2074 7275 652c 0d0a 2020  main": true,..  
-00000100: 2020 2020 2020 2274 6f6f 6c74 6970 223a        "tooltip":
-00000110: 2022 5761 726e 696e 673a 206c 6175 6e63   "Warning: launc
-00000120: 6865 7320 7072 6f63 6573 7320 746f 2072  hes process to r
-00000130: 756e 2070 7974 686f 6e20 6d6f 6465 6c20  un python model 
-00000140: 6f6e 2073 6176 6522 0d0a 2020 2020 7d2c  on save"..    },
-00000150: 0d0a 2020 2020 226d 6f6e 6974 6f72 696e  ..    "monitorin
-00000160: 675f 6469 7265 6374 6f72 7922 3a20 2222  g_directory": ""
-00000170: 2c0d 0a20 2020 2022 636f 6e64 615f 656e  ,..    "conda_en
-00000180: 7669 726f 6e6d 656e 7422 3a20 226c 6173  vironment": "las
-00000190: 2d67 656f 6835 222c 0d0a 2020 2020 2263  -geoh5",..    "c
-000001a0: 6f6e 6461 5f65 6e76 6972 6f6e 6d65 6e74  onda_environment
-000001b0: 5f62 6f6f 6c65 616e 223a 2066 616c 7365  _boolean": false
-000001c0: 2c0d 0a20 2020 2022 776f 726b 7370 6163  ,..    "workspac
-000001d0: 6522 3a20 2222 2c0d 0a20 2020 2022 6472  e": "",..    "dr
-000001e0: 696c 6c68 6f6c 655f 6772 6f75 7022 3a20  illhole_group": 
-000001f0: 7b0d 0a20 2020 2020 2020 2022 6d61 696e  {..        "main
-00000200: 223a 2074 7275 652c 0d0a 2020 2020 2020  ": true,..      
-00000210: 2020 226c 6162 656c 223a 2022 4472 696c    "label": "Dril
-00000220: 6c68 6f6c 6520 6772 6f75 7022 2c0d 0a20  lhole group",.. 
-00000230: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00000240: 2222 2c0d 0a20 2020 2020 2020 2022 6772  "",..        "gr
-00000250: 6f75 7054 7970 6522 3a20 5b0d 0a20 2020  oupType": [..   
-00000260: 2020 2020 2020 2020 2022 7b38 3235 3432           "{82542
-00000270: 3466 622d 6332 6336 2d34 6665 612d 3966  4fb-c2c6-4fea-9f
-00000280: 3262 2d36 6364 3030 3032 3364 3339 337d  2b-6cd00023d393}
-00000290: 220d 0a20 2020 2020 2020 205d 0d0a 2020  "..        ]..  
-000002a0: 2020 7d2c 0d0a 2020 2020 226e 616d 6522    },..    "name"
-000002b0: 3a20 7b0d 0a20 2020 2020 2020 2022 6d61  : {..        "ma
-000002c0: 696e 223a 2074 7275 652c 0d0a 2020 2020  in": true,..    
-000002d0: 2020 2020 226c 6162 656c 223a 2022 5072      "label": "Pr
-000002e0: 6f70 6572 7479 2067 726f 7570 206e 616d  operty group nam
-000002f0: 6522 2c0d 0a20 2020 2020 2020 2022 7661  e",..        "va
-00000300: 6c75 6522 3a20 2222 2c0d 0a20 2020 2020  lue": "",..     
-00000310: 2020 2022 6f70 7469 6f6e 616c 223a 2074     "optional": t
-00000320: 7275 652c 0d0a 2020 2020 2020 2020 2265  rue,..        "e
-00000330: 6e61 626c 6564 223a 2066 616c 7365 0d0a  nabled": false..
-00000340: 2020 2020 7d0d 0a7d 0d0a                     }..}..
+00000000: 2320 2043 6f70 7972 6967 6874 2028 6329  #  Copyright (c)
+00000010: 2032 3032 3420 4d69 7261 2047 656f 7363   2024 Mira Geosc
+00000020: 6965 6e63 6520 4c74 642e 0d0a 230d 0a23  ience Ltd...#..#
+00000030: 2020 5468 6973 2066 696c 6520 6973 2070    This file is p
+00000040: 6172 7420 6f66 206c 6173 2d67 656f 6835  art of las-geoh5
+00000050: 2070 726f 6a65 6374 2e0d 0a23 0d0a 2320   project...#..# 
+00000060: 206c 6173 2d67 656f 6835 2069 7320 6469   las-geoh5 is di
+00000070: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00000080: 7468 6520 7465 726d 7320 616e 6420 636f  the terms and co
+00000090: 6e64 6974 696f 6e73 206f 6620 7468 6520  nditions of the 
+000000a0: 4d49 5420 4c69 6365 6e73 650d 0a23 2020  MIT License..#  
+000000b0: 2873 6565 204c 4943 454e 5345 2066 696c  (see LICENSE fil
+000000c0: 6520 6174 2074 6865 2072 6f6f 7420 6f66  e at the root of
+000000d0: 2074 6869 7320 736f 7572 6365 2063 6f64   this source cod
+000000e0: 6520 7061 636b 6167 6529 2e0d 0a23 0d0a  e package)...#..
+000000f0: 0d0a 6672 6f6d 2063 6f70 7920 696d 706f  ..from copy impo
+00000100: 7274 2064 6565 7063 6f70 790d 0a0d 0a66  rt deepcopy....f
+00000110: 726f 6d20 6765 6f68 3570 792e 7569 5f6a  rom geoh5py.ui_j
+00000120: 736f 6e2e 636f 6e73 7461 6e74 7320 696d  son.constants im
+00000130: 706f 7274 2064 6566 6175 6c74 5f75 695f  port default_ui_
+00000140: 6a73 6f6e 0d0a 0d0a 7569 5f6a 736f 6e20  json....ui_json 
+00000150: 3d20 6469 6374 280d 0a20 2020 2064 6565  = dict(..    dee
+00000160: 7063 6f70 7928 6465 6661 756c 745f 7569  pcopy(default_ui
+00000170: 5f6a 736f 6e29 2c0d 0a20 2020 202a 2a7b  _json),..    **{
+00000180: 0d0a 2020 2020 2020 2020 2274 6974 6c65  ..        "title
+00000190: 223a 2022 4c41 5320 6669 6c65 2064 6972  ": "LAS file dir
+000001a0: 6563 746f 7269 6573 2074 6f20 4472 696c  ectories to Dril
+000001b0: 6c68 6f6c 6520 6772 6f75 7022 2c0d 0a20  lhole group",.. 
+000001c0: 2020 2020 2020 2022 7275 6e5f 636f 6d6d         "run_comm
+000001d0: 616e 6422 3a20 226c 6173 5f67 656f 6835  and": "las_geoh5
+000001e0: 2e69 6d70 6f72 745f 6469 7265 6374 6f72  .import_director
+000001f0: 6965 732e 6472 6976 6572 222c 0d0a 2020  ies.driver",..  
+00000200: 2020 2020 2020 2263 6f6e 6461 5f65 6e76        "conda_env
+00000210: 6972 6f6e 6d65 6e74 223a 2022 6c61 732d  ironment": "las-
+00000220: 6765 6f68 3522 2c0d 0a20 2020 2020 2020  geoh5",..       
+00000230: 2022 6472 696c 6c68 6f6c 655f 6772 6f75   "drillhole_grou
+00000240: 7022 3a20 7b0d 0a20 2020 2020 2020 2020  p": {..         
+00000250: 2020 2022 6d61 696e 223a 2054 7275 652c     "main": True,
+00000260: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+00000270: 6162 656c 223a 2022 4472 696c 6c68 6f6c  abel": "Drillhol
+00000280: 6520 6772 6f75 7022 2c0d 0a20 2020 2020  e group",..     
+00000290: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000002a0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+000002b0: 2020 2022 6772 6f75 7054 7970 6522 3a20     "groupType": 
+000002c0: 5b22 7b38 3235 3432 3466 622d 6332 6336  ["{825424fb-c2c6
+000002d0: 2d34 6665 612d 3966 3262 2d36 6364 3030  -4fea-9f2b-6cd00
+000002e0: 3032 3364 3339 337d 225d 2c0d 0a20 2020  023d393}"],..   
+000002f0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
+00000300: 2022 7061 7265 6e74 5f66 6f6c 6465 7222   "parent_folder"
+00000310: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00000320: 2022 6d61 696e 223a 2054 7275 652c 0d0a   "main": True,..
+00000330: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+00000340: 656c 223a 2022 4469 7265 6374 6f72 7922  el": "Directory"
+00000350: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000360: 7661 6c75 6522 3a20 4e6f 6e65 2c0d 0a20  value": None,.. 
+00000370: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+00000380: 4465 7363 7269 7074 696f 6e22 3a20 5b22  Description": ["
+00000390: 4469 7265 6374 6f72 7922 5d2c 0d0a 2020  Directory"],..  
+000003a0: 2020 2020 2020 2020 2020 2266 696c 6554            "fileT
+000003b0: 7970 6522 3a20 5b22 6469 7265 6374 6f72  ype": ["director
+000003c0: 7922 5d2c 0d0a 2020 2020 2020 2020 2020  y"],..          
+000003d0: 2020 2264 6972 6563 746f 7279 4f6e 6c79    "directoryOnly
+000003e0: 223a 2054 7275 652c 0d0a 2020 2020 2020  ": True,..      
+000003f0: 2020 2020 2020 2266 696c 654d 756c 7469        "fileMulti
+00000400: 223a 2046 616c 7365 2c0d 0a20 2020 2020  ": False,..     
+00000410: 2020 207d 2c0d 0a20 2020 207d 0d0a 290d     },..    }..).
+00000420: 0a                                       .
```

### Comparing `las_geoh5-0.1.0/las_geoh5/uijson/import_las_files.ui.json` & `las_geoh5-0.2.0a1/las_geoh5_assets/uijson/import_las_files.ui.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.77609126984127%*

 * *Differences: {"'collar_x_name'": "{'label': 'Easting', 'group': 'Collar', 'main': True, 'tooltip': 'Name of "*

 * *                    "header field containing the collar easting.'}",*

 * * "'collar_y_name'": "{'label': 'Northing', 'group': 'Collar', 'main': True, 'tooltip': 'Name of "*

 * *                    "header field containing the collar northing.'}",*

 * * "'collar_z_name'": "{'label': 'Elevation', 'group': 'Collar', 'main': True, 'tooltip': 'Name of "*

 * *                    "header field containing the collar elevation.'}",*

 * * "'collo […]*

```diff
@@ -1,38 +1,46 @@
 {
     "collar_x_name": {
         "enabled": false,
-        "group": "Import fields",
-        "label": "Collar x",
+        "group": "Collar",
+        "label": "Easting",
+        "main": true,
         "optional": true,
+        "tooltip": "Name of header field containing the collar easting.",
         "value": "X"
     },
     "collar_y_name": {
         "enabled": false,
-        "group": "Import fields",
-        "label": "Collar y",
+        "group": "Collar",
+        "label": "Northing",
+        "main": true,
         "optional": true,
+        "tooltip": "Name of header field containing the collar northing.",
         "value": "Y"
     },
     "collar_z_name": {
         "enabled": false,
-        "group": "Import fields",
-        "label": "Collar z",
+        "group": "Collar",
+        "label": "Elevation",
+        "main": true,
         "optional": true,
+        "tooltip": "Name of header field containing the collar elevation.",
         "value": "ELEV"
     },
+    "collocation_tolerance": {
+        "group": "Property group",
+        "label": "Collocation tolerance",
+        "main": true,
+        "tooltip": [
+            "Tolerance for determining collocation of data locations and ultimately deciding if incoming data should belong to an existing property group."
+        ],
+        "value": 0.01
+    },
     "conda_environment": "las-geoh5",
     "conda_environment_boolean": false,
-    "depths_name": {
-        "enabled": false,
-        "group": "Import fields",
-        "label": "Depths",
-        "optional": true,
-        "value": "DEPTH"
-    },
     "drillhole_group": {
         "groupType": [
             "{825424fb-c2c6-4fea-9f2b-6cd00023d393}"
         ],
         "label": "Drillhole group",
         "main": true,
         "value": ""
@@ -48,26 +56,35 @@
         "label": "Files",
         "main": true,
         "value": ""
     },
     "geoh5": "",
     "monitoring_directory": "",
     "name": {
-        "label": "Name",
+        "group": "Property group",
+        "label": "Property group name",
         "main": true,
         "value": ""
     },
     "run_command": "las_geoh5.import_files.driver",
     "run_command_boolean": {
         "label": "Run python module",
         "main": true,
         "tooltip": "Warning: launches process to run python model on save",
         "value": false
     },
     "skip_empty_header": {
+        "group": "Collar",
         "label": "Skip empty header",
+        "main": true,
         "tooltip": "Importing files without collar information results in drillholes placed at the origin. Check this box to skip these files.",
         "value": false
     },
     "title": "LAS files to Drillhole group",
+    "warnings": {
+        "label": "Warnings",
+        "main": true,
+        "tooltip": "Show warnings during import.",
+        "value": true
+    },
     "workspace": ""
 }
```

### Comparing `las_geoh5-0.1.0/LICENSE.txt` & `las_geoh5-0.2.0a1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Mira Geoscience
+Copyright (c) 2024 Mira Geoscience
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `las_geoh5-0.1.0/pyproject.toml` & `las_geoh5-0.2.0a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tool.poetry]
 name = "las-geoh5"
-version = "0.1.0"
+version = "0.2.0-alpha.1"
 description = "Las/Geoh5 conversion"
 license = "MIT"
 readme = "README.rst"
 homepage = "https://mirageoscience.com"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 keywords = ["geology", "geophysics", "earth sciences", "io", "data", "interoperability"]
+packages = [
+    { include = "las_geoh5" },
+    { include = "las_geoh5_assets" },
+]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
@@ -18,29 +22,33 @@
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9, <3.11"
+python = "^3.10, <3.11"
+pydantic = "~2.5"
 
 ## dependencies on github repos
-#geoh5py = { url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.8.0.zip#sha256=" }
-geoh5py = {version ="~0.8.0rc3", allow-prereleases = true}
+#geoh5py = {git = "https://github.com/MiraGeoscience/geoh5py.git", branch = "release/0.9.0"}
+geoh5py = {version ="~0.9.0-alpha.4", allow-prereleases = true}
 
 ## pip dependencies
 lasio = "~0.31"
 tqdm = "^4.64.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 tomli = "*"
+sphinx = "*"
+sphinx-autodoc-typehints = "*"
+sphinx-rtd-theme = "*"
 
 [tool.isort]
 # settings for compatibility between ``isort`` and ``black`` formatting
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
@@ -57,32 +65,27 @@
 show_column_numbers = true
 check_untyped_defs = true
 
 plugins = [
     #    'numpy.typing.mypy_plugin'
 ]
 
-[tool.pytest.ini_options]
-addopts = "--cov las_geoh5 --cov-report html --cov-report term-missing:skip-covered"
-
 [tool.coverage.run]
 branch = true
 source = ["las_geoh5"]
 omit = []
 
 [tool.coverage.report]
 exclude_lines = [
     "raise NotImplementedError",
     "pass",
     "if TYPE_CHECKING",
     "pragma: no cover"
 ]
 
-fail_under = 80
-
 [tool.coverage.html]
 skip_empty = true
 skip_covered = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

