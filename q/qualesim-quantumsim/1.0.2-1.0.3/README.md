# Comparing `tmp/qualesim-quantumsim-1.0.2.tar.gz` & `tmp/qualesim-quantumsim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quantumsim-1.0.2.tar", last modified: Fri Apr 19 08:10:33 2024, max compression
+gzip compressed data, was "qualesim-quantumsim-1.0.3.tar", last modified: Tue Apr 23 03:10:49 2024, max compression
```

## Comparing `qualesim-quantumsim-1.0.2.tar` & `qualesim-quantumsim-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:10:33.128466 qualesim-quantumsim-1.0.2/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-07-04 13:48:17.000000 qualesim-quantumsim-1.0.2/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-04-19 08:10:33.128466 qualesim-quantumsim-1.0.2/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       81 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.2/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:10:33.124467 qualesim-quantumsim-1.0.2/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:10:33.128466 qualesim-quantumsim-1.0.2/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.2/data/bin/dqcsbequantumsim
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:10:33.128466 qualesim-quantumsim-1.0.2/qualesim_quantumsim/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        2 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim/__init__.py
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11550 2024-04-19 08:05:15.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim/backend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7614 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim/qubit.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:10:33.128466 qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-04-19 08:10:33.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      390 2024-04-19 08:10:33.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-19 08:10:33.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       22 2024-04-19 08:10:33.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       20 2024-04-19 08:10:33.000000 qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-19 08:10:33.128466 qualesim-quantumsim-1.0.2/setup.cfg
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1113 2024-04-19 08:09:50.000000 qualesim-quantumsim-1.0.2/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:10:49.023384 qualesim-quantumsim-1.0.3/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-07-04 13:48:17.000000 qualesim-quantumsim-1.0.3/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-04-23 03:10:49.023384 qualesim-quantumsim-1.0.3/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       81 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.3/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:10:49.015384 qualesim-quantumsim-1.0.3/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:10:49.015384 qualesim-quantumsim-1.0.3/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.3/data/bin/dqcsbequantumsim
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:10:49.019384 qualesim-quantumsim-1.0.3/qualesim_quantumsim/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        2 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim/__init__.py
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11914 2024-04-23 03:05:07.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim/backend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7447 2024-04-19 13:15:04.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim/qubit.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:10:49.023384 qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-04-23 03:10:48.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      390 2024-04-23 03:10:48.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-23 03:10:48.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       22 2024-04-23 03:10:48.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       20 2024-04-23 03:10:48.000000 qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-23 03:10:49.023384 qualesim-quantumsim-1.0.3/setup.cfg
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1113 2024-04-19 12:24:50.000000 qualesim-quantumsim-1.0.3/setup.py
```

### Comparing `qualesim-quantumsim-1.0.2/LICENSE` & `qualesim-quantumsim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quantumsim-1.0.2/PKG-INFO` & `qualesim-quantumsim-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quantumsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: QuaLeSim backend for QuantumSim.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quantumsim.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: QuaLeSim quantumsim
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quantumsim-1.0.2/qualesim_quantumsim/backend.py` & `qualesim-quantumsim-1.0.3/qualesim_quantumsim/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from qualesim.common import *
 from qualesim_quantumsim.qubit import Qubit
 import struct
 import numpy as np
 from quantumsim.dm_np import DensityNP
 
 # import copy
-
+def bitwise_reverse_sort(lst, k):
+    sorted_lst = []
+    for i in range(len(lst)):
+        sorted_lst.append(lst[int("0b" + bin(i)[2:].zfill(k)[::-1], 2)])
+    return sorted_lst
 
 @plugin("QuantumSim interface for QuaLeSim", "Dingdong Liu", "0.0.1")
 class QuantumSimInterface(Backend):
     # QuantumSim's SparseDM object doesn't support adding or removing qubits.
     # However, any qubits that haven't been entangled yet are purely classical.
     # Therefore, we can just allocate a large number of qubits at startup and
     # use those when we need them. This is that large number.
@@ -143,66 +147,57 @@
             basis[3].real - basis[3].imag * 1j,
         ]
 
         # Perform the measurements.
         measurements = []
         msg = dict()
         msmt = []
-        qu_re = [i - 1 for i in qubit_refs]
-        state_res_before = self._partial_trace(self.sdm.full_dm, qu_re)
         st = dict()
         res_l = []
+        state_res_before = self._dm_to_vec(self.sdm.full_dm.to_array())
         for qubit_ref in qubit_refs:
             st[qubit_ref] = self._partial_trace(self.sdm.full_dm, [qubit_ref - 1])
             self.handle_unitary_gate([qubit_ref], basis_hermetian, None)
             qubit: Qubit = self.qubits[qubit_ref]
-            qubit.apply_pending_error()
-            if qubit.qs_ref is not None:
-                p0, p1 = qubit.qsi.sdm.peak_measurement(qubit.qs_ref)
-                trace = p0 + p1
-                p0 /= trace
-                p1 /= trace
-                qubit.classical = int(qubit.qsi.random_float() < p1)
-                qubit.qsi.sdm.project_measurement(
-                    qubit.qs_ref, int(bool(qubit.classical))
-                )
-                qubit.qsi.sdm.renormalize()
-                if qubit.classical:
-                    p = p1
-                else:
-                    p = p0
+            p = qubit.measure()
+            self.handle_unitary_gate([qubit_ref], basis, None)
             msg[qubit_ref] = (qubit.classical, p)
             self.cls_dict[qubit_ref] = qubit.classical
             res_l.append(qubit.classical)
         msmt.append(res_l)
