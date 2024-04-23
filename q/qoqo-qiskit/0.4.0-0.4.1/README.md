# Comparing `tmp/qoqo_qiskit-0.4.0.tar.gz` & `tmp/qoqo_qiskit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_qiskit-0.4.0.tar", last modified: Thu Apr 18 12:29:18 2024, max compression
+gzip compressed data, was "qoqo_qiskit-0.4.1.tar", last modified: Mon Apr 22 12:45:30 2024, max compression
```

## Comparing `qoqo_qiskit-0.4.0.tar` & `qoqo_qiskit-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.117527 qoqo_qiskit-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-18 12:29:18.117527 qoqo_qiskit-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.109527 qoqo_qiskit-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:29:18.117527 qoqo_qiskit-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.109527 qoqo_qiskit-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.109527 qoqo_qiskit-0.4.0/src/qoqo_qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/queued_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/backend/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/backend/test_queued_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/interface/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.640054 qoqo_qiskit-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.632054 qoqo_qiskit-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:45:30.640054 qoqo_qiskit-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.632054 qoqo_qiskit-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.632054 qoqo_qiskit-0.4.1/src/qoqo_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/queued_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/src/qoqo_qiskit/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit/interface/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-22 12:45:30.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-22 12:45:30.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:45:30.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-22 12:45:30.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 12:45:30.000000 qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/tests/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/tests/backend/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/tests/backend/test_queued_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:45:30.636054 qoqo_qiskit-0.4.1/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-22 12:45:19.000000 qoqo_qiskit-0.4.1/tests/interface/test_interface.py
```

### Comparing `qoqo_qiskit-0.4.0/LICENSE` & `qoqo_qiskit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/PKG-INFO` & `qoqo_qiskit-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.4.0
+Version: 0.4.1
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qoqo_qiskit-0.4.0/README.md` & `qoqo_qiskit-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/docs/Makefile` & `qoqo_qiskit-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/docs/conf.py` & `qoqo_qiskit-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/pyproject.toml` & `qoqo_qiskit-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_qiskit"
-version = "0.4.0"
+version = "0.4.1"
 license = { file = "LICENSE" }
 authors = [
     { name = "HQS Quantum Simulation GmbH", email = "info@quantumsimulations.de" },
 ]
 maintainers = [
     { name = "Matteo Lodi", email = "matteo.lodi@quantumsimulations.de" },
 ]
```

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/__init__.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/__init__.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/backend.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,17 +335,29 @@
 
             (
                 tmp_bit_register_dict,
                 tmp_float_register_dict,
                 tmp_complex_register_dict,
             ) = self.run_circuit(run_circuit)
 
-            output_bit_register_dict.update(tmp_bit_register_dict)
-            output_float_register_dict.update(tmp_float_register_dict)
-            output_complex_register_dict.update(tmp_complex_register_dict)
+            for key, value_bools in tmp_bit_register_dict.items():
+                if key in output_bit_register_dict:
+                    output_bit_register_dict[key].extend(value_bools)
+                else:
+                    output_bit_register_dict[key] = value_bools
+            for key, value_floats in tmp_float_register_dict.items():
+                if key in output_float_register_dict:
+                    output_float_register_dict[key].extend(value_floats)
+                else:
+                    output_float_register_dict[key] = value_floats
+            for key, value_complexes in tmp_complex_register_dict.items():
+                if key in output_complex_register_dict:
+                    output_complex_register_dict[key].extend(value_complexes)
+                else:
+                    output_complex_register_dict[key] = value_complexes
 
         return (
             output_bit_register_dict,
             output_float_register_dict,
             output_complex_register_dict,
         )
```

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/post_processing.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/post_processing.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/queued_results.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/queued_results.py`

 * *Files 17% similar despite different names*

```diff
@@ -184,17 +184,29 @@
         self._registers: Tuple[
             Dict[str, List[List[bool]]],
             Dict[str, List[List[float]]],
             Dict[str, List[List[complex]]],
         ] = ({}, {}, {})
         for circuit in self._queued_circuits:
             if circuit._qoqo_result is not None:
