# Comparing `tmp/masscube-0.0.7.tar.gz` & `tmp/masscube-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masscube-0.0.7.tar", last modified: Mon Apr 15 23:29:23 2024, max compression
+gzip compressed data, was "masscube-0.0.8.tar", last modified: Mon Apr 22 21:50:04 2024, max compression
```

## Comparing `masscube-0.0.7.tar` & `masscube-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.525569 masscube-0.0.7/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.7/LICENSE
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-15 23:29:23.525417 masscube-0.0.7/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.7/README.md
--rw-r--r--   0 jiemoniu   (501) staff       (20)      962 2024-04-15 23:29:15.000000 masscube-0.0.7/pyproject.toml
--rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-15 23:29:23.525616 masscube-0.0.7/setup.cfg
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.519690 masscube-0.0.7/src/
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.524490 masscube-0.0.7/src/masscube/
--rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.7/src/masscube/__init__.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    17035 2024-04-12 00:19:22.000000 masscube-0.0.7/src/masscube/alignment.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.7/src/masscube/annotation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2062 2024-04-11 23:20:27.000000 masscube-0.0.7/src/masscube/feature_evaluation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     8772 2024-04-03 20:16:56.000000 masscube-0.0.7/src/masscube/feature_grouping.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.7/src/masscube/feature_table_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.7/src/masscube/network.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     3477 2024-03-22 03:35:49.000000 masscube-0.0.7/src/masscube/normalization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10243 2024-04-03 00:15:40.000000 masscube-0.0.7/src/masscube/params.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10750 2024-04-12 17:33:27.000000 masscube-0.0.7/src/masscube/peak_detect.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    29438 2024-04-11 20:41:17.000000 masscube-0.0.7/src/masscube/raw_data_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     5479 2024-04-11 22:19:50.000000 masscube-0.0.7/src/masscube/stats.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.7/src/masscube/utils_functions.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    12646 2024-04-12 00:24:57.000000 masscube-0.0.7/src/masscube/visualization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10842 2024-04-15 22:58:59.000000 masscube-0.0.7/src/masscube/workflows.py
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.525237 masscube-0.0.7/src/masscube.egg-info/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/SOURCES.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/dependency_links.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      141 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/entry_points.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/requires.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/top_level.txt
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.188064 masscube-0.0.8/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.8/LICENSE
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-22 21:50:04.187880 masscube-0.0.8/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.8/README.md
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      962 2024-04-22 21:49:49.000000 masscube-0.0.8/pyproject.toml
+-rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-22 21:50:04.188097 masscube-0.0.8/setup.cfg
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.183512 masscube-0.0.8/src/
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.186805 masscube-0.0.8/src/masscube/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.8/src/masscube/__init__.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    17856 2024-04-22 20:04:50.000000 masscube-0.0.8/src/masscube/alignment.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.8/src/masscube/annotation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2820 2024-04-17 22:13:13.000000 masscube-0.0.8/src/masscube/feature_evaluation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     8772 2024-04-03 20:16:56.000000 masscube-0.0.8/src/masscube/feature_grouping.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.8/src/masscube/feature_table_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.8/src/masscube/network.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     4075 2024-04-18 05:25:59.000000 masscube-0.0.8/src/masscube/normalization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    12247 2024-04-22 20:19:43.000000 masscube-0.0.8/src/masscube/params.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    10980 2024-04-19 09:37:18.000000 masscube-0.0.8/src/masscube/peak_detect.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    30273 2024-04-17 21:14:22.000000 masscube-0.0.8/src/masscube/raw_data_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     5479 2024-04-11 22:19:50.000000 masscube-0.0.8/src/masscube/stats.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.8/src/masscube/utils_functions.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    12826 2024-04-17 21:34:57.000000 masscube-0.0.8/src/masscube/visualization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    13228 2024-04-22 20:22:02.000000 masscube-0.0.8/src/masscube/workflows.py
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.187651 masscube-0.0.8/src/masscube.egg-info/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/SOURCES.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/dependency_links.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      141 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/entry_points.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/requires.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/top_level.txt
```

### Comparing `masscube-0.0.7/LICENSE` & `masscube-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/PKG-INFO` & `masscube-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.7
+Version: 0.0.8
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `masscube-0.0.7/README.md` & `masscube-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/pyproject.toml` & `masscube-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masscube"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Accurate and fast data processing for metabolomics"
```

### Comparing `masscube-0.0.7/src/masscube/alignment.py` & `masscube-0.0.8/src/masscube/alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,19 @@
                 labeled_v[idx] = False
                 feature_table.loc[idx, file_name] = current_table.loc[j, "peak_height"]
                 # update the m/z and RT of the feature by averaging the values
                 feature_table.loc[idx, "m/z"] = (feature_table.loc[idx, "m/z"]*i + current_table.loc[j, "m/z"])/(i+1)
                 feature_table.loc[idx, "RT"] = (feature_table.loc[idx, "RT"]*i + current_table.loc[j, "RT"])/(i+1)
                 # if the intensity is the largest, update the reference file
                 if current_table.loc[j, "peak_height"] > int_seq[idx]:
-                    feature_table.iloc[idx, 3:10] = [current_table.loc[j, "adduct"], current_table.loc[j, "is_isotope"], 
+                    feature_table.iloc[idx, 3:11] = [current_table.loc[j, "adduct"], current_table.loc[j, "is_isotope"], 
                                                      current_table.loc[j, "is_in_source_fragment"], current_table.loc[j, "Gaussian_similarity"], 
-                                                     current_table.loc[j, "noise_level"], current_table.loc[j, "charge"], 
-                                                     current_table.loc[j, "isotopes"]]
+                                                     current_table.loc[j, "noise_level"], current_table.loc[j, "asymmetry_factor"],
+                                                     current_table.loc[j, "charge"], current_table.loc[j, "isotopes"]]
+
                     # only overwrite the MS2 if the current MS2 is not nan
                     if current_table.loc[j, "MS2"] == current_table.loc[j, "MS2"]:
                         feature_table.loc[idx,"MS2"] = current_table.loc[j, "MS2"]
                     feature_table.loc[idx, "alignment_reference"] = file_name
                     int_seq[idx] = current_table.loc[j, "peak_height"]
 
             # if the feature is not in the aligned feature table, add the feature to the table
@@ -109,14 +110,15 @@
         new_feature_table.index = range(last_file_feature_idx, last_file_feature_idx+len(new_feature_table))
         a = last_file_feature_idx+len(new_feature_table)-1
         feature_table.loc[last_file_feature_idx:a, "m/z"] = new_feature_table["m/z"]
         feature_table.loc[last_file_feature_idx:a, "RT"] = new_feature_table["RT"]
         feature_table.loc[last_file_feature_idx:a, "adduct"] = new_feature_table["adduct"]
         feature_table.loc[last_file_feature_idx:a, "noise_level"] = new_feature_table["noise_level"]
         feature_table.loc[last_file_feature_idx:a, "Gaussian_similarity"] = new_feature_table["Gaussian_similarity"]
