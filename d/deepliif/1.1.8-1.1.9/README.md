# Comparing `tmp/deepliif-1.1.8.tar.gz` & `tmp/deepliif-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepliif-1.1.8.tar", last modified: Fri Jan 19 17:11:28 2024, max compression
+gzip compressed data, was "deepliif-1.1.9.tar", last modified: Mon Jan 29 21:36:33 2024, max compression
```

## Comparing `deepliif-1.1.8.tar` & `deepliif-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:28.187394 deepliif-1.1.8/
--rw-rw-rw-   0        0        0      956 2022-11-10 15:00:10.000000 deepliif-1.1.8/LICENSE.md
--rw-rw-rw-   0        0        0    24703 2024-01-19 17:11:28.188394 deepliif-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    24262 2023-12-21 23:54:45.000000 deepliif-1.1.8/README.md
--rw-rw-rw-   0        0        0    39723 2024-01-17 23:15:35.000000 deepliif-1.1.8/cli.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:27.893377 deepliif-1.1.8/deepliif/
--rw-rw-rw-   0        0        0        0 2022-03-16 15:16:26.000000 deepliif-1.1.8/deepliif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:27.998383 deepliif-1.1.8/deepliif/data/
--rw-rw-rw-   0        0        0     5281 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/__init__.py
--rw-rw-rw-   0        0        0     4405 2023-12-21 23:54:45.000000 deepliif-1.1.8/deepliif/data/aligned_dataset.py
--rw-rw-rw-   0        0        0     5564 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/base_dataset.py
--rw-rw-rw-   0        0        0     2808 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/colorization_dataset.py
--rw-rw-rw-   0        0        0     2006 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/image_folder.py
--rw-rw-rw-   0        0        0     1553 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/single_dataset.py
--rw-rw-rw-   0        0        0     3592 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/template_dataset.py
--rw-rw-rw-   0        0        0     3393 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/data/unaligned_dataset.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:28.052386 deepliif-1.1.8/deepliif/models/
--rw-rw-rw-   0        0        0    14527 2023-12-21 23:54:45.000000 deepliif-1.1.8/deepliif/models/DeepLIIFExt_model.py
--rw-rw-rw-   0        0        0    20872 2023-12-21 23:54:45.000000 deepliif-1.1.8/deepliif/models/DeepLIIF_model.py
--rw-rw-rw-   0        0        0    22565 2024-01-17 21:50:34.000000 deepliif-1.1.8/deepliif/models/__init__.py
--rw-rw-rw-   0        0        0    15583 2023-12-21 23:54:45.000000 deepliif-1.1.8/deepliif/models/base_model.py
--rw-rw-rw-   0        0        0    32177 2023-03-13 14:58:54.000000 deepliif-1.1.8/deepliif/models/networks.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:28.098389 deepliif-1.1.8/deepliif/options/
--rw-rw-rw-   0        0        0     4581 2023-12-21 23:54:45.000000 deepliif-1.1.8/deepliif/options/__init__.py
--rw-rw-rw-   0        0        0     9852 2023-12-22 16:14:43.000000 deepliif-1.1.8/deepliif/options/base_options.py
--rw-rw-rw-   0        0        0     2947 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/options/processing_options.py
--rw-rw-rw-   0        0        0     1114 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/options/test_options.py
--rw-rw-rw-   0        0        0     3580 2023-03-13 14:58:54.000000 deepliif-1.1.8/deepliif/options/train_options.py
--rw-rw-rw-   0        0        0    17327 2024-01-17 22:21:37.000000 deepliif-1.1.8/deepliif/postprocessing.py
--rw-rw-rw-   0        0        0    15757 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/train.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:28.154392 deepliif-1.1.8/deepliif/util/
--rw-rw-rw-   0        0        0    16924 2023-03-15 11:44:25.000000 deepliif-1.1.8/deepliif/util/__init__.py
--rw-rw-rw-   0        0        0     3749 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/util/get_data.py
--rw-rw-rw-   0        0        0     3309 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/util/html.py
--rw-rw-rw-   0        0        0     2280 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/util/image_pool.py
--rw-rw-rw-   0        0        0     4636 2023-03-13 14:58:41.000000 deepliif-1.1.8/deepliif/util/util.py
--rw-rw-rw-   0        0        0    15636 2022-11-10 15:00:10.000000 deepliif-1.1.8/deepliif/util/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:27.925378 deepliif-1.1.8/deepliif.egg-info/
--rw-rw-rw-   0        0        0    24703 2024-01-19 17:11:27.000000 deepliif-1.1.8/deepliif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2024-01-19 17:11:27.000000 deepliif-1.1.8/deepliif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-19 17:11:27.000000 deepliif-1.1.8/deepliif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-01-19 17:11:27.000000 deepliif-1.1.8/deepliif.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      182 2024-01-19 17:11:27.000000 deepliif-1.1.8/deepliif.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-19 17:11:27.000000 deepliif-1.1.8/deepliif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      230 2024-01-19 17:11:28.190394 deepliif-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1175 2024-01-19 16:38:26.000000 deepliif-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-19 17:11:28.186393 deepliif-1.1.8/tests/
--rw-rw-rw-   0        0        0      156 2023-12-21 23:54:45.000000 deepliif-1.1.8/tests/test_args.py
--rw-rw-rw-   0        0        0    19235 2023-12-21 23:54:45.000000 deepliif-1.1.8/tests/test_cli_inference.py
--rw-rw-rw-   0        0        0      698 2023-12-21 23:54:45.000000 deepliif-1.1.8/tests/test_cli_serialize.py
--rw-rw-rw-   0        0        0     3530 2023-12-21 23:54:45.000000 deepliif-1.1.8/tests/test_cli_train.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.363089 deepliif-1.1.9/
+-rw-rw-rw-   0        0        0      956 2022-11-10 15:00:10.000000 deepliif-1.1.9/LICENSE.md
+-rw-rw-rw-   0        0        0    24704 2024-01-29 21:36:33.364090 deepliif-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    24263 2024-01-29 20:38:59.000000 deepliif-1.1.9/README.md
+-rw-rw-rw-   0        0        0    39723 2024-01-17 23:15:35.000000 deepliif-1.1.9/cli.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:32.969067 deepliif-1.1.9/deepliif/
+-rw-rw-rw-   0        0        0        0 2022-03-16 15:16:26.000000 deepliif-1.1.9/deepliif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.106075 deepliif-1.1.9/deepliif/data/
+-rw-rw-rw-   0        0        0     5281 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/__init__.py
+-rw-rw-rw-   0        0        0     4405 2023-12-21 23:54:45.000000 deepliif-1.1.9/deepliif/data/aligned_dataset.py
+-rw-rw-rw-   0        0        0     5564 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/base_dataset.py
+-rw-rw-rw-   0        0        0     2808 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/colorization_dataset.py
+-rw-rw-rw-   0        0        0     2006 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/image_folder.py
+-rw-rw-rw-   0        0        0     1553 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/single_dataset.py
+-rw-rw-rw-   0        0        0     3592 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/template_dataset.py
+-rw-rw-rw-   0        0        0     3393 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/data/unaligned_dataset.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.178079 deepliif-1.1.9/deepliif/models/
+-rw-rw-rw-   0        0        0    14527 2023-12-21 23:54:45.000000 deepliif-1.1.9/deepliif/models/DeepLIIFExt_model.py
+-rw-rw-rw-   0        0        0    20872 2023-12-21 23:54:45.000000 deepliif-1.1.9/deepliif/models/DeepLIIF_model.py
+-rw-rw-rw-   0        0        0    22674 2024-01-25 22:16:11.000000 deepliif-1.1.9/deepliif/models/__init__.py
+-rw-rw-rw-   0        0        0    15583 2023-12-21 23:54:45.000000 deepliif-1.1.9/deepliif/models/base_model.py
+-rw-rw-rw-   0        0        0    32177 2023-03-13 14:58:54.000000 deepliif-1.1.9/deepliif/models/networks.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.242083 deepliif-1.1.9/deepliif/options/
+-rw-rw-rw-   0        0        0     4581 2023-12-21 23:54:45.000000 deepliif-1.1.9/deepliif/options/__init__.py
+-rw-rw-rw-   0        0        0     9852 2023-12-22 16:14:43.000000 deepliif-1.1.9/deepliif/options/base_options.py
+-rw-rw-rw-   0        0        0     2947 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/options/processing_options.py
+-rw-rw-rw-   0        0        0     1114 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/options/test_options.py
+-rw-rw-rw-   0        0        0     3580 2023-03-13 14:58:54.000000 deepliif-1.1.9/deepliif/options/train_options.py
+-rw-rw-rw-   0        0        0    17589 2024-01-25 22:15:50.000000 deepliif-1.1.9/deepliif/postprocessing.py
+-rw-rw-rw-   0        0        0    15757 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/train.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.316087 deepliif-1.1.9/deepliif/util/
+-rw-rw-rw-   0        0        0    16924 2023-03-15 11:44:25.000000 deepliif-1.1.9/deepliif/util/__init__.py
+-rw-rw-rw-   0        0        0     3749 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/util/get_data.py
+-rw-rw-rw-   0        0        0     3309 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/util/html.py
+-rw-rw-rw-   0        0        0     2280 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/util/image_pool.py
+-rw-rw-rw-   0        0        0     4636 2023-03-13 14:58:41.000000 deepliif-1.1.9/deepliif/util/util.py
+-rw-rw-rw-   0        0        0    15636 2022-11-10 15:00:10.000000 deepliif-1.1.9/deepliif/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.010069 deepliif-1.1.9/deepliif.egg-info/
+-rw-rw-rw-   0        0        0    24704 2024-01-29 21:36:32.000000 deepliif-1.1.9/deepliif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2024-01-29 21:36:32.000000 deepliif-1.1.9/deepliif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-29 21:36:32.000000 deepliif-1.1.9/deepliif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-01-29 21:36:32.000000 deepliif-1.1.9/deepliif.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      182 2024-01-29 21:36:32.000000 deepliif-1.1.9/deepliif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-01-29 21:36:32.000000 deepliif-1.1.9/deepliif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      230 2024-01-29 21:36:33.367090 deepliif-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2024-01-29 21:25:55.000000 deepliif-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 21:36:33.360089 deepliif-1.1.9/tests/
+-rw-rw-rw-   0        0        0      156 2023-12-21 23:54:45.000000 deepliif-1.1.9/tests/test_args.py
+-rw-rw-rw-   0        0        0    19235 2023-12-21 23:54:45.000000 deepliif-1.1.9/tests/test_cli_inference.py
+-rw-rw-rw-   0        0        0      698 2023-12-21 23:54:45.000000 deepliif-1.1.9/tests/test_cli_serialize.py
+-rw-rw-rw-   0        0        0     3530 2023-12-21 23:54:45.000000 deepliif-1.1.9/tests/test_cli_train.py
```

### Comparing `deepliif-1.1.8/LICENSE.md` & `deepliif-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/PKG-INFO` & `deepliif-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepliif
-Version: 1.1.8
+Version: 1.1.9
 Summary: DeepLIIF: Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification
 Home-page: https://github.com/nadeemlab/DeepLIIF
 Author: Parmida93
 Author-email: ghahremani.parmida@gmail.com
 Keywords: DeepLIIF,IHC,Segmentation,Classification
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -255,15 +255,15 @@
 
 Parameters
 
 img (required)
 file: image to run the models on
 
 resolution
