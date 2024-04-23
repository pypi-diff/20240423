# Comparing `tmp/prominence_delineator-0.0.5.tar.gz` & `tmp/prominence_delineator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prominence_delineator-0.0.5.tar", last modified: Mon Apr 22 10:01:15 2024, max compression
+gzip compressed data, was "prominence_delineator-0.0.6.tar", last modified: Tue Apr 23 09:12:24 2024, max compression
```

## Comparing `prominence_delineator-0.0.5.tar` & `prominence_delineator-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.898204 prominence_delineator-0.0.5/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.5/LICENSE
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-22 10:01:15.896839 prominence_delineator-0.0.5/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.5/README.md
--rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-22 10:00:03.000000 prominence_delineator-0.0.5/pyproject.toml
--rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-22 10:01:15.898543 prominence_delineator-0.0.5/setup.cfg
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.845334 prominence_delineator-0.0.5/src/
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.861924 prominence_delineator-0.0.5/src/prominence_delineator/
--rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.5/src/prominence_delineator/__init__.py
--rw-r--r--   0 jea7h      (922) spgstud    (504)    17412 2024-04-22 10:00:58.000000 prominence_delineator-0.0.5/src/prominence_delineator/prominence_delineator.py
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-22 10:01:15.889603 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/SOURCES.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/dependency_links.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/requires.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-22 10:01:15.000000 prominence_delineator-0.0.5/src/prominence_delineator.egg-info/top_level.txt
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.722903 prominence_delineator-0.0.6/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.6/LICENSE
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-23 09:12:24.721332 prominence_delineator-0.0.6/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.6/README.md
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-23 08:53:19.000000 prominence_delineator-0.0.6/pyproject.toml
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-23 09:12:24.723157 prominence_delineator-0.0.6/setup.cfg
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.683998 prominence_delineator-0.0.6/src/
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.694961 prominence_delineator-0.0.6/src/prominence_delineator/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.6/src/prominence_delineator/__init__.py
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    17870 2024-04-23 09:12:09.000000 prominence_delineator-0.0.6/src/prominence_delineator/prominence_delineator.py
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-23 09:12:24.714596 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/SOURCES.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/dependency_links.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/requires.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-23 09:12:24.000000 prominence_delineator-0.0.6/src/prominence_delineator.egg-info/top_level.txt
```

### Comparing `prominence_delineator-0.0.5/LICENSE` & `prominence_delineator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.5/PKG-INFO` & `prominence_delineator-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `prominence_delineator-0.0.5/README.md` & `prominence_delineator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.5/pyproject.toml` & `prominence_delineator-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prominence-delineator"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
   "numpy",
   "scipy",
 ]
 requires-python = ">=3.8"
 authors = [
     {name="Jonas Emrich", email="mail@jonasemrich.de"}
```

### Comparing `prominence_delineator-0.0.5/src/prominence_delineator/prominence_delineator.py` & `prominence_delineator-0.0.6/src/prominence_delineator/prominence_delineator.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,23 +159,26 @@
                     tol=tol,
                     accept_forall_factor=accept_forall_factor,
                     accept_factor=accept_factor,
                 )
 
         return waves
 
-    def find_waves(self, sig, rpeaks):
+    def find_waves(self, sig, rpeaks, include_nodetections=False):
         """Delineate ECG waves for the given single lead ECG signal.
 
         Args
         ----
         sig : ndarray
             The input signal representing a single unfiltered ECG lead.
         rpeaks : ndarray
             The R-peak positions of the signal.
+        include_nodetections : bool, optional
+            If True, the output will include `None` when no wave is found in the current beat/complex.
+            This results in equally sized arrays for each wave. Defaults to False.
 
         Returns
         -------
         dict: A dictionary of ndarrays containing the indices of the detected waves. The keys are 'P', 'R', 'T',
         'P_on', 'P_off', 'R_on', 'R_off', 'T_on', 'T_off'.
 
         """
@@ -232,21 +235,25 @@
                 )
                 self._find_on_offsets(
                     s, local_minima, local_maxima, weight_maxima, current_wave
                 )
 
             # append waves
             for key in waves:
-                if key in current_wave:
+                if key == "R":
+                    waves[key].append(rpeaks[i])
+                elif key in current_wave:
                     waves[key].append(current_wave[key] + l)
-        waves["R"] = rpeaks
+                elif include_nodetections:
+                    waves[key].append(None)
 
         # cast into np.array int
+        dtype = float if include_nodetections else int
         for key in waves:
-            waves[key] = np.array(waves[key], dtype=int)
+            waves[key] = np.array(waves[key], dtype=dtype)
 
         return waves
 
     def clean_ecg(self, sig):
         """Cleaning the given ECG signal.
 
         Args
```

### Comparing `prominence_delineator-0.0.5/src/prominence_delineator.egg-info/PKG-INFO` & `prominence_delineator-0.0.6/src/prominence_delineator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