+        feature_table.loc[last_file_feature_idx:a, "asymmetry_factor"] = new_feature_table["asymmetry_factor"]
         feature_table.loc[last_file_feature_idx:a, "charge"] = new_feature_table["charge"]
         feature_table.loc[last_file_feature_idx:a, "isotopes"] = new_feature_table["isotopes"]
         feature_table.loc[last_file_feature_idx:a, "MS2"] = new_feature_table["MS2"]
         feature_table.loc[last_file_feature_idx:a, "alignment_reference"] = file_name
         feature_table.loc[last_file_feature_idx:a, "is_isotope"] = new_feature_table["is_isotope"]
         feature_table.loc[last_file_feature_idx:a, "is_in_source_fragment"] = new_feature_table["is_in_source_fragment"]
         feature_table.loc[last_file_feature_idx:a, file_name] = new_feature_table["peak_height"]
@@ -182,14 +184,32 @@
                 d = read_raw_file_to_obj(matched_raw_file_name, int_tol=parameters.int_tol)
                 for i in range(len(feature_table)):
                     if pd.isna(feature_table.loc[i, file_name]):
                         _, eic_int, _, _ = d.get_eic_data(feature_table.loc[i, "m/z"], feature_table.loc[i, "RT"], parameters.align_mz_tol, 0.05)
                         feature_table.loc[i, file_name] = np.max(eic_int)
     return feature_table
 
+def output_feature_table(feature_table, output_path):
+    """
+    A function to output the aligned feature table.
+
+    Parameters
+    ----------------------------------------------------------
+    feature_table: DataFrame
+        The aligned feature table.
+    output_path: str
+        The path to save the aligned feature table.
+    """
+
+    # keep four digits for the m/z column and three digits for the RT column
+    feature_table["m/z"] = feature_table["m/z"].apply(lambda x: round(x, 4))
+    feature_table["RT"] = feature_table["RT"].apply(lambda x: round(x, 3))
+
+    feature_table.to_csv(output_path, index=False, sep="\t")
+
 
 class AlignedFeature:
     """
     A class to model an aligned feature from different files.
     """
 
     def __init__(self):