-string: resolution used to scan the slide (10x, 20x, 40x), defaults to 20x 
+string: resolution used to scan the slide (10x, 20x, 40x), defaults to 40x 
 
 pil
 boolean: if true, use PIL.Image.open() to load the image, instead of python-bioformats
 
 slim
 boolean: if true, return only the segmentation result image
 ```
@@ -284,17 +284,17 @@
 filename = 'ROI_1.png'
 
 res = requests.post(
     url='https://deepliif.org/api/infer',
     files={
         'img': open(f'{images_dir}/{filename}', 'rb')
     },
-    # optional param that can be 10x, 20x (default) or 40x
+    # optional param that can be 10x, 20x, or 40x (default)
     params={
-        'resolution': '20x'
+        'resolution': '40x'
     }
 )
 
 data = res.json()
 
 def b64_to_pil(b):
     return Image.open(BytesIO(base64.b64decode(b.encode())))
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepliif Version: 1.1.8 Summary: DeepLIIF: Deep-
+Metadata-Version: 2.1 Name: deepliif Version: 1.1.9 Summary: DeepLIIF: Deep-
 Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image
 Quantification Home-page: https://github.com/nadeemlab/DeepLIIF Author:
 Parmida93 Author-email: ghahremani.parmida@gmail.com Keywords:
 DeepLIIF,IHC,Segmentation,Classification Description-Content-Type: text/
 markdown License-File: LICENSE.md
                          [./images/DeepLIIF_logo.png]
          ******** DDeeeepp--LLeeaarrnniinngg IInnffeerrrreedd MMuullttiipplleexx IImmmmuunnoofflluuoorreesscceennccee ffoorr
@@ -191,23 +191,23 @@
 GPU or appropriate hardware and don't want to install ImageJ, we have also
 created a [cloud-native DeepLIIF deployment](https://deepliif.org) with a user-
 friendly interface to upload images, visualize, interact, and download the
 final results. ![DeepLIIF Website Demo](images/deepliif-website-demo-03.gif)
 DeepLIIF can also be accessed programmatically through an endpoint by posting a
 multipart-encoded request containing the original image file: ``` POST /api/
 infer Parameters img (required) file: image to run the models on resolution
