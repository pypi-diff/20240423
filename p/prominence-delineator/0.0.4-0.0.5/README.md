# Comparing `tmp/prominence_delineator-0.0.4.tar.gz` & `tmp/prominence_delineator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prominence_delineator-0.0.4.tar", last modified: Fri Apr 19 10:22:37 2024, max compression
+gzip compressed data, was "prominence_delineator-0.0.5.tar", last modified: Mon Apr 22 10:01:15 2024, max compression
```

## Comparing `prominence_delineator-0.0.4.tar` & `prominence_delineator-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.488569 prominence_delineator-0.0.4/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.4/LICENSE
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-19 10:22:37.487465 prominence_delineator-0.0.4/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.4/README.md
--rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-19 10:19:34.000000 prominence_delineator-0.0.4/pyproject.toml
--rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-19 10:22:37.488780 prominence_delineator-0.0.4/setup.cfg
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.455399 prominence_delineator-0.0.4/src/
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.464391 prominence_delineator-0.0.4/src/prominence_delineator/
--rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.4/src/prominence_delineator/__init__.py
--rw-r--r--   0 jea7h      (922) spgstud    (504)    17329 2024-04-04 10:04:51.000000 prominence_delineator-0.0.4/src/prominence_delineator/prominence_delineator.py
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.481078 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/SOURCES.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/dependency_links.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/requires.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/top_level.txt
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.898204 prominence_delineator-0.0.5/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.5/LICENSE
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-22 10:01:15.896839 prominence_delineator-0.0.5/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.5/README.md
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-22 10:00:03.000000 prominence_delineator-0.0.5/pyproject.toml
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-22 10:01:15.898543 prominence_delineator-0.0.5/setup.cfg
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.845334 prominence_delineator-0.0.5/src/
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.861924 prominence_delineator-0.0.5/src/prominence_delineator/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.5/src/prominence_delineator/__init__.py
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    17412 2024-04-22 10:00:58.000000 prominence_delineator-0.0.5/src/prominence_delineator/prominence_delineator.py
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.889603 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/SOURCES.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/dependency_links.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/requires.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/top_level.txt
```

### Comparing `prominence_delineator-0.0.4/LICENSE` & `prominence_delineator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.4/PKG-INFO` & `prominence_delineator-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `prominence_delineator-0.0.4/README.md` & `prominence_delineator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.4/pyproject.toml` & `prominence_delineator-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prominence-delineator"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
   "numpy",
   "scipy",
 ]
 requires-python = ">=3.8"
 authors = [
     {name="Jonas Emrich", email="mail@jonasemrich.de"}
```

### Comparing `prominence_delineator-0.0.4/src/prominence_delineator/prominence_delineator.py` & `prominence_delineator-0.0.5/src/prominence_delineator/prominence_delineator.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,16 @@
         }
 
         # process all leads
         for l, lead in enumerate(sig_multilead):
             result = self.find_waves(lead, rpeaks=waves["R"][l])
             # append result for lead
             for wave in waves.keys():
-                waves[wave].append(result[wave])
+                if wave in result:
+                    waves[wave].append(result[wave])
 
         # correct multi-lead predictions
         if multilead_correction:
             for wave, leads in waves.items():
                 waves[wave] = self._correct_multiLeads(
                     leads,
                     tol=tol,
@@ -231,15 +232,16 @@
                 )
                 self._find_on_offsets(
                     s, local_minima, local_maxima, weight_maxima, current_wave
                 )
 
             # append waves
             for key in waves:
-                waves[key].append(current_wave[key] + l)
+                if key in current_wave:
+                    waves[key].append(current_wave[key] + l)
         waves["R"] = rpeaks
 
         # cast into np.array int
         for key in waves:
             waves[key] = np.array(waves[key], dtype=int)
 
         return waves
```

### Comparing `prominence_delineator-0.0.4/src/prominence_delineator.egg-info/PKG-INFO` & `prominence_delineator-0.0.5/src/prominence_delineator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