@@ -357,13 +377,14 @@
         self.is_in_source_fragment = self.highest_roi.is_in_source_fragment
         self.adduct_type = self.highest_roi.adduct_type
 
 
 # generate an empty feature table with 100000 rows
 def _init_feature_table(rows=5000, sample_names=[]):
     tmp = pd.DataFrame(
-        columns=["ID", "m/z", "RT", "adduct", "is_isotope", "is_in_source_fragment", "Gaussian_similarity", "noise_level", "charge", "isotopes", "MS2", 
+        columns=["ID", "m/z", "RT", "adduct", "is_isotope", "is_in_source_fragment", "Gaussian_similarity", "noise_level", "asymmetry_factor",
+                 "charge", "isotopes", "MS2", 
                 "matched_MS2", "search_mode", "annotation", "formula", "similarity", "matched_peak_number", "SMILES", "InChIKey", 
                 "fill_percentage", "alignment_reference"] + sample_names,
         index=range(rows)
     )
     return tmp
```

### Comparing `masscube-0.0.7/src/masscube/annotation.py` & `masscube-0.0.8/src/masscube/annotation.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/src/masscube/feature_evaluation.py` & `masscube-0.0.8/src/masscube/feature_evaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -96,13 +96,51 @@
 
     y = y[y > np.max(y) * 0.05]
 
     if len(y) < 5:
         return 0.0
 
     diff = np.diff(y)
-    counter = 0
+    signs = np.sign(diff)
+    counter = -1
     for i in range(1, len(diff)):
-        if diff[i] * diff[i - 1] < 0:
+        if signs[i] != signs[i-1]:
             counter += 1
     
     return counter / (len(y)-2)
+
+
+def calculate_asymmetry_factor(y):
+    """
+    Calcualte the asymmetry factor of the peak at 10% of the peak height.
+
+    Parameters
+    ----------
+    y: numpy array
+        Intensity
+
+    Returns
+    -------
+    float
+        asymmetry factor
+    """
+
+    y = y[y > np.max(y) * 0.05]
+    if len(y) < 5:
+        return 0.0
+    
+    # interpolate y to get 100 points
+    x = np.linspace(0, 1, 100)
+    y = np.interp(x, np.linspace(0, 1, len(y)), y)
+
+    ten_height = np.max(y) * 0.1
+    idx = np.argmax(y)
+
+    if idx == 0 or idx == len(y) - 1:
+        return -1
+
+    left_idx = np.argmin(np.abs(y[:idx] - ten_height))
+    right_idx = np.argmin(np.abs(y[idx:] - ten_height)) + idx
+
+    return (right_idx - idx) / (idx - left_idx)
+
+
```

### Comparing `masscube-0.0.7/src/masscube/feature_grouping.py` & `masscube-0.0.8/src/masscube/feature_grouping.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/src/masscube/feature_table_utils.py` & `masscube-0.0.8/src/masscube/feature_table_utils.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/src/masscube/network.py` & `masscube-0.0.8/src/masscube/network.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/src/masscube/normalization.py` & `masscube-0.0.8/src/masscube/normalization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 # Author: Hauxu Yu
 
-# A module for sample normalization
+# A module for normalization
+# There are two types of normalization:
+# 1. Sample normalization - to normalize samples with different total amounts/concentrations.
+# 2. Signal normalization - to address the signal drifts in the mass spectrometry data.
 
 import numpy as np
 
+"""
+Sample normalization
+====================
+
+Provides
+    1. Find the normalization factors.
+    2. Find reference sample.
+    3. Normalize samples by factors.
+"""
+
 def find_normalization_factors(array, method='pqn'):
     """ 
     A function to find the normalization factors for a data frame.
 
     Parameters
     ----------
     array : numpy array
@@ -114,8 +127,21 @@
     array = sample_normalization_by_factors(array, v)
 
     if blank_number == 0:
         feature_table.iloc[:, -total_number:] = array
     else:
         feature_table.iloc[:, -total_number:-total_number+array.shape[1]] = array
 
-    return feature_table
+    return feature_table
+
+
+
+"""
+Signal normalization
+====================
+
+Provides
+    1. Feature-wise normalization based on timestamp.
+    2. QC-based normalization.
+    3. Internal standard-based normalization (to be implemented).
+"""
+
```

### Comparing `masscube-0.0.7/src/masscube/params.py` & `masscube-0.0.8/src/masscube/params.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         # MS data acquisition
         self.rt_range = [0.0, 1000.0]       # RT range in minutes, list of two floats
         self.ion_mode = "positive"          # Ionization mode, "positive" or "negative", character string
 
         # Feature detection
         self.mz_tol_ms1 = 0.01              # m/z tolerance for MS1, default is 0.01
         self.mz_tol_ms2 = 0.015             # m/z tolerance for MS2, default is 0.015
-        self.int_tol = 1000                 # Intensity tolerance, default is 30000 for Orbitrap and 1000 for other instruments, integer
-        self.roi_gap = 50                   # Gap within a feature, default is 2 (i.e. 2 consecutive scans without signal), integer
+        self.int_tol = 30000                # Intensity tolerance, default is 30000 for Orbitrap and 1000 for other instruments, integer
+        self.roi_gap = 10                   # Gap within a feature, default is 10 (i.e. 10 consecutive scans without signal), integer
         self.min_ion_num = 10               # Minimum scan number a feature, default is 10, integer
 
         # Parameters for feature alignment
         self.align_mz_tol = 0.01            # m/z tolerance for MS1, default is 0.01
         self.align_rt_tol = 0.2             # RT tolerance, default is 0.2
 
         # Parameters for feature annotation
@@ -91,14 +91,17 @@
                     value = True
                 elif value.lower() == "false":
                     value = False
 
             setattr(self, df.iloc[i, 0], value)
         
         self.rt_range = [self.rt_start, self.rt_end]
+
+        # check if the parameters are correct
+        self.check_parameters()
     
 
     def _untargeted_metabolomics_workflow_preparation(self):
         """
         Prepare the parameters for the untargeted metabolomics workflow.
         """
     
@@ -114,73 +117,84 @@
         self.statistics_dir = os.path.join(self.project_dir, "statistics")
         
         # STEP 2: check if the required files are prepared
         #         three items are required: raw MS data, sample table, parameter file
         if not os.path.exists(self.sample_dir) or len(os.listdir(self.sample_dir)) == 0:
             raise ValueError("No raw MS data is found in the project directory.")
         if not os.path.exists(os.path.join(self.project_dir, "sample_table.csv")):
-            raise ValueError("No sample table is found in the project directory.")
+            print("No sample table is found in the project directory. No statistical analysis and sample normalization will be performed.")
         if not os.path.exists(os.path.join(self.project_dir, "parameters.csv")):
-            raise ValueError("No parameter file is found in the project directory.")
+            print("No parameter file is found in the project directory. Default parameters will be used.")
+            print("To perform feature annotation, please specify the path of MS/MS library in the parameter file.")
 
         # STEP 3: create the output directories if not exist
         if not os.path.exists(self.single_file_dir):
             os.makedirs(self.single_file_dir)
         if not os.path.exists(self.ms2_matching_dir):
             os.makedirs(self.ms2_matching_dir)
         if not os.path.exists(self.bpc_dir):
             os.makedirs(self.bpc_dir)
         if not os.path.exists(self.network_dir):
             os.makedirs(self.network_dir)
         if not os.path.exists(self.statistics_dir):
             os.makedirs(self.statistics_dir)
-
-        # STEP 4: read the sample table and allocate the sample groups
-        #         reorder the samples by qc, sample, and blank
-        sample_table = pd.read_csv(os.path.join(self.project_dir, "sample_table.csv"))
-        try:
-            sample_table.iloc[:, 1] = sample_table.iloc[:, 1].str.lower()
-        except:
-            raise ValueError("The second column of the sample table is not correct.")
-        sample_groups_pre = list(set(sample_table.iloc[:, 1]))
-        sample_groups = [i for i in sample_groups_pre if i not in ["qc", "blank"]]
-        self.sample_group_num = len(sample_groups)
-        if "qc" in sample_groups_pre:
-            sample_groups = ["qc"] + sample_groups
-        if "blank" in sample_groups_pre:
-            sample_groups = sample_groups + ["blank"]
-
-        sample_table_new = pd.DataFrame(columns=sample_table.columns)
-        for i in range(len(sample_groups)):
-            sample_table_new = pd.concat([sample_table_new, sample_table[sample_table.iloc[:, 1].str.contains(sample_groups[i])]])
-        self.sample_names = list(sample_table_new.iloc[:, 0])
-        self.sample_groups = sample_groups
-        self.individual_sample_groups = []
-        for name in self.sample_names:
-            self.individual_sample_groups.append(sample_table_new[sample_table_new.iloc[:, 0] == name].iloc[0, 1])
-
-        # STEP 5: read the parameters from csv file or use default values
+        
+        # STEP 4: read the parameters from csv file or use default values
         if os.path.exists(os.path.join(self.project_dir, "parameters.csv")):
             self.read_parameters_from_csv(os.path.join(self.project_dir, "parameters.csv"))
         else:
             print("Using default parameters...")
             # determine the type of MS and ion mode
             file_names = os.listdir(self.sample_dir)
             file_names = [f for f in file_names if f.lower().endswith(".mzml") or f.lower().endswith(".mzxml")]
             file_name = os.path.join(self.sample_dir, file_names[0])
-            ms_type, ion_mode = find_ms_info(file_name)
+            ms_type, ion_mode, _ = find_ms_info(file_name)
             self.set_default(ms_type, ion_mode)
             self.run_statistics = True
             self.plot_bpc = True
+            # annotation will not be performed if no MS/MS library is provided
             self.plot_ms2 = False
 
+        # STEP 5: read the sample table and allocate the sample groups
+        #         reorder the samples by qc, sample, and blank
+        if not os.path.exists(os.path.join(self.project_dir, "sample_table.csv")):
+            self.sample_names = [f.split(".")[0] for f in os.listdir(self.sample_dir)]
+            self.sample_groups = ["sample"] * len(self.sample_names)
+            self.individual_sample_groups = ["sample"] * len(self.sample_names)
+            self.sample_group_num = 1
+            # skip the normalization and statistics if no sample table is provided
+            self.run_normalization = False
+            self.run_statistics = False
+        else:
+            sample_table = pd.read_csv(os.path.join(self.project_dir, "sample_table.csv"))
+            try:
+                sample_table.iloc[:, 1] = sample_table.iloc[:, 1].str.lower()
+            except:
+                raise ValueError("The second column of the sample table is not correct.")
+            sample_groups_pre = list(set(sample_table.iloc[:, 1]))
+            sample_groups = [i for i in sample_groups_pre if i not in ["qc", "blank"]]
+            self.sample_group_num = len(sample_groups)
+            if "qc" in sample_groups_pre:
+                sample_groups = ["qc"] + sample_groups
+            if "blank" in sample_groups_pre:
+                sample_groups = sample_groups + ["blank"]
+
+            sample_table_new = pd.DataFrame(columns=sample_table.columns)
+            for i in range(len(sample_groups)):
+                sample_table_new = pd.concat([sample_table_new, sample_table[sample_table.iloc[:, 1].str.contains(sample_groups[i])]])
+            self.sample_names = list(sample_table_new.iloc[:, 0])
+            self.sample_groups = sample_groups
+            self.individual_sample_groups = []
+            for name in self.sample_names:
+                self.individual_sample_groups.append(sample_table_new[sample_table_new.iloc[:, 0] == name].iloc[0, 1])
+
         # STEP 6: set output
         self.output_single_file = True
         self.output_aligned_file = True
-    
+
 
     def set_default(self, ms_type, ion_mode):
         """
         Set the parameters by the type of MS.
         --------------------------------------
         ms_type: character string
             The type of MS, "orbitrap" or "tof".
@@ -192,15 +206,27 @@
             self.int_tol = 30000
         elif ms_type == "tof":
             self.int_tol = 1000
         if ion_mode == "positive":
             self.ion_mode = "positive"
         elif ion_mode == "negative":
             self.ion_mode = "negative"
+    
+
+    def check_parameters(self):
+        """
+        Check if the parameters are correct using PARAMETER_RAGEES.
+        ------------------------------------
+        """
 
+        for key, value in PARAMETER_RAGEES.items():
+            if not value[0] <= getattr(self, key) <= value[1]:
+                print(f"Parameter {key} is not out of range. The value is set to the default value.")
+                setattr(self, key, PARAMETER_DEFAULT[key])
+        
 
 def find_ms_info(file_name):
     """
     Find the type of MS and ion mode from the raw file.
 
     Parameters
     ----------
@@ -211,23 +237,52 @@
     -------
     ms_type : str
         The type of MS.
     ion_mode : str
         The ion mode.
     """
 
-    ms_type = None
-    ion_mode = None
+    ms_type = 'tof'
+    ion_mode = 'positive'
+    centroid = False
 
     with open(file_name, 'r') as f:
-        for line in f:
+        for i, line in enumerate(f):
             if 'orbitrap' in line.lower():
                 ms_type = 'orbitrap'
-            if 'tof' in line.lower():
-                ms_type = 'tof'
-            if 'positive' in line.lower():
-                ion_mode = 'positive'
             if 'negative' in line.lower():
                 ion_mode = 'negative'
-            if ms_type is not None and ion_mode is not None:
+            if "centroid spectrum" in line.lower():
+                centroid = True
+            if i > 200:
                 break
-    return ms_type, ion_mode
+
+    return ms_type, ion_mode, centroid
+
+
+PARAMETER_RAGEES = {
+    "rt_start": [0.0, 1000.0],
+    "rt_end": [0.0, 1000.0],
+    "mz_tol_ms1": [0.0, 0.015],
+    "mz_tol_ms2": [0.0, 0.015],
+    "int_tol": [0, 1e10],
+    "roi_gap": [0, 50],
+    "min_ion_num": [5, 50],
+    "align_mz_tol": [0.0, 0.02],
+    "align_rt_tol": [0.0, 2.0],
+    "ppr": [0.5, 1.0],
+    "ms2_sim_tol": [0.0, 1.0]
+}
+
+PARAMETER_DEFAULT = {
+    "rt_start": 0.0,
+    "rt_end": 1000.0,
+    "mz_tol_ms1": 0.01,
+    "mz_tol_ms2": 0.015,
+    "int_tol": 30000,
+    "roi_gap": 10,
+    "min_ion_num": 10,
+    "align_mz_tol": 0.01,
+    "align_rt_tol": 0.2,
+    "ppr": 0.7,
+    "ms2_sim_tol": 0.7
+}
```

### Comparing `masscube-0.0.7/src/masscube/peak_detect.py` & `masscube-0.0.8/src/masscube/peak_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Import modules
 import numpy as np
 from scipy.signal import find_peaks
 from scipy.ndimage import gaussian_filter1d
 from copy import deepcopy
 from .feature_evaluation import calculate_noise_level
 
-from .feature_evaluation import calculate_gaussian_similarity
+from .feature_evaluation import calculate_gaussian_similarity, calculate_asymmetry_factor
 
 def find_rois(d):
     """
     A function to find the region of interest (ROI) in the MS data.
 
     Parameters
     ----------------------------------------------------------
@@ -92,21 +92,21 @@
 
 def cut_roi(r, int_tol=1000):
     """
     Function to cut an ROI by providing the start and end positions.
     """
 
     r.int_seq = np.array(r.int_seq)
-    r.noise_level = calculate_noise_level(r.int_seq)
+    # r.noise_level = calculate_noise_level(r.int_seq)
 
-    if r.noise_level > 0.5 or len(r.int_seq) < 10 or r.peak_height < 3*int_tol:
+    if  len(r.int_seq) < 10 or r.peak_height < 3*int_tol or np.max(r.int_seq)/np.mean(r.int_seq) < 3:
         return [r]
 
-    ss = gaussian_filter1d(r.int_seq, sigma=1)
-    peaks, _ = find_peaks(ss, prominence=np.max(ss)*0.01, distance=5)
+    ss = gaussian_filter1d(r.int_seq, sigma=1.5)
+    peaks, _ = find_peaks(ss, prominence=np.max(ss)*0.05, distance=5)
 
     peaks = peaks[r.int_seq[peaks] > 2*int_tol]
 
     if len(peaks) < 2:
         return [r]
 
     if len(peaks) > 4:
@@ -173,14 +173,15 @@
         self.peak_area = np.nan
         self.peak_height = np.nan
         self.best_ms2 = None
         self.length = 0
         self.merged = False
         self.gaussian_similarity = 0.0
         self.noise_level = 0.0
+        self.asymmetry_factor = 0.0
         self.cut = False
         
         # Isotopes
         self.charge_state = 1
         self.is_isotope = False
         self.isotope_mz_seq = []
         self.isotope_int_seq = []
@@ -285,15 +286,15 @@
 
         d = np.sort(self.int_seq)[-num:]
         # calculate mean of non-zero values
         d = d[d != 0]
         self.top_average = np.mean(d, dtype=np.int64)
     
 
-    def sum_roi(self, cal_gss=True):
+    def sum_roi(self, cal_g_score=True, cal_a_score=True):
         """
         Function to summarize the ROI to generate attributes.
         """
         self.int_seq = np.array(self.int_seq)
         end_idx = len(self.int_seq)-1
 
         while self.int_seq[end_idx] == 0 and self.int_seq[end_idx-1] == 0:
@@ -307,16 +308,19 @@
         self.rt_seq = self.rt_seq[:end_idx]
         self.scan_idx_seq = self.scan_idx_seq[:end_idx]
         
         self.find_rt_ph_pa()
 
         self.noise_level = calculate_noise_level(self.int_seq)
 
-        if cal_gss:
+        if cal_g_score:
             self.gaussian_similarity = calculate_gaussian_similarity(self.rt_seq, self.int_seq)
+        if cal_a_score:
+            self.asymmetry_factor = calculate_asymmetry_factor(self.int_seq)
+            
         self.length = np.sum(self.int_seq > 0)
     
 
     def subset_roi(self, start, end):
         """
         Function to subset the ROI by providing the positions.
```

### Comparing `masscube-0.0.7/src/masscube/raw_data_utils.py` & `masscube-0.0.8/src/masscube/raw_data_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Import modules
 from pyteomics import mzml, mzxml
 import numpy as np
 import os
 import matplotlib.pyplot as plt
 import pandas as pd
 from datetime import datetime
+from time import time
 
 from .params import Params
 from .peak_detect import find_rois, cut_roi
 
 
 class MSData:
     """
@@ -72,23 +73,23 @@
 
             self.file_name = os.path.splitext(os.path.basename(file_name))[0]
 
             self.start_time = get_start_time(file_name)
 
             if ext.lower() == ".mzml":
                 with mzml.MzML(file_name) as reader:
-                    self.extract_scan_mzml(reader, centroid)
+                    self.extract_scan_mzml(reader, params.int_tol, centroid)
             elif ext.lower() == ".mzxml":
                 with mzxml.MzXML(file_name) as reader:
-                    self.extract_scan_mzxml(reader, centroid)
+                    self.extract_scan_mzxml(reader, params.int_tol, centroid)
         else:
             print("File does not exist.")
 
 
-    def extract_scan_mzml(self, spectra, centroid=True):
+    def extract_scan_mzml(self, spectra, int_tol, centroid=True):
         """
         Function to extract all scans and convert them to Scan objects.
 
         Parameters
         ----------------------------------------------------------
         spectra: pyteomics object
             An iteratable object that contains all MS1 and MS2 scans.
@@ -111,24 +112,30 @@
             if rt_unit == 'second':
                 rt = rt / 60
 
             # Check if the retention time is within the range
             if self.params.rt_range[0] < rt < self.params.rt_range[1]:
                 if spec['ms level'] == 1:
                     temp_scan = Scan(level=1, scan=idx, rt=rt)
-                    mz_array = spec['m/z array']
-                    int_array = spec['intensity array']
+                    mz_array = np.array(spec['m/z array'], dtype=np.float64)
+                    int_array = np.array(spec['intensity array'], dtype=np.int64)
+                    mz_array = mz_array[int_array > int_tol]
+                    int_array = int_array[int_array > int_tol]
+
+                    if len(mz_array) == 0:
+                        continue
+
                     if centroid:
                         mz_array, int_array = _centroid(mz_array, int_array)
 
                     temp_scan.add_info_by_level(mz_seq=mz_array, int_seq=int_array)
                     self.ms1_idx.append(idx)
 
                     # update base peak chromatogram
-                    self.bpc_int.append(np.max(spec['intensity array']))
+                    self.bpc_int.append(np.max(int_array))
                     self.ms1_rt_seq.append(rt)
 
                 elif spec['ms level'] == 2:
                     temp_scan = Scan(level=2, scan=idx, rt=rt)
                     precursor_mz = spec['precursorList']['precursor'][0]['selectedIonList']['selectedIon'][0]['selected ion m/z']
                     peaks = np.array([spec['m/z array'], spec['intensity array']], dtype=np.float64).T
                     temp_scan.add_info_by_level(precursor_mz=precursor_mz, peaks=peaks)
@@ -163,24 +170,28 @@
             if rt_unit == 'second':
                 rt = rt / 60
 
             # Check if the retention time is within the range
             if self.params.rt_range[0] < rt < self.params.rt_range[1]:
                 if spec['msLevel'] == 1:
                     temp_scan = Scan(level=1, scan=idx, rt=rt)
-                    mz_array = spec['m/z array']
-                    int_array = spec['intensity array']
+                    mz_array = np.array(spec['m/z array'], dtype=np.float64)
+                    int_array = np.array(spec['intensity array'], dtype=np.int64)
+
+                    mz_array = mz_array[int_array > self.params.int_tol]
+                    int_array = int_array[int_array > self.params.int_tol]
+
                     if centroid:
                         mz_array, int_array = _centroid(mz_array, int_array)
 
                     temp_scan.add_info_by_level(mz_seq=mz_array, int_seq=int_array)
                     self.ms1_idx.append(idx)
 
                     # update base peak chromatogram
-                    self.bpc_int.append(np.max(spec['intensity array']))
+                    self.bpc_int.append(np.max(int_array))
                     self.ms1_rt_seq.append(rt)
 
                 elif spec['msLevel'] == 2:
                     temp_scan = Scan(level=2, scan=idx, rt=rt)
                     precursor_mz = spec['precursorMz'][0]['precursorMz']
                     peaks = np.array([spec['m/z array'], spec['intensity array']], dtype=np.float64).T
                     temp_scan.add_info_by_level(precursor_mz=precursor_mz, peaks=peaks)
@@ -228,26 +239,26 @@
         tmp = []
         for roi in self.rois:
             tmp.extend(roi)
 
         self.rois = tmp
 
 
-    def summarize_roi(self, cal_gss=True):
+    def summarize_roi(self, cal_g_score=True, cal_a_score=True):
         """
         Function to process ROIs.
 
         Parameters
         ----------------------------------------------------------
         params: Params object
             A Params object that contains the parameters.
         """      
 
         for roi in self.rois:
-            roi.sum_roi(cal_gss=cal_gss)
+            roi.sum_roi(cal_g_score, cal_a_score)
 
         # sort rois by m/z
         self.rois.sort(key=lambda x: x.mz)
 
         # index the rois
         for idx in range(len(self.rois)):
             self.rois[idx].id = idx
@@ -293,28 +304,36 @@
 
         self.rois = [roi for roi in self.rois if not roi.is_isotope]
 
         for idx in range(len(self.rois)):
             self.rois[idx].id = idx
     
 
-    def plot_bpc(self, label_name=False, output=False):
+    def plot_bpc(self, rt_range=None, label_name=False, output=False):
         """
         Function to plot base peak chromatogram.
 
         Parameters
         ----------------------------------------------------------
         output: str
             Output file name. If not specified, the plot will be shown.
         """
 
+        if rt_range is not None:
+            x = [rt for rt in self.ms1_rt_seq if rt > rt_range[0] and rt < rt_range[1]]
+            y = [intensity for rt, intensity in zip(self.ms1_rt_seq, self.bpc_int) if rt > rt_range[0] and rt < rt_range[1]]
+
+        else:
+            x = self.ms1_rt_seq
+            y = self.bpc_int
+
         plt.figure(figsize=(10, 3))
         plt.rcParams['font.size'] = 14
         plt.rcParams['font.family'] = 'Arial'
-        plt.plot(self.ms1_rt_seq, self.bpc_int, linewidth=1, color="black")
+        plt.plot(x, y, linewidth=1, color="black")
         plt.xlabel("Retention Time (min)", fontsize=18, fontname='Arial')
         plt.ylabel("Intensity", fontsize=18, fontname='Arial')
         plt.xticks(fontsize=14, fontname='Arial')
         plt.yticks(fontsize=14, fontname='Arial')
         if label_name:
             plt.text(self.ms1_rt_seq[0], np.max(self.bpc_int)*0.9, self.file_name, fontsize=12, fontname='Arial', color="gray")
 
@@ -347,27 +366,28 @@
             if roi.best_ms2 is not None:
                 for i in range(len(roi.best_ms2.peaks)):
                     ms2 += str(np.round(roi.best_ms2.peaks[i, 0], decimals=4)) + ";" + str(np.round(roi.best_ms2.peaks[i, 1], decimals=0)) + "|"
                 ms2 = ms2[:-1]
 
             temp = [roi.id, roi.mz.__round__(4), roi.rt.__round__(3), roi.length, roi.rt_seq[0],
                     roi.rt_seq[-1], roi.peak_area, roi.peak_height, roi.gaussian_similarity.__round__(2), 
-                    roi.noise_level.__round__(2), roi.charge_state, roi.is_isotope, str(roi.isotope_id_seq)[1:-1], iso_dist,
+                    roi.noise_level.__round__(2), roi.asymmetry_factor.__round__(2), roi.charge_state, roi.is_isotope, str(roi.isotope_id_seq)[1:-1], iso_dist,
                     roi.is_in_source_fragment, roi.isf_parent_roi_id, str(roi.isf_child_roi_id)[1:-1],
                     roi.adduct_type, roi.adduct_parent_roi_id, str(roi.adduct_child_roi_id)[1:-1],
                     ]
             
             temp.extend([ms2, roi.annotation, roi.formula, roi.similarity, roi.matched_peak_number, roi.smiles, roi.inchikey])
 
             result.append(temp)
 
         # convert result to a pandas dataframe
         columns = [ "ID", "m/z", "RT", "length", "RT_start", "RT_end", "peak_area", "peak_height",
-                    "Gaussian_similarity", "noise_level", "charge", "is_isotope", "isotope_IDs", "isotopes", "is_in_source_fragment",
-                    "ISF_parent_ID", "ISF_child_ID", "adduct", "adduct_base_ID", "adduct_other_ID"]
+                    "Gaussian_similarity", "noise_level", "asymmetry_factor", "charge", "is_isotope", 
+                    "isotope_IDs", "isotopes", "is_in_source_fragment", "ISF_parent_ID", 
+                    "ISF_child_ID", "adduct", "adduct_base_ID", "adduct_other_ID"]
                     
         
         columns.extend(["MS2", "annotation", "formula", "similarity", "matched_peak_number", "SMILES", "InChIKey"])
 
         df = pd.DataFrame(result, columns=columns)
         
         # save the dataframe to csv file
