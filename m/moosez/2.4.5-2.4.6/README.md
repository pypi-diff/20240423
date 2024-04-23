# Comparing `tmp/moosez-2.4.5.tar.gz` & `tmp/moosez-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.4.5.tar", last modified: Wed Apr 10 09:25:55 2024, max compression
+gzip compressed data, was "moosez-2.4.6.tar", last modified: Tue Apr 23 17:34:31 2024, max compression
```

## Comparing `moosez-2.4.5.tar` & `moosez-2.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.327526 moosez-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 09:25:47.000000 moosez-2.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 09:25:55.323526 moosez-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-04-10 09:25:47.000000 moosez-2.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.323526 moosez-2.4.5/moosez/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/moosez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.323526 moosez-2.4.5/moosez/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.323526 moosez-2.4.5/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:25:55.327526 moosez-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-10 09:25:47.000000 moosez-2.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.776019 moosez-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 17:34:22.000000 moosez-2.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 17:34:31.776019 moosez-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-04-23 17:34:22.000000 moosez-2.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.772019 moosez-2.4.6/moosez/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/moosez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.772019 moosez-2.4.6/moosez/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.772019 moosez-2.4.6/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:34:31.776019 moosez-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 17:34:22.000000 moosez-2.4.6/setup.py
```

### Comparing `moosez-2.4.5/LICENSE` & `moosez-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/PKG-INFO` & `moosez-2.4.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.5
+Version: 2.4.6
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
-Home-page: https://github.com/QIMP-Team/mooseZ
+Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
-License: Apache 2.0
+License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.9.2
+Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: nnunetv2
 Requires-Dist: nibabel~=3.2.2
 Requires-Dist: halo~=0.0.31
 Requires-Dist: pandas~=1.4.1
 Requires-Dist: SimpleITK~=2.2.1
 Requires-Dist: pydicom~=2.2.2