-                self._registers[0].update(circuit._qoqo_result[0])
-                self._registers[1].update(circuit._qoqo_result[1])
-                self._registers[2].update(circuit._qoqo_result[2])
+                for key, value_bools in circuit._qoqo_result[0].items():
+                    if key in self._registers[0]:
+                        self._registers[0][key].extend(value_bools)
+                    else:
+                        self._registers[0][key] = value_bools
+                for key, value_floats in circuit._qoqo_result[1].items():
+                    if key in self._registers[1]:
+                        self._registers[1][key].extend(value_floats)
+                    else:
+                        self._registers[1][key] = value_floats
+                for key, value_complexes in circuit._qoqo_result[2].items():
+                    if key in self._registers[2]:
+                        self._registers[2][key].extend(value_complexes)
+                    else:
+                        self._registers[2][key] = value_complexes
 
     def to_json(self) -> str:
         """Convert self to a JSON string.
 
         Returns:
             str: self as a JSON string.
 
@@ -246,17 +258,29 @@
             Dict[str, List[List[float]]],
             Dict[str, List[List[complex]]],
         ] = ({}, {}, {})
         for circuit in json_dict["queued_circuits"]:
             circ_instance = QueuedCircuitRun.from_json(circuit)
             queued_circuits_deserialised.append(circ_instance)
             if circ_instance._qoqo_result is not None:
-                registers[0].update(circ_instance._qoqo_result[0])
-                registers[1].update(circ_instance._qoqo_result[1])
-                registers[2].update(circ_instance._qoqo_result[2])
+                for key, value_bools in circ_instance._qoqo_result[0].items():
+                    if key in registers[0]:
+                        registers[0][key].extend(value_bools)
+                    else:
+                        registers[0][key] = value_bools
+                for key, value_floats in circ_instance._qoqo_result[1].items():
+                    if key in registers[1]:
+                        registers[1][key].extend(value_floats)
+                    else:
+                        registers[1][key] = value_floats
+                for key, value_complexes in circ_instance._qoqo_result[2].items():
+                    if key in registers[2]:
+                        registers[2][key].extend(value_complexes)
+                    else:
+                        registers[2][key] = value_complexes
 
         if json_dict["measurement_type"] == "PauliZProduct":
             measurement = measurements.PauliZProduct.from_json(json_dict["measurement"])
         elif json_dict["measurement_type"] == "CheatedPauliZProduct":
             measurement = measurements.CheatedPauliZProduct.from_json(json_dict["measurement"])
         elif json_dict["measurement_type"] == "Cheated":
             measurement = measurements.Cheated.from_json(json_dict["measurement"])
@@ -290,17 +314,29 @@
         Raises:
             RuntimeError: The jobs failed or were cancelled.
         """
         all_finished = [False] * len(self._queued_circuits)
         for i, queued_circuit in enumerate(self._queued_circuits):
             res = queued_circuit.poll_result()
             if res is not None:
-                self._registers[0].update(res[0])  # add results to bit registers
-                self._registers[1].update(res[1])  # add results to float registers
-                self._registers[2].update(res[2])  # add results to complex registers
+                for key, value_bools in res[0].items():
+                    if key in self._registers[0]:
+                        self._registers[0][key].extend(value_bools)
+                    else:
+                        self._registers[0][key] = value_bools
+                for key, value_floats in res[1].items():
+                    if key in self._registers[1]:
+                        self._registers[1][key].extend(value_floats)
+                    else:
+                        self._registers[1][key] = value_floats
+                for key, value_complexes in res[2].items():
+                    if key in self._registers[2]:
+                        self._registers[2][key].extend(value_complexes)
+                    else:
+                        self._registers[2][key] = value_complexes
                 all_finished[i] = True
 
         if not all(all_finished):
             return None
         else:
             if isinstance(self._measurement, measurements.ClassicalRegister):
                 return self._registers