@@ -749,30 +769,30 @@
     
     if ms2.peaks.shape[0] > 0:
         ms2.peaks = ms2.peaks[ms2.peaks[:, 0] < ms2.precursor_mz - offset]
     if ms2.peaks.shape[0] > 0:
         ms2.peaks = ms2.peaks[ms2.peaks[:, 1] > 0.01 * np.max(ms2.peaks[:, 1])]
 
 
-def _centroid(mz_seq, int_seq, centroiding_mz_tol=0.005):
+def _centroid(mz_seq, int_seq, mz_tol=0.005):
     """
     Function to centroid the m/z and intensity sequences.
 
     Parameters
     ----------
     mz_seq: numpy array or list
         m/z sequence.
     int_seq: numpy array or list
         Intensity sequence.
-    centroiding_mz_tol: float
+    mz_tol: float
         m/z tolerance for centroiding. Default is 0.005.
     """
 
     diff = np.diff(mz_seq)
-    tmp = np.where(diff < centroiding_mz_tol)[0]
+    tmp = np.where(diff < mz_tol)[0]
 
     if len(tmp) == 0:
         return mz_seq, int_seq
     
     mz_seq = list(mz_seq)
     int_seq = list(int_seq)
     for i in tmp[::-1]:
@@ -780,15 +800,15 @@
         int_seq[i] += int_seq[i+1]
         mz_seq.pop(i+1)
         int_seq.pop(i+1)
 
     return np.array(mz_seq), int_seq
 
 
