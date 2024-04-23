# Comparing `tmp/carlschader_ml_utils-0.4.1.tar.gz` & `tmp/carlschader_ml_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carlschader_ml_utils-0.4.1.tar", last modified: Sat Apr 13 15:02:29 2024, max compression
+gzip compressed data, was "carlschader_ml_utils-0.4.2.tar", last modified: Tue Apr 23 18:48:35 2024, max compression
```

## Comparing `carlschader_ml_utils-0.4.1.tar` & `carlschader_ml_utils-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 15:02:29.432218 carlschader_ml_utils-0.4.1/
--rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-03-25 18:47:30.000000 carlschader_ml_utils-0.4.1/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-13 15:02:29.432218 carlschader_ml_utils-0.4.1/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 18:48:53.000000 carlschader_ml_utils-0.4.1/README.md
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 15:02:29.432218 carlschader_ml_utils-0.4.1/carlschader_ml_utils/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 20:37:15.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1563 2024-04-12 22:16:57.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils/embedding_utils.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5132 2024-04-13 15:02:18.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils/image_utils.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 15:02:29.432218 carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-13 15:02:29.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      360 2024-04-13 15:02:29.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-13 15:02:29.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-13 15:02:29.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       26 2024-04-13 15:02:29.000000 carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      872 2024-04-13 15:02:18.000000 carlschader_ml_utils-0.4.1/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-13 15:02:29.432218 carlschader_ml_utils-0.4.1/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 18:48:35.189609 carlschader_ml_utils-0.4.2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-03-25 18:47:30.000000 carlschader_ml_utils-0.4.2/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-23 18:48:35.189609 carlschader_ml_utils-0.4.2/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 18:48:53.000000 carlschader_ml_utils-0.4.2/README.md
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 18:48:35.186276 carlschader_ml_utils-0.4.2/carlschader_ml_utils/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 20:37:15.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1563 2024-04-12 22:16:57.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils/embedding_utils.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5231 2024-04-23 18:47:38.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils/image_utils.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 18:48:35.189609 carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-23 18:48:35.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      360 2024-04-23 18:48:35.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-23 18:48:35.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-23 18:48:35.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       26 2024-04-23 18:48:35.000000 carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      872 2024-04-23 18:48:03.000000 carlschader_ml_utils-0.4.2/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-23 18:48:35.189609 carlschader_ml_utils-0.4.2/setup.cfg
```

### Comparing `carlschader_ml_utils-0.4.1/LICENSE` & `carlschader_ml_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carlschader_ml_utils-0.4.1/PKG-INFO` & `carlschader_ml_utils-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carlschader_ml_utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: A collection of utilities for machine learning projects
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ml-utils
 Project-URL: Issues, https://github.com/carlschader/ml-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `carlschader_ml_utils-0.4.1/carlschader_ml_utils/embedding_utils.py` & `carlschader_ml_utils-0.4.2/carlschader_ml_utils/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `carlschader_ml_utils-0.4.1/carlschader_ml_utils/image_utils.py` & `carlschader_ml_utils-0.4.2/carlschader_ml_utils/image_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, shutil
+import os, shutil, multiprocessing
 import torch
 import torchvision
 from torchvision.datasets import ImageFolder
 import torchvision.transforms as transforms
 from torchvision import datasets
 
 # def embed_image(
@@ -27,19 +27,20 @@
     transform=torchvision.transforms.Compose([
         torchvision.transforms.Resize((244, 244)),
         torchvision.transforms.ToTensor(),
         torchvision.transforms.Normalize(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
     ]),
     batch_size=32,
     averages_only=False,
+    num_workers=max(multiprocessing.cpu_count() - 1, 0),
     device=torch.device('cpu'),
     verbose=False,
     ):
     dataset = ImageFolder(root=data_folder, transform=transform)
-    data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=False)
+    data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, num_workers=num_workers, shuffle=False)
     
     shutil.rmtree(save_dir, ignore_errors=True)
     os.mkdir(save_dir)
 
     # get output shape of model by sampling a single image
     sample_image, _ = dataset[0]
     sample_image = sample_image.unsqueeze(0).to(device)
```

### Comparing `carlschader_ml_utils-0.4.1/carlschader_ml_utils.egg-info/PKG-INFO` & `carlschader_ml_utils-0.4.2/carlschader_ml_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carlschader_ml_utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: A collection of utilities for machine learning projects
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ml-utils
 Project-URL: Issues, https://github.com/carlschader/ml-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `carlschader_ml_utils-0.4.1/pyproject.toml` & `carlschader_ml_utils-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carlschader_ml_utils"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "A collection of utilities for machine learning projects"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

