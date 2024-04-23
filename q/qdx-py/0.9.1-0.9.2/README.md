# Comparing `tmp/qdx_py-0.9.1.tar.gz` & `tmp/qdx_py-0.9.2.tar.gz`

## Comparing `qdx_py-0.9.1.tar` & `qdx_py-0.9.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 qdx_py-0.9.1/Cargo.toml
--rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.9.1/.github/workflows/CI.yml
--rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.9.1/.gitignore
--rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.9.1/README.md
--rw-r--r--   0     1000      100      513 2024-04-15 06:01:05.000000 qdx_py-0.9.1/src/lib.rs
--rw-r--r--   0     1000      100     7083 2024-04-15 05:53:38.000000 qdx_py-0.9.1/src/qdx.rs
--rw-r--r--   0     1000      100    27482 2024-04-15 06:38:06.000000 qdx_py-0.9.1/Cargo.lock
--rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 qdx_py-0.9.2/Cargo.toml
+-rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.9.2/.github/workflows/CI.yml
+-rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.9.2/.gitignore
+-rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.9.2/README.md
+-rw-r--r--   0     1000      100      513 2024-04-15 06:01:05.000000 qdx_py-0.9.2/src/lib.rs
+-rw-r--r--   0     1000      100     7083 2024-04-15 05:53:38.000000 qdx_py-0.9.2/src/qdx.rs
+-rw-r--r--   0     1000      100    27482 2024-04-23 06:08:13.000000 qdx_py-0.9.2/Cargo.lock
+-rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.9.2/PKG-INFO
```

### Comparing `qdx_py-0.9.1/Cargo.toml` & `qdx_py-0.9.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qdx-py"
-version = "0.9.1"
+version = "0.9.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "qdx_py"
 crate-type = ["rlib", "cdylib"]
```

### Comparing `qdx_py-0.9.1/.github/workflows/CI.yml` & `qdx_py-0.9.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.1/.gitignore` & `qdx_py-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.1/README.md` & `qdx_py-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.1/src/lib.rs` & `qdx_py-0.9.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.1/src/qdx.rs` & `qdx_py-0.9.2/src/qdx.rs`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.1/Cargo.lock` & `qdx_py-0.9.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,29 @@
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
  "windows-targets 0.52.5",
@@ -386,26 +386,26 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -414,61 +414,61 @@
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "qdx-common"
 version = "0.8.2"
-source = "git+ssh://git@github.com/talo/qdx-common.git#4c4bbdaed55a957d86f801e51b29d13504ac4745"
+source = "git+ssh://git@github.com/talo/qdx-common.git#88fca4d78fec1a712b0b367a4fe5a428b0984763"
 dependencies = [
  "anyhow",
  "assertables",
  "base64",
  "euclid",
  "half",
  "itertools",
@@ -487,15 +487,15 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "qdx-py"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "pyo3",
  "qdx-common",
  "serde",
  "serde_json",
 ]
 
@@ -595,17 +595,17 @@
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-xml-rs"
 version = "0.6.0"
@@ -616,28 +616,28 @@
  "serde",
  "thiserror",
  "xml-rs",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -672,43 +672,43 @@
  "quote",
  "rustversion",
  "syn",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `qdx_py-0.9.1/PKG-INFO` & `qdx_py-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdx-py
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # QDX-py
```

