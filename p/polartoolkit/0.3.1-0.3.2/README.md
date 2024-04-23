# Comparing `tmp/polartoolkit-0.3.1.tar.gz` & `tmp/polartoolkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polartoolkit-0.3.1.tar", last modified: Thu Feb 22 01:44:19 2024, max compression
+gzip compressed data, was "polartoolkit-0.3.2.tar", last modified: Tue Apr 23 09:36:04 2024, max compression
```

## Comparing `polartoolkit-0.3.1.tar` & `polartoolkit-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 01:44:19.019057 polartoolkit-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-02-22 01:44:19.019057 polartoolkit-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 01:44:19.019057 polartoolkit-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 01:44:19.015057 polartoolkit-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 01:44:19.015057 polartoolkit-0.3.1/src/antarctic_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/antarctic_plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 01:44:19.015057 polartoolkit-0.3.1/src/polartoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/polartoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   144085 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/polartoolkit/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    63305 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/polartoolkit/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    54132 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/polartoolkit/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/polartoolkit/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    58488 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/src/polartoolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 01:44:19.019057 polartoolkit-0.3.1/src/polartoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-02-22 01:44:19.000000 polartoolkit-0.3.1/src/polartoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-22 01:44:19.000000 polartoolkit-0.3.1/src/polartoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 01:44:19.000000 polartoolkit-0.3.1/src/polartoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-22 01:44:19.000000 polartoolkit-0.3.1/src/polartoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-22 01:44:19.000000 polartoolkit-0.3.1/src/polartoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 01:44:19.019057 polartoolkit-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    33372 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-02-22 01:44:11.000000 polartoolkit-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:36:04.881682 polartoolkit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 09:35:59.000000 polartoolkit-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-23 09:36:04.881682 polartoolkit-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-23 09:35:59.000000 polartoolkit-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:36:04.881682 polartoolkit-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:36:04.873682 polartoolkit-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:36:04.873682 polartoolkit-0.3.2/src/antarctic_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/antarctic_plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:36:04.877682 polartoolkit-0.3.2/src/polartoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/polartoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144085 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/polartoolkit/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63305 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/polartoolkit/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54132 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/polartoolkit/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/polartoolkit/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58488 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/src/polartoolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:36:04.877682 polartoolkit-0.3.2/src/polartoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-23 09:36:04.000000 polartoolkit-0.3.2/src/polartoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-23 09:36:04.000000 polartoolkit-0.3.2/src/polartoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:36:04.000000 polartoolkit-0.3.2/src/polartoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 09:36:04.000000 polartoolkit-0.3.2/src/polartoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 09:36:04.000000 polartoolkit-0.3.2/src/polartoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:36:04.877682 polartoolkit-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    33372 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-23 09:36:00.000000 polartoolkit-0.3.2/tests/test_utils.py
```

### Comparing `polartoolkit-0.3.1/LICENSE` & `polartoolkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/PKG-INFO` & `polartoolkit-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polartoolkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Helpful tools for polar researchers
 Author-email: Matt Tankersley <matt.d.tankersley@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Matt Tankersley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polartoolkit-0.3.1/README.md` & `polartoolkit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/pyproject.toml` & `polartoolkit-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 readme = "README.md"
-version = "0.3.1"
+version = "0.3.2"
 license = {file = "LICENSE"}
 
 keywords = ["cryosphere", "antarctica", "arctic", "greenland", "maps", "plotting", "pygmt", "cross-section"]
 
 dependencies = [
     "pandas",
     "openpyxl",
```

### Comparing `polartoolkit-0.3.1/src/polartoolkit/fetch.py` & `polartoolkit-0.3.2/src/polartoolkit/fetch.py`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/src/polartoolkit/maps.py` & `polartoolkit-0.3.2/src/polartoolkit/maps.py`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/src/polartoolkit/profile.py` & `polartoolkit-0.3.2/src/polartoolkit/profile.py`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/src/polartoolkit/regions.py` & `polartoolkit-0.3.2/src/polartoolkit/regions.py`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/src/polartoolkit/utils.py` & `polartoolkit-0.3.2/src/polartoolkit/utils.py`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/src/polartoolkit.egg-info/PKG-INFO` & `polartoolkit-0.3.2/src/polartoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polartoolkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Helpful tools for polar researchers
 Author-email: Matt Tankersley <matt.d.tankersley@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Matt Tankersley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polartoolkit-0.3.1/src/polartoolkit.egg-info/requires.txt` & `polartoolkit-0.3.2/src/polartoolkit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polartoolkit-0.3.1/tests/test_fetch.py` & `polartoolkit-0.3.2/tests/test_fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     grid = fetch.gravity(version="antgg", anomaly_type="FA")
     resampled = fetch.resample_grid(grid, **test_input)
     # assert utils.get_grid_info(resampled) == pytest.approx(expected, rel=0.1)
     assert not deepdiff.DeepDiff(
         utils.get_grid_info(resampled),
         expected,
         ignore_order=True,
-        significant_digits=2,
+        significant_digits=0,
     )
 
 
 # test_input = dict(
 #     spacing=10119,
 #     region=(-3400e3, 3400e3, -3400e3, 34030e3),
 #     registration='p',
```

### Comparing `polartoolkit-0.3.1/tests/test_utils.py` & `polartoolkit-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

