# Comparing `tmp/qoqo_qiskit_devices-0.4.1.tar.gz` & `tmp/qoqo_qiskit_devices-0.4.2.tar.gz`

## Comparing `qoqo_qiskit_devices-0.4.1.tar` & `qoqo_qiskit_devices-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0     1001      127      802 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/Cargo.toml
--rw-r--r--   0     1001      127    11357 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/LICENSE
--rw-r--r--   0     1001      127      406 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/README.md
--rw-r--r--   0     1001      127    15120 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_belem.rs
--rw-r--r--   0     1001      127    15315 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_jakarta.rs
--rw-r--r--   0     1001      127    15201 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_lagos.rs
--rw-r--r--   0     1001      127    15048 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_lima.rs
--rw-r--r--   0     1001      127    15065 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_manila.rs
--rw-r--r--   0     1001      127    15231 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_nairobi.rs
--rw-r--r--   0     1001      127    15201 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_perth.rs
--rw-r--r--   0     1001      127    15064 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_quito.rs
--rw-r--r--   0     1001      127    23452 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices.rs
--rw-r--r--   0     1001      127     1001 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/lib.rs
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/Cargo.toml
--rw-r--r--   0     1001      127    11357 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/LICENSE
--rw-r--r--   0     1001      127     1260 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/README.md
--rw-r--r--   0     1001      127    13157 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_belem.rs
--rw-r--r--   0     1001      127    13261 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_jakarta.rs
--rw-r--r--   0     1001      127    13156 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_lagos.rs
--rw-r--r--   0     1001      127    13140 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_lima.rs
--rw-r--r--   0     1001      127    13245 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_manila.rs
--rw-r--r--   0     1001      127    13260 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_nairobi.rs
--rw-r--r--   0     1001      127    13156 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_perth.rs
--rw-r--r--   0     1001      127    13157 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_quito.rs
--rw-r--r--   0     1001      127     3768 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/mod.rs
--rw-r--r--   0     1001      127     1437 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/lib.rs
--rw-r--r--   0     1001      127    20575 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/Cargo.lock
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 qoqo_qiskit_devices-0.4.1/pyproject.toml
--rw-r--r--   0     1001      127     2007 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/mocked_properties.py
--rw-r--r--   0     1001      127    11595 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/device_property.py
--rw-r--r--   0     1001      127      879 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/__init__.py
--rw-r--r--   0     1001      127    11880 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      127     2404 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/PYTHON_LICENSE
--rw-r--r--   0     1001      127  1052849 2024-04-22 12:48:09.000000 qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/DEPENDENCIES
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 qoqo_qiskit_devices-0.4.1/PKG-INFO
+-rw-r--r--   0     1001      127      802 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/Cargo.toml
+-rw-r--r--   0     1001      127    11357 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/LICENSE
+-rw-r--r--   0     1001      127      406 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/README.md
+-rw-r--r--   0     1001      127    15120 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_belem.rs
+-rw-r--r--   0     1001      127    15315 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_jakarta.rs
+-rw-r--r--   0     1001      127    15201 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_lagos.rs
+-rw-r--r--   0     1001      127    15048 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_lima.rs
+-rw-r--r--   0     1001      127    15065 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_manila.rs
+-rw-r--r--   0     1001      127    15231 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_nairobi.rs
+-rw-r--r--   0     1001      127    15201 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_perth.rs
+-rw-r--r--   0     1001      127    15064 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_quito.rs
+-rw-r--r--   0     1001      127    23452 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices.rs
+-rw-r--r--   0     1001      127     1001 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/lib.rs
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/Cargo.toml
+-rw-r--r--   0     1001      127    11357 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/LICENSE
+-rw-r--r--   0     1001      127     1260 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/README.md
+-rw-r--r--   0     1001      127    13157 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_belem.rs
+-rw-r--r--   0     1001      127    13261 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_jakarta.rs
+-rw-r--r--   0     1001      127    13156 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_lagos.rs
+-rw-r--r--   0     1001      127    13140 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_lima.rs
+-rw-r--r--   0     1001      127    13245 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_manila.rs
+-rw-r--r--   0     1001      127    13260 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_nairobi.rs
+-rw-r--r--   0     1001      127    13156 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_perth.rs
+-rw-r--r--   0     1001      127    13157 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_quito.rs
+-rw-r--r--   0     1001      127     3768 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/mod.rs
+-rw-r--r--   0     1001      127     1437 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/lib.rs
+-rw-r--r--   0     1001      127    20575 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/Cargo.lock
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 qoqo_qiskit_devices-0.4.2/pyproject.toml
+-rw-r--r--   0     1001      127     2007 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/mocked_properties.py
+-rw-r--r--   0     1001      127    11595 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/device_property.py
+-rw-r--r--   0     1001      127      879 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/__init__.py
+-rw-r--r--   0     1001      127    11880 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      127     2404 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/PYTHON_LICENSE
+-rw-r--r--   0     1001      127  1052849 2024-04-23 10:51:57.000000 qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/DEPENDENCIES
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 qoqo_qiskit_devices-0.4.2/PKG-INFO
```

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/Cargo.toml` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo_qiskit_devices"
-version = "0.4.1"
+version = "0.4.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2021"
 categories = ["science", "simulation"]
 readme = "README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qiskit"
 description = "IBM's Qiskit devices interface for roqoqo rust quantum computing toolkit"
