# Comparing `tmp/falconz-2.1.0.tar.gz` & `tmp/falconz-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falconz-2.1.0.tar", last modified: Mon Apr  8 13:18:37 2024, max compression
+gzip compressed data, was "falconz-2.1.1.tar", last modified: Tue Apr 23 18:20:41 2024, max compression
```

## Comparing `falconz-2.1.0.tar` & `falconz-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:18:37.011156 falconz-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 13:18:32.000000 falconz-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 13:18:37.011156 falconz-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-08 13:18:32.000000 falconz-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:18:37.011156 falconz-2.1.0/falconz/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/falconz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19478 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-08 13:18:32.000000 falconz-2.1.0/falconz/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:18:37.011156 falconz-2.1.0/falconz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 13:18:37.000000 falconz-2.1.0/falconz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 13:18:36.000000 falconz-2.1.0/falconz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:18:37.011156 falconz-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-08 13:18:32.000000 falconz-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:20:41.474444 falconz-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 18:20:32.000000 falconz-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-23 18:20:41.474444 falconz-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-23 18:20:32.000000 falconz-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:20:41.470444 falconz-2.1.1/falconz/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/falconz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19478 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-23 18:20:32.000000 falconz-2.1.1/falconz/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:20:41.470444 falconz-2.1.1/falconz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-23 18:20:41.000000 falconz-2.1.1/falconz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 18:20:41.000000 falconz-2.1.1/falconz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:20:41.000000 falconz-2.1.1/falconz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 18:20:41.000000 falconz-2.1.1/falconz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-23 18:20:41.000000 falconz-2.1.1/falconz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 18:20:41.000000 falconz-2.1.1/falconz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:20:41.474444 falconz-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-23 18:20:32.000000 falconz-2.1.1/setup.py
```

### Comparing `falconz-2.1.0/LICENSE` & `falconz-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/PKG-INFO` & `falconz-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: falconz
-Version: 2.1.0
+Version: 2.1.1
 Summary: FalconZ: A streamlined Python package for PET motion correction.
 Home-page: https://github.com/QIMP-Team/FALCON
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET motion correction,diffeomorphic imaging,image processing
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
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `falconz-2.1.0/README.md` & `falconz-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 <p align="center">
-<img src="https://github.com/LalithShiyam/FALCON/blob/main/Images/Falcon-logo.png">
+<img src="https://github.com/ENHANCE-PET/FALCON/blob/main/Images/falcon-upscaled.png">
 
 </p>
 
-## 🦅 About FALCON 2.0
+## 🦅 FALCON 2.0: PET Motion Correction: Any Tracer, Any Region.
 [![PyPI version](https://img.shields.io/pypi/v/falconz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/falconz/) [![Documentation Status](https://readthedocs.org/projects/falconz/badge/?version=latest)](https://falconz.readthedocs.io/en/latest/?badge=latest) [![Monthly Downloads](https://img.shields.io/pypi/dm/falconz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/falconz/) [![Daily Downloads](https://img.shields.io/pypi/dd/falconz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/falconz/)[![Discord](https://img.shields.io/badge/Discord-Join%20Chat-800080.svg?logo=discord&logoColor=white)](https://discord.gg/Q7ge3psMT9) [![YouTube](https://img.shields.io/badge/YouTube-MoCo%20Action-FF0000?logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLZQERorVWrbeNKLOdJMDi4lARvaK3ceeO)
 
 FALCON V2 (Fast Algorithms for motion correction) is an advanced, fully-automatic tool for motion correction in dynamic total-body or whole-body PET imaging. Designed with flexibility and reliability at its core, it's now even more versatile, capable of operating across various operating systems and architectures. 🚀
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/QIMP-Team/FALCON/blob/main/Images/Falcon_story_darkmode.gif" width="500" height="500">
@@ -203,14 +203,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/LalithShiyam"><img src="https://github.com/LalithShiyam.png?s=100" width="100px;" alt="Lalith Kumar Shiyam Sundar"/><br /><sub><b>Lalith Kumar Shiyam Sundar</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/FALCON/commits?author=LalithShiyam" title="Code">💻</a> <a href="https://github.com/ENHANCE-PET/FALCON/commits?author=LalithShiyam" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Keyn34"><img src="https://github.com/Keyn34.png?s=100" width="100px;" alt="Sebastian Gutschmayer"/><br /><sub><b>Sebastian Gutschmayer</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/FALCON/commits?author=Keyn34" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/christanmod"><img src="https://avatars.githubusercontent.com/u/54258479?v=4?s=100" width="100px;" alt="Z.K Li"/><br /><sub><b>Z.K Li</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/FALCON/commits?author=christanmod" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mprires"><img src="https://avatars.githubusercontent.com/u/48754309?v=4?s=100" width="100px;" alt="Manuel Pires"/><br /><sub><b>Manuel Pires</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/FALCON/commits?author=mprires" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `falconz-2.1.0/falconz/constants.py` & `falconz-2.1.1/falconz/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 project_root = file_utilities.get_virtual_env_root()
 
 # Set the path to the binary folder
 BINARY_PATH = os.path.join(project_root, 'bin')
 
 # Set the paths to the binaries based on the operating system
 if file_utilities.get_system()[0] == 'windows':
-    GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy.exe')
-    C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    C3D_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d.exe')
     DCM2NIIX_PATH = os.path.join(BINARY_PATH,
-                                 f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+                                 f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                  'dcm2niix.exe')
 elif file_utilities.get_system()[0] in ['linux', 'mac']:
-    GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy')
-    C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    C3D_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d')
-    DCM2NIIX_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    DCM2NIIX_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                     'dcm2niix')
 else:
     raise ValueError('Unsupported OS')
 
 # Define color codes for console output
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[32m'
```

### Comparing `falconz-2.1.0/falconz/display.py` & `falconz-2.1.1/falconz/display.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz/download.py` & `falconz-2.1.1/falconz/download.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz/falconz.py` & `falconz-2.1.1/falconz/falconz.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz/file_utilities.py` & `falconz-2.1.1/falconz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz/image_conversion.py` & `falconz-2.1.1/falconz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz/image_processing.py` & `falconz-2.1.1/falconz/image_processing.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz/input_validation.py` & `falconz-2.1.1/falconz/input_validation.py`

 * *Files identical despite different names*

### Comparing `falconz-2.1.0/falconz.egg-info/PKG-INFO` & `falconz-2.1.1/falconz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: falconz
-Version: 2.1.0
+Version: 2.1.1
 Summary: FalconZ: A streamlined Python package for PET motion correction.
 Home-page: https://github.com/QIMP-Team/FALCON
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET motion correction,diffeomorphic imaging,image processing
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
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `falconz-2.1.0/setup.py` & `falconz-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falconz',
-    version='2.1.0',
+    version='2.1.1',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='FalconZ: A streamlined Python package for PET motion correction.',
     python_requires='>=3.10',
     long_description='FalconZ is a robust and comprehensive Python package that offers a simplified approach to PET ('
                      'Positron Emission Tomography) motion correction. The software is equipped to handle both head '
                      'and total-body scans, ensuring high-accuracy results in diverse settings. Built around the '
@@ -19,15 +19,15 @@
                      'for accurate PET scan analysis.',
     url='https://github.com/QIMP-Team/FALCON',
     license='GPLv3',
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

