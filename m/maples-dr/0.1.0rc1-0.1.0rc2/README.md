# Comparing `tmp/maples_dr-0.1.0rc1.tar.gz` & `tmp/maples_dr-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maples_dr-0.1.0rc1.tar", last modified: Mon Apr 22 21:30:35 2024, max compression
+gzip compressed data, was "maples_dr-0.1.0rc2.tar", last modified: Tue Apr 23 15:51:20 2024, max compression
```

## Comparing `maples_dr-0.1.0rc1.tar` & `maples_dr-0.1.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-22 21:30:35.983489 maples_dr-0.1.0rc1/
--rw-r--r--   0 gaby      (1000) gaby      (1000)     7048 2023-12-21 00:27:55.000000 maples_dr-0.1.0rc1/LICENSE
--rw-r--r--   0 gaby      (1000) gaby      (1000)     4396 2024-04-22 21:30:35.982489 maples_dr-0.1.0rc1/PKG-INFO
--rw-r--r--   0 gaby      (1000) gaby      (1000)     3107 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/README.md
--rw-r--r--   0 gaby      (1000) gaby      (1000)     1551 2024-04-22 21:28:23.000000 maples_dr-0.1.0rc1/pyproject.toml
--rw-r--r--   0 gaby      (1000) gaby      (1000)       38 2024-04-22 21:30:35.983489 maples_dr-0.1.0rc1/setup.cfg
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-22 21:30:35.978489 maples_dr-0.1.0rc1/src/
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-22 21:30:35.980489 maples_dr-0.1.0rc1/src/maples_dr/
--rw-r--r--   0 gaby      (1000) gaby      (1000)      644 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/src/maples_dr/__init__.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     5829 2024-04-22 21:24:44.000000 maples_dr-0.1.0rc1/src/maples_dr/config.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)    37072 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/src/maples_dr/dataset.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)    25777 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/src/maples_dr/loader.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     5546 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/src/maples_dr/preprocessing.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     4018 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/src/maples_dr/quick_api.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)    16870 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/src/maples_dr/utilities.py
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-22 21:30:35.981490 maples_dr-0.1.0rc1/src/maples_dr.egg-info/
--rw-r--r--   0 gaby      (1000) gaby      (1000)     4396 2024-04-22 21:30:35.000000 maples_dr-0.1.0rc1/src/maples_dr.egg-info/PKG-INFO
--rw-r--r--   0 gaby      (1000) gaby      (1000)      590 2024-04-22 21:30:35.000000 maples_dr-0.1.0rc1/src/maples_dr.egg-info/SOURCES.txt
--rw-r--r--   0 gaby      (1000) gaby      (1000)        1 2024-04-22 21:30:35.000000 maples_dr-0.1.0rc1/src/maples_dr.egg-info/dependency_links.txt
--rw-r--r--   0 gaby      (1000) gaby      (1000)      211 2024-04-22 21:30:35.000000 maples_dr-0.1.0rc1/src/maples_dr.egg-info/requires.txt
--rw-r--r--   0 gaby      (1000) gaby      (1000)       10 2024-04-22 21:30:35.000000 maples_dr-0.1.0rc1/src/maples_dr.egg-info/top_level.txt
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-22 21:30:35.981490 maples_dr-0.1.0rc1/tests/
--rw-r--r--   0 gaby      (1000) gaby      (1000)    10142 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/tests/test_maples_dr_cache.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)      266 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/tests/test_maples_dr_config.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     5995 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/tests/test_maples_dr_dataset.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     1207 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/tests/test_maples_dr_download.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)      757 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/tests/test_maples_dr_fundus.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)      462 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc1/tests/test_maples_dr_quickapi.py
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 15:51:20.462201 maples_dr-0.1.0rc2/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     7048 2023-12-21 00:27:55.000000 maples_dr-0.1.0rc2/LICENSE
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     4439 2024-04-23 15:51:20.462201 maples_dr-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     3107 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/README.md
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     1561 2024-04-23 15:50:40.000000 maples_dr-0.1.0rc2/pyproject.toml
+-rw-r--r--   0 gaby      (1000) gaby      (1000)       38 2024-04-23 15:51:20.462201 maples_dr-0.1.0rc2/setup.cfg
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 15:51:20.458201 maples_dr-0.1.0rc2/src/
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 15:51:20.459201 maples_dr-0.1.0rc2/src/maples_dr/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      644 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/src/maples_dr/__init__.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     5829 2024-04-22 21:24:44.000000 maples_dr-0.1.0rc2/src/maples_dr/config.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    37072 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/src/maples_dr/dataset.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    26633 2024-04-23 14:57:47.000000 maples_dr-0.1.0rc2/src/maples_dr/loader.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     6609 2024-04-23 15:33:10.000000 maples_dr-0.1.0rc2/src/maples_dr/preprocessing.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     4018 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/src/maples_dr/quick_api.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    16870 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/src/maples_dr/utilities.py
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 15:51:20.460201 maples_dr-0.1.0rc2/src/maples_dr.egg-info/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     4439 2024-04-23 15:51:20.000000 maples_dr-0.1.0rc2/src/maples_dr.egg-info/PKG-INFO
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      590 2024-04-23 15:51:20.000000 maples_dr-0.1.0rc2/src/maples_dr.egg-info/SOURCES.txt
+-rw-r--r--   0 gaby      (1000) gaby      (1000)        1 2024-04-23 15:51:20.000000 maples_dr-0.1.0rc2/src/maples_dr.egg-info/dependency_links.txt
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      219 2024-04-23 15:51:20.000000 maples_dr-0.1.0rc2/src/maples_dr.egg-info/requires.txt
+-rw-r--r--   0 gaby      (1000) gaby      (1000)       10 2024-04-23 15:51:20.000000 maples_dr-0.1.0rc2/src/maples_dr.egg-info/top_level.txt
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 15:51:20.460201 maples_dr-0.1.0rc2/tests/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    10142 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/tests/test_maples_dr_cache.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      266 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/tests/test_maples_dr_config.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     5995 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/tests/test_maples_dr_dataset.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     1207 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/tests/test_maples_dr_download.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      757 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/tests/test_maples_dr_fundus.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      462 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc2/tests/test_maples_dr_quickapi.py
```

### Comparing `maples_dr-0.1.0rc1/LICENSE` & `maples_dr-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/PKG-INFO` & `maples_dr-0.1.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: maples-dr
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Utilities python library for the public dataset: MAPLES-DR.
 Author-email: Gabriel Lepetit-Aimon <gabriel.lepetit-aimon@polymtl.ca>
 Project-URL: Homepage, https://liv4d.github.io/MAPLES-DR/en/welcome/maples_dr
 Project-URL: Documentation, https://liv4d.github.io/MAPLES-DR/en/
 Project-URL: Source, https://github.com/LIV4D/MAPlES-DR
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: xlrd
 Requires-Dist: pyyaml
 Requires-Dist: rich
