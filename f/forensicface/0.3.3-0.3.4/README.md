# Comparing `tmp/forensicface-0.3.3.tar.gz` & `tmp/forensicface-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forensicface-0.3.3.tar", last modified: Thu Feb 22 00:01:42 2024, max compression
+gzip compressed data, was "forensicface-0.3.4.tar", last modified: Tue Apr 23 21:17:03 2024, max compression
```

## Comparing `forensicface-0.3.3.tar` & `forensicface-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2024-02-22 00:01:42.633438 forensicface-0.3.3/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     1510 2023-06-21 19:39:31.000000 forensicface-0.3.3/LICENSE
--rw-r--r--   0 rafael    (1000) rafael    (1000)      111 2023-06-21 19:39:31.000000 forensicface-0.3.3/MANIFEST.in
--rw-r--r--   0 rafael    (1000) rafael    (1000)     5891 2024-02-22 00:01:42.633438 forensicface-0.3.3/PKG-INFO
--rw-r--r--   0 rafael    (1000) rafael    (1000)     5133 2023-12-13 01:36:33.000000 forensicface-0.3.3/README.md
-drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2024-02-22 00:01:42.623438 forensicface-0.3.3/forensicface/
--rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2024-02-21 23:55:36.000000 forensicface-0.3.3/forensicface/__init__.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)     5398 2024-02-21 23:55:36.000000 forensicface-0.3.3/forensicface/_modidx.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    24149 2024-02-21 23:55:36.000000 forensicface-0.3.3/forensicface/app.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)      142 2023-06-21 19:39:31.000000 forensicface-0.3.3/forensicface/core.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)     3279 2023-06-21 19:39:31.000000 forensicface-0.3.3/forensicface/forensicface.py
-drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2024-02-22 00:01:42.633438 forensicface-0.3.3/forensicface.egg-info/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     5891 2024-02-22 00:01:42.000000 forensicface-0.3.3/forensicface.egg-info/PKG-INFO
--rw-r--r--   0 rafael    (1000) rafael    (1000)      423 2024-02-22 00:01:42.000000 forensicface-0.3.3/forensicface.egg-info/SOURCES.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2024-02-22 00:01:42.000000 forensicface-0.3.3/forensicface.egg-info/dependency_links.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)       46 2024-02-22 00:01:42.000000 forensicface-0.3.3/forensicface.egg-info/entry_points.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2023-06-21 19:59:31.000000 forensicface-0.3.3/forensicface.egg-info/not-zip-safe
--rw-r--r--   0 rafael    (1000) rafael    (1000)       77 2024-02-22 00:01:42.000000 forensicface-0.3.3/forensicface.egg-info/requires.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)       13 2024-02-22 00:01:42.000000 forensicface-0.3.3/forensicface.egg-info/top_level.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)     1028 2024-02-21 23:53:22.000000 forensicface-0.3.3/settings.ini
--rw-r--r--   0 rafael    (1000) rafael    (1000)       38 2024-02-22 00:01:42.633438 forensicface-0.3.3/setup.cfg
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2541 2023-06-21 19:39:31.000000 forensicface-0.3.3/setup.py
+drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-23 21:17:03.952401 forensicface-0.3.4/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     1510 2023-06-21 19:39:31.000000 forensicface-0.3.4/LICENSE
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      111 2023-06-21 19:39:31.000000 forensicface-0.3.4/MANIFEST.in
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     5891 2024-04-23 21:17:03.952401 forensicface-0.3.4/PKG-INFO
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     5133 2023-12-13 01:36:33.000000 forensicface-0.3.4/README.md
+drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-23 21:17:03.952401 forensicface-0.3.4/forensicface/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2024-04-23 21:07:00.000000 forensicface-0.3.4/forensicface/__init__.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     5398 2024-04-23 21:07:00.000000 forensicface-0.3.4/forensicface/_modidx.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    23874 2024-04-23 21:07:00.000000 forensicface-0.3.4/forensicface/app.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      142 2023-06-21 19:39:31.000000 forensicface-0.3.4/forensicface/core.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     3279 2023-06-21 19:39:31.000000 forensicface-0.3.4/forensicface/forensicface.py
+drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-23 21:17:03.952401 forensicface-0.3.4/forensicface.egg-info/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     5891 2024-04-23 21:17:03.000000 forensicface-0.3.4/forensicface.egg-info/PKG-INFO
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      423 2024-04-23 21:17:03.000000 forensicface-0.3.4/forensicface.egg-info/SOURCES.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2024-04-23 21:17:03.000000 forensicface-0.3.4/forensicface.egg-info/dependency_links.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       46 2024-04-23 21:17:03.000000 forensicface-0.3.4/forensicface.egg-info/entry_points.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2023-06-21 19:59:31.000000 forensicface-0.3.4/forensicface.egg-info/not-zip-safe
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       77 2024-04-23 21:17:03.000000 forensicface-0.3.4/forensicface.egg-info/requires.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       13 2024-04-23 21:17:03.000000 forensicface-0.3.4/forensicface.egg-info/top_level.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     1028 2024-04-23 21:03:23.000000 forensicface-0.3.4/settings.ini
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       38 2024-04-23 21:17:03.952401 forensicface-0.3.4/setup.cfg
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2541 2023-06-21 19:39:31.000000 forensicface-0.3.4/setup.py
```

### Comparing `forensicface-0.3.3/LICENSE` & `forensicface-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `forensicface-0.3.3/PKG-INFO` & `forensicface-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forensicface
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for forensic face examination
 Home-page: https://github.com/rafribeiro/forensicface
 Author: Rafael O. Ribeiro
 Author-email: rafaeloliveiraribeiro@gmail.com
 License: BSD License
 Keywords: nbdev jupyter python face recognition forensics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `forensicface-0.3.3/README.md` & `forensicface-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `forensicface-0.3.3/forensicface/_modidx.py` & `forensicface-0.3.4/forensicface/_modidx.py`

 * *Files identical despite different names*

