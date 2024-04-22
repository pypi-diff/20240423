# Comparing `tmp/utilsforecast-0.1.5.tar.gz` & `tmp/utilsforecast-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsforecast-0.1.5.tar", last modified: Fri Apr 19 18:40:58 2024, max compression
+gzip compressed data, was "utilsforecast-0.1.6.tar", last modified: Mon Apr 22 21:10:46 2024, max compression
```

## Comparing `utilsforecast-0.1.5.tar` & `utilsforecast-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:40:58.086383 utilsforecast-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-19 18:40:58.086383 utilsforecast-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:40:58.086383 utilsforecast-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:40:58.082383 utilsforecast-0.1.5/utilsforecast/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-19 18:40:54.000000 utilsforecast-0.1.5/utilsforecast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:40:58.086383 utilsforecast-0.1.5/utilsforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-19 18:40:58.000000 utilsforecast-0.1.5/utilsforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 18:40:58.000000 utilsforecast-0.1.5/utilsforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:40:58.000000 utilsforecast-0.1.5/utilsforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 18:40:58.000000 utilsforecast-0.1.5/utilsforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:40:57.000000 utilsforecast-0.1.5/utilsforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 18:40:58.000000 utilsforecast-0.1.5/utilsforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:40:58.000000 utilsforecast-0.1.5/utilsforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:10:46.388116 utilsforecast-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-22 21:10:46.388116 utilsforecast-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:10:46.388116 utilsforecast-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:10:46.384116 utilsforecast-0.1.6/utilsforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-22 21:10:36.000000 utilsforecast-0.1.6/utilsforecast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:10:46.384116 utilsforecast-0.1.6/utilsforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 21:10:46.000000 utilsforecast-0.1.6/utilsforecast.egg-info/top_level.txt
```

### Comparing `utilsforecast-0.1.5/CONTRIBUTING.md` & `utilsforecast-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/LICENSE` & `utilsforecast-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/PKG-INFO` & `utilsforecast-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.5
+Version: 0.1.6
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
-Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
 Requires-Dist: scipy; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
-Requires-Dist: polars; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: numba; extra == "dev"
 Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: polars; extra == "dev"
+Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.5/README.md` & `utilsforecast-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/settings.ini` & `utilsforecast-0.1.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utilsforecast
 lib_name = utilsforecast
-version = 0.1.5
+version = 0.1.6
 min_python = 3.8
 license = apache2
 black_formatting = True
 doc_path = _docs
 lib_path = utilsforecast
 nbs_path = nbs
 recursive = True
```

### Comparing `utilsforecast-0.1.5/setup.py` & `utilsforecast-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/_modidx.py` & `utilsforecast-0.1.6/utilsforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/compat.py` & `utilsforecast-0.1.6/utilsforecast/compat.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/data.py` & `utilsforecast-0.1.6/utilsforecast/data.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/evaluation.py` & `utilsforecast-0.1.6/utilsforecast/evaluation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/feature_engineering.py` & `utilsforecast-0.1.6/utilsforecast/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/grouped_array.py` & `utilsforecast-0.1.6/utilsforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/losses.py` & `utilsforecast-0.1.6/utilsforecast/losses.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/plotting.py` & `utilsforecast-0.1.6/utilsforecast/plotting.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/preprocessing.py` & `utilsforecast-0.1.6/utilsforecast/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,33 +120,37 @@
                     eager=True,
                 ).alias(time_col)
             )
         grid = grid.explode(time_col)
         return grid.join(df, on=[id_col, time_col], how="left")
     if isinstance(freq, str):
         offset = pd.tseries.frequencies.to_offset(freq)
+        n = offset.n
         if isinstance(offset.base, pd.offsets.Minute):
             # minutes are represented as 'm' in numpy
             freq = "m"
         elif isinstance(offset.base, pd.offsets.BusinessDay):
             if offset.n != 1:
                 raise NotImplementedError("Multiple of a business day")
             freq = "D"
         elif isinstance(offset.base, pd.offsets.Hour):
             # hours are represented as 'h' in numpy
             freq = "h"
-        if offset.n > 1:
-            freq = freq.replace(str(offset.n), "")
+        elif isinstance(offset.base, (pd.offsets.QuarterBegin, pd.offsets.QuarterEnd)):
+            n *= 3
+            freq = "M"
+        if n > 1:
+            freq = freq.replace(str(n), "")
         try:
             pd.Timedelta(offset)
         except ValueError:
             # irregular freq, try using first letter of abbreviation
             # such as MS = 'Month Start' -> 'M', YS = 'Year Start' -> 'Y'
             freq = freq[0]
-        delta: Union[np.timedelta64, int] = np.timedelta64(offset.n, freq)
+        delta: Union[np.timedelta64, int] = np.timedelta64(n, freq)
     else:
         delta = freq
     times_by_id = df.groupby(id_col, observed=True)[time_col].agg(["min", "max"])
     starts = _determine_bound(start, freq, times_by_id, "min")
     ends = _determine_bound(end, freq, times_by_id, "max") + delta
     sizes = ((ends - starts) / delta).astype(np.int64)
     times = np.hstack(
```

### Comparing `utilsforecast-0.1.5/utilsforecast/processing.py` & `utilsforecast-0.1.6/utilsforecast/processing.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/target_transforms.py` & `utilsforecast-0.1.6/utilsforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast/validation.py` & `utilsforecast-0.1.6/utilsforecast/validation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.5/utilsforecast.egg-info/PKG-INFO` & `utilsforecast-0.1.6/utilsforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.5
+Version: 0.1.6
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
-Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
 Requires-Dist: scipy; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
-Requires-Dist: polars; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: numba; extra == "dev"
 Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: polars; extra == "dev"
+Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.5/utilsforecast.egg-info/SOURCES.txt` & `utilsforecast-0.1.6/utilsforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

