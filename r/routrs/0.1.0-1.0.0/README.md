# Comparing `tmp/routrs-0.1.0.tar.gz` & `tmp/routrs-1.0.0.tar.gz`

## Comparing `routrs-0.1.0.tar` & `routrs-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 routrs-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     3888 2024-04-22 10:23:32.000000 routrs-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0      501       20      663 2024-04-22 10:23:32.000000 routrs-0.1.0/.gitignore
--rw-r--r--   0      501       20     1070 2024-04-22 10:23:32.000000 routrs-0.1.0/LICENSE
--rw-r--r--   0      501       20      102 2024-04-22 10:23:32.000000 routrs-0.1.0/README.md
--rw-r--r--   0      501       20       36 2024-04-22 10:23:32.000000 routrs-0.1.0/mypy.ini
--rw-r--r--   0      501       20    14402 2024-04-22 10:23:32.000000 routrs-0.1.0/poetry.lock
--rw-r--r--   0      501       20       97 2024-04-22 10:23:32.000000 routrs-0.1.0/pytest.ini
--rw-r--r--   0      501       20      130 2024-04-22 10:23:32.000000 routrs-0.1.0/routrs.pyi
--rw-r--r--   0      501       20      567 2024-04-22 10:23:32.000000 routrs-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      607 2024-04-22 10:23:32.000000 routrs-0.1.0/src/maritime.rs
--rw-r--r--   0      501       20        0 2024-04-22 10:23:32.000000 routrs-0.1.0/test/conftest.py
--rw-r--r--   0      501       20      297 2024-04-22 10:23:32.000000 routrs-0.1.0/test/test_routrs.py
--rw-r--r--   0      501       20    66231 2024-04-22 10:23:46.000000 routrs-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      655 2024-04-22 10:23:32.000000 routrs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      222 1970-01-01 00:00:00.000000 routrs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 routrs-1.0.0/Cargo.toml
+-rw-r--r--   0      501       20      715 2024-04-23 09:59:22.000000 routrs-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0      501       20     3127 2024-04-23 09:59:22.000000 routrs-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0      501       20      663 2024-04-23 09:59:22.000000 routrs-1.0.0/.gitignore
+-rw-r--r--   0      501       20     1070 2024-04-23 09:59:22.000000 routrs-1.0.0/LICENSE
+-rw-r--r--   0      501       20      148 2024-04-23 09:59:22.000000 routrs-1.0.0/README.md
+-rw-r--r--   0      501       20       36 2024-04-23 09:59:22.000000 routrs-1.0.0/mypy.ini
+-rw-r--r--   0      501       20    14402 2024-04-23 09:59:22.000000 routrs-1.0.0/poetry.lock
+-rw-r--r--   0      501       20       97 2024-04-23 09:59:22.000000 routrs-1.0.0/pytest.ini
+-rw-r--r--   0      501       20     4260 2024-04-23 09:59:22.000000 routrs-1.0.0/routrs.pyi
+-rw-r--r--   0      501       20     1612 2024-04-23 09:59:22.000000 routrs-1.0.0/src/highways.rs
+-rw-r--r--   0      501       20     2101 2024-04-23 09:59:22.000000 routrs-1.0.0/src/lib.rs
+-rw-r--r--   0      501       20     1549 2024-04-23 09:59:22.000000 routrs-1.0.0/src/maritime.rs
+-rw-r--r--   0      501       20     1618 2024-04-23 09:59:22.000000 routrs-1.0.0/src/railways.rs
+-rw-r--r--   0      501       20        0 2024-04-23 09:59:22.000000 routrs-1.0.0/test/conftest.py
+-rw-r--r--   0      501       20     2307 2024-04-23 09:59:22.000000 routrs-1.0.0/test/test_routrs.py
+-rw-r--r--   0      501       20    66287 2024-04-23 09:59:39.000000 routrs-1.0.0/Cargo.lock
+-rw-r--r--   0      501       20      656 2024-04-23 09:59:22.000000 routrs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 routrs-1.0.0/PKG-INFO
```

### Comparing `routrs-0.1.0/.github/workflows/ci.yml` & `routrs-1.0.0/.github/workflows/release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,17 @@
-name: ci
+name: release
 
 on:
   release:
     types: [created]
   workflow_dispatch:
 
 jobs:
-  check:
-    name: Check
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-      - uses: dtolnay/rust-toolchain@stable
-      - run: cargo check
-
-  test:
-    name: Test suite
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-    steps:
-      - uses: actions/checkout@v4
-      - uses: dtolnay/rust-toolchain@stable
-      - run: cargo test --all
-
-  fmt:
-    name: Rustfmt
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-      - uses: dtolnay/rust-toolchain@stable
-        with:
-          components: rustfmt
-      - run: cargo fmt --all -- --check
-
   macos:
     runs-on: macos-latest