```

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/LICENSE` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_belem.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_belem.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_jakarta.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_jakarta.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_lagos.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_lagos.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_lima.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_lima.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_manila.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_manila.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_nairobi.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_nairobi.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_perth.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_perth.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices/ibm_quito.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices/ibm_quito.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/devices.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/devices.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/roqoqo_qiskit_devices/src/lib.rs` & `qoqo_qiskit_devices-0.4.2/roqoqo_qiskit_devices/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/Cargo.toml` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo_qiskit_devices"
-version = "0.4.1"
+version = "0.4.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2021"
 categories = ["science", "simulation"]
 readme = "README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qiskit"
 description = "IBM's Qiskit devices interface for qoqo python quantum computing toolkit"
```

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/LICENSE` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/README.md` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_belem.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_belem.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_jakarta.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_jakarta.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_lagos.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_lagos.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_lima.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_lima.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_manila.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_manila.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_nairobi.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_nairobi.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_perth.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_perth.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/ibm_quito.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/ibm_quito.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/devices/mod.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/devices/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/src/lib.rs` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/Cargo.lock` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/Cargo.lock`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/pyproject.toml` & `qoqo_qiskit_devices-0.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_qiskit_devices"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
   'qoqo_calculator_pyo3>=1.1',
   'qoqo>=1.9',
   'qiskit<0.46',
   'qiskit-ibm-provider',
   'struqture_py',
   "setuptools; python_version>='3.12'",
```

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/mocked_properties.py` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/mocked_properties.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/device_property.py` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/device_property.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/__init__.py` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/LICENSE_FOR_BINARY_DISTRIBUTION` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/LICENSE_FOR_BINARY_DISTRIBUTION`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/PYTHON_LICENSE` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit_devices-0.4.1/qoqo_qiskit_devices/DEPENDENCIES` & `qoqo_qiskit_devices-0.4.2/qoqo_qiskit_devices/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -33361,15 +33361,15 @@
 00082500: 7373 696f 6e73 2061 6e64 0a20 2020 6c69  ssions and.   li
 00082510: 6d69 7461 7469 6f6e 7320 756e 6465 7220  mitations under 
 00082520: 7468 6520 4c69 6365 6e73 652e 0a0a 0a3d  the License....=
 00082530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00082540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00082550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00082560: 3d3d 3d0a 716f 716f 5f71 6973 6b69 745f  ===.qoqo_qiskit_
-00082570: 6465 7669 6365 7320 302e 342e 310a 6874  devices 0.4.1.ht
+00082570: 6465 7669 6365 7320 302e 342e 320a 6874  devices 0.4.2.ht
 00082580: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00082590: 2f48 5153 7175 616e 7475 6d73 696d 756c  /HQSquantumsimul
 000825a0: 6174 696f 6e73 2f71 6f71 6f5f 7169 736b  ations/qoqo_qisk
 000825b0: 6974 0a62 7920 4851 5320 5175 616e 7475  it.by HQS Quantu
 000825c0: 6d20 5369 6d75 6c61 7469 6f6e 7320 3c69  m Simulations <i
 000825d0: 6e66 6f40 7175 616e 7475 6d73 696d 756c  nfo@quantumsimul
 000825e0: 6174 696f 6e73 2e64 653e 0a49 424d 2773  ations.de>.IBM's
@@ -40040,15 +40040,15 @@
 0009c670: 2020 206c 696d 6974 6174 696f 6e73 2075     limitations u
 0009c680: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
 0009c690: 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ....============
 0009c6a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0009c6b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0009c6c0: 3d3d 3d3d 3d3d 3d3d 0a72 6f71 6f71 6f5f  ========.roqoqo_
 0009c6d0: 7169 736b 6974 5f64 6576 6963 6573 2030  qiskit_devices 0
-0009c6e0: 2e34 2e31 0a68 7474 7073 3a2f 2f67 6974  .4.1.https://git
+0009c6e0: 2e34 2e32 0a68 7474 7073 3a2f 2f67 6974  .4.2.https://git
 0009c6f0: 6875 622e 636f 6d2f 4851 5371 7561 6e74  hub.com/HQSquant
 0009c700: 756d 7369 6d75 6c61 7469 6f6e 732f 716f  umsimulations/qo
 0009c710: 716f 5f71 6973 6b69 740a 6279 2048 5153  qo_qiskit.by HQS
 0009c720: 2051 7561 6e74 756d 2053 696d 756c 6174   Quantum Simulat
 0009c730: 696f 6e73 203c 696e 666f 4071 7561 6e74  ions <info@quant
 0009c740: 756d 7369 6d75 6c61 7469 6f6e 732e 6465  umsimulations.de
 0009c750: 3e0a 4942 4d27 7320 5169 736b 6974 2064  >.IBM's Qiskit d
```

### Comparing `qoqo_qiskit_devices-0.4.1/PKG-INFO` & `qoqo_qiskit_devices-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qoqo_qiskit_devices
-Version: 0.4.1
+Version: 0.4.2
 Requires-Dist: qoqo-calculator-pyo3 >=1.1
 Requires-Dist: qoqo >=1.9
 Requires-Dist: qiskit <0.46
 Requires-Dist: qiskit-ibm-provider
 Requires-Dist: struqture-py
 Requires-Dist: setuptools ; python_version >= '3.12'
 Requires-Dist: numpy ; extra == 'docs'
```