-string: resolution used to scan the slide (10x, 20x, 40x), defaults to 20x pil
+string: resolution used to scan the slide (10x, 20x, 40x), defaults to 40x pil
 boolean: if true, use PIL.Image.open() to load the image, instead of python-
 bioformats slim boolean: if true, return only the segmentation result image ```
 For example, in Python: ```python import os import json import base64 from io
 import BytesIO import requests from PIL import Image # Use the sample images
 from the main DeepLIIF repo images_dir = './Sample_Large_Tissues' filename =
 'ROI_1.png' res = requests.post( url='https://deepliif.org/api/infer', files=
 { 'img': open(f'{images_dir}/{filename}', 'rb') }, # optional param that can be
-10x, 20x (default) or 40x params={ 'resolution': '20x' } ) data = res.json()
+10x, 20x, or 40x (default) params={ 'resolution': '40x' } ) data = res.json()
 def b64_to_pil(b): return Image.open(BytesIO(base64.b64decode(b.encode()))) for
 name, img in data['images'].items(): output_filepath = f'{images_dir}/
 {os.path.splitext(filename)[0]}_{name}.png' with open(output_filepath, 'wb') as
 f: b64_to_pil(img).save(f, format='PNG') print(json.dumps(data['scoring'],
 indent=2)) ``` ## Synthetic Data Generation The first version of DeepLIIF model
 suffered from its inability to separate IHC positive cells in some large
 clusters, resulting from the absence of clustered positive cells in our
```

