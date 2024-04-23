# Comparing `tmp/moosez-2.4.6.tar.gz` & `tmp/moosez-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.4.6.tar", last modified: Tue Apr 23 17:34:31 2024, max compression
+gzip compressed data, was "moosez-2.4.7.tar", last modified: Tue Apr 23 18:28:25 2024, max compression
```

## Comparing `moosez-2.4.6.tar` & `moosez-2.4.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.776019 moosez-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 17:34:22.000000 moosez-2.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 17:34:31.776019 moosez-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-04-23 17:34:22.000000 moosez-2.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.772019 moosez-2.4.6/moosez/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/moosez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.772019 moosez-2.4.6/moosez/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-23 17:34:22.000000 moosez-2.4.6/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:34:31.772019 moosez-2.4.6/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 17:34:31.000000 moosez-2.4.6/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:34:31.776019 moosez-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 17:34:22.000000 moosez-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 18:28:18.000000 moosez-2.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 18:28:25.191945 moosez-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-04-23 18:28:18.000000 moosez-2.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/moosez/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/moosez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/moosez/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:28:25.191945 moosez-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 18:28:18.000000 moosez-2.4.7/setup.py
```

### Comparing `moosez-2.4.6/LICENSE` & `moosez-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/PKG-INFO` & `moosez-2.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.6
+Version: 2.4.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.6/README.md` & `moosez-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/constants.py` & `moosez-2.4.7/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/display.py` & `moosez-2.4.7/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/download.py` & `moosez-2.4.7/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/file_utilities.py` & `moosez-2.4.7/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/image_conversion.py` & `moosez-2.4.7/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/image_processing.py` & `moosez-2.4.7/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/input_validation.py` & `moosez-2.4.7/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/moosez.py` & `moosez-2.4.7/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py` & `moosez-2.4.7/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/nnUNet_custom_trainer/utility.py` & `moosez-2.4.7/moosez/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/predict.py` & `moosez-2.4.7/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/moosez/resources.py` & `moosez-2.4.7/moosez/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         "directory": "Dataset001_body",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [5, 5, 5],
         "multilabel_prefix": "CT_Body_",
         "configuration": "3d_fullres"
     },
     "clin_ct_ribs": {
-        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_body_27112023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_ribs_19032024.zip",
         "filename": "Dataset444_Ribs.zip",
         "directory": "Dataset444_Ribs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Ribs_",
         "configuration": "3d_fullres_big_patch"
     },
@@ -138,15 +138,15 @@
         "directory": "Dataset111_Vertebrae",
         "trainer": "nnUNetTrainer_2000_epochs_DA5NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Vertebrae_",
         "configuration": "3d_fullres"
     },
     "clin_ct_cardiac": {
-        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_vertebrae_da5_03102023.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_cardiac_26012024.zip",
         "filename": "Dataset888_Cardiac.zip",
         "directory": "Dataset888_Cardiac",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Cardiac_",
         "configuration": "3d_fullres"
     },
@@ -183,24 +183,24 @@
         "directory": "Dataset002_PUMA",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_PUMA_",
         "configuration": "3d_fullres"
     },
     "clin_pt_fdg_brain_v1": {
-        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_puma_04042024.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_fdg_pt_brain_v1_17112023.zip",
         "filename": "Dataset100_Brain_v1.zip",
         "directory": "Dataset100_Brain_v1",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [2.03125, 2.0862598419189453, 2.0862600803375244],
         "multilabel_prefix": "Clin_PT_FDG_brain_",
         "configuration": "3d_fullres"
     },
     "clin_ct_ALPACA": {
-        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_puma_04042024.zip",
+        "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/moose/clin_ct_ALPACA.zip",
         "filename": "Dataset080_ALPACA.zip",
         "directory": "Dataset080_ALPACA",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_ALPACA_",
         "configuration": "3d_fullres"
     },
```

### Comparing `moosez-2.4.6/moosez.egg-info/PKG-INFO` & `moosez-2.4.7/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.6
+Version: 2.4.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.6/moosez.egg-info/SOURCES.txt` & `moosez-2.4.7/moosez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moosez-2.4.6/setup.py` & `moosez-2.4.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.4.6',
+    version='2.4.7',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.10',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