-def read_raw_file_to_obj(file_name, params=None, int_tol=0.0, centroid=True, print_summary=False):
+def read_raw_file_to_obj(file_name, params=None, int_tol=1000, centroid=True, print_summary=False):
     """
     Read a raw file to a MSData object.
     It's a useful function for data visualization or brief data analysis.
 
     Parameters
     ----------
     file_name : str
@@ -812,19 +832,17 @@
 
     # create a MSData object
     d = MSData()
 
     # read raw data
     if params is None:
         params = Params()
+        params.int_tol = int_tol
+    
     d.read_raw_data(file_name, params, centroid)
-
-    if int_tol > 0:
-        d.params.int_tol = int_tol
-        d.drop_ion_by_int()
     
     if print_summary:
         print("Number of MS1 scans: " + str(len(d.ms1_idx)), "Number of MS2 scans: " + str(len(d.ms2_idx)))
     
     return d
```

### Comparing `masscube-0.0.7/src/masscube/stats.py` & `masscube-0.0.8/src/masscube/stats.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/src/masscube/utils_functions.py` & `masscube-0.0.8/src/masscube/utils_functions.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.7/src/masscube/visualization.py` & `masscube-0.0.8/src/masscube/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,28 +52,28 @@
     color = random.choice(list(mcolors.CSS4_COLORS.keys()))
     return color
 
 
 _color_list = ["red", "blue", "green", "orange", "purple", "brown", "pink", "gray", "olive", "cyan"]
 
 
-def plot_roi(d, roi, mz_tol=0.005, rt_tol=1.0, output=False, break_scan=None):
+def plot_roi(d, roi, mz_tol=0.01, rt_tol=1.0, output=False, break_scan=None):
     """
     Function to plot EIC of a target m/z.
     """
     rt_range = [roi.rt_seq[0]-rt_tol, roi.rt_seq[-1]+rt_tol]
     # get the eic data
     eic_rt, eic_int, _, eic_scan_idx = d.get_eic_data(target_mz=roi.mz, rt_range=rt_range, mz_tol=mz_tol)
     idx_start = np.where(eic_scan_idx == roi.scan_idx_seq[0])[0][0]
     idx_end = np.where(eic_scan_idx == roi.scan_idx_seq[-1])[0][0] + 1
 
     if break_scan is not None:
         idx_middle = np.where(eic_scan_idx == break_scan)[0][0]
 
-    max_int = np.max(eic_int)
+    max_int = np.max(eic_int[idx_start:idx_end])
 
     plt.figure(figsize=(9, 3))
     plt.rcParams['font.size'] = 14
     plt.rcParams['font.family'] = 'Arial'
     plt.plot(eic_rt, eic_int, linewidth=0.5, color="black")
     plt.ylim(0, max_int*1.2)
 
@@ -89,15 +89,16 @@
     plt.xlabel("Retention Time (min)", fontsize=18, fontname='Arial')
     plt.ylabel("Intensity", fontsize=18, fontname='Arial')
     plt.xticks(fontsize=14, fontname='Arial')
     plt.yticks(fontsize=14, fontname='Arial')
     plt.text(eic_rt[0], max_int*1.1, "m/z = {:.4f}".format(roi.mz), fontsize=11, fontname='Arial')
     plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.2, max_int*1.1, "G-score = {:.2f}".format(roi.gaussian_similarity), fontsize=11, fontname='Arial', color="blue")
     plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.4, max_int*1.1, "N-score = {:.2f}".format(roi.noise_level), fontsize=11, fontname='Arial', color="red")
-    plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.6,max_int*1.1, d.file_name, fontsize=11, fontname='Arial', color="gray")
+    plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.6, max_int*1.1, "A-score = {:.2f}".format(roi.asymmetry_factor), fontsize=11, fontname='Arial', color="darkgreen")
+    plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.8,max_int*1.1, d.file_name, fontsize=7, fontname='Arial', color="gray")
 
     if output:
         plt.savefig(output, dpi=600, bbox_inches="tight")
         plt.close()
     else:
         plt.show()
```

### Comparing `masscube-0.0.7/src/masscube/workflows.py` & `masscube-0.0.8/src/masscube/workflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 import multiprocessing
 import pickle
 from copy import deepcopy
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 
-from .raw_data_utils import MSData, get_start_time, read_raw_file_to_obj
+from .raw_data_utils import MSData, get_start_time
 from .params import Params, find_ms_info
 from .feature_grouping import annotate_isotope, annotate_adduct, annotate_in_source_fragment
-from .alignment import feature_alignment, gap_filling
+from .alignment import feature_alignment, gap_filling, output_feature_table
 from .annotation import feature_annotation, annotate_rois
 from .normalization import sample_normalization
 from .visualization import plot_ms2_matching_from_feature_table
 from .network import network_analysis
 from .stats import statistical_analysis
 from .feature_table_utils import calculate_fill_percentage
 
 
 # 1. Untargeted feature detection for a single file
-def feature_detection(file_name, params=None, cal_gss=True, anno_isotope=True,  
-                      anno_adduct=True, anno_in_source_fragment=True, annotation=False, 
-                      ms2_library_path=None, output_dir=None):
+def feature_detection(file_name, params=None, cal_g_score=True, cal_a_score=True,
+                      anno_isotope=True, anno_adduct=True, anno_in_source_fragment=True, 
+                      annotation=False, ms2_library_path=None, output_dir=None):
     """
     Untargeted feature detection from a single file (.mzML or .mzXML).
 
     Parameters
     ----------
     file_name : str
         Path to the raw file.