### Comparing `deepliif-1.1.8/README.md` & `deepliif-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
 Parameters
 
 img (required)
 file: image to run the models on
 
 resolution
-string: resolution used to scan the slide (10x, 20x, 40x), defaults to 20x 
+string: resolution used to scan the slide (10x, 20x, 40x), defaults to 40x 
 
 pil
 boolean: if true, use PIL.Image.open() to load the image, instead of python-bioformats
 
 slim
 boolean: if true, return only the segmentation result image
 ```
@@ -273,17 +273,17 @@
 filename = 'ROI_1.png'
 
 res = requests.post(
     url='https://deepliif.org/api/infer',
     files={
         'img': open(f'{images_dir}/{filename}', 'rb')
     },
-    # optional param that can be 10x, 20x (default) or 40x
+    # optional param that can be 10x, 20x, or 40x (default)
     params={
-        'resolution': '20x'
+        'resolution': '40x'
     }
 )
 
 data = res.json()
 
 def b64_to_pil(b):
     return Image.open(BytesIO(base64.b64decode(b.encode())))
```

#### html2text {}

```diff
@@ -185,23 +185,23 @@
 GPU or appropriate hardware and don't want to install ImageJ, we have also
 created a [cloud-native DeepLIIF deployment](https://deepliif.org) with a user-
 friendly interface to upload images, visualize, interact, and download the
 final results. ![DeepLIIF Website Demo](images/deepliif-website-demo-03.gif)
 DeepLIIF can also be accessed programmatically through an endpoint by posting a
 multipart-encoded request containing the original image file: ``` POST /api/
 infer Parameters img (required) file: image to run the models on resolution
