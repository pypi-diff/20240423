# Comparing `tmp/light-curve-python-0.9.0a0.tar.gz` & `tmp/light_curve_python-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light-curve-python-0.9.0a0.tar", last modified: Tue Mar  5 22:09:49 2024, max compression
+gzip compressed data, was "light_curve_python-0.9.1.tar", last modified: Tue Apr 23 13:51:52 2024, max compression
```

## Comparing `light-curve-python-0.9.0a0.tar` & `light_curve_python-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:09:49.363646 light-curve-python-0.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-05 22:09:41.000000 light-curve-python-0.9.0a0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-05 22:09:41.000000 light-curve-python-0.9.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-05 22:09:49.363646 light-curve-python-0.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-05 22:09:41.000000 light-curve-python-0.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:09:49.363646 light-curve-python-0.9.0a0/light_curve_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-05 22:09:49.000000 light-curve-python-0.9.0a0/light_curve_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-05 22:09:49.000000 light-curve-python-0.9.0a0/light_curve_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 22:09:49.000000 light-curve-python-0.9.0a0/light_curve_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-05 22:09:49.000000 light-curve-python-0.9.0a0/light_curve_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 22:09:49.000000 light-curve-python-0.9.0a0/light_curve_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 22:09:41.000000 light-curve-python-0.9.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-05 22:09:49.363646 light-curve-python-0.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-05 22:09:41.000000 light-curve-python-0.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:51:52.725120 light_curve_python-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-23 13:51:42.000000 light_curve_python-0.9.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 13:51:42.000000 light_curve_python-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 13:51:52.725120 light_curve_python-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 13:51:42.000000 light_curve_python-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:51:52.725120 light_curve_python-0.9.1/light_curve_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 13:51:52.000000 light_curve_python-0.9.1/light_curve_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 13:51:52.000000 light_curve_python-0.9.1/light_curve_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:51:52.000000 light_curve_python-0.9.1/light_curve_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 13:51:52.000000 light_curve_python-0.9.1/light_curve_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:51:52.000000 light_curve_python-0.9.1/light_curve_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 13:51:42.000000 light_curve_python-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-23 13:51:52.725120 light_curve_python-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-23 13:51:42.000000 light_curve_python-0.9.1/setup.py
```

### Comparing `light-curve-python-0.9.0a0/Cargo.toml` & `light_curve_python-0.9.1/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "light-curve-python"
-version = "0.9.0-alpha.0"
+version = "0.9.1"
 authors = ["Konstantin Malanchev <hombit@gmail.com>", "Anastasia Lavrukhina <lavrukhina.ad@gmail.com>"]
 description = "Feature extractor from noisy time series"
 readme = "README.md"
 repository = "https://github.com/light-curve/light-curve-python"
 license = "GPL-3.0-or-later"
 edition = "2021"
 rust-version = "1.67"
@@ -14,15 +14,15 @@
 crate-type = ["cdylib"]
 
 [profile.release]
 lto = true
 codegen-units = 1
 
 [features]
-default = ["ceres-source", "fftw-source", "gsl", "mimalloc"]
+default = ["abi3", "ceres-source", "fftw-source", "gsl", "mimalloc"]
 abi3 = ["pyo3/abi3-py38"]
 ceres-source = ["light-curve-feature/ceres-source"]
 ceres-system = ["light-curve-feature/ceres-system"]
 fftw-source = ["light-curve-feature/fftw-source"]
 fftw-system = ["light-curve-feature/fftw-system"]
 fftw-mkl = ["light-curve-feature/fftw-mkl"]
 gsl = ["light-curve-feature/gsl"]
@@ -31,24 +31,24 @@
 [dependencies]
 const_format = "0.2.32"
 conv = "0.3.3"
 enum-iterator = "2.0.0"
 enumflags2 = { version = "0.7.7", features = ["serde"] }
 itertools = "0.12.1"
 macro_const = "0.1.0"
-mimalloc = { version = "0.1.39", features = ["local_dynamic_tls"], optional=true }
+mimalloc = { version = "0.1.39", features = ["local_dynamic_tls"], optional = true }
 ndarray = { version = "0.15.3", features = ["rayon"] }
-numpy = "0.19.0"
+numpy = "0.21.0"
 num_cpus = "1.13.0"
 num-traits = "0.2"
 once_cell = "1"
-pyo3 = {version = "0.19.2", features = ["extension-module", "multiple-pymethods"]}
+pyo3 = { version = "0.21.2", features = ["extension-module", "multiple-pymethods", "gil-refs"] }
 rand = "0.8.5"
 rand_xoshiro = "0.6.0"
-rayon = "1.8.1"
+rayon = "1.10.0"
 serde = { version = "1", features = ["derive"] }
 serde-pickle = "1"
 serde_json = "1"
 thiserror = "1.0.50"
 unzip3 = "1.0.0"
 
 [dependencies.light-curve-dmdt]
```

### Comparing `light-curve-python-0.9.0a0/PKG-INFO` & `light_curve_python-0.9.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: light-curve-python
-Version: 0.9.0a0
+Version: 0.9.1
 Summary: An alias to light-curve package
 Home-page: http://github.com/hombit/light-curve
 Author: Konstantin Malanchev
 Author-email: hombit@gmail.com
 License: MIT
 Keywords: science,astrophysics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-Requires-Dist: light-curve[full]==0.9.0-alpha.0
+Requires-Dist: light-curve[full]==0.9.1
 
 # `light-curve-python`
 
 `light-curve-python` had been a previous name of the [`light-curve`](https://github.com/light-curve/light-curve-python) package.
 Now this is an empty package which depends on `light-curve` only.
```

### Comparing `light-curve-python-0.9.0a0/light_curve_python.egg-info/PKG-INFO` & `light_curve_python-0.9.1/light_curve_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: light-curve-python
-Version: 0.9.0a0
+Version: 0.9.1
 Summary: An alias to light-curve package
 Home-page: http://github.com/hombit/light-curve
 Author: Konstantin Malanchev
 Author-email: hombit@gmail.com
 License: MIT
 Keywords: science,astrophysics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-Requires-Dist: light-curve[full]==0.9.0-alpha.0
+Requires-Dist: light-curve[full]==0.9.1
 
 # `light-curve-python`
 
 `light-curve-python` had been a previous name of the [`light-curve`](https://github.com/light-curve/light-curve-python) package.
 Now this is an empty package which depends on `light-curve` only.
```

### Comparing `light-curve-python-0.9.0a0/setup.cfg` & `light_curve_python-0.9.1/setup.cfg`

 * *Files identical despite different names*