@@ -49,68 +49,75 @@
 
     Returns
     -------
     d : MSData object
         An MSData object containing the processed data.
     """
 
-    # create a MSData object
-    d = MSData()
+    try:
+        # create a MSData object
+        d = MSData()
+
+        # set parameters
+        # if params is None, use the default parameters
+        ms_type, ion_mode, centrod = find_ms_info(file_name)
+        if not centrod:
+            print("File: " + file_name + " is not centroided and skipped.")
+            return None
+        
+        if params is None:
+            params = Params()
+            print("MS type: " + ms_type, "Ion mode: " + ion_mode)
+            params.set_default(ms_type, ion_mode)
+        
+        if ms2_library_path is not None:
+            params.msms_library = ms2_library_path
 
-    # set parameters
-    # if params is None, use the default parameters
-    if params is None:
-        params = Params()
-        ms_type, ion_mode = find_ms_info(file_name)
-        print("MS type: " + ms_type, "Ion mode: " + ion_mode)
-        params.set_default(ms_type, ion_mode)
-    
-    if ms2_library_path is not None:
-        params.msms_library = ms2_library_path
+        # read raw data
+        d.read_raw_data(file_name, params)
 
-    # read raw data
-    d.read_raw_data(file_name, params)
+        # detect region of interests (ROIs)
+        d.find_rois()
 
-    # drop ions by intensity (defined in params.int_tol)
-    d.drop_ion_by_int()
-    # detect region of interests (ROIs)
-    d.find_rois()
-
-    # cut ROIs
-    d.cut_rois()
-
-    # label short ROIs, find the best MS2, and sort ROIs by m/z
-    d.summarize_roi(cal_gss=cal_gss)
-
-    # # annotate isotopes, adducts, and in-source fragments
-    if anno_isotope:
-        annotate_isotope(d)
-    if anno_in_source_fragment:
-        annotate_in_source_fragment(d)
-    if anno_adduct:
-        annotate_adduct(d)
-
-    # annotate MS2 spectra
-    if annotation and d.params.msms_library is not None:
-        annotate_rois(d)
-
-    if params.plot_bpc:
-        d.plot_bpc(label_name=True, output=os.path.join(params.bpc_dir, d.file_name + "_bpc.png"))
-
-    # output single file to a txt file
-    if d.params.output_single_file:
-        d.output_single_file()
-    elif output_dir is not None:
-        d.output_single_file(output_dir)
+        # cut ROIs
+        d.cut_rois()
+
+        # label short ROIs, find the best MS2, and sort ROIs by m/z
+        d.summarize_roi(cal_g_score=cal_g_score, cal_a_score=cal_a_score)
+
+        # # annotate isotopes, adducts, and in-source fragments
+        if anno_isotope:
+            annotate_isotope(d)
+        if anno_in_source_fragment:
+            annotate_in_source_fragment(d)
+        if anno_adduct:
+            annotate_adduct(d)
+
+        # annotate MS2 spectra
+        if annotation and d.params.msms_library is not None:
+            annotate_rois(d)
+
+        if params.plot_bpc:
+            d.plot_bpc(label_name=True, output=os.path.join(params.bpc_dir, d.file_name + "_bpc.png"))
+
+        # output single file to a txt file
+        if d.params.output_single_file:
+            d.output_single_file()
+        elif output_dir is not None:
+            d.output_single_file(os.path.join(output_dir, d.file_name + ".txt"))
 
-    return d
+        return d
+    
+    except Exception as e:
+        print("Error: " + str(e))
+        return None
 
 
 # 2. Untargeted metabolomics workflow
-def untargeted_metabolomics_workflow(path=None):
+def untargeted_metabolomics_workflow(path=None, batch_size=100):
     """
     The untargeted metabolomics workflow. See the documentation for details.
 
     Parameters
     ----------
     path : str
         The working directory. If None, the current working directory is used.