-string: resolution used to scan the slide (10x, 20x, 40x), defaults to 20x pil
+string: resolution used to scan the slide (10x, 20x, 40x), defaults to 40x pil
 boolean: if true, use PIL.Image.open() to load the image, instead of python-
 bioformats slim boolean: if true, return only the segmentation result image ```
 For example, in Python: ```python import os import json import base64 from io
 import BytesIO import requests from PIL import Image # Use the sample images
 from the main DeepLIIF repo images_dir = './Sample_Large_Tissues' filename =
 'ROI_1.png' res = requests.post( url='https://deepliif.org/api/infer', files=
 { 'img': open(f'{images_dir}/{filename}', 'rb') }, # optional param that can be
-10x, 20x (default) or 40x params={ 'resolution': '20x' } ) data = res.json()
+10x, 20x, or 40x (default) params={ 'resolution': '40x' } ) data = res.json()
 def b64_to_pil(b): return Image.open(BytesIO(base64.b64decode(b.encode()))) for
 name, img in data['images'].items(): output_filepath = f'{images_dir}/
 {os.path.splitext(filename)[0]}_{name}.png' with open(output_filepath, 'wb') as
 f: b64_to_pil(img).save(f, format='PNG') print(json.dumps(data['scoring'],
 indent=2)) ``` ## Synthetic Data Generation The first version of DeepLIIF model
 suffered from its inability to separate IHC positive cells in some large
 clusters, resulting from the absence of clustered positive cells in our
```

### Comparing `deepliif-1.1.8/cli.py` & `deepliif-1.1.9/cli.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/__init__.py` & `deepliif-1.1.9/deepliif/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/aligned_dataset.py` & `deepliif-1.1.9/deepliif/data/aligned_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/base_dataset.py` & `deepliif-1.1.9/deepliif/data/base_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/colorization_dataset.py` & `deepliif-1.1.9/deepliif/data/colorization_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/image_folder.py` & `deepliif-1.1.9/deepliif/data/image_folder.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/single_dataset.py` & `deepliif-1.1.9/deepliif/data/single_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/template_dataset.py` & `deepliif-1.1.9/deepliif/data/template_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/data/unaligned_dataset.py` & `deepliif-1.1.9/deepliif/data/unaligned_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/models/DeepLIIFExt_model.py` & `deepliif-1.1.9/deepliif/models/DeepLIIFExt_model.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/models/DeepLIIF_model.py` & `deepliif-1.1.9/deepliif/models/DeepLIIF_model.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/models/__init__.py` & `deepliif-1.1.9/deepliif/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,19 @@
     if mode == 'train':
         opt = Options(path_file=os.path.join(model_dir,'train_opt.txt'), mode=mode)
     elif mode == 'test':
         try:
             opt = Options(path_file=os.path.join(model_dir,'test_opt.txt'), mode=mode)
         except:
             opt = Options(path_file=os.path.join(model_dir,'train_opt.txt'), mode=mode)
+        opt.use_dp = False
+        opt.gpu_ids = list(range(torch.cuda.device_count()))
     return opt
 
+
 def find_model_using_name(model_name):
     """Import the module "models/[model_name]_model.py".
 
     In the file, the class called DatasetNameModel() will
     be instantiated. It has to be a subclass of BaseModel,
     and it is case-insensitive.
     """
