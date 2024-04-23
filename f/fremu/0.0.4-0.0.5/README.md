# Comparing `tmp/fremu-0.0.4.tar.gz` & `tmp/fremu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fremu-0.0.4.tar", last modified: Tue Apr 23 07:51:04 2024, max compression
+gzip compressed data, was "fremu-0.0.5.tar", last modified: Tue Apr 23 07:56:23 2024, max compression
```

## Comparing `fremu-0.0.4.tar` & `fremu-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.485891 fremu-0.0.4/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       22 2024-04-23 06:36:44.000000 fremu-0.0.4/MANIFEST.in
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:51:04.485891 fremu-0.0.4/PKG-INFO
--rw-rw-r--   0 baijc     (1000) baijc     (1000)        0 2024-04-23 04:19:30.000000 fremu-0.0.4/README.md
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.481891 fremu-0.0.4/fremu/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 06:30:52.000000 fremu-0.0.4/fremu/__ini__.py
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.485891 fremu-0.0.4/fremu/cache/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)     7216 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/k.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_0.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_0.5.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_1.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_2.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_3.0.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_0.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_0.5.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_1.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_2.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/pc_ann_3.0.pth
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      761 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/scaler.pkl
--rw-rw-r--   0 baijc     (1000) baijc     (1000)     2128 2024-04-23 04:14:13.000000 fremu-0.0.4/fremu/cache/sigma.npy
--rw-rw-r--   0 baijc     (1000) baijc     (1000)     9101 2024-04-23 07:49:26.000000 fremu-0.0.4/fremu/fremu.py
-drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:51:04.481891 fremu-0.0.4/fremu.egg-info/
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/PKG-INFO
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      519 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/SOURCES.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)        1 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/dependency_links.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/requires.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)        6 2024-04-23 07:51:04.000000 fremu-0.0.4/fremu.egg-info/top_level.txt
--rw-rw-r--   0 baijc     (1000) baijc     (1000)       38 2024-04-23 07:51:04.485891 fremu-0.0.4/setup.cfg
--rw-rw-r--   0 baijc     (1000) baijc     (1000)      753 2024-04-23 07:50:56.000000 fremu-0.0.4/setup.py
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:56:23.298761 fremu-0.0.5/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       22 2024-04-23 06:36:44.000000 fremu-0.0.5/MANIFEST.in
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:56:23.298761 fremu-0.0.5/PKG-INFO
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)        0 2024-04-23 04:19:30.000000 fremu-0.0.5/README.md
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:56:23.294761 fremu-0.0.5/fremu/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       25 2024-04-23 06:30:52.000000 fremu-0.0.5/fremu/__ini__.py
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:56:23.298761 fremu-0.0.5/fremu/cache/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)     7216 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/k.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_0.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_0.5.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_1.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_2.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)    62128 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_3.0.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_ann_0.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_ann_0.5.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_ann_1.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_ann_2.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)   100904 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/pc_ann_3.0.pth
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      761 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/scaler.pkl
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)     2128 2024-04-23 04:14:13.000000 fremu-0.0.5/fremu/cache/sigma.npy
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)     9101 2024-04-23 07:49:26.000000 fremu-0.0.5/fremu/fremu.py
+drwxrwxr-x   0 baijc     (1000) baijc     (1000)        0 2024-04-23 07:56:23.294761 fremu-0.0.5/fremu.egg-info/
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      415 2024-04-23 07:56:23.000000 fremu-0.0.5/fremu.egg-info/PKG-INFO
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      519 2024-04-23 07:56:23.000000 fremu-0.0.5/fremu.egg-info/SOURCES.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)        1 2024-04-23 07:56:23.000000 fremu-0.0.5/fremu.egg-info/dependency_links.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       30 2024-04-23 07:56:23.000000 fremu-0.0.5/fremu.egg-info/requires.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)        6 2024-04-23 07:56:23.000000 fremu-0.0.5/fremu.egg-info/top_level.txt
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)       38 2024-04-23 07:56:23.298761 fremu-0.0.5/setup.cfg
+-rw-rw-r--   0 baijc     (1000) baijc     (1000)      760 2024-04-23 07:56:12.000000 fremu-0.0.5/setup.py
```

### Comparing `fremu-0.0.4/fremu/cache/k.npy` & `fremu-0.0.5/fremu/cache/k.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_0.0.npy` & `fremu-0.0.5/fremu/cache/pc_0.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_0.5.npy` & `fremu-0.0.5/fremu/cache/pc_0.5.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_1.0.npy` & `fremu-0.0.5/fremu/cache/pc_1.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_2.0.npy` & `fremu-0.0.5/fremu/cache/pc_2.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_3.0.npy` & `fremu-0.0.5/fremu/cache/pc_3.0.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_ann_0.0.pth` & `fremu-0.0.5/fremu/cache/pc_ann_0.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_ann_0.5.pth` & `fremu-0.0.5/fremu/cache/pc_ann_0.5.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_ann_1.0.pth` & `fremu-0.0.5/fremu/cache/pc_ann_1.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_ann_2.0.pth` & `fremu-0.0.5/fremu/cache/pc_ann_2.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/pc_ann_3.0.pth` & `fremu-0.0.5/fremu/cache/pc_ann_3.0.pth`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/scaler.pkl` & `fremu-0.0.5/fremu/cache/scaler.pkl`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/cache/sigma.npy` & `fremu-0.0.5/fremu/cache/sigma.npy`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu/fremu.py` & `fremu-0.0.5/fremu/fremu.py`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/fremu.egg-info/SOURCES.txt` & `fremu-0.0.5/fremu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fremu-0.0.4/setup.py` & `fremu-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fremu",
-    version="0.0.4",
+    version="0.0.5",
     author="Jiachen Bai",
     author_email="astrobaijc@gmail.com",  
     description="Emulator for f(R) gravity",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/astrobai/fremu",
     py_modules=['fremu'],
     packages=['fremu'],
     package_data={'fremu': ['cache/*']},
     install_requires=[
         'numpy',
         'scipy',
         'torch',
-        'pickle',
+        'pickle >= 1.0',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
```