@@ -127,24 +134,24 @@
     with open(os.path.join(params.project_dir, "project.mc"), "wb") as f:
         pickle.dump(params, f)
     
     raw_file_names = os.listdir(params.sample_dir)
     raw_file_names = [f for f in raw_file_names if f.lower().endswith(".mzml") or f.lower().endswith(".mzxml")]
     raw_file_names = [os.path.join(params.sample_dir, f) for f in raw_file_names]
 
-    # process files by multiprocessing, each batch contains 300 files
+    # process files by multiprocessing, each batch contains 100 files by default (tunable in batch_size)
     print("Processing files by multiprocessing...")
     workers = int(multiprocessing.cpu_count() * 0.8)
-    for i in range(0, len(raw_file_names), 300):
-        if len(raw_file_names) - i < 300:
+    for i in range(0, len(raw_file_names), batch_size):
+        if len(raw_file_names) - i < batch_size:
             print("Processing files from " + str(i) + " to " + str(len(raw_file_names)))
         else:
-            print("Processing files from " + str(i) + " to " + str(i+300))
+            print("Processing files from " + str(i) + " to " + str(i+batch_size))
         p = multiprocessing.Pool(workers)
-        p.starmap(feature_detection, [(f, params) for f in raw_file_names[i:i+300]])
+        p.starmap(feature_detection, [(f, params) for f in raw_file_names[i:i+batch_size]])
         p.close()
         p.join()
 
     # feature alignment
     print("Aligning features...")
     feature_table = feature_alignment(params.single_file_dir, params)
 
