# Comparing `tmp/doppy-0.1.3.tar.gz` & `tmp/doppy-0.1.4.tar.gz`

## Comparing `doppy-0.1.3.tar` & `doppy-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0     1001      127      206 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doprs/Cargo.toml
--rw-r--r--   0     1001      127       21 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doprs/.gitignore
--rw-r--r--   0     1001      127       13 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doprs/src/lib.rs
--rw-r--r--   0     1001      127     2043 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doprs/src/raw/error.rs
--rw-r--r--   0     1001      127     9448 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doprs/src/raw/halo_hpl.rs
--rw-r--r--   0     1001      127       33 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doprs/src/raw.rs
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 doppy-0.1.3/crates/doppy_rs/Cargo.toml
--rw-r--r--   0     1001      127      279 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doppy_rs/src/lib.rs
--rw-r--r--   0     1001      127     4526 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doppy_rs/src/raw/halo_hpl.rs
--rw-r--r--   0     1001      127      204 2024-03-20 13:19:56.000000 doppy-0.1.3/crates/doppy_rs/src/raw.rs
--rw-r--r--   0     1001      127    18041 2024-03-20 13:20:00.000000 doppy-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      182 1970-01-01 00:00:00.000000 doppy-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     2398 2024-03-20 13:19:56.000000 doppy-0.1.3/pyproject.toml
--rw-r--r--   0     1001      127      191 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/__init__.py
--rw-r--r--   0     1001      127    19705 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/product/stare.py
--rw-r--r--   0     1001      127      103 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/product/__init__.py
--rw-r--r--   0     1001      127    11105 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/product/wind.py
--rw-r--r--   0     1001      127        0 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/data/__init__.py
--rw-r--r--   0     1001      127      996 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/data/cache.py
--rw-r--r--   0     1001      127     1735 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/data/api.py
--rw-r--r--   0     1001      127       89 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/data/exceptions.py
--rw-r--r--   0     1001      127       38 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/defaults.py
--rw-r--r--   0     1001      127      205 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/options.py
--rw-r--r--   0     1001      127        0 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/py.typed
--rw-r--r--   0     1001      127      194 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/raw/__init__.py
--rw-r--r--   0     1001      127     4809 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/raw/halo_bg.py
--rw-r--r--   0     1001      127     9685 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/raw/windcube.py
--rw-r--r--   0     1001      127     3937 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/raw/halo_sys_params.py
--rw-r--r--   0     1001      127    18504 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/raw/halo_hpl.py
--rw-r--r--   0     1001      127      248 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/bench.py
--rw-r--r--   0     1001      127      346 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/__main__.py
--rw-r--r--   0     1001      127     3416 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/netcdf.py
--rw-r--r--   0     1001      127      138 2024-03-20 13:19:56.000000 doppy-0.1.3/src/doppy/exceptions.py
--rw-r--r--   0     1001      127      279 2024-03-20 13:19:56.000000 doppy-0.1.3/README.md
--rw-r--r--   0     1001      127     1089 2024-03-20 13:19:56.000000 doppy-0.1.3/LICENSE
--rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 doppy-0.1.3/PKG-INFO
+-rw-r--r--   0     1001      127      206 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/Cargo.toml
+-rw-r--r--   0     1001      127       21 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/.gitignore
+-rw-r--r--   0     1001      127       13 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/lib.rs
+-rw-r--r--   0     1001      127     2043 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/raw/error.rs
+-rw-r--r--   0     1001      127     9448 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/raw/halo_hpl.rs
+-rw-r--r--   0     1001      127       33 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/raw.rs
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 doppy-0.1.4/crates/doppy_rs/Cargo.toml
+-rw-r--r--   0     1001      127      279 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doppy_rs/src/lib.rs
+-rw-r--r--   0     1001      127     4526 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doppy_rs/src/raw/halo_hpl.rs
+-rw-r--r--   0     1001      127      204 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doppy_rs/src/raw.rs
+-rw-r--r--   0     1001      127    18041 2024-04-23 13:09:39.000000 doppy-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      182 1970-01-01 00:00:00.000000 doppy-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127     2398 2024-04-23 13:09:28.000000 doppy-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      127      205 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/options.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/py.typed
+-rw-r--r--   0     1001      127     4809 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/halo_bg.py
+-rw-r--r--   0     1001      127    18625 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/halo_hpl.py
+-rw-r--r--   0     1001      127     9685 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/windcube.py
+-rw-r--r--   0     1001      127     3937 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/halo_sys_params.py
+-rw-r--r--   0     1001      127      194 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/__init__.py
+-rw-r--r--   0     1001      127     1735 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/api.py
+-rw-r--r--   0     1001      127      996 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/cache.py
+-rw-r--r--   0     1001      127        0 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/__init__.py
+-rw-r--r--   0     1001      127       89 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/exceptions.py
+-rw-r--r--   0     1001      127      191 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/__init__.py
+-rw-r--r--   0     1001      127      248 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/bench.py
+-rw-r--r--   0     1001      127    19733 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/product/stare.py
+-rw-r--r--   0     1001      127      103 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/product/__init__.py
+-rw-r--r--   0     1001      127    11133 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/product/wind.py
+-rw-r--r--   0     1001      127      346 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/__main__.py
+-rw-r--r--   0     1001      127       38 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/defaults.py
+-rw-r--r--   0     1001      127      138 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/exceptions.py
+-rw-r--r--   0     1001      127     3416 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/netcdf.py
+-rw-r--r--   0     1001      127      279 2024-04-23 13:09:28.000000 doppy-0.1.4/README.md
+-rw-r--r--   0     1001      127     1089 2024-04-23 13:09:28.000000 doppy-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 doppy-0.1.4/PKG-INFO
```

### Comparing `doppy-0.1.3/crates/doprs/src/raw/error.rs` & `doppy-0.1.4/crates/doprs/src/raw/error.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/crates/doprs/src/raw/halo_hpl.rs` & `doppy-0.1.4/crates/doprs/src/raw/halo_hpl.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/crates/doppy_rs/src/raw/halo_hpl.rs` & `doppy-0.1.4/crates/doppy_rs/src/raw/halo_hpl.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/Cargo.lock` & `doppy-0.1.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -102,24 +102,24 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "doppy_rs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "doprs",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "doprs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "chrono",
  "rayon",
  "regex",
 ]
 
 [[package]]
