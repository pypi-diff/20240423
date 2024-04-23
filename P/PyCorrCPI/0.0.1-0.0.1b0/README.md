# Comparing `tmp/PyCorrCPI-0.0.1.tar.gz` & `tmp/PyCorrCPI-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCorrCPI-0.0.1.tar", last modified: Tue Apr 23 17:42:06 2024, max compression
+gzip compressed data, was "PyCorrCPI-0.0.1b0.tar", last modified: Tue Apr 23 17:49:37 2024, max compression
```

## Comparing `PyCorrCPI-0.0.1.tar` & `PyCorrCPI-0.0.1b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-04-23 17:42:06.572470 PyCorrCPI-0.0.1/
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)    35149 2024-04-23 17:19:14.000000 PyCorrCPI-0.0.1/LICENSE
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      450 2024-04-23 17:42:06.572189 PyCorrCPI-0.0.1/PKG-INFO
-drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-04-23 17:42:06.568714 PyCorrCPI-0.0.1/PyCorrCPI/
--rwx------   0 fallum   (778712529) SLAC\Domain Users (1704612529)     8288 2024-04-19 18:42:34.000000 PyCorrCPI-0.0.1/PyCorrCPI/VMI_data.py
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      130 2024-04-23 17:22:50.000000 PyCorrCPI-0.0.1/PyCorrCPI/__init__.py
--rwx------   0 fallum   (778712529) SLAC\Domain Users (1704612529)    38502 2024-04-23 17:22:44.000000 PyCorrCPI-0.0.1/PyCorrCPI/covariance.py
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)     8288 2024-04-23 17:22:38.000000 PyCorrCPI-0.0.1/PyCorrCPI/data.py
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)     2813 2024-04-19 17:49:13.000000 PyCorrCPI-0.0.1/PyCorrCPI/helpers_numba.py
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      694 2024-04-19 21:23:08.000000 PyCorrCPI-0.0.1/PyCorrCPI/imports.py
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)     5765 2024-04-23 17:22:53.000000 PyCorrCPI-0.0.1/PyCorrCPI/output_functions.py
-drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-04-23 17:42:06.571681 PyCorrCPI-0.0.1/PyCorrCPI.egg-info/
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      450 2024-04-23 17:42:06.000000 PyCorrCPI-0.0.1/PyCorrCPI.egg-info/PKG-INFO
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      354 2024-04-23 17:42:06.000000 PyCorrCPI-0.0.1/PyCorrCPI.egg-info/SOURCES.txt
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)        1 2024-04-23 17:42:06.000000 PyCorrCPI-0.0.1/PyCorrCPI.egg-info/dependency_links.txt
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       36 2024-04-23 17:42:06.000000 PyCorrCPI-0.0.1/PyCorrCPI.egg-info/requires.txt
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       10 2024-04-23 17:42:06.000000 PyCorrCPI-0.0.1/PyCorrCPI.egg-info/top_level.txt
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       85 2024-04-23 17:23:41.000000 PyCorrCPI-0.0.1/README.md
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       38 2024-04-23 17:42:06.572601 PyCorrCPI-0.0.1/setup.cfg
--rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      661 2024-04-23 17:16:55.000000 PyCorrCPI-0.0.1/setup.py
+drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-04-23 17:49:37.002097 PyCorrCPI-0.0.1b0/
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)    35149 2024-04-23 17:19:14.000000 PyCorrCPI-0.0.1b0/LICENSE
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      454 2024-04-23 17:49:37.001704 PyCorrCPI-0.0.1b0/PKG-INFO
+drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-04-23 17:49:36.995503 PyCorrCPI-0.0.1b0/PyCorrCPI/
+-rwx------   0 fallum   (778712529) SLAC\Domain Users (1704612529)     8288 2024-04-19 18:42:34.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/VMI_data.py
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      130 2024-04-23 17:22:50.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/__init__.py
+-rwx------   0 fallum   (778712529) SLAC\Domain Users (1704612529)    38502 2024-04-23 17:22:44.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/covariance.py
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)     8288 2024-04-23 17:22:38.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/data.py
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)     2813 2024-04-19 17:49:13.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/helpers_numba.py
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      694 2024-04-19 21:23:08.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/imports.py
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)     5765 2024-04-23 17:22:53.000000 PyCorrCPI-0.0.1b0/PyCorrCPI/output_functions.py
+drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-04-23 17:49:37.001139 PyCorrCPI-0.0.1b0/PyCorrCPI.egg-info/
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      454 2024-04-23 17:49:36.000000 PyCorrCPI-0.0.1b0/PyCorrCPI.egg-info/PKG-INFO
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      354 2024-04-23 17:49:36.000000 PyCorrCPI-0.0.1b0/PyCorrCPI.egg-info/SOURCES.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)        1 2024-04-23 17:49:36.000000 PyCorrCPI-0.0.1b0/PyCorrCPI.egg-info/dependency_links.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       36 2024-04-23 17:49:36.000000 PyCorrCPI-0.0.1b0/PyCorrCPI.egg-info/requires.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       10 2024-04-23 17:49:36.000000 PyCorrCPI-0.0.1b0/PyCorrCPI.egg-info/top_level.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       85 2024-04-23 17:23:41.000000 PyCorrCPI-0.0.1b0/README.md
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       38 2024-04-23 17:49:37.002259 PyCorrCPI-0.0.1b0/setup.cfg
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      664 2024-04-23 17:49:22.000000 PyCorrCPI-0.0.1b0/setup.py
```

### Comparing `PyCorrCPI-0.0.1/LICENSE` & `PyCorrCPI-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/PyCorrCPI/VMI_data.py` & `PyCorrCPI-0.0.1b0/PyCorrCPI/VMI_data.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/PyCorrCPI/covariance.py` & `PyCorrCPI-0.0.1b0/PyCorrCPI/covariance.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/PyCorrCPI/data.py` & `PyCorrCPI-0.0.1b0/PyCorrCPI/data.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/PyCorrCPI/helpers_numba.py` & `PyCorrCPI-0.0.1b0/PyCorrCPI/helpers_numba.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/PyCorrCPI/imports.py` & `PyCorrCPI-0.0.1b0/PyCorrCPI/imports.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/PyCorrCPI/output_functions.py` & `PyCorrCPI-0.0.1b0/PyCorrCPI/output_functions.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.1/setup.py` & `PyCorrCPI-0.0.1b0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.1b' 
 DESCRIPTION = 'PyCorrCPI - corelation analysis for charged-particle imaging experiments'
 
 setup(
         name="PyCorrCPI", 
         version=VERSION,
         author="Felix Allum",
         author_email="fallum@stanford.edu",
         description=DESCRIPTION,
         packages=find_packages(),
         install_requires=['numpy', 'matplotlib', 'scipy', 'pandas', 'numba'],
         url='https://github.com/f-allum/PyCCorrCPI/',
-        download_url='https://github.com/f-allum/PyCESim/archive/refs/tags/v0.0.1.tar.gz',
+        download_url='https://github.com/f-allum/PyCorrCPI/archive/refs/tags/v0.0.1.tar.gz',
         keywords=['Coincidence', 'Covariance', 'Cumulant', 'Velocity-map Imaging']
 )
```