@@ -160,15 +167,16 @@
     if params.msms_library is not None and os.path.exists(params.msms_library):
         feature_annotation(feature_table, params)
     else:
         print("No MS2 library is found. Skipping annotation...")
 
     # normalization
     if params.run_normalization:
-        feature_table.to_csv(os.path.join(params.project_dir, "aligned_feature_table_before_normalization.txt"), index=False, sep="\t")
+        output_path = os.path.join(params.project_dir, "aligned_feature_table_before_normalization.txt")
+        output_feature_table(feature_table, output_path)
         feature_table_before_normalization = deepcopy(feature_table)
         print("Running normalization...")
         feature_table = sample_normalization(feature_table, params.individual_sample_groups, params.normalization_method)
 
     # statistical analysis
     if params.run_statistics:
         print("Running statistical analysis...")
@@ -182,15 +190,16 @@
 
     # plot annoatated metabolites
     if params.plot_ms2:
         print("Plotting annotated metabolites...")
         plot_ms2_matching_from_feature_table(feature_table, params)
     
     # output feature table
-    feature_table.to_csv(os.path.join(params.project_dir, "aligned_feature_table.txt"), index=False, sep="\t")
+    output_path = os.path.join(params.project_dir, "aligned_feature_table.txt")
+    output_feature_table(feature_table, output_path)
     print("The workflow is completed.")
 
 
 # 3. Get analytical metadata from mzML files
 def get_analytical_metadata(path):
     """
     Get metadata from mzML or mzXML files.
@@ -273,51 +282,116 @@
 
     Parameters
     ----------
     path : str
         The working directory. If None, the current working directory is used.
     """
 
-    # 
+    pass
 
 
 # 6. Single-file peak picking (batch mode)
-def single_file_processing(path=None, params=None):
+def batch_file_processing(path=None, params=None, cal_g_score=True, cal_a_score=True,
+                          anno_isotope=True, anno_adduct=True, anno_in_source_fragment=True, 
+                          annotation=False, ms2_library_path=None):
+    """
+    Single MS data processing for multiple files in batch mode.
+
+    Parameters
+    ----------
+    path : str
+        Path to the mzML or mzXML files.
+    params : Params object
+        Parameters for feature detection.
+    """
     
-    params = Params()
     # obtain the working directory
     if path is not None:
-        params.project_dir = path
+        wd = path
     else:
-        params.project_dir = os.getcwd()
-    params._untargeted_metabolomics_workflow_preparation()
+        wd = os.getcwd()
+    
+    if os.path.exists(os.path.join(wd, "parameters.csv")):
+        params = Params()
+        params.read_parameters_from_csv(os.path.join(wd, "parameters.csv"))
 
-    with open(os.path.join(params.project_dir, "project.mc"), "wb") as f:
-        pickle.dump(params, f)
     
-    raw_file_names = os.listdir(params.sample_dir)
-    raw_file_names = [f for f in raw_file_names if f.lower().endswith(".mzml") or f.lower().endswith(".mzxml")]
-    raw_file_names = [os.path.join(params.sample_dir, f) for f in raw_file_names]
+    all_file_names = os.listdir(wd)
+    raw_file_names = [f for f in all_file_names if f.lower().endswith(".mzml") or f.lower().endswith(".mzxml")]
+    txt_files = [f.split(".")[0] for f in all_file_names if f.lower().endswith(".txt")]
+
+    # if the file has been processed, skip it
+    raw_file_names = [f for f in raw_file_names if f.split(".")[0]+"_feature_table" not in txt_files]
+    raw_file_names = [f for f in raw_file_names if f.split(".")[0] not in txt_files]
+    raw_file_names = [os.path.join(wd, f) for f in raw_file_names]
+
+    print("Total number of files to be processed: " + str(len(raw_file_names)))
 
     # process files by multiprocessing, each batch contains 300 files
     print("Processing files by multiprocessing...")
     workers = int(multiprocessing.cpu_count() * 0.8)
-    for i in range(0, len(raw_file_names), 300):
-        if len(raw_file_names) - i < 300:
+    for i in range(0, len(raw_file_names), 50):
+        if len(raw_file_names) - i < 50:
             print("Processing files from " + str(i) + " to " + str(len(raw_file_names)))
         else:
-            print("Processing files from " + str(i) + " to " + str(i+300))
+            print("Processing files from " + str(i) + " to " + str(i+50))
         p = multiprocessing.Pool(workers)
-        p.starmap(feature_detection, [(f, params) for f in raw_file_names[i:i+300]])
+        p.starmap(feature_detection, [(f, params, cal_g_score, cal_a_score, anno_isotope, anno_adduct, anno_in_source_fragment, 
+                                       annotation, ms2_library_path, wd) for f in raw_file_names[i:i+50]])
         p.close()
         p.join()
 
 
-# 7. Determine normalization factors
+# 7. Determine sample total amount
+def sample_total_amount(path):
+    """
+    Determine the total amount of the samples based on LC-MS data. See the documentation for details.
+
+    Parameters
+    ----------
+    path : str
+        Path to the mzML or mzXML files.
+    """
 
+    pass
 
 # 8. Serial QC calibration
+def qc_calibration(path):
+    """
+    Serial QC calibration. See the documentation for details.
+
+    Parameters
+    ----------
+    path : str
+        Path to the mzML or mzXML files.
+    """
+
+    pass
+
+
 
 # 9. Mass calibration
+def mass_calibration(path):
+    """
+    Mass calibration. See the documentation for details.
+
+    Parameters
+    ----------
+    path : str
+        Path to the mzML or mzXML files.
+    """
+
+    pass
 
 
 # 10. Untargeted metabolomics workflow with multiple analytical modes (RP+, RP-, HILIC+, HILIC-)
+def untargeted_metabolomics_workflow_multi_mode(path=None):
+    """
+    The untargeted metabolomics workflow with multiple analytical modes. See the documentation for details.
+
+    Parameters
+    ----------
+    path : str
+        The working directory. If None, the current working directory is used.
+    """
+
+    pass
```

### Comparing `masscube-0.0.7/src/masscube.egg-info/PKG-INFO` & `masscube-0.0.8/src/masscube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.7
+Version: 0.0.8
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `masscube-0.0.7/src/masscube.egg-info/SOURCES.txt` & `masscube-0.0.8/src/masscube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