-
         if measure_mod == "measureforres":
-            state_res = str([self.cls_dict, state_res_before])
+            
+            state_res = str([self.cls_dict, st[qubit_ref]])
+            state_for_res = str([self.cls_dict, state_res_before])
             for qubit_ref in qubit_refs:
                 measurements.append(
                     Measurement(
                         qubit_ref,
                         msg[qubit_ref][0],
                         struct.pack("<d", msg[qubit_ref][1]),
                         probability=msg[qubit_ref][1],
                         state_vector=state_res,
+                        state_for_res=state_for_res,
+                        state_vector_be=state_for_res,
                         one_shot=msmt,
                     )
                 )
                 self.handle_unitary_gate([qubit_ref], basis, None)
         else:
+            state_for_res = str([self.cls_dict, state_res_before])
             for qubit_ref in qubit_refs:
                 state_res = str([self.cls_dict, st[qubit_ref]])
                 measurements.append(
                     Measurement(
                         qubit_ref,
                         msg[qubit_ref][0],
                         struct.pack("<d", msg[qubit_ref][1]),
                         probability=msg[qubit_ref][1],
                         state_vector=state_res,
+                        state_vector_be=state_for_res,
                         one_shot=msmt,
                     )
                 )
                 self.handle_unitary_gate([qubit_ref], basis, None)
         return measurements
 
     def _dm_to_vec(self, dm_array):
@@ -222,14 +217,15 @@
                 cur_max_norm = norm
         return list(state_vec)
 
     def _partial_trace(self, full_dm, qubits_ref):
         """Method for partial trace of a density matrix."""
         dm_array = full_dm.to_array()
         num_qubits = int(np.log2(dm_array.shape[0]))  # Total number of qubits
+        qubits_ref = [num_qubits - qubits_ref[0] - 1]
         qubits_to_trace = [i for i in range(num_qubits) if i not in qubits_ref]
         num_qubits_to_trace = len(qubits_to_trace)  # Number of qubits to trace out
 
         # Compute the dimensions of the reduced density matrix
         reduced_dm_dim = 2 ** (num_qubits - num_qubits_to_trace)
 
         # Initialize the reduced density matrix
@@ -238,18 +234,26 @@
         # Compute the indices of the qubits to keep
         qubits_to_keep = sorted(set(range(num_qubits)) - set(qubits_to_trace))
 
         # Iterate over all elements of the full density matrix
         for i in range(2**num_qubits):
             # Compute the indices of the corresponding element in the reduced density matrix
             reduced_dm_index = tuple(np.array([i >> q & 1 for q in qubits_to_keep]))
-
             # Update the corresponding element in the reduced density matrix
             reduced_dm[reduced_dm_index] += dm_array[i, i]
-        return self._dm_to_vec(reduced_dm)
+        # Normalize each column of the reduced density matrix
+        for i in range(reduced_dm_dim):
+            col_norm = np.linalg.norm(reduced_dm[i, :])
+            if col_norm != 0:
+                reduced_dm[i, :] /= col_norm
+
+        # Choose the column with the maximum norm as the state vector
+        state_vec = reduced_dm[:, np.argmax(np.abs(reduced_dm.sum(axis=0)))]
+
+        return list(state_vec)
 
     def handle_prepare_gate(self, qubit_refs, basis, _arb):
         measurements = []
         for qubit_ref in qubit_refs:
             self.qubits[qubit_ref].prep()
             self.handle_unitary_gate([qubit_ref], basis, None)
         return measurements
```

### Comparing `qualesim-quantumsim-1.0.2/qualesim_quantumsim/qubit.py` & `qualesim-quantumsim-1.0.3/qualesim_quantumsim/qubit.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,15 @@
                     raise ValueError("cannot project to 1, qubit state was classical 0")
             else:
                 raise ValueError("unknown measurement method %r" % method)
 
             # The probability is always 1.0
             p = 1.0
 
-        return Measurement(
-            self.qubit_ref,
-            self.classical,
-            struct.pack("<d", p),
-            probability=p,
-            typ=measure_mod,
-        )
+        return p
 
     def prep(self):
         """Put this qubit in the |0> state."""
 
         # Reset idle time.
         self._idle_time = 0
```

### Comparing `qualesim-quantumsim-1.0.2/qualesim_quantumsim.egg-info/PKG-INFO` & `qualesim-quantumsim-1.0.3/qualesim_quantumsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quantumsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: QuaLeSim backend for QuantumSim.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quantumsim.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: QuaLeSim quantumsim
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quantumsim-1.0.2/setup.py` & `qualesim-quantumsim-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quantumsim",
-    version="1.0.2",
+    version="1.0.3",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim backend for QuantumSim.",
     license="GPLv3",
     keywords="QuaLeSim quantumsim",
     url="https://gitee.com/hpcl_quanta/dqcsim-quantumsim.git",
     long_description=read("README.md"),
```

