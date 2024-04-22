# Comparing `tmp/np_aind_metadata-0.1.3.tar.gz` & `tmp/np_aind_metadata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_aind_metadata-0.1.3.tar", last modified: Thu Apr 18 00:35:41 2024, max compression
+gzip compressed data, was "np_aind_metadata-0.1.4.tar", last modified: Mon Apr 22 23:19:56 2024, max compression
```

## Comparing `np_aind_metadata-0.1.3.tar` & `np_aind_metadata-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.341930 np_aind_metadata-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-18 00:35:41.341930 np_aind_metadata-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 00:35:38.000000 np_aind_metadata-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:35:41.341930 np_aind_metadata-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.333930 np_aind_metadata-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.337930 np_aind_metadata-0.1.3/src/np_aind_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.337930 np_aind_metadata-0.1.3/src/np_aind_metadata/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/init/dynamic_routing_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.337930 np_aind_metadata-0.1.3/src/np_aind_metadata/np/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/np/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-18 00:35:35.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/np/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.337930 np_aind_metadata-0.1.3/src/np_aind_metadata/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.337930 np_aind_metadata-0.1.3/src/np_aind_metadata/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/update/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/update/dynamic_routing_task_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/src/np_aind_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.341930 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-18 00:35:41.000000 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 00:35:41.000000 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:35:41.000000 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 00:35:41.000000 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 00:35:41.000000 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 00:35:41.000000 np_aind_metadata-0.1.3/src/np_aind_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:35:41.337930 np_aind_metadata-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-18 00:35:02.000000 np_aind_metadata-0.1.3/tests/test_np_codeocean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-22 23:19:53.000000 np_aind_metadata-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.427611 np_aind_metadata-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.431611 np_aind_metadata-0.1.4/src/np_aind_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.431611 np_aind_metadata-0.1.4/src/np_aind_metadata/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/init/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-22 23:19:50.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.431611 np_aind_metadata-0.1.4/src/np_aind_metadata/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/src/np_aind_metadata/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-22 23:19:50.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_storage.py
```

### Comparing `np_aind_metadata-0.1.3/LICENSE` & `np_aind_metadata-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.3/pyproject.toml` & `np_aind_metadata-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dependencies = [
     "h5py>=3.10.0",
     "pyyaml>=6.0.1",
     "np-session>=0.6.40",
     "np-config>=0.4.27",
     "aind-metadata-mapper==0.6.2",
 ]
-version = "0.1.3"
+version = "0.1.4"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
@@ -33,15 +33,14 @@
 
 [project.urls]
 Repository = "https://github.com/AllenInstitute/np-aind-metadata"
 Issues = "https://github.com/AllenInstitute/np-aind-metadata/issues"
 
 [project.optional-dependencies]
 np = [
-    "np-session>=0.6.40",
     "np-config>=0.4.27",
 ]
 
 [build-system]
 requires = [
     "setuptools>=61",
     "wheel",
@@ -129,14 +128,15 @@
     "--cov-report=html",
     "--cov-config=pyproject.toml",
     "--doctest-glob=*README.md",
     "-x",
 ]
 markers = [
     "onprem",
+    "storage",
 ]
 doctest_optionflags = [
     "NORMALIZE_WHITESPACE",
     "IGNORE_EXCEPTION_DETAIL",
     "ELLIPSIS",
 ]
 testpaths = [
@@ -204,16 +204,17 @@
     "mkdocstrings[python]>=0.23",
     "tomli>=2.0; python_version < '3.11'",
 ]
 
 [tool.pdm.scripts]
 ruff = "ruff check src --fix-only"
 black = "black src"