```

### Comparing `moosez-2.4.5/README.md` & `moosez-2.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Moose-logo](Images/Moose-logo-new-2.png)
+![Moose-logo](Images/moose.png)
 ## MOOSE 2.0 🦌- Leaner. Meaner. Stronger 💪
 [![Documentation Status](https://img.shields.io/readthedocs/moosez/latest.svg?style=flat-square&logo=read-the-docs&color=CC00FF)](https://moosez.rtfd.io/en/latest/?badge=latest) [![PyPI version](https://img.shields.io/pypi/v/moosez?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/moosez/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Discord](https://img.shields.io/badge/Discord-Chat-blue.svg?style=flat-square&logo=discord&color=0000FF)](https://discord.gg/9uTHYhWCA5) [![Monthly Downloads](https://img.shields.io/pypi/dm/moosez?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/moosez/) [![Daily Downloads](https://img.shields.io/pypi/dd/moosez?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/moosez/)
 
 Unveiling a new dimension in 3D medical image segmentation: MOOSE 2.0 🚀
 
 Crafted meticulously from the core principles of data-centric AI, MOOSE 2.0 is our response to the demands of both preclinical and clinical imaging.
 
@@ -309,14 +309,15 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/LalithShiyam"><img src="https://github.com/LalithShiyam.png?s=100" width="100px;" alt="Lalith Kumar Shiyam Sundar"/><br /><sub><b>Lalith Kumar Shiyam Sundar</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=LalithShiyam" title="Code">💻</a> <a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=LalithShiyam" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Keyn34"><img src="https://github.com/Keyn34.png?s=100" width="100px;" alt="Sebastian Gutschmayer"/><br /><sub><b>Sebastian Gutschmayer</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=Keyn34" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/n7k-dobri"><img src="https://avatars.githubusercontent.com/u/114534264?v=4?s=100" width="100px;" alt="n7k-dobri"/><br /><sub><b>n7k-dobri</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=n7k-dobri" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mprires"><img src="https://avatars.githubusercontent.com/u/48754309?v=4?s=100" width="100px;" alt="Manuel Pires"/><br /><sub><b>Manuel Pires</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=mprires" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.meduniwien.ac.at/web/forschung/researcher-profiles/researcher-profiles/index.php?id=688&res=zacharias_chalampalakis1"><img src="https://avatars.githubusercontent.com/u/62066397?v=4?s=100" width="100px;" alt="Zach Chalampalakis"/><br /><sub><b>Zach Chalampalakis</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=zax0s" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dhaberl"><img src="https://avatars.githubusercontent.com/u/54232863?v=4?s=100" width="100px;" alt="David Haberl"/><br /><sub><b>David Haberl</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=dhaberl" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/W7ebere"><img src="https://avatars.githubusercontent.com/u/166598214?v=4?s=100" width="100px;" alt="W7ebere"/><br /><sub><b>W7ebere</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=W7ebere" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `moosez-2.4.5/moosez/constants.py` & `moosez-2.4.6/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/display.py` & `moosez-2.4.6/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/download.py` & `moosez-2.4.6/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/file_utilities.py` & `moosez-2.4.6/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/image_conversion.py` & `moosez-2.4.6/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/image_processing.py` & `moosez-2.4.6/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/input_validation.py` & `moosez-2.4.6/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/moosez.py` & `moosez-2.4.6/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py` & `moosez-2.4.6/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/nnUNet_custom_trainer/utility.py` & `moosez-2.4.6/moosez/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/predict.py` & `moosez-2.4.6/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/moosez/resources.py` & `moosez-2.4.6/moosez/resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,159 +57,159 @@
 #    spacing generated by nnunetv2, and you can find this in the plans.json file of the model.
 #    - multilabel_prefix: A prefix to distinguish between different types of labels in multi-label models.
 #
 # To include your own model, add a new entry to this dictionary following the above format.
 
 MODELS = {
     "clin_ct_lungs": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_lungs_24062023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_lungs_24062023.zip",
         "filename": "Dataset333_HMS3dlungs.zip",
         "directory": "Dataset333_HMS3dlungs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Lungs_",
         "configuration": "3d_fullres"
     },
     "clin_ct_organs": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/MOOSEv2_bspline_organs23062023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_organs_23062023.zip",
         "filename": "Dataset123_Organs.zip",
         "directory": "Dataset123_Organs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Organs_",
         "configuration": "3d_fullres"
     },
     "preclin_mr_all": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/preclin_mr_all_05122023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/preclin_mr_all_05122023.zip",
         "filename": "Dataset234_minimoose.zip",
         "directory": "Dataset234_minimoose",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [0.4000000059604645, 0.4000000059604645, 0.4000000059604645],
         "multilabel_prefix": "Preclin_MR_all_",
         "configuration": "3d_fullres"
     },
     "clin_ct_body": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_body_27112023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_body_27112023.zip",
         "filename": "Dataset001_body.zip",
         "directory": "Dataset001_body",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [5, 5, 5],
         "multilabel_prefix": "CT_Body_",
         "configuration": "3d_fullres"
     },
     "clin_ct_ribs": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_ribs_19032024.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_body_27112023.zip",
         "filename": "Dataset444_Ribs.zip",
         "directory": "Dataset444_Ribs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Ribs_",
         "configuration": "3d_fullres_big_patch"
     },
     "clin_ct_muscles": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_muscles_28082023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_muscles_06022024.zip",
         "filename": "Dataset555_Muscles.zip",
         "directory": "Dataset555_Muscles",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Muscles_",
         "configuration": "3d_fullres"
     },
     "clin_ct_peripheral_bones": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_peripheral_bones_28082023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_peripheral_bones_28082023.zip",
         "filename": "Dataset666_Peripheral-Bones.zip",
         "directory": "Dataset666_Peripheral-Bones",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Peripheral-Bones_",
         "configuration": "3d_fullres"
     },
     "clin_ct_fat": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_fat_31082023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_fat_31082023.zip",
         "filename": "Dataset777_Fat.zip",
         "directory": "Dataset777_Fat",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Fat_",
         "configuration": "3d_fullres"
     },
     "clin_ct_vertebrae": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_vertebrae_da5_03102023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_vertebrae_da5_03102023.zip",
         "filename": "Dataset111_Vertebrae.zip",
         "directory": "Dataset111_Vertebrae",
         "trainer": "nnUNetTrainer_2000_epochs_DA5NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Vertebrae_",
         "configuration": "3d_fullres"
     },
     "clin_ct_cardiac": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_cardiac_10092023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_vertebrae_da5_03102023.zip",
         "filename": "Dataset888_Cardiac.zip",
         "directory": "Dataset888_Cardiac",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Cardiac_",
         "configuration": "3d_fullres"
     },
     "clin_ct_digestive": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_digestive10092023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_digestive_10092023.zip",
         "filename": "Dataset999_Digestive.zip",
         "directory": "Dataset999_Digestive",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Digestive_",
         "configuration": "3d_fullres"
     },
     "preclin_ct_legs": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/preclin_ct_legs_05122023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/preclin_ct_legs_05122023.zip",
         "filename": "Dataset256_Preclin_leg_muscles.zip",
         "directory": "Dataset256_Preclin_leg_muscles",
         "trainer": "nnUNetTrainerNoMirroring",
         "voxel_spacing": [0.18000000715255737, 0.18000000715255737, 0.18000000715255737],
         "multilabel_prefix": "Preclin_CT_legs_",
         "configuration": "3d_fullres"
     },
     "clin_ct_all_bones_v1": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_all_bones_25102023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_all_bones_25102023.zip",
         "filename": "Dataset600_Original_bones.zip",
         "directory": "Dataset600_Original_bones",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_all_bones_",
         "configuration": "3d_fullres"
     },
     "clin_ct_PUMA": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_puma_04042024.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_puma_04042024.zip",
         "filename": "Dataset002_PUMA.zip",
         "directory": "Dataset002_PUMA",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_PUMA_",
         "configuration": "3d_fullres"
     },
     "clin_pt_fdg_brain_v1": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_fdg_pt_brain_v1_17112023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_puma_04042024.zip",
         "filename": "Dataset100_Brain_v1.zip",
         "directory": "Dataset100_Brain_v1",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [2.03125, 2.0862598419189453, 2.0862600803375244],
         "multilabel_prefix": "Clin_PT_FDG_brain_",
         "configuration": "3d_fullres"
     },
     "clin_ct_ALPACA": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_ALPACA.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_puma_04042024.zip",
         "filename": "Dataset080_ALPACA.zip",
         "directory": "Dataset080_ALPACA",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_ALPACA_",
         "configuration": "3d_fullres"
     },
     "clin_ct_PUMA4": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_PUMA4_06032024.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_PUMA4_06032024.zip",
         "filename": "Dataset003_PUMA4.zip",
         "directory": "Dataset003_PUMA4",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [4, 4, 4],
         "multilabel_prefix": "Clin_CT_PUMA4_",
         "configuration": "3d_fullres"
     }
```

### Comparing `moosez-2.4.5/moosez.egg-info/PKG-INFO` & `moosez-2.4.6/moosez.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.5
+Version: 2.4.6
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
-Home-page: https://github.com/QIMP-Team/mooseZ
+Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
-License: Apache 2.0
+License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.9.2
+Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: nnunetv2
 Requires-Dist: nibabel~=3.2.2
 Requires-Dist: halo~=0.0.31
 Requires-Dist: pandas~=1.4.1
 Requires-Dist: SimpleITK~=2.2.1
 Requires-Dist: pydicom~=2.2.2
```

### Comparing `moosez-2.4.5/moosez.egg-info/SOURCES.txt` & `moosez-2.4.6/moosez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moosez-2.4.5/setup.py` & `moosez-2.4.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.4.5',
+    version='2.4.6',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
-    python_requires='>=3.9.2',
+    python_requires='>=3.10',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
                      'reliable tool for medical imaging applications.',
-    url='https://github.com/QIMP-Team/mooseZ',
-    license='Apache 2.0',
+    url='https://github.com/ENHANCE-PET/MOOSE',
+    license='GPLv3',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Healthcare Industry',
-        'License :: OSI Approved :: Apache Software License',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
     ],
```