-Requires-Dist: scikit-image
 Provides-Extra: examples
 Requires-Dist: plotly; extra == "examples"
 Requires-Dist: rich; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
+Requires-Dist: scikit-image; extra == "examples"
 Requires-Dist: scipy; extra == "examples"
 Requires-Dist: tqdm; extra == "examples"
 Requires-Dist: jppype; extra == "examples"
 Provides-Extra: dev
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinxcontrib-bibtex; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: sphinx-intl; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # MAPLES-DR
 
 [![doc](https://github.com/LIV4D/MAPLES-DR/actions/workflows/documentation.yml/badge.svg?branch=dev)](https://liv4d.github.io/MAPLES-DR/en/)
 
 **MAPLES-DR _(MESSIDOR Anatomical and Pathological Labels for Explainable Screening of Diabetic Retinopathy)_** is a public dataset which provides diagnoses for DR and ME as well as pixel-wise segmentation maps for 10 retinal structures for 198 images of MESSIDOR. This repository provides a python library of utility codes to ease the use of the database.
```

### Comparing `maples_dr-0.1.0rc1/README.md` & `maples_dr-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/pyproject.toml` & `maples_dr-0.1.0rc2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 [project]
 
 name = "maples-dr"
-version = '0.1.0rc1'
+version = '0.1.0rc2'
 authors = [
     {name= 'Gabriel Lepetit-Aimon', email= 'gabriel.lepetit-aimon@polymtl.ca'},
 ]
 description = """Utilities python library for the public dataset: MAPLES-DR."""
 readme = 'README.md'
 
 requires-python = '>=3.10'
 dependencies = [
     'numpy',
     'Pillow',
     'pandas',
     'xlrd',
     'pyyaml',
     'rich',
-    'scikit-image', 
 ]
 
 [project.optional-dependencies]
 examples = [
     'plotly',
     'rich',
     'scikit-learn', 
+    'scikit-image',
     'scipy',
     'tqdm',
     'jppype',
 ]
 dev = [
     'sphinx',
     'sphinx-rtd-theme',
     'sphinx-copybutton',
     'sphinxcontrib-bibtex',
     'nbsphinx',
     'sphinx-intl',
     'ipython',
+]
+test = [
     'pytest',
 ]
 
 [project.urls]
 Homepage = 'https://liv4d.github.io/MAPLES-DR/en/welcome/maples_dr'
 Documentation = 'https://liv4d.github.io/MAPLES-DR/en/'
 Source = 'https://github.com/LIV4D/MAPlES-DR'
```

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/__init__.py` & `maples_dr-0.1.0rc2/src/maples_dr/__init__.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/config.py` & `maples_dr-0.1.0rc2/src/maples_dr/config.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/dataset.py` & `maples_dr-0.1.0rc2/src/maples_dr/dataset.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/loader.py` & `maples_dr-0.1.0rc2/src/maples_dr/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,28 @@
 from typing import Dict, Optional, Tuple
 from urllib.request import urlopen
 from zipfile import ZipFile
 
 import pandas as pd
 import yaml
 
-from .config import DOWNLOAD, DatasetConfig, ImageFormat, InvalidConfigError, Preprocessing
-from .dataset import BiomarkerField, BiomarkersAnnotationInfos, BiomarkersAnnotationTasks, Dataset, FundusField
+from .config import (
+    DOWNLOAD,
+    DatasetConfig,
+    ImageFormat,
+    InvalidConfigError,
+    Preprocessing,
+)
+from .dataset import (
+    BiomarkerField,
+    BiomarkersAnnotationInfos,
+    BiomarkersAnnotationTasks,
+    Dataset,
+    FundusField,
+)
 from .utilities import RichProgress, xdg_data_home
 
 #   === CONSTANTS ===
 # Figshare public urls of the MAPLES DR dataset
 MAPLES_DR_ADDITIONAL_URL = "https://figshare.com/ndownloader/files/45795384"
 
 #: Unset constant
@@ -45,15 +57,17 @@
 
 
 class NotConfiguredError(Exception):
     """
     Exception raised when the dataset loader is not configured.
     """
 
-    def __init__(self, message: str = "MAPLES-DR dataset is not configured yet.", *args):
+    def __init__(
+        self, message: str = "MAPLES-DR dataset is not configured yet.", *args
+    ):
         super().__init__(message, *args)
 
 
 class DatasetLoader:
     """
     Loader for MAPLES-DR dataset.
     """
@@ -159,40 +173,50 @@
                 maples_dr_path = cache / "AdditionalData"
 
         if maples_dr_path is not UNSET and self._maples_dr_path != maples_dr_path:
             # Set the path and download the dataset if needed.
             maples_dr_path = self._change_maples_dr_path(maples_dr_path)
 
             # Load the dataset infos.
-            self.dataset_record, self._messidor_ROIs = self.load_dataset_record_and_rois(maples_dr_path)
+            (
+                self.dataset_record,
+                self._messidor_ROIs,
+            ) = self.load_dataset_record_and_rois(maples_dr_path)
             self._annotations_infos = self.load_biomarkers_annotation_infos(
                 maples_dr_path / "biomarkers_annotation_infos.xls"
             )
 
             # Check the integrity of the dataset.
             if not disable_check:
                 self.check_maples_dr_integrity(
                     path=maples_dr_path,
                     biomarkers=list(self.dataset_record["biomarkers"]),
                     images_names=self.image_names(DatasetSubset.ALL_WITH_DUPLICATES),
                 )
 
-            self._diagnosis = self.load_maples_dr_diagnosis(maples_dr_path / "diagnosis_infos.xls")
+            self._diagnosis = self.load_maples_dr_diagnosis(
+                maples_dr_path / "diagnosis_infos.xls"
+            )
 
         # === Prepare MESSIDOR ===
         if messidor_path is UNSET:
-            if self._messidor_paths is None and cache is not None and (cache / "MESSIDOR").is_dir():
+            if (
+                self._messidor_paths is None
+                and cache is not None
+                and (cache / "MESSIDOR").is_dir()
+            ):
                 messidor_path = cache / "MESSIDOR"
 
         if messidor_path is not UNSET:
             if messidor_path is None:
                 self._messidor_paths = None
             else:
                 self._messidor_paths = self.discover_messidor_images(
-                    self.image_names(subset=DatasetSubset.ALL_WITH_DUPLICATES), messidor_path
+                    self.image_names(subset=DatasetSubset.ALL_WITH_DUPLICATES),
+                    messidor_path,
                 )
 
     def clear_cache(self):
         """
         Clear the cache.
         """
         if self.cfg.cache_path is not None:
@@ -236,15 +260,17 @@
         previous_cache = self.cfg.cache_path
         if previous_cache is not None and path.absolute() == previous_cache.absolute():
             return path
 
         # If a cache already existed, copy the MAPLES-DR original dataset to the new cache path.
         if previous_cache is not None:
             if (previous_cache / "AdditionalData").is_dir():
-                shutil.copytree(previous_cache / "AdditionalData", path / "AdditionalData")
+                shutil.copytree(
+                    previous_cache / "AdditionalData", path / "AdditionalData"
+                )
             if (previous_cache / "MESSIDOR").is_dir():
                 shutil.copytree(previous_cache / "MESSIDOR", path / "MESSIDOR")
 
         self.cfg._cache = path
         return path
 
     # --- Maples-DR path configuration ---
@@ -289,28 +315,31 @@
                     zip_file.extractall(path)
                 (path / "maples_dr.zip").unlink()
 
         elif path.name.endswith(".zip"):
             # === If the path is a zip file, unzip it to a temporary folder ===
             zip_path = path
             if not zip_path.exists():
-                raise InvalidConfigError(f"Invalid Maples DR archive: {zip_path} doesn't exist.")
+                raise InvalidConfigError(
+                    f"Invalid Maples DR archive: {zip_path} doesn't exist."
+                )
 
             # Create a temporary folder.
             if self.cfg.cache_path is not None:
                 path = self.cfg.cache_path / "AdditionalData"
             else:
                 path = Path(mkdtemp())
             # Unzip the dataset to the temporary folder.
             try:
                 with ZipFile(zip_path, "r") as zip_file:
                     zip_file.extractall(path)
             except Exception as e:
                 raise InvalidConfigError(
-                    f"Invalid Maples DR archive: {zip_path}:" "\n\t the provided archive is impossible to unzip."
+                    f"Invalid Maples DR archive: {zip_path}:"
+                    "\n\t the provided archive is impossible to unzip."
                 ) from e
             else:
                 # Test if the zip file contains maples_dr folder.
                 if not (path / "dataset_record.yaml").exists():
                     raise InvalidConfigError(
                         f"Invalid Maples DR archive:  {path}:"
                         '\n\t the provided archive doesn\'t contains the file "dataset_record.yaml".'
@@ -382,26 +411,30 @@
             infos = annotation_infos_data[sheet_name][biomarker_infos].copy()
             infos["Time"] = pd.to_timedelta(infos["Time"])
             infos = infos.rename(
                 columns={
                     "Retinologist": task + "_" + BiomarkersAnnotationInfos.RETINOLOGIST,
                     "Comment": task + "_" + BiomarkersAnnotationInfos.COMMENT,
                     "Time": task + "_" + BiomarkersAnnotationInfos.ANNOTATION_TIME,
-                    "Annotation #": task + "_" + BiomarkersAnnotationInfos.ANNOTATION_ID,
+                    "Annotation #": task
+                    + "_"
+                    + BiomarkersAnnotationInfos.ANNOTATION_ID,
                 },
             )
 
             if annotation_infos is None:
                 annotation_infos = infos
             else:
                 annotation_infos = annotation_infos.join(infos)
 
         return annotation_infos
 
-    def check_maples_dr_integrity(self, path: Path, biomarkers: list[str], images_names: list[str]):
+    def check_maples_dr_integrity(
+        self, path: Path, biomarkers: list[str], images_names: list[str]
+    ):
         """
         Check if the MAPLES-DR dataset contains all segmentation maps.
         """
         missing_images = 0
         for biomarker in biomarkers:
             for img in images_names:
                 if (
@@ -437,15 +470,17 @@
             .astype(str)
             .replace("nan", "")
         )
         return dr_diagnosis.join(me_diagnosis).join(dr_me_comments)
 
     # --- MESSIDOR path configuration ---
     @staticmethod
-    def discover_messidor_images(images: list[str], path: Optional[str | Path] = None) -> Dict[str, Path]:
+    def discover_messidor_images(
+        images: list[str], path: Optional[str | Path] = None
+    ) -> Dict[str, Path]:
         """
         Discover the MESSIDOR images corresponding to the given MAPLES-DR images.
 
         :param images: List of MAPLES-DR images names. The image name should not contain the extension.
         :param path: Path to the MESSIDOR dataset.
         """
         path = Path(path)
@@ -454,83 +489,93 @@
         if not path.is_dir():
             raise InvalidConfigError(f"Invalid MESSIDOR path: {path} is not a folder.")
 
         # Scan the MESSIDOR subfolders and list images.
 
         # Scan MESSIDOR subfolders to find each MAPLES-DR images.
         missing_images = set(images)
-        for jpg in chain.from_iterable(path.glob(f"**/*.{ext}") for ext in ("tif", "jpg", "png")):
+        for img_path in chain.from_iterable(
+            path.glob(f"**/*.{ext}") for ext in ("tif", "jpg", "png")
+        ):
             try:
-                missing_images.remove(jpg.stem)
+                missing_images.remove(img_path.stem)
             except KeyError:
                 pass
             else:
-                messidor_paths[jpg.stem] = jpg.absolute()
+                messidor_paths[img_path.stem] = img_path.absolute()
                 if len(missing_images) == 0:
-                    break
+                    return messidor_paths
 
         # If some images are missing, try to unzip the MESSIDOR subfolders.
         unzip_folder = path / "maples_dr"
+        unzip_folder.mkdir(parents=True, exist_ok=True)
+
         total_missing = len(missing_images)
         with RichProgress.iteration(
             "Retrieving MESSIDOR fundus from zip files...",
             total=total_missing,
             done_message=f"Extracted {total_missing} images in {'{t}'} second.",
         ) as progress:
             for zip_path in path.glob("**/*.zip"):
                 with ZipFile(zip_path, "r") as zip_file:
                     # If the zip file contains a MESSIDOR subfolder, unzip it.
-                    for zip_content in zip_file.namelist():
-                        if zip_content.endswith(".tif"):
-                            stem = (zip_content.rsplit("/", 1)[-1])[:-4]
+                    for zip_info in zip_file.infolist():
+                        if not zip_info.is_dir() and zip_info.filename.endswith(".tif"):
+                            img_filename = Path(zip_info.filename).name
+                            img_stem = Path(zip_info.filename).stem
                             try:
-                                missing_images.remove(stem)
+                                missing_images.remove(img_stem)
                             except KeyError:
-                                pass
-                            else:
-                                unzip_folder.mkdir(parents=True, exist_ok=True)
-                                unzip_path = unzip_folder / (stem + ".tif")
-                                zip_file.extract(zip_content, unzip_folder)
-                                messidor_paths[stem] = unzip_path.absolute()
-                                progress.update(1)
-                                if len(missing_images) == 0:
-                                    break
+                                continue
 
-        # If some images are still missing, raise an error.
-        if len(missing_images) > 0:
-            raise InvalidConfigError(
-                f"The provided folder to the MESSIDOR dataset is incomplete: "
-                f"{len(missing_images)} images included in MAPLES-DR are missing."
-            )
+                            zip_info.filename = img_filename
+                            zip_file.extract(zip_info, unzip_folder)
+                            messidor_paths[img_stem] = (
+                                unzip_folder / img_filename
+                            ).absolute()
+
+                            progress.update(1)
+                            if len(missing_images) == 0:
+                                return messidor_paths
 
-        return messidor_paths
+        # If some images are still missing, raise an error.
+        raise InvalidConfigError(
+            f"The provided folder to the MESSIDOR dataset is incomplete: "
+            f"{len(missing_images)} images included in MAPLES-DR are missing."
+        )
 
     # === DATASETS FACTORIES ===
-    def load_dataset(self, subset: DatasetSubset | str | list[str] = DatasetSubset.ALL) -> Dataset:
+    def load_dataset(
+        self, subset: DatasetSubset | str | list[str] = DatasetSubset.ALL
+    ) -> Dataset:
         """
         Return the MAPLES-DR dataset.
 
         :param subset: Subset of the dataset to return. If None, return the whole dataset.
                        Must be either None, "train" or "test" or a list of valid image name.
         """
         if not self.is_configured():
             self.configure()
         if isinstance(subset, list):
             # Check that all images are valid.
             valid_images = set(self.image_names(DatasetSubset.ALL_WITH_DUPLICATES))
             for img in subset:
                 if img not in valid_images:
-                    raise ValueError(f"Invalid image name: {img} is not a valid image name.")
+                    raise ValueError(
+                        f"Invalid image name: {img} is not a valid image name."
+                    )
             names = subset
         else:
             names = self.image_names(subset)
 
         paths = {}
         if self._messidor_paths is not None:
-            paths[FundusField.FUNDUS.value] = [self._messidor_paths[name] for name in names]
+            paths[FundusField.FUNDUS.value] = [
+                self._messidor_paths[name] for name in names
+            ]
 
         biomarkers_folder = {
             BiomarkerField.BRIGHT_UNCERTAINS.value: "BrightUncertains",
             BiomarkerField.COTTON_WOOL_SPOTS.value: "CottonWoolSpots",
             BiomarkerField.DRUSENS.value: "Drusens",
             BiomarkerField.EXUDATES.value: "Exudates",
             BiomarkerField.HEMORRHAGES.value: "Hemorrhages",
@@ -540,36 +585,44 @@
             BiomarkerField.OPTIC_CUP.value: "OpticCup",
             BiomarkerField.OPTIC_DISC.value: "OpticDisc",
             BiomarkerField.RED_UNCERTAINS.value: "RedUncertains",
             BiomarkerField.VESSELS.value: "Vessels",
         }
         for bio, bio_folder in biomarkers_folder.items():
             folder = self.maples_dr_folder / "annotations" / bio_folder
-            paths[bio] = [folder / (n + ".png") if self.is_biomarker_segmented(bio, n) else None for n in names]
+            paths[bio] = [
+                folder / (n + ".png") if self.is_biomarker_segmented(bio, n) else None
+                for n in names
+            ]
 
         preannotations_folder = {
             BiomarkerField.EXUDATES.value: "Exudates",
             BiomarkerField.HEMORRHAGES.value: "Hemorrhages",
             BiomarkerField.MICROANEURYSMS.value: "Microaneurysms",
             BiomarkerField.VESSELS.value: "Vessels",
         }
         for bio, bio_folder in preannotations_folder.items():
             paths[bio + "_pre"] = [
-                self.maples_dr_folder / "preannotations" / bio_folder / (name + ".png") for name in names
+                self.maples_dr_folder / "preannotations" / bio_folder / (name + ".png")
+                for name in names
             ]
 
         data = pd.DataFrame(paths, index=names)
 
         # Add the diagnosis and annotations infos.
         data = data.join(self._diagnosis).join(self._annotations_infos)
 
         return Dataset(data, self.cfg, self._messidor_ROIs)
 
     # === UTILITIES ===
-    def image_names(self, subset: DatasetSubset | str = DatasetSubset.ALL, extension: bool | str = False) -> list[str]:
+    def image_names(
+        self,
+        subset: DatasetSubset | str = DatasetSubset.ALL,
+        extension: bool | str = False,
+    ) -> list[str]:
         """
         Return the list of images names of the given subset.
 
         Parameters
         ----------
         subset
             Subset to return the images names from. If None, return all images names.
@@ -582,27 +635,37 @@
             - If a string, return the images names with the given extension.
         """
         if not self.is_configured():
             raise NotConfiguredError()
         subset = DatasetSubset(subset)
 
         names = []
-        if subset in (DatasetSubset.TRAIN, DatasetSubset.ALL, DatasetSubset.ALL_WITH_DUPLICATES):
+        if subset in (
+            DatasetSubset.TRAIN,
+            DatasetSubset.ALL,
+            DatasetSubset.ALL_WITH_DUPLICATES,
+        ):
             names += self.dataset_record["train"]
-        if subset in (DatasetSubset.TEST, DatasetSubset.ALL, DatasetSubset.ALL_WITH_DUPLICATES):
+        if subset in (
+            DatasetSubset.TEST,
+            DatasetSubset.ALL,
+            DatasetSubset.ALL_WITH_DUPLICATES,
+        ):
             names += self.dataset_record["test"]
         if subset in (DatasetSubset.DUPLICATES, DatasetSubset.ALL_WITH_DUPLICATES):
             names += list(self.dataset_record["duplicates"].values())
         if extension:
             if isinstance(extension, bool):
                 extension = "png"
             names = [name + "." + extension for name in names]
         return names
 
-    def is_biomarker_segmented(self, biomarker: BiomarkerField | str, name: str) -> bool:
+    def is_biomarker_segmented(
+        self, biomarker: BiomarkerField | str, name: str
+    ) -> bool:
         """
         Check if the given biomarker is segmented in the MAPLES-DR dataset.
 
         .. note::
 
             The macula segmentation is missing for one image centered on the optic disc.
 
@@ -620,27 +683,35 @@
         -------
         bool
             True if the biomarker is segmented, False otherwise.
         """
         if not self.is_configured():
             raise NotConfiguredError()
         biomarker = BiomarkerField.parse(biomarker)
-        if biomarker is BiomarkerField.MACULA and name in self.dataset_record["no_macula"]:
+        if (
+            biomarker is BiomarkerField.MACULA
+            and name in self.dataset_record["no_macula"]
+        ):
             return False
-        if biomarker is BiomarkerField.OPTIC_CUP and name in self.dataset_record["no_cup"]:
+        if (
+            biomarker is BiomarkerField.OPTIC_CUP
+            and name in self.dataset_record["no_cup"]
+        ):
             return False
         return True
 
 
 GLOBAL_LOADER = DatasetLoader()
 
 
 def download(url: str, path: str | Path, description: Optional[str] = None):
     """
     Download the file at the given url to the given path.
     """
     response = urlopen(url)
-    with RichProgress.download(description, byte_size=int(response.info()["Content-length"])) as progress:
+    with RichProgress.download(
+        description, byte_size=int(response.info()["Content-length"])
+    ) as progress:
         with open(path, "wb") as dest_file:
             for data in iter(partial(response.read, 32768), b""):
                 dest_file.write(data)
                 progress.update(len(data))
```

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/preprocessing.py` & `maples_dr-0.1.0rc2/src/maples_dr/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,44 @@
 from typing import Optional
 
 import numpy as np
-from skimage import measure as skmeasure
-from skimage import morphology as skmorph
 
 from .config import Preprocessing
 
+try:
+    import cv2
+except ImportError:
+    cv2 = None
+
+try:
+    from skimage import measure as skmeasure
+    from skimage import morphology as skmorph
+except ImportError:
+    skmeasure = None
+    skmorph = None
+
+
+__all__ = ["preprocess_fundus", "clahe_preprocessing", "median_preprocessing", "fundus_roi"]
+
+
+def ensure_imports(cv2_needed=False, skimage_needed=False):
+    if cv2_needed and skimage_needed and (cv2 is None and skmeasure is None):
+        raise ImportError(
+            "OpenCV and Scikit-Image are required for this function.\n"
+            "Please install them using 'pip install opencv-python-headless scikit-image'."
+        )
+    if cv2_needed and not cv2:
+        raise ImportError(
+            "OpenCV is required for this function." "Please install it using 'pip install opencv-python-headless'."
+        )
+    if skimage_needed and not skmeasure:
+        raise ImportError(
+            "Scikit-Image is required for this function." "Please install it using 'pip install scikit-image'."
+        )
+
 
 def preprocess_fundus(fundus: np.ndarray, preprocessing: Preprocessing | str) -> np.ndarray:
     """Preprocess a fundus image.
 
     Parameters
     ----------
     fundus:
@@ -54,15 +83,15 @@
     assert (
         len(fundus.shape) == 3 and fundus.shape[2] == 3
     ), f"Fundus image must be a 3-channel RGB image with shape (height, width, 3) instead of {fundus.shape}."
     mask = fundus_roi(fundus) if mask is None else mask
     assert mask.shape == fundus.shape[:2], "Mask must have the same shape as the fundus image."
 
     # CV2 is required for this preprocessing
-    import cv2
+    ensure_imports(cv2_needed=True)
 
     # Preprocessing
     mean_b = np.median(fundus[..., 0][mask])
     mean_g = np.median(fundus[..., 1][mask])
     mean_r = np.median(fundus[..., 2][mask])
     mean_channels = np.asarray([mean_b, mean_g, mean_r])
 
@@ -100,15 +129,15 @@
     assert isinstance(fundus, np.ndarray), f"Fundus image must be a numpy array instead of {type(fundus)}."
     assert fundus.dtype == np.uint8, f"Fundus image must be a 8-bit unsigned integer array instead of {fundus.dtype}."
     assert (
         len(fundus.shape) == 3 and fundus.shape[2] == 3
     ), "Fundus image must be a 3-channel RGB image with shape (height, width, 3) instead of {fundus.shape}."
 
     # CV2 is required for this preprocessing
-    import cv2
+    ensure_imports(cv2_needed=True)
 
     k = np.max(fundus.shape) // 20 * 2 + 1
     bg = cv2.medianBlur(fundus, k)
     return cv2.addWeighted(fundus, 4, bg, -4, 128)
 
 
 def fundus_roi(
@@ -141,15 +170,15 @@
 
         By default: 4.
 
     Returns:
         The ROI mask.
 
     """
-    import cv2
+    ensure_imports(skimage_needed=True, skimage_needed=morphological_clean or final_erosion > 0)
 
     fundus = cv2.medianBlur(fundus[..., 1], blur_radius * 2 - 1)
     mask = fundus > 10
 
     if morphological_clean:
         # Remove small objects
         mask = skmorph.remove_small_objects(mask, 5000)
```

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/quick_api.py` & `maples_dr-0.1.0rc2/src/maples_dr/quick_api.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/src/maples_dr/utilities.py` & `maples_dr-0.1.0rc2/src/maples_dr/utilities.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/src/maples_dr.egg-info/PKG-INFO` & `maples_dr-0.1.0rc2/src/maples_dr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: maples-dr
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Utilities python library for the public dataset: MAPLES-DR.
 Author-email: Gabriel Lepetit-Aimon <gabriel.lepetit-aimon@polymtl.ca>
 Project-URL: Homepage, https://liv4d.github.io/MAPLES-DR/en/welcome/maples_dr
 Project-URL: Documentation, https://liv4d.github.io/MAPLES-DR/en/
 Project-URL: Source, https://github.com/LIV4D/MAPlES-DR
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: xlrd
 Requires-Dist: pyyaml
 Requires-Dist: rich
-Requires-Dist: scikit-image
 Provides-Extra: examples
 Requires-Dist: plotly; extra == "examples"
 Requires-Dist: rich; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
+Requires-Dist: scikit-image; extra == "examples"
 Requires-Dist: scipy; extra == "examples"
 Requires-Dist: tqdm; extra == "examples"
 Requires-Dist: jppype; extra == "examples"
 Provides-Extra: dev
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinxcontrib-bibtex; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: sphinx-intl; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # MAPLES-DR
 
 [![doc](https://github.com/LIV4D/MAPLES-DR/actions/workflows/documentation.yml/badge.svg?branch=dev)](https://liv4d.github.io/MAPLES-DR/en/)
 
 **MAPLES-DR _(MESSIDOR Anatomical and Pathological Labels for Explainable Screening of Diabetic Retinopathy)_** is a public dataset which provides diagnoses for DR and ME as well as pixel-wise segmentation maps for 10 retinal structures for 198 images of MESSIDOR. This repository provides a python library of utility codes to ease the use of the database.
```

### Comparing `maples_dr-0.1.0rc1/src/maples_dr.egg-info/SOURCES.txt` & `maples_dr-0.1.0rc2/src/maples_dr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/tests/test_maples_dr_cache.py` & `maples_dr-0.1.0rc2/tests/test_maples_dr_cache.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/tests/test_maples_dr_dataset.py` & `maples_dr-0.1.0rc2/tests/test_maples_dr_dataset.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/tests/test_maples_dr_download.py` & `maples_dr-0.1.0rc2/tests/test_maples_dr_download.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc1/tests/test_maples_dr_fundus.py` & `maples_dr-0.1.0rc2/tests/test_maples_dr_fundus.py`

 * *Files identical despite different names*