### Comparing `forensicface-0.3.3/forensicface/app.py` & `forensicface-0.3.4/forensicface/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,26 @@
     def __init__(
         self,
         model: str = "sepaelv2",
         det_size: int = 320,
         use_gpu: bool = True,
         gpu: int = 0,  # which GPU to use
         extended=True,
+        det_thresh: float = 0.5,
     ):
         """
         A face comparison tool for forensic analysis and comparison of facial images.
 
         Args:
         - model (str): The name of the face recognition model to use (default: "sepaelv2").
         - det_size (int): The size of the input images for face detection (default: 320).
         - use_gpu (bool): Whether to use a GPU for inference (default: True).
         - gpu (int): The ID of the GPU to use (default: 0).
-        - magface (bool): Whether to use MagFace for face recognition (default: False).
         - extended (bool): Whether to use extended modules (detection, landmark_3d_68, genderage) (default: True).
+        - det_thresh (float): threshold for the face detector (default = 0.5).
         """
         self.extended = extended
         if self.extended == True:
             allowed_modules = ["detection", "landmark_3d_68", "genderage"]
             self.ort_fiqa = onnxruntime.InferenceSession(
                 osp.join(
                     osp.expanduser("~/.insightface/models"),
@@ -57,27 +58,32 @@
                     else ["CPUExecutionProvider"]
                 ),
             )
         else:
             allowed_modules = ["detection"]
 
         self.det_size = (det_size, det_size)
+        self.det_thresh = det_thresh
 
         self.model = model
 
         self.detectmodel = FaceAnalysis(
             name=model,
             allowed_modules=allowed_modules,
             providers=(
                 [("CUDAExecutionProvider", {"device_id": gpu})]
                 if use_gpu
                 else ["CPUExecutionProvider"]
             ),
         )
