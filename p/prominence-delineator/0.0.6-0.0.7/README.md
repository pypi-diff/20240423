# Comparing `tmp/prominence_delineator-0.0.6.tar.gz` & `tmp/prominence_delineator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prominence_delineator-0.0.6.tar", last modified: Tue Apr 23 09:12:24 2024, max compression
+gzip compressed data, was "prominence_delineator-0.0.7.tar", last modified: Tue Apr 23 09:25:27 2024, max compression
```

## Comparing `prominence_delineator-0.0.6.tar` & `prominence_delineator-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.722903 prominence_delineator-0.0.6/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.6/LICENSE
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-23 09:12:24.721332 prominence_delineator-0.0.6/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.6/README.md
--rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-23 08:53:19.000000 prominence_delineator-0.0.6/pyproject.toml
--rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-23 09:12:24.723157 prominence_delineator-0.0.6/setup.cfg
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.683998 prominence_delineator-0.0.6/src/
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.694961 prominence_delineator-0.0.6/src/prominence_delineator/
--rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.6/src/prominence_delineator/__init__.py
--rw-r--r--   0 jea7h      (922) spgstud    (504)    17870 2024-04-23 09:12:09.000000 prominence_delineator-0.0.6/src/prominence_delineator/prominence_delineator.py
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.714596 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/SOURCES.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/dependency_links.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/requires.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/top_level.txt
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:25:27.227913 prominence_delineator-0.0.7/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.7/LICENSE
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-23 09:25:27.226615 prominence_delineator-0.0.7/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.7/README.md
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-23 09:25:09.000000 prominence_delineator-0.0.7/pyproject.toml
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-23 09:25:27.228159 prominence_delineator-0.0.7/setup.cfg
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:25:27.192873 prominence_delineator-0.0.7/src/
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:25:27.202898 prominence_delineator-0.0.7/src/prominence_delineator/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.7/src/prominence_delineator/__init__.py
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    17858 2024-04-23 09:25:01.000000 prominence_delineator-0.0.7/src/prominence_delineator/prominence_delineator.py
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:25:27.220318 prominence_delineator-0.0.7/src/prominence_delineator.egg-info/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-23 09:25:27.000000 prominence_delineator-0.0.7/src/prominence_delineator.egg-info/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-23 09:25:27.000000 prominence_delineator-0.0.7/src/prominence_delineator.egg-info/SOURCES.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-23 09:25:27.000000 prominence_delineator-0.0.7/src/prominence_delineator.egg-info/dependency_links.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-23 09:25:27.000000 prominence_delineator-0.0.7/src/prominence_delineator.egg-info/requires.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-23 09:25:27.000000 prominence_delineator-0.0.7/src/prominence_delineator.egg-info/top_level.txt
```

### Comparing `prominence_delineator-0.0.6/LICENSE` & `prominence_delineator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.6/PKG-INFO` & `prominence_delineator-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `prominence_delineator-0.0.6/README.md` & `prominence_delineator-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.6/pyproject.toml` & `prominence_delineator-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prominence-delineator"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
   "numpy",
   "scipy",
 ]
 requires-python = ">=3.8"
 authors = [
     {name="Jonas Emrich", email="mail@jonasemrich.de"}
```

### Comparing `prominence_delineator-0.0.6/src/prominence_delineator/prominence_delineator.py` & `prominence_delineator-0.0.7/src/prominence_delineator/prominence_delineator.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,17 +243,17 @@
                     waves[key].append(rpeaks[i])
                 elif key in current_wave:
                     waves[key].append(current_wave[key] + l)
                 elif include_nodetections:
                     waves[key].append(None)
 
         # cast into np.array int
-        dtype = float if include_nodetections else int
-        for key in waves:
-            waves[key] = np.array(waves[key], dtype=dtype)
+        if not include_nodetections:
+            for key in waves:
+                waves[key] = np.array(waves[key], dtype=int)
 
         return waves
 
     def clean_ecg(self, sig):
         """Cleaning the given ECG signal.
 
         Args
```

### Comparing `prominence_delineator-0.0.6/src/prominence_delineator.egg-info/PKG-INFO` & `prominence_delineator-0.0.7/src/prominence_delineator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