-pytest = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'not onprem'"
-pytest-onprem = "pytest --cov-report term-missing:skip-covered --cov-report=html"
+pytest = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'not onprem and not storage'"
+pytest-storage = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'storage'"
+pytest-onprem = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'onprem'"
 mypy = "mypy src --install-types --non-interactive"
 log = "git-changelog -o CHANGELOG.md"
 dryrun = "pdm publish --repository testpypi --dry-run"
 post_init = "pdm install --plugins"
 
 [tool.pdm.scripts.test]
 composite = [
```

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/__init__.py` & `np_aind_metadata-0.1.4/src/np_aind_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/common.py` & `np_aind_metadata-0.1.4/src/np_aind_metadata/common.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/init/dynamic_routing_task.py` & `np_aind_metadata-0.1.4/src/np_aind_metadata/init/neuropixels_rig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,67 @@
-import pathlib
+import datetime
+import logging
+import typing
 
 from aind_data_schema.core import rig
 from aind_data_schema.models import coordinates, devices, organizations
 
 from np_aind_metadata import common
 
 COPA_NOTES = (
     "The rotation matrix is represented as: a,b,c,d,e,f,g,h,i. Wherein a, b, "
     "c correspond to the first row of the matrix. The translation matrix is "
     "represented as: x,y,z."
 )
+DEFAULT_HOSTNAME = "127.0.0.1"
+
+
+logger = logging.getLogger(__name__)
+
+
+def get_rig_room(rig_name: common.RigName) -> typing.Union[str, None]:
+    rig_to_room = {
+        "NP0": "325",
+        "NP1": "325",
+        "NP2": "327",
+        "NP3": "342",
+    }
+    try:
+        return rig_to_room[rig_name]
+    except KeyError:
+        logger.debug("No room found for rig: %s" % rig_name)
+        return None
 
 
 def init(
-    config: common.DynamicRoutingRigDetails,
-    output_directory: pathlib.Path = pathlib.Path("."),
-) -> pathlib.Path:
+    rig_name: common.RigName,
+    modification_date: typing.Optional[datetime.date] = None,
+    manipulator_infos: list[common.ManipulatorInfo] = [],
+    mon_computer_name: str = DEFAULT_HOSTNAME,
+    stim_computer_name: str = DEFAULT_HOSTNAME,
+    sync_computer_name: str = DEFAULT_HOSTNAME,
+) -> rig.Rig:
     """Initializes a rig model for the dynamic routing project.
 
+    >>> rig_model = init("NP3")
+
     Notes
     -----
     - rig_id is expected to be in the format:
         <ROOM NAME>_<RIG NAME>_<MODIFICATION DATE>
     - The DR task does not set the brightness and contrast of the monitor.
      These are hardcoded and assumed to be static.
     """
-    rig_id = f"{config.rig_name}_{config.modification_date.strftime('%y%m%d')}"
-    if config.room_name is not None:
-        rig_id = f"{config.room_name}_{rig_id}"
+    if not modification_date:
+        modification_date = datetime.date.today()
+
+    room_name = get_rig_room(rig_name)
+    rig_id = f"{rig_name}_{modification_date.strftime('%y%m%d')}"
+    if room_name is not None:
+        rig_id = f"{room_name}_{rig_id}"
 
     shared_camera_props = {
         "detector_type": "Camera",
         "model": "G-032",
         "max_frame_rate": 102,
         "sensor_width": 7400,
         "sensor_height": 7400,
@@ -67,24 +97,24 @@
         ],
         "notes": COPA_NOTES,
     }
 
     ephys_assemblies = []
     for assembly_letter in ["A", "B", "C", "D", "E", "F"]:
         serial_number = None
-        for manipulator_info in config.manipulator_infos:
+        for manipulator_info in manipulator_infos:
             if manipulator_info.assembly_name == f"Ephys Assembly {assembly_letter}":
                 serial_number = manipulator_info.serial_number
                 break
         ephys_assemblies.append(
             rig.EphysAssembly(
                 name=f"Ephys Assembly {assembly_letter}",
                 manipulator=devices.Manipulator(
                     name=f"Ephys Assembly {assembly_letter} Manipulator",
-                    manufacturer=organizations.Organization.NEW_SCALE_TECHNOLOGIES,
+                    manufacturer=(organizations.Organization.NEW_SCALE_TECHNOLOGIES),
                     model="06591-M-0004",
                     serial_number=serial_number,
                 ),
                 probes=[
                     devices.EphysProbe(
                         name=f"Probe{assembly_letter}",
                         probe_model="Neuropixels 1.0",
@@ -92,15 +122,15 @@
                     )
                 ],
             )
         )
 
     model = rig.Rig(
         rig_id=rig_id,
-        modification_date=config.modification_date,
+        modification_date=modification_date,
         modalities=[
             rig.Modality.BEHAVIOR_VIDEOS,
             rig.Modality.BEHAVIOR,
             rig.Modality.ECEPHYS,
         ],
         mouse_platform=devices.Disc(
             name="Mouse Platform",
@@ -305,15 +335,15 @@
                 name="Front",
                 camera_target="Face forward",
                 camera=devices.Camera(
                     name="Front camera",
                     manufacturer=organizations.Organization.ALLIED,
                     chroma="Monochrome",
                     data_interface="Ethernet",
-                    computer_name=config.mon_computer_name,
+                    computer_name=mon_computer_name,
                     **shared_camera_props,
                 ),
                 filter=devices.Filter(
                     name="Front filter",
                     manufacturer=organizations.Organization.SEMROCK,
                     model="FF01-715_LP-25",
                     filter_type=devices.FilterType.LONGPASS,
@@ -351,15 +381,15 @@
                 name="Side",
                 camera_target="Body",
                 camera=devices.Camera(
                     name="Side camera",
                     manufacturer=organizations.Organization.ALLIED,
                     chroma="Monochrome",
                     data_interface="Ethernet",
-                    computer_name=config.mon_computer_name,
+                    computer_name=mon_computer_name,
                     **shared_camera_props,
                 ),
                 filter=devices.Filter(
                     name="Side filter",
                     manufacturer=organizations.Organization.SEMROCK,
                     model="FF01-747/33-25",
                     filter_type=devices.FilterType.BANDPASS,
@@ -386,26 +416,26 @@
                 name="Eye",
                 camera_target="Eye",
                 camera=devices.Camera(
                     name="Eye camera",
                     manufacturer=organizations.Organization.ALLIED,
                     chroma="Monochrome",
                     data_interface="Ethernet",
-                    computer_name=config.mon_computer_name,
+                    computer_name=mon_computer_name,
                     **shared_camera_props,
                 ),
                 filter=devices.Filter(
                     name="Eye filter",
                     manufacturer=organizations.Organization.SEMROCK,
                     model="FF01-850/10-25",
                     filter_type=devices.FilterType.BANDPASS,
                 ),
                 lens=devices.Lens(
                     name="Eye lens",
-                    manufacturer=organizations.Organization.INFINITY_PHOTO_OPTICAL,
+                    manufacturer=(organizations.Organization.INFINITY_PHOTO_OPTICAL),
                     focal_length=6.0,
                     focal_length_unit="millimeter",
                     model="213073",
                     notes="Model number is SKU.",
                 ),
                 position=coordinates.RelativePosition(
                     device_position_transformations=[
@@ -430,36 +460,36 @@
                 ),
             ),
         ],
         daqs=[
             devices.DAQDevice(
                 manufacturer=organizations.Organization.NATIONAL_INSTRUMENTS,
                 name="Sync",
-                computer_name=config.sync_computer_name,
+                computer_name=sync_computer_name,
                 model="NI-6612",
                 data_interface=devices.DataInterface.PCIE,
             ),
             devices.DAQDevice(
                 manufacturer=organizations.Organization.NATIONAL_INSTRUMENTS,
                 name="Behavior",
-                computer_name=config.stim_computer_name,
+                computer_name=stim_computer_name,
                 model="NI-6323",
                 data_interface=devices.DataInterface.USB,
             ),
             devices.DAQDevice(
                 manufacturer=organizations.Organization.NATIONAL_INSTRUMENTS,
                 name="BehaviorSync",
-                computer_name=config.stim_computer_name,
+                computer_name=stim_computer_name,
                 model="NI-6001",
                 data_interface=devices.DataInterface.PCIE,
             ),
             devices.DAQDevice(
                 manufacturer=organizations.Organization.NATIONAL_INSTRUMENTS,
                 name="Opto",
-                computer_name=config.stim_computer_name,
+                computer_name=stim_computer_name,
                 model="NI-9264",
                 data_interface=devices.DataInterface.ETH,
             ),
         ],
         detectors=[
             devices.Detector(
                 name="vsync photodiode",
@@ -520,17 +550,15 @@
                 core_diameter=125.0,
                 numerical_aperture=0.10,
                 notes=("Numerical aperture is approximately between 0.10 and " "0.14."),
             ),
         ],
     )
 
-    validated = rig.Rig.model_validate(model)
-    validated.write_standard_file(output_directory)
-    return output_directory / "rig.json"
+    return rig.Rig.model_validate(model)
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod(
         optionflags=(doctest.IGNORE_EXCEPTION_DETAIL | doctest.NORMALIZE_WHITESPACE)
```

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/np_codeocean.py` & `np_aind_metadata-0.1.4/tests/test_np_codeocean.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,98 @@
-"""Utilities for interacting with NP Code Ocean."""
-
-import logging
 import pathlib
 import shutil
 
+import pytest
 from aind_data_schema.core import rig, session
 
-from np_aind_metadata import storage
-from np_aind_metadata.np import dynamic_routing_task as dynamic_routing_task_np
+from np_aind_metadata import np_codeocean, storage
+from np_aind_metadata.update import (
+    dynamic_routing_task as dynamic_routing_task_update
+)
+
+
+def _copy_resource_files(
+    source: pathlib.Path,
+    dest: pathlib.Path,
+) -> pathlib.Path:
+    """Test utility. Copies all files from source to dest. Recursively
+     traverses directories and copies their files.
+    """
+    for file in source.iterdir():
+        if file.is_dir():
+            dest_dir = dest / file.name
+            (dest_dir).mkdir()
+            _copy_resource_files(file, dest_dir)
+        else:
+            shutil.copy2(file, dest / file.name)
+    return dest
+
+
+RESOURCES_DIRECTORY = pathlib.Path("tests") / "resources"
+
+
+@pytest.mark.onprem
+def test_update_session_and_rig(tmp_path: pathlib.Path) -> None:
+    """Runs two tests to ensure order is correct.
+    """
+    np_codeocean.logger.setLevel("DEBUG")
+    storage.logger.setLevel("DEBUG")
+    dynamic_routing_task_update.logger.setLevel("DEBUG")
+    # setup temporary test directories
+    rig_directory_temp = tmp_path / "rig"
+    rig_directory_temp.mkdir()
+    rig_directory = _copy_resource_files(
+        RESOURCES_DIRECTORY / "rig-directory",
+        rig_directory_temp,
+    )
+    session_directory_0_temp = tmp_path / "session-0"
+    session_directory_0_temp.mkdir()
+    session_directory_0 = _copy_resource_files(
+        RESOURCES_DIRECTORY / "session-directory-0",
+        session_directory_0_temp,
+    )
+    session_directory_1_temp = tmp_path / "session-1"
+    session_directory_1_temp.mkdir()
+    session_directory_1 = _copy_resource_files(
+        RESOURCES_DIRECTORY / "session-directory-1",
+        session_directory_1_temp,
+    )
 
-logger = logging.getLogger(__name__)
+    def get_current_rig_model() -> rig.Rig:
+        return rig.Rig.model_validate_json(
+            storage.get_item(
+                rig_directory,
+                "NP3",
+                "dynamic-routing",
+            ).read_text()
+        )
 
+    initial_rig_model = get_current_rig_model()
 
-def update_session_and_rig(
-    session_directory: pathlib.Path,
-    rig_directory: pathlib.Path,
-    project_name: str,
-) -> None:
-    """Update the session and rig metadata in the given directories."""
-    try:
-        session_path = next(session_directory.glob("**/*session.json"))
-    except StopIteration as err:
-        raise Exception("No session.json found in directory.") from err
-    logger.debug("Scraped session model path: %s" % session_path)
-    session_model = session.Session.model_validate_json(session_path.read_text())
-    rig_name = session_model.rig_id.split("_")[-2]
+    # Test no update
+    np_codeocean.add_rig_to_dynamic_routing_session_dir(
+        session_directory_0,
+        rig_directory,
+    )
+    updated_session_0 = session.Session.model_validate_json(
+        next(session_directory_0.glob("*session.json")).read_text()
+    )
 
-    rig_path = storage.get_latest_base_rig(
+    non_updated_rig_model = get_current_rig_model()
+    assert initial_rig_model == non_updated_rig_model
+    assert updated_session_0.rig_id == non_updated_rig_model.rig_id
+
+    # Test update
+    np_codeocean.add_rig_to_dynamic_routing_session_dir(
+        session_directory_1,
         rig_directory,
-        project_name,
-        rig_name,
     )
-    logger.debug("Base rig model path: %s" % rig_path)
-    original_rig_id = rig.Rig.model_validate_json(rig_path.read_text()).rig_id
 
-    update_context = dynamic_routing_task_np.update_rig_from_session_dir(
-        rig_path,
-        session_directory,
-        output_dir=session_directory,
-        include=["open_ephys_context"],
-    )
-    if not update_context.updated:
-        logger.debug("Failed to update rig json. Using current base rig.")
-        shutil.copy2(
-            rig_path,
-            session_directory / "rig.json",
-        )
-        return
+    updated_rig_model = get_current_rig_model()
+    assert initial_rig_model != updated_rig_model
+    assert updated_rig_model.rig_id != initial_rig_model.rig_id
 
-    updated_rig_id = rig.Rig.model_validate_json(
-        update_context.updated.read_text()
-    ).rig_id
-
-    if original_rig_id != updated_rig_id:
-        logger.debug("Rig id updated. Updating session.")
-        session_model.rig_id = updated_rig_id
-        session_model.write_standard_file(
-            session_path.parent,
-        )
-        logger.debug("Rig json updated. Updating base rig.")
-        storage.update_base_rig(
-            rig_directory,
-            project_name,
-            rig_name,
-            update_context.updated,
-        )
+    updated_session_1 = session.Session.model_validate_json(
+        next(session_directory_1.glob("*session.json")).read_text()
+    )
+
+    assert updated_session_1.rig_id == updated_rig_model.rig_id
```

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/update/dynamic_routing_task.py` & `np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import datetime
-import json
 import logging
 import pathlib
 import shutil
 import tempfile
 import typing
 
-from aind_data_schema.core import rig
+from aind_data_schema.core import rig, session
 from aind_metadata_mapper.neuropixels import (
     mvr_rig,
     neuropixels_rig,
     open_ephys_rig,
     sync_rig,
 )
 
-from np_aind_metadata import common
 from np_aind_metadata.update.dynamic_routing_task_etl import DynamicRoutingTaskRigEtl
 
 logger = logging.getLogger(__name__)
 
 
 def _run_neuropixels_rig_etl(
     etl_class: neuropixels_rig.NeuropixelsRigEtl,
@@ -33,150 +31,165 @@
         etl.run_job()
         return output_dir / "rig.json"
     except Exception:
         logger.debug("Error calling: %s" % etl_class, exc_info=True)
         return input_source
 
 
-# cannot type hint due to np import failing in github actions
-def scrape_update_context(
-    path: pathlib.Path,
-    context: common.DynamicRoutingTaskUpdateContext,
-    manipulators: typing.Optional[list[common.ManipulatorInfo]] = None,
-) -> common.DynamicRoutingTaskUpdateContext:
-    """Scrapes the given directory for relevant files and updates
-    UpdateContext.
-    """
-    # dr task
-    try:
-        task_source = next(path.glob("**/Dynamic*.hdf5"))
-        context.task_context = common.DynamicRoutingTaskContext(
-            source=task_source,
-        )
-    except StopIteration:
-        logger.debug("No task output found.")
+def scrape_rig_id(session_directory: pathlib.Path) -> str:
+    """Scrapes the rig id from the given session directory."""
+    matches = list(session_directory.glob("**/session.json"))
+    logger.debug("Scraped session model paths: %s" % matches)
+    return session.Session.model_validate_json(matches[0].read_text()).rig_id
 
-    # sync
-    try:
-        sync_source = next(path.glob("**/sync.yml"))
-        context.sync_context = common.SyncContext(
-            source=sync_source,
-        )
-    except StopIteration:
-        logger.debug("No sync config found.")
 
-    # mvr
-    try:
-        mvr_source = next(path.glob("**/mvr.ini"))
-        context.mvr_context = common.MVRContext(
-            source=mvr_source,
-        )
-    except StopIteration:
-        logger.debug("No mvr config found.")
-
-    # open ephys
-    settings_sources = list(path.glob("**/settings.xml"))
-    if len(settings_sources) < 1:
-        logger.debug("No open ephys settings found.")
-
-    context.open_ephys_context = common.OpenEphysContext(
-        source=settings_sources,
-        manipulators=manipulators,
-    )
-
-    return context
-
-
-def update_rig(
-    context: common.DynamicRoutingTaskUpdateContext,
+def _fix_modification_date(prev: pathlib.Path, new: pathlib.Path) -> None:
+    """Fixes an unintentional side effect introduced with open ephys etl.
+    Reverts the rig_id if probe serial numbers have not changed.
+    """
+    prev_rig = rig.Rig.model_validate_json(prev.read_text())
+    new_rig = rig.Rig.model_validate_json(new.read_text())
+    prev_probe_serial_numbers = [
+        ephys_assembly.probes[0].serial_number
+        for ephys_assembly in prev_rig.ephys_assemblies
+    ]
+    new_probe_serial_numbers = [
+        ephys_assembly.probes[0].serial_number
+        for ephys_assembly in new_rig.ephys_assemblies
+    ]
+    if prev_probe_serial_numbers != new_probe_serial_numbers:
+        logger.debug("Probe serial numbers changed. Not reverting modification date.")
+        logger.debug(f"Previous: {prev_probe_serial_numbers}")
+        logger.debug(f"New: {new_probe_serial_numbers}")
+        return
+
+    logger.debug("Probe serial numbers match. Reverting modification date.")
+    with tempfile.TemporaryDirectory() as temp_dir:
+        new_rig.rig_id = prev_rig.rig_id
+        new_rig.modification_date = prev_rig.modification_date
+        new_rig.write_standard_file(temp_dir)
+        shutil.copy2(pathlib.Path(temp_dir) / "rig.json", new)
+
+
+def update_rig_from_dynamic_routing_session_context(
+    rig_source: pathlib.Path,
+    task_source: typing.Optional[pathlib.Path] = None,
+    reward_calibration_date: typing.Optional[datetime.date] = None,
+    sound_calibration_date: typing.Optional[datetime.date] = None,
+    open_ephys_settings_sources: typing.Optional[list[pathlib.Path]] = None,
+    sync_source: typing.Optional[pathlib.Path] = None,
+    mvr_source: typing.Optional[pathlib.Path] = None,
+    mvr_mapping: typing.Optional[dict[str, str]] = None,
     output_path: pathlib.Path = pathlib.Path("rig.json"),
-    modification_date: typing.Optional[datetime.date] = None,
-    include: typing.Optional[list[str]] = None,
-) -> common.DynamicRoutingTaskUpdateContext:
+) -> pathlib.Path:
     """Generates a new rig json file with the metadata from the given sources.
 
     Notes
     -----
     - If rig_source is None, the rig will be initialized with the default
      values.
     - *_source, if present will update various values in the rig model.
     """
     # build model in a temporary directory
     build_dir = pathlib.Path(tempfile.mkdtemp())
-    build_source = build_dir / "rig.json"
-    shutil.copy(context.source, build_source)
-    if include:
-        logger.debug("Including only: %s" % json.dumps(include))
-        context = common.DynamicRoutingTaskUpdateContext(
-            source=context.source, **{k: getattr(context, k) for k in include}
-        )
-        logger.debug("Updated context: %s" % context.model_dump_json())
 
-    rig_model = rig.Rig.model_validate_json(build_source.read_text())
-
-    if context.task_context:
+    build_source = pathlib.Path(shutil.copy2(rig_source, build_dir))
+    logger.debug("Rig build source: %s" % build_source)
+    if task_source:
         logger.debug("Updating rig model with dynamic routing task context.")
         _run_neuropixels_rig_etl(
             DynamicRoutingTaskRigEtl,
             build_source,
             build_dir,
-            task_source=context.task_context.source,
-            sound_calibration_date=rig_model.modification_date,
-            reward_calibration_date=rig_model.modification_date,
+            task_source=task_source,
+            sound_calibration_date=sound_calibration_date,
+            reward_calibration_date=reward_calibration_date,
         )
 
-    if context.open_ephys_context:
+    if open_ephys_settings_sources:
         logger.debug("Updating rig model with open ephys context.")
-        if context.open_ephys_context.manipulators:
-            manipulators = [
-                (
-                    m.assembly_name,
-                    m.serial_number,
-                )
-                for m in context.open_ephys_context.manipulators
-            ]
-        else:
-            manipulators = []
         _run_neuropixels_rig_etl(
             open_ephys_rig.OpenEphysRigEtl,
             build_source,
             build_dir,
-            open_ephys_settings_sources=context.open_ephys_context.source,
-            probe_manipulator_serial_numbers=manipulators,
-            modification_date=modification_date,
+            open_ephys_settings_sources=open_ephys_settings_sources,
         )
 
-    if context.sync_context:
-        logger.debug("Updating rig model with sync source file.")
+    if sync_source:
+        logger.debug("Updating rig model with sync context.")
         _run_neuropixels_rig_etl(
             sync_rig.SyncRigEtl,
             build_source,
             build_dir,
-            config_source=context.sync_context.source,
+            config_source=sync_source,
         )
 
-    if context.mvr_context:
-        logger.debug("Updating rig model with mvr source file.")
-        if context.mvr_context.mapping:
-            camera_aliases = {
-                m.mvr_name: m.camera_assembly_name for m in context.mvr_context.mapping
-            }
-        else:
-            camera_aliases = None
+    if mvr_source and mvr_mapping:
+        logger.debug("Updating rig model with mvr context.")
         _run_neuropixels_rig_etl(
             mvr_rig.MvrRigEtl,
             build_source,
             build_dir,
-            mvr_config_source=context.mvr_context.source,
-            mvr_mapping=camera_aliases,
+            mvr_config_source=mvr_source,
+            mvr_mapping=mvr_mapping,
         )
 
+    _fix_modification_date(rig_source, build_source)
+
     shutil.copy2(build_source, output_path)
-    context.updated = output_path
-    return context
+    return output_path
+
+
+def update_rig_from_dynamic_routing_session_dir(
+    rig_source: pathlib.Path,
+    session_dir: pathlib.Path,
+    output_path: pathlib.Path = pathlib.Path("rig.json"),
+) -> pathlib.Path:
+    """Scrapes dynamic routing session directory for various rig
+    configuration/settings and updates `rig_source`.
+    """
+    try:
+        task_source = next(session_dir.glob("**/Dynamic*.hdf5"))
+        logger.debug("Scraped task source: %s" % task_source)
+    except StopIteration:
+        task_source = None
+
+    # sync
+    try:
+        sync_source = next(session_dir.glob("**/sync.yml"))
+        logger.debug("Scraped sync source: %s" % sync_source)
+    except StopIteration:
+        sync_source = None
+
+    # mvr
+    try:
+        mvr_source = next(session_dir.glob("**/mvr.ini"))
+        mvr_mapping = {
+            "Camera 1": "Side",
+            "Camera 2": "Eye",
+            "Camera 3": "Front",
+        }
+        logger.debug("Scraped mvr source: %s" % mvr_source)
+    except StopIteration:
+        mvr_source = None
+        mvr_mapping = None
+
+    # open ephys
+    settings_sources = list(session_dir.glob("**/settings.xml"))
+    logger.debug("Scraped open ephys settings: %s" % settings_sources)
+
+    return update_rig_from_dynamic_routing_session_context(
+        rig_source,
+        task_source=task_source,
+        sync_source=sync_source,
+        mvr_source=mvr_source,
+        mvr_mapping=mvr_mapping,
+        open_ephys_settings_sources=settings_sources,
+        output_path=output_path,
+    )
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod(
         optionflags=(doctest.IGNORE_EXCEPTION_DETAIL | doctest.NORMALIZE_WHITESPACE)
```

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/update/dynamic_routing_task_etl.py` & `np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task_etl.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.3/src/np_aind_metadata/utils.py` & `np_aind_metadata-0.1.4/src/np_aind_metadata/utils.py`

 * *Files identical despite different names*