@@ -144,15 +147,15 @@
     
     opt_args: to overwrite opt arguments in train_opt.txt, typically used in inference stage
               for example, opt_args={'phase':'test'}
     """ 
     if opt is None:
         opt = get_opt(model_dir, mode=phase)
         opt.use_dp = False
-        print_options(opt)
+        #print_options(opt)
     
     if opt.model == 'DeepLIIF':
         net_groups = [
             ('G1', 'G52'),
             ('G2', 'G53'),
             ('G3', 'G54'),
             ('G4', 'G55'),
@@ -164,15 +167,15 @@
         else:
             net_groups = [(f'G_{i+1}',) for i in range(opt.modalities_no)]
     else:
         raise Exception(f'init_nets() not implemented for model {opt.model}')
 
     number_of_gpus_all = torch.cuda.device_count()
     number_of_gpus = len(opt.gpu_ids)
-    print(number_of_gpus)
+    #print(number_of_gpus)
     if number_of_gpus > 0:
         mapping_gpu_ids = {i:idx for i,idx in enumerate(opt.gpu_ids)}
         chunks = [itertools.chain.from_iterable(c) for c in chunker(net_groups, number_of_gpus)]
         # chunks = chunks[1:]
         devices = {n: torch.device(f'cuda:{mapping_gpu_ids[i]}') for i, g in enumerate(chunks) for n in g}
         # devices = {n: torch.device(f'cuda:{i}') for i, g in enumerate(chunks) for n in g}
     else:
@@ -347,15 +350,15 @@
     return images
 
 
 def inference(img, tile_size, overlap_size, model_path, use_torchserve=False, eager_mode=False,
               color_dapi=False, color_marker=False, opt=None):
     if not opt:
         opt = get_opt(model_path)
-        print_options(opt)
+        #print_options(opt)
     
     if opt.model == 'DeepLIIF':
         rescaled, rows, cols = format_image_for_tiling(img, tile_size, overlap_size)
     
         run_fn = run_torchserve if use_torchserve else run_dask
     
         images = {}
@@ -420,26 +423,26 @@
     
         return images
     
     else:
         raise Exception(f'inference() not implemented for model {opt.model}')
 
 
-def postprocess(orig, images, tile_size, seg_thresh=150, size_thresh='default', marker_thresh='default', size_thresh_upper=None, opt=None):
-    if opt.model == 'DeepLIIF':
+def postprocess(orig, images, tile_size, model, seg_thresh=150, size_thresh='auto', marker_thresh='auto', size_thresh_upper=None):
+    if model == 'DeepLIIF':
         resolution = '40x' if tile_size > 384 else ('20x' if tile_size > 192 else '10x')
         overlay, refined, scoring = compute_results(np.array(orig), np.array(images['Seg']),
-                                                    np.array(images['Marker'].convert('L')), resolution,
-                                                    seg_thresh, size_thresh, marker_thresh, size_thresh_upper)
+                                                    np.array(images['Marker'].convert('L')) if 'Marker' in images else None,
+                                                    resolution, seg_thresh, size_thresh, marker_thresh, size_thresh_upper)
         processed_images = {}
         processed_images['SegOverlaid'] = Image.fromarray(overlay)
         processed_images['SegRefined'] = Image.fromarray(refined)
         return processed_images, scoring
 
-    elif opt.model == 'DeepLIIFExt':
+    elif model == 'DeepLIIFExt':
         resolution = '40x' if tile_size > 768 else ('20x' if tile_size > 384 else '10x')
         processed_images = {}
         scoring = {}
         for img_name in list(images.keys()):
             if 'Seg' in img_name:
                 seg_img = images[img_name]
                 overlay, refined, score = compute_results(np.array(orig), np.array(images[img_name]),
@@ -448,30 +451,30 @@
     
                 processed_images[img_name + '_Overlaid'] = Image.fromarray(overlay)
                 processed_images[img_name + '_Refined'] = Image.fromarray(refined)
                 scoring[img_name] = score
         return processed_images, scoring
 
     else:
-        raise Exception(f'postprocess() not implemented for model {opt.model}')
+        raise Exception(f'postprocess() not implemented for model {model}')
 
 
 def infer_modalities(img, tile_size, model_dir, eager_mode=False,
                      color_dapi=False, color_marker=False, opt=None):
     """
     This function is used to infer modalities for the given image using a trained model.
     :param img: The input image.
     :param tile_size: The tile size.
     :param model_dir: The directory containing serialized model files.
     :return: The inferred modalities and the segmentation mask.
     """
     if opt is None:
         opt = get_opt(model_dir)
         opt.use_dp = False
-        print_options(opt)
+        #print_options(opt)
     
     if not tile_size:
         tile_size = check_multi_scale(Image.open('./images/target.png').convert('L'),
                                       img.convert('L'))
     tile_size = int(tile_size)
 
     images = inference(
@@ -482,15 +485,15 @@
         eager_mode=eager_mode,
         color_dapi=color_dapi,
         color_marker=color_marker,
         opt=opt
     )
     
     if not hasattr(opt,'seg_gen') or (hasattr(opt,'seg_gen') and opt.seg_gen): # the first condition accounts for old settings of deepliif; the second refers to deepliifext models
-        post_images, scoring = postprocess(img, images, tile_size, opt=opt)
+        post_images, scoring = postprocess(img, images, tile_size, opt.model)
         images = {**images, **post_images}
         return images, scoring
     else:
         return images, None
 
 
 def infer_results_for_wsi(input_dir, filename, output_dir, model_dir, tile_size, region_size=20000):
```

### Comparing `deepliif-1.1.8/deepliif/models/base_model.py` & `deepliif-1.1.9/deepliif/models/base_model.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/models/networks.py` & `deepliif-1.1.9/deepliif/models/networks.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/options/__init__.py` & `deepliif-1.1.9/deepliif/options/__init__.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/options/base_options.py` & `deepliif-1.1.9/deepliif/options/base_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/options/processing_options.py` & `deepliif-1.1.9/deepliif/options/processing_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/options/test_options.py` & `deepliif-1.1.9/deepliif/options/test_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/options/train_options.py` & `deepliif-1.1.9/deepliif/options/train_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/postprocessing.py` & `deepliif-1.1.9/deepliif/postprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,31 +397,38 @@
         nonzero = marker[marker != 0]
         marker_range = (round(np.percentile(nonzero, 0.1)), round(np.percentile(nonzero, 99.9))) if nonzero.shape[0] > 0 else (0, 0)
         return round((marker_range[1] - marker_range[0]) * 0.9) + marker_range[0]
     else:
         return 0
 
 
-def compute_results(orig, seg, marker, resolution=None, seg_thresh=150, size_thresh='default', marker_thresh='default', size_thresh_upper=None):
+def compute_results(orig, seg, marker, resolution=None, seg_thresh=150, size_thresh='auto', marker_thresh='auto', size_thresh_upper=None):
     mask = create_posneg_mask(seg, seg_thresh)
     mark_background(mask)
 
-    if size_thresh == 'default':
+    if size_thresh == 'auto':
         size_thresh = calc_default_size_thresh(mask, resolution)
-    if marker_thresh == 'default':
+    if marker_thresh is None:
+        marker_thresh = 0
+        marker = None
+    elif marker_thresh == 'auto':
         marker_thresh = calc_default_marker_thresh(marker)
 
-    counts = compute_cell_classification(mask, marker, size_thresh, marker_thresh, size_thresh_upper=None)
+    counts = compute_cell_classification(mask, marker, size_thresh, marker_thresh, size_thresh_upper)
     enlarge_cell_boundaries(mask)
 
     scoring = {
         'num_total': counts['num_total'],
         'num_pos': counts['num_pos'],
         'num_neg': counts['num_neg'],
-        'percent_pos': round(counts['num_pos'] / counts['num_total'] * 100, 1) if counts['num_pos'] > 0 else 0
+        'percent_pos': round(counts['num_pos'] / counts['num_total'] * 100, 1) if counts['num_pos'] > 0 else 0,
+        'prob_thresh': seg_thresh,
+        'size_thresh': size_thresh,
+        'size_thresh_upper': size_thresh_upper,
+        'marker_thresh': marker_thresh if marker is not None else None,
     }
 
     overlay = np.copy(orig)
     overlay[mask == MASK_BOUNDARY_POSITIVE] = (255, 0, 0)
     overlay[mask == MASK_BOUNDARY_NEGATIVE] = (0, 0, 255)
 
     refined = np.zeros_like(seg)
```

### Comparing `deepliif-1.1.8/deepliif/train.py` & `deepliif-1.1.9/deepliif/train.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/util/__init__.py` & `deepliif-1.1.9/deepliif/util/__init__.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/util/get_data.py` & `deepliif-1.1.9/deepliif/util/get_data.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/util/html.py` & `deepliif-1.1.9/deepliif/util/html.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/util/image_pool.py` & `deepliif-1.1.9/deepliif/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/util/util.py` & `deepliif-1.1.9/deepliif/util/util.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif/util/visualizer.py` & `deepliif-1.1.9/deepliif/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/deepliif.egg-info/PKG-INFO` & `deepliif-1.1.9/deepliif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepliif
-Version: 1.1.8
+Version: 1.1.9
 Summary: DeepLIIF: Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification
 Home-page: https://github.com/nadeemlab/DeepLIIF
 Author: Parmida93
 Author-email: ghahremani.parmida@gmail.com
 Keywords: DeepLIIF,IHC,Segmentation,Classification
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -255,15 +255,15 @@
 
 Parameters
 
 img (required)
 file: image to run the models on
 
 resolution
-string: resolution used to scan the slide (10x, 20x, 40x), defaults to 20x 
+string: resolution used to scan the slide (10x, 20x, 40x), defaults to 40x 
 
 pil
 boolean: if true, use PIL.Image.open() to load the image, instead of python-bioformats
 
 slim
 boolean: if true, return only the segmentation result image
 ```
@@ -284,17 +284,17 @@
 filename = 'ROI_1.png'
 
 res = requests.post(
     url='https://deepliif.org/api/infer',
     files={
         'img': open(f'{images_dir}/{filename}', 'rb')
     },
-    # optional param that can be 10x, 20x (default) or 40x
+    # optional param that can be 10x, 20x, or 40x (default)
     params={
-        'resolution': '20x'
+        'resolution': '40x'
     }
 )
 
 data = res.json()
 
 def b64_to_pil(b):
     return Image.open(BytesIO(base64.b64decode(b.encode())))
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepliif Version: 1.1.8 Summary: DeepLIIF: Deep-
+Metadata-Version: 2.1 Name: deepliif Version: 1.1.9 Summary: DeepLIIF: Deep-
 Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image
 Quantification Home-page: https://github.com/nadeemlab/DeepLIIF Author:
 Parmida93 Author-email: ghahremani.parmida@gmail.com Keywords:
 DeepLIIF,IHC,Segmentation,Classification Description-Content-Type: text/
 markdown License-File: LICENSE.md
                          [./images/DeepLIIF_logo.png]
          ******** DDeeeepp--LLeeaarrnniinngg IInnffeerrrreedd MMuullttiipplleexx IImmmmuunnoofflluuoorreesscceennccee ffoorr
@@ -191,23 +191,23 @@
 GPU or appropriate hardware and don't want to install ImageJ, we have also
 created a [cloud-native DeepLIIF deployment](https://deepliif.org) with a user-
 friendly interface to upload images, visualize, interact, and download the
 final results. ![DeepLIIF Website Demo](images/deepliif-website-demo-03.gif)
 DeepLIIF can also be accessed programmatically through an endpoint by posting a
 multipart-encoded request containing the original image file: ``` POST /api/
 infer Parameters img (required) file: image to run the models on resolution
-string: resolution used to scan the slide (10x, 20x, 40x), defaults to 20x pil
+string: resolution used to scan the slide (10x, 20x, 40x), defaults to 40x pil
 boolean: if true, use PIL.Image.open() to load the image, instead of python-
 bioformats slim boolean: if true, return only the segmentation result image ```
 For example, in Python: ```python import os import json import base64 from io
 import BytesIO import requests from PIL import Image # Use the sample images
 from the main DeepLIIF repo images_dir = './Sample_Large_Tissues' filename =
 'ROI_1.png' res = requests.post( url='https://deepliif.org/api/infer', files=
 { 'img': open(f'{images_dir}/{filename}', 'rb') }, # optional param that can be
-10x, 20x (default) or 40x params={ 'resolution': '20x' } ) data = res.json()
+10x, 20x, or 40x (default) params={ 'resolution': '40x' } ) data = res.json()
 def b64_to_pil(b): return Image.open(BytesIO(base64.b64decode(b.encode()))) for
 name, img in data['images'].items(): output_filepath = f'{images_dir}/
 {os.path.splitext(filename)[0]}_{name}.png' with open(output_filepath, 'wb') as
 f: b64_to_pil(img).save(f, format='PNG') print(json.dumps(data['scoring'],
 indent=2)) ``` ## Synthetic Data Generation The first version of DeepLIIF model
 suffered from its inability to separate IHC positive cells in some large
 clusters, resulting from the absence of clustered positive cells in our
```

### Comparing `deepliif-1.1.8/deepliif.egg-info/SOURCES.txt` & `deepliif-1.1.9/deepliif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/setup.py` & `deepliif-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='deepliif',
-    version='1.1.8',
+    version='1.1.9',
     packages=['deepliif', 'deepliif.data', 'deepliif.models', 'deepliif.util', 'deepliif.options'],
 
     description='DeepLIIF: Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification',
     author='Parmida93',
     author_email='ghahremani.parmida@gmail.com',
     url='https://github.com/nadeemlab/DeepLIIF',
     long_description=README,
```

### Comparing `deepliif-1.1.8/tests/test_cli_inference.py` & `deepliif-1.1.9/tests/test_cli_inference.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/tests/test_cli_serialize.py` & `deepliif-1.1.9/tests/test_cli_serialize.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.8/tests/test_cli_train.py` & `deepliif-1.1.9/tests/test_cli_train.py`

 * *Files identical despite different names*