-        self.detectmodel.prepare(ctx_id=gpu if use_gpu else -1, det_size=self.det_size)
+        self.detectmodel.prepare(
+            ctx_id=gpu if use_gpu else -1,
+            det_size=self.det_size,
+            det_thresh=self.det_thresh,
+        )
 
         onnx_rec_model = glob(
             osp.join(
                 osp.expanduser("~/.insightface/models"),
                 model,
                 "adaface",
                 "adaface_*.onnx",
@@ -190,46 +196,43 @@
 
                 - 'pitch': A float representing the pitch angle for each face in the image.
 
                 - 'yaw': A float representing the yaw angle for each face in the image.
 
                 - 'roll': A float representing the roll angle for each face in the image.
 
-                If the 'magface' attribute is set to True, the dictionary will also contain the following keys:
-                - 'magface_embedding': A 1D numpy array of shape (512,) containing the magface
-                                          embedding for each face in the image.
-
-                - 'magface_norm': A float representing the L2 norm of the magface embedding for
-                                     each face in the image.
+                - 'det_score': A float representing the face detection score.
         """
         if type(imgpath) == str:  # image path passed as argument
             bgr_img = cv2.imread(imgpath)
         else:  # image array passed as argument
             bgr_img = imgpath.copy()
         faces = self.detectmodel.get(bgr_img)
         if len(faces) == 0:
             return {}
 
         idx, kps = self.get_larger_face(bgr_img, faces)
 
         bbox = faces[idx].bbox.astype("int")
         bgr_aligned_face = face_align.norm_crop(bgr_img, kps)
         ipd = np.linalg.norm(kps[0] - kps[1])
+        det_score = faces[idx].det_score
 
         ada_inputs = {
             self.ort_ada.get_inputs()[0].name: self._to_input_ada(bgr_aligned_face)
         }
         normalized_embedding, norm = self.ort_ada.run(None, ada_inputs)
 
         ret = {
             "keypoints": kps,
             "ipd": ipd,
             "embedding": normalized_embedding.flatten() * norm.flatten()[0],
             "norm": norm.flatten()[0],
             "bbox": bbox,
+            "det_score": det_score,
             "aligned_face": cv2.cvtColor(bgr_aligned_face, cv2.COLOR_BGR2RGB),
         }
 
         if self.extended:
             gender = "M" if faces[idx].gender == 1 else "F"
             age = faces[idx].age
             pitch, yaw, roll = faces[idx].pose
@@ -285,20 +288,17 @@
 
             - 'pitch': A float representing the pitch angle for each face in the image.
 
             - 'yaw': A float representing the yaw angle for each face in the image.
 
             - 'roll: A float representing the roll angle for each face in the image.
 
-         If the 'magface' attribute is set to True, the dictionary will also contain the following keys:
-            - 'magface_embedding': A 1D numpy array of shape (512,) containing the magface
-                                    embedding for each face in the image.
+            - 'fiqa_score': A float representing image quality estimated by the CR-FIQA(L) model (https://doi.org/10.1109/CVPR52729.2023.00565).
 
-            - 'magface_norm': A float representing the L2 norm of the magface embedding for
-                                each face in the image.
+            - 'det_score': A float representing the face detection score
 
         Args:
             - imgpath (str): The file path to the image to be processed.
 
         Returns:
             - A list of dictionaries, with each dictionary representing a face in the image.
         """
@@ -311,24 +311,26 @@
             return []
         ret = []
         for face in faces:
             kps = face.kps
             bbox = face.bbox.astype("int")
             bgr_aligned_face = face_align.norm_crop(bgr_img, kps)
             ipd = np.linalg.norm(kps[0] - kps[1])
+            det_score = face.det_score
             ada_inputs = {
                 self.ort_ada.get_inputs()[0].name: self._to_input_ada(bgr_aligned_face)
             }
             normalized_embedding, norm = self.ort_ada.run(None, ada_inputs)
             face_ret = {
                 "keypoints": kps,
                 "ipd": ipd,
                 "embedding": normalized_embedding.flatten() * norm.flatten()[0],
                 "norm": norm.flatten()[0],
                 "bbox": bbox,
+                "det_score": det_score,
                 "aligned_face": cv2.cvtColor(bgr_aligned_face, cv2.COLOR_BGR2RGB),
             }
 
             if self.extended:
                 gender = "M" if face.gender == 1 else "F"
                 age = face.age
                 pitch, yaw, roll = face.pose
```

### Comparing `forensicface-0.3.3/forensicface/forensicface.py` & `forensicface-0.3.4/forensicface/forensicface.py`

 * *Files identical despite different names*

### Comparing `forensicface-0.3.3/forensicface.egg-info/PKG-INFO` & `forensicface-0.3.4/forensicface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forensicface
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for forensic face examination
 Home-page: https://github.com/rafribeiro/forensicface
 Author: Rafael O. Ribeiro
 Author-email: rafaeloliveiraribeiro@gmail.com
 License: BSD License
 Keywords: nbdev jupyter python face recognition forensics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `forensicface-0.3.3/settings.ini` & `forensicface-0.3.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = forensicface
 lib_name = %(repo)s
-version = 0.3.3
+version = 0.3.4
 min_python = 3.8
 license = bsd3
 
 ### nbdev ###
 doc_path = _docs
 lib_path = forensicface
 nbs_path = nbs
```

### Comparing `forensicface-0.3.3/setup.py` & `forensicface-0.3.4/setup.py`

 * *Files identical despite different names*