-    needs: [check, test, fmt]
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: 3.9
           architecture: x64
       - uses: dtolnay/rust-toolchain@nightly
@@ -68,15 +38,14 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
     runs-on: windows-latest
-    needs: [check, test, fmt]
     strategy:
       matrix:
         target: [x64, x86]
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
@@ -97,15 +66,14 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   linux:
     runs-on: ubuntu-latest
-    needs: [check, test, fmt]
     strategy:
       matrix:
         target: [x86_64, i686]
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
@@ -130,15 +98,15 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     environment: pypi
-    needs: [check, test, fmt, macos, windows, linux]
+    needs: [macos, windows, linux]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `routrs-0.1.0/.gitignore` & `routrs-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `routrs-0.1.0/LICENSE` & `routrs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `routrs-0.1.0/poetry.lock` & `routrs-1.0.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `routrs-0.1.0/src/maritime.rs` & `routrs-1.0.0/src/maritime.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,51 @@
+use routrs::concurrency::*;
 use routrs::maritime;
 use routrs::prelude::*;
 
 pub fn distance(origin: &Geoloc, destination: &Geoloc) -> DistanceResult {
     maritime::distance(origin, destination)
 }
 
+pub fn par_distance(legs: &[Leg<Geoloc>]) -> Result<Vec<(f64, Path<Geoloc>)>, String> {
+    maritime::geograph()
+        .par_distance(legs)
+        .into_iter()
+        .map(|result| result.map(|(distance, path, _)| (distance, path)))
+        .collect()
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
-    #[test]
-    fn it_calculates_maritime_distance() {
+    fn geoloc_fixtures() -> (Geoloc, Geoloc) {
         let from: Geoloc = (40.6759, -74.0504); // USNYC
         let to: Geoloc = (41.0067858, 28.9732219); // TRIST
+        (from, to)
+    }
+
+    #[test]
+    fn it_calculates_maritime_distance() {
+        let (from, to) = geoloc_fixtures();
         let (distance, path, path_type) = distance(&from, &to).unwrap();
 
         assert_eq!(distance, 9224.95741604269);
         assert_eq!(path.len(), 118);
         assert_eq!(path_type, PathType::ViaWaypoints);
     }
+
+    #[test]
+    fn it_parallel_calculates_maritime_distance() {
+        let (from, to) = geoloc_fixtures();
+        let (expected_distance, expected_path, _) = distance(&from, &to).unwrap();
+
+        let legs: Vec<_> = (0..100).map(|_| Leg((from, to))).collect();
+        let distances = par_distance(&legs).unwrap();
+
+        assert_eq!(distances.len(), legs.len());
+        for (distance, path) in distances {
+            assert_eq!(distance, expected_distance);
+            assert_eq!(path.len(), expected_path.len());
+        }
+    }
 }
```

### Comparing `routrs-0.1.0/Cargo.lock` & `routrs-1.0.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -895,17 +895,17 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.35"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3979b5c37ece694f1f5e51e7ecc871fdb0f517ed04ee45f88d15d6d553cb9664"
+checksum = "81eb4061c0582dedea1cbc7aff2240300dd6982e0239d1c99e65c1dbf4a30ba7"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libredox"
@@ -1045,17 +1045,17 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.39"
+version = "0.1.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa01922b5ea280a911e323e4d2fd24b7fe5cc4042e0d2cda3c40775cdc4bdc9c"
+checksum = "9f41a2280ded0da56c8cf898babb86e8f10651a34adcfff190ae9a1159c6908d"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -1569,19 +1569,19 @@
  "spin",
  "untrusted",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "routrs"
-version = "0.1.0"
+version = "1.0.0"
 dependencies = [
  "maturin",
  "pyo3",
- "routrs 1.0.0",
+ "routrs 1.0.0 (registry+https://github.com/rust-lang/crates.io-index)",
 ]
 
 [[package]]
 name = "routrs"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "242ef6a6a2e66cb83f260df766ecbfaa8508803abbf4ecdaa5943e8ac3dfa9cc"
@@ -1633,17 +1633,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.33"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3cc72858054fcff6d7dea32df2aeaee6a7c24227366d7ea429aada2f26b16ad"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
@@ -1676,17 +1676,17 @@
 name = "rustls-pki-types"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
```

### Comparing `routrs-0.1.0/pyproject.toml` & `routrs-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "pyroutrs"
-version = "0.1.0"
+version = "1.0.0"
 description = "Geograph-based shortest distance calculation for Python. 100% in Rust."
 authors = ["Carlo Casorzo <carlo@deepblu.dev>"]
 license = "MIT"
 readme = "README.md"
 
+
 [tool.poe.tasks]
 test = "pytest"
 "build:dev" = "maturin develop --manifest-path bindings/Cargo.toml"
 "build" = "maturin build --release --out dist --manifest-path bindings/Cargo.toml"
 
 
 [tool.poetry.dependencies]
```

