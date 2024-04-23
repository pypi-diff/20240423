# Comparing `tmp/fremu-0.0.3.tar.gz` & `tmp/fremu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fremu-0.0.3.tar", last modified: Tue Apr 23 07:02:12 2024, max compression
+gzip compressed data, was "fremu-0.0.4.tar", last modified: Tue Apr 23 07:51:04 2024, max compression
```

## Comparing `fremu-0.0.3.tar` & `fremu-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:02:12.116860 fremu-0.0.3/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       22 2024-04-23 06:36:44.000000 fremu-0.0.3/MANIFEST.in
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:02:12.116860 fremu-0.0.3/PKG-INFO
--rw-rw-r--   0 baijc     (1000) baijc     (1000)        0 2024-04-23 04:19:30.000000 fremu-0.0.3/README.md
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:02:12.116860 fremu-0.0.3/fremu/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 06:30:52.000000 fremu-0.0.3/fremu/__ini__.py
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:02:12.116860 fremu-0.0.3/fremu/cache/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)     7216 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/k.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_0.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_0.5.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_1.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_2.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_3.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_ann_0.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_ann_0.5.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_ann_1.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_ann_2.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/pc_ann_3.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      761 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/scaler.pkl
--rw-rw-r--   0 baijc     (1000) baijc     (1000)     2128 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/cache/sigma.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)     9057 2024-04-23 04:14:13.000000 fremu-0.0.3/fremu/fremu.py
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:02:12.116860 fremu-0.0.3/fremu.egg-info/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:02:12.000000 fremu-0.0.3/fremu.egg-info/PKG-INFO
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      519 2024-04-23 07:02:12.000000 fremu-0.0.3/fremu.egg-info/SOURCES.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)        1 2024-04-23 07:02:12.000000 fremu-0.0.3/fremu.egg-info/dependency_links.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 07:02:12.000000 fremu-0.0.3/fremu.egg-info/requires.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)        6 2024-04-23 07:02:12.000000 fremu-0.0.3/fremu.egg-info/top_level.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       38 2024-04-23 07:02:12.116860 fremu-0.0.3/setup.cfg
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      753 2024-04-23 07:01:32.000000 fremu-0.0.3/setup.py
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.485891 fremu-0.0.4/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       22 2024-04-23 06:36:44.000000 fremu-0.0.4/MANIFEST.in
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:51:04.485891 fremu-0.0.4/PKG-INFO
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)        0 2024-04-23 04:19:30.000000 fremu-0.0.4/README.md
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.481891 fremu-0.0.4/fremu/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 06:30:52.000000 fremu-0.0.4/fremu/__ini__.py
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.485891 fremu-0.0.4/fremu/cache/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)     7216 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/k.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_0.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_0.5.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_1.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_2.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_3.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_0.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_0.5.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_1.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_2.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_3.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      761 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/scaler.pkl
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)     2128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/sigma.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)     9101 2024-04-23 07:49:26.000000 fremu-0.0.4/fremu/fremu.py
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.481891 fremu-0.0.4/fremu.egg-info/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/PKG-INFO
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      519 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/SOURCES.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)        1 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/dependency_links.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/requires.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)        6 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/top_level.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       38 2024-04-23 07:51:04.485891 fremu-0.0.4/setup.cfg
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      753 2024-04-23 07:50:56.000000 fremu-0.0.4/setup.py
```

### Comparing `fremu-0.0.3/fremu/cache/k.npy` & `fremu-0.0.4/fremu/cache/k.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_0.0.npy` & `fremu-0.0.4/fremu/cache/pc_0.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_0.5.npy` & `fremu-0.0.4/fremu/cache/pc_0.5.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_1.0.npy` & `fremu-0.0.4/fremu/cache/pc_1.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_2.0.npy` & `fremu-0.0.4/fremu/cache/pc_2.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_3.0.npy` & `fremu-0.0.4/fremu/cache/pc_3.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_ann_0.0.pth` & `fremu-0.0.4/fremu/cache/pc_ann_0.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_ann_0.5.pth` & `fremu-0.0.4/fremu/cache/pc_ann_0.5.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_ann_1.0.pth` & `fremu-0.0.4/fremu/cache/pc_ann_1.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_ann_2.0.pth` & `fremu-0.0.4/fremu/cache/pc_ann_2.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/pc_ann_3.0.pth` & `fremu-0.0.4/fremu/cache/pc_ann_3.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/scaler.pkl` & `fremu-0.0.4/fremu/cache/scaler.pkl`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/cache/sigma.npy` & `fremu-0.0.4/fremu/cache/sigma.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/fremu/fremu.py` & `fremu-0.0.4/fremu/fremu.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 import torch.nn as nn
 import pickle
 import numpy as np
 from scipy.interpolate import CubicSpline
 import os
 import camb
 
-
-#=====================================================================================================
-#=====================================================================================================
-# neural network
 class BkANN(nn.Module):
     def __init__(self, input_size, hidden_size1, output_size):
         super(BkANN, self).__init__()
         self.hidden_layer1 = nn.Linear(input_size, hidden_size1)
         self.hidden_activation1 = nn.Sigmoid()
         self.output_layer = nn.Linear(hidden_size1, output_size)
 
@@ -22,43 +18,46 @@
         x = self.hidden_activation1(x)
         x = self.output_layer(x)
         return x
     
 class emulator:
     def __init__(self):
         
-        self.ks = np.load('./cache/k.npy')
+        module_path = os.path.dirname(__file__)
+        cache_path = os.path.join(module_path, 'cache') 
+        
+        self.ks = np.load(os.path.join(cache_path, 'k.npy'))
         self.ks = self.ks[:250]
         
         self.scaler = None
-        with open('./cache/scaler.pkl', 'rb') as scaler_file:
+        with open(os.path.join(cache_path,'scaler.pkl'), 'rb') as scaler_file:
             self.scaler = pickle.load(scaler_file)
         
         self.pc = {}
         self.mean = {}
         
         for z in [0.0, 0.5, 1.0, 2.0, 3.0]:
-            pc = np.load(f'./cache/pc_{z:.1f}.npy')
+            pc = np.load(os.path.join(cache_path,f'pc_{z:.1f}.npy'))
             self.mean[z] = pc[0, :]
             self.pc[z] = pc[1:, :]
         n_hidd = 650
         n_out = 30
         self.model0 = BkANN(7, n_hidd, n_out)
         self.model05 = BkANN(7, n_hidd, n_out)
         self.model1 = BkANN(7, n_hidd, n_out)
         self.model2 = BkANN(7, n_hidd, n_out)
         self.model3 = BkANN(7, n_hidd, n_out)
             
-        self.model0.load_state_dict(torch.load('./cache/pc_ann_0.0.pth'))
-        self.model05.load_state_dict(torch.load('./cache/pc_ann_0.5.pth'))
-        self.model1.load_state_dict(torch.load('./cache/pc_ann_1.0.pth'))
-        self.model2.load_state_dict(torch.load('./cache/pc_ann_2.0.pth'))
-        self.model3.load_state_dict(torch.load('./cache/pc_ann_3.0.pth'))
+        self.model0.load_state_dict(torch.load(os.path.join(cache_path,'pc_ann_0.0.pth')))
+        self.model05.load_state_dict(torch.load(os.path.join(cache_path,'pc_ann_0.5.pth')))
+        self.model1.load_state_dict(torch.load(os.path.join(cache_path,'pc_ann_1.0.pth')))
+        self.model2.load_state_dict(torch.load(os.path.join(cache_path,'pc_ann_2.0.pth')))
+        self.model3.load_state_dict(torch.load(os.path.join(cache_path,'pc_ann_3.0.pth')))
         
-        self.sigma = np.load('./cache/sigma.npy')
+        self.sigma = np.load(os.path.join(cache_path,'sigma.npy'))
         
     def get_error(self, k=None):      
         if k is None:
             return self.sigma
         sigma_interp = CubicSpline(self.ks,self.sigma)
         err = sigma_interp(k)
         return err
```

### Comparing `fremu-0.0.3/fremu.egg-info/SOURCES.txt` & `fremu-0.0.4/fremu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fremu-0.0.3/setup.py` & `fremu-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fremu",
-    version="0.0.3",
+    version="0.0.4",
     author="Jiachen Bai",
     author_email="astrobaijc@gmail.com",  
     description="Emulator for f(R) gravity",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/astrobai/fremu",
     py_modules=['fremu'],
```

