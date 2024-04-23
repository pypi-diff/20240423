# Comparing `tmp/fc_pruning-0.0.1.tar.gz` & `tmp/fc_pruning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc_pruning-0.0.1.tar", last modified: Mon Apr 15 22:18:02 2024, max compression
+gzip compressed data, was "fc_pruning-0.0.2.tar", last modified: Tue Apr 23 17:25:08 2024, max compression
```

## Comparing `fc_pruning-0.0.1.tar` & `fc_pruning-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-15 22:18:02.989425 fc_pruning-0.0.1/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc_pruning-0.0.1/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-15 22:18:02.989330 fc_pruning-0.0.1/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-15 22:17:45.000000 fc_pruning-0.0.1/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-15 22:18:02.989149 fc_pruning-0.0.1/fc_pruning.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-15 22:18:02.000000 fc_pruning-0.0.1/fc_pruning.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      195 2024-04-15 22:18:02.000000 fc_pruning-0.0.1/fc_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-04-15 22:18:02.000000 fc_pruning-0.0.1/fc_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-04-15 22:18:02.000000 fc_pruning-0.0.1/fc_pruning.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-04-15 22:18:02.000000 fc_pruning-0.0.1/fc_pruning.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-04-15 22:18:02.989480 fc_pruning-0.0.1/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1052 2024-04-15 22:17:45.000000 fc_pruning-0.0.1/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:25:08.252511 fc_pruning-0.0.2/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:25:08.251247 fc_pruning-0.0.2/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:07:18.000000 fc_pruning-0.0.2/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     5617 2024-04-19 19:55:07.000000 fc_pruning-0.0.2/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4071 2024-04-19 19:55:07.000000 fc_pruning-0.0.2/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc_pruning-0.0.2/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-23 17:25:08.252384 fc_pruning-0.0.2/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-15 22:17:45.000000 fc_pruning-0.0.2/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:25:08.252096 fc_pruning-0.0.2/fc_pruning.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      255 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        9 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-04-23 17:25:08.252563 fc_pruning-0.0.2/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1052 2024-04-23 17:22:45.000000 fc_pruning-0.0.2/setup.py
```

### Comparing `fc_pruning-0.0.1/LICENSE` & `fc_pruning-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.1/PKG-INFO` & `fc_pruning-0.0.2/fc_pruning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: fc_pruning
-Version: 0.0.1
+Name: fc-pruning
+Version: 0.0.2
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [FeatureCloud Pruning](https://github.com/AidaMehammed/Image-Classification-Pruning)
 ### Model Compression with Pruning
 
 The FC Pruning package offers a streamlined approach to model compression using advanced pruning techniques. With support for federated learning frameworks and integration with the [Torch-Pruning](https://github.com/VainF/Torch-Pruning/tree/master) library, this package enables efficient distributed training, suitable for a wide range of machine learning tasks.
```

### Comparing `fc_pruning-0.0.1/README.md` & `fc_pruning-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.1/fc_pruning.egg-info/PKG-INFO` & `fc_pruning-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: fc-pruning
-Version: 0.0.1
+Name: fc_pruning
+Version: 0.0.2
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [FeatureCloud Pruning](https://github.com/AidaMehammed/Image-Classification-Pruning)
 ### Model Compression with Pruning
 
 The FC Pruning package offers a streamlined approach to model compression using advanced pruning techniques. With support for federated learning frameworks and integration with the [Torch-Pruning](https://github.com/VainF/Torch-Pruning/tree/master) library, this package enables efficient distributed training, suitable for a wide range of machine learning tasks.
```

### Comparing `fc_pruning-0.0.1/setup.py` & `fc_pruning-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc_pruning",
-                 version="0.0.1",
+                 version="0.0.2",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Pruning",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc_pruning",
                  project_urls={
@@ -16,12 +16,12 @@
                  },
                  packages=setuptools.find_packages(include=['Compress','Compress.*']),
 
                  classifiers=[
                      "Programming Language :: Python :: 3",
                      "Operating System :: OS Independent",
                  ],
-                 python_requires=">=3.7",
+                 python_requires=">=3.8",
                  
                  install_requires=['featurecloud','torch_pruning']
 
                  )
```