```

### Comparing `doppy-0.1.3/pyproject.toml` & `doppy-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/src/doppy/product/stare.py` & `doppy-0.1.4/src/doppy/product/stare.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         if len(raws) == 0:
             raise doppy.exceptions.NoDataError("HaloHpl data missing")
 
         raw = (
             doppy.raw.HaloHpl.merge(_select_raws_for_stare(raws))
             .sorted_by_time()
             .non_strictly_increasing_timesteps_removed()
+            .nans_removed()
         )
 
         bgs = doppy.raw.HaloBg.from_srcs(data_bg)
         bgs = [bg[:, : raw.header.ngates] for bg in bgs]
         bgs_stare = [bg for bg in bgs if bg.ngates == raw.header.ngates]
 
         if len(bgs_stare) == 0:
```

### Comparing `doppy-0.1.3/src/doppy/product/wind.py` & `doppy-0.1.4/src/doppy/product/wind.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         if len(raws) == 0:
             raise doppy.exceptions.NoDataError("HaloHpl data missing")
 
         raw = (
             doppy.raw.HaloHpl.merge(_select_raws_for_wind(raws))
             .sorted_by_time()
             .non_strictly_increasing_timesteps_removed()
+            .nans_removed()
         )
         if len(raw.time) == 0:
             raise doppy.exceptions.NoDataError("No suitable data for the wind product")
 
         groups = _group_scans_by_azimuth_rotation(raw)
         time_list = []
         elevation_list = []
```

### Comparing `doppy-0.1.3/src/doppy/data/cache.py` & `doppy-0.1.4/src/doppy/data/cache.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/src/doppy/data/api.py` & `doppy-0.1.4/src/doppy/data/api.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/src/doppy/raw/halo_bg.py` & `doppy-0.1.4/src/doppy/raw/halo_bg.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/src/doppy/raw/windcube.py` & `doppy-0.1.4/src/doppy/raw/windcube.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/src/doppy/raw/halo_sys_params.py` & `doppy-0.1.4/src/doppy/raw/halo_sys_params.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/src/doppy/raw/halo_hpl.py` & `doppy-0.1.4/src/doppy/raw/halo_hpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,18 @@
         for i, t in enumerate(self.time[1:], start=1):
             if t <= latest_time:
                 mask[i] = False
             else:
                 latest_time = t
         return self[mask]
 
+    def nans_removed(self) -> HaloHpl:
+        is_ok = ~np.isnan(self.intensity).any(axis=1)
+        return self[is_ok]
+
 
 @dataclass(slots=True)
 class HaloHplHeader:
     filename: str
     gate_points: int
     nrays: int | None
     nwaypoints: int | None
```

### Comparing `doppy-0.1.3/src/doppy/netcdf.py` & `doppy-0.1.4/src/doppy/netcdf.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/LICENSE` & `doppy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doppy-0.1.3/PKG-INFO` & `doppy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: doppy
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