```

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/utils.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/backend/utils.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/__init__.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/interface.py` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit/interface/interface.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/PKG-INFO` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.4.0
+Version: 0.4.1
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/SOURCES.txt` & `qoqo_qiskit-0.4.1/src/qoqo_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/tests/__init__.py` & `qoqo_qiskit-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/tests/backend/__init__.py` & `qoqo_qiskit-0.4.1/tests/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/tests/backend/test_backend.py` & `qoqo_qiskit-0.4.1/tests/backend/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,14 +382,48 @@
     clas_regs["ro"] = 1
     clas_regs["ri"] = 2
     shot_result_ws = "01 1"
     shot_result_no_ws = "011"
 
     assert _split(shot_result_ws, clas_regs) == _split(shot_result_no_ws, clas_regs)
 
+def test_overwrite() -> None:
+    """Tests overwriting registers."""
+    backend = QoqoQiskitBackend()
+
+    circuit_1 = Circuit()
+    circuit_1 += ops.DefinitionBit("same", 1, True)
+    circuit_1 += ops.PauliX(0)
+    circuit_1 += ops.MeasureQubit(0, "same", 0)
+    circuit_1 += ops.PragmaSetNumberOfMeasurements(2, "same")
+
+    circuit_2 = Circuit()
+    circuit_2 += ops.DefinitionBit("same", 1, True)
+    circuit_2 += ops.PauliX(0)
+    circuit_2 += ops.PauliX(0)
+    circuit_2 += ops.MeasureQubit(0, "same", 0)
+    circuit_2 += ops.PragmaSetNumberOfMeasurements(2, "same")
+
+
+    measurement = ClassicalRegister(constant_circuit=None, circuits=[circuit_1, circuit_2])
+
+    try:
+        output = backend.run_measurement_registers(measurement=measurement)
+    except Exception:
+        assert False
+
+    # output should look like ({'same': [[True], [True], [False], [False]]}, {}, {})
+    assert len(output[0]["same"]) == 4
+    assert output[0]["same"][0][0]
+    assert output[0]["same"][1][0]
+    assert not output[0]["same"][2][0]
+    assert not output[0]["same"][3][0]
+    assert not output[1]
+    assert not output[2]
+
 def test_run_program() -> None:
     """Test QoqoQiskitBackend.run_program method."""
     backend = QoqoQiskitBackend()
     
     init_circuit = Circuit()
     init_circuit += ops.RotateX(0, "angle_0")
     init_circuit += ops.RotateY(0, "angle_1")
```

### Comparing `qoqo_qiskit-0.4.0/tests/backend/test_queued_results.py` & `qoqo_qiskit-0.4.1/tests/backend/test_queued_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -162,10 +162,58 @@
     res_qpr, _, _ = qpr.poll_result()
 
     assert res_qcr["ri"]
     assert res_qpr["ro"]
     assert res_qpr["ri"]
 
 
+def test_overwrite() -> None:
+    """Test overwriting registers."""
+    run_0 = _mocked_run(memory="True")
+    run_1 = _mocked_run()
+
+    qcr_0 = QueuedCircuitRun(
+        job=run_0[0],
+        memory=True,
+        sim_type=run_0[1],
+        registers_info=run_0[2],
+    )
+    qcr_1 = QueuedCircuitRun(
+        job=run_1[0],
+        memory=False,
+        sim_type=run_1[1],
+        registers_info=run_1[2],
+    )
+
+    measurement = ClassicalRegister(constant_circuit=None, circuits=[run_0[3], run_1[3]])
+    qpr = QueuedProgramRun(
+        measurement=measurement,
+        queued_circuits=[qcr_0, qcr_1],
+    )
+
+    # Making sure that the simulations are finished
+    time.sleep(1)
+
+    res_qpr, _, _ = qpr.poll_result()
+
+    assert len(res_qpr["ri"]) == 20
+
+    run_2 = _mocked_run()
+    qcr_2 = QueuedCircuitRun(
+        job=run_2[0],
+        memory=False,
+        sim_type=run_2[1],
+        registers_info=run_2[2],
+    )
+    qcr_2.poll_result()
+
+    qpr = QueuedProgramRun(
+        measurement=measurement,
+        queued_circuits=[qcr_0, qcr_1, qcr_2],
+    )
+
+    assert len(qpr._registers[0]["ri"]) == 30
+
+
 # For pytest
 if __name__ == "__main__":
     pytest.main(sys.argv)
```

### Comparing `qoqo_qiskit-0.4.0/tests/interface/__init__.py` & `qoqo_qiskit-0.4.1/tests/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.4.0/tests/interface/test_interface.py` & `qoqo_qiskit-0.4.1/tests/interface/test_interface.py`

 * *Files identical despite different names*

