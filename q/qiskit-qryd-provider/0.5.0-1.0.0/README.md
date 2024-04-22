# Comparing `tmp/qiskit_qryd_provider-0.5.0.tar.gz` & `tmp/qiskit_qryd_provider-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_qryd_provider-0.5.0.tar", max compression
+gzip compressed data, was "qiskit_qryd_provider-1.0.0.tar", max compression
```

## Comparing `qiskit_qryd_provider-0.5.0.tar` & `qiskit_qryd_provider-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11358 2023-12-03 18:07:59.091296 qiskit_qryd_provider-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     3412 2023-12-03 18:07:56.955256 qiskit_qryd_provider-0.5.0/README.md
--rw-r--r--   0        0        0     1088 2023-12-03 18:07:56.955256 qiskit_qryd_provider-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      550 2023-12-03 18:07:56.963256 qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/__init__.py
--rw-r--r--   0        0        0     5082 2023-12-03 18:07:56.963256 qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/pcp_gate.py
--rw-r--r--   0        0        0     5434 2023-12-03 18:07:56.963256 qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/pcz_gate.py
--rw-r--r--   0        0        0    35013 2023-12-03 18:07:56.963256 qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/qryd_backend.py
--rw-r--r--   0        0        0    11276 2023-12-03 18:07:56.963256 qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/qryd_job.py
--rw-r--r--   0        0        0     5017 2023-12-03 18:07:56.963256 qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/qryd_provider.py
--rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 qiskit_qryd_provider-0.5.0/setup.py
--rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 qiskit_qryd_provider-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-22 23:06:50.738073 qiskit_qryd_provider-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3799 2024-04-22 23:06:50.730073 qiskit_qryd_provider-1.0.0/README.md
+-rw-r--r--   0        0        0     1082 2024-04-22 23:06:51.722086 qiskit_qryd_provider-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      500 2024-04-22 23:06:50.726073 qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/__init__.py
+-rw-r--r--   0        0        0     5082 2024-04-22 23:06:50.730073 qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/pcp_gate.py
+-rw-r--r--   0        0        0     5434 2024-04-22 23:06:50.730073 qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/pcz_gate.py
+-rw-r--r--   0        0        0    34207 2024-04-22 23:06:50.730073 qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/qryd_backend.py
+-rw-r--r--   0        0        0    11222 2024-04-22 23:06:50.726073 qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/qryd_job.py
+-rw-r--r--   0        0        0     4827 2024-04-22 23:06:50.730073 qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/qryd_provider.py
+-rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 qiskit_qryd_provider-1.0.0/PKG-INFO
```

### Comparing `qiskit_qryd_provider-0.5.0/LICENSE.txt` & `qiskit_qryd_provider-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_qryd_provider-0.5.0/README.md` & `qiskit_qryd_provider-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,27 +38,41 @@
 
 ```python
 backend = provider.get_backend("qryd_emulator$triangle")
 ```
 
 If you use these backends, the compilation of quantum circuits happens on our servers. The circuits are compiled to comply with the native gate set and connectivity of the Rydberg platform, using a decomposer developed by [HQS Quantum Simulations](https://quantumsimulations.de/).
 
-After selecting a backend, you can run a circuit on the backend:
+After selecting a backend, you can run a circuit on the backend, using the `transpile` function followed by `backend.run`:
 
 ```python
-from qiskit import QuantumCircuit, execute
+from qiskit import QuantumCircuit, transpile
 
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
-job = execute(qc, backend, shots=200)
+job = backend.run(transpile(qc, backend), shots=200)
 print(job.result().get_counts())
 ```
 
+Alternatively, you can use the `BackendSampler` primitive:
+
+```python
+from qiskit import QuantumCircuit
+from qiskit.primitives import BackendSampler
+
+qc = QuantumCircuit(2, 2)
+qc.h(0)
+qc.cx(0, 1)
+qc.measure([0, 1], [0, 1])
+job = BackendSampler(backend).run(qc, shots=200)
+print(job.result().quasi_dists[0])
+```
+
 ## Expert Options
 
 The provider adds the phase-shifted controlled-Z gate ([PCZGate](https://thequantumlaend.de/docs/gates.html#qiskit_qryd_provider.PCZGate)) and the phase-shifted controlled-phase gate ([PCPGate](https://thequantumlaend.de/docs/gates.html#qiskit_qryd_provider.PCPGate)) to Qiskit. These gates equal the controlled-Z/phase gates up to single-qubit phase gates. The gates can be realized by the Rydberg platform in multiple ways [[1](https://doi.org/10.1103/PhysRevLett.123.170503), [2](https://doi.org/10.1103/PhysRevResearch.4.033019), [3](https://doi.org/10.22331/q-2022-05-13-712)]. The value of the phase shift of the PCZGate can be modified before using the backend via:
 
 ```python
 from qiskit_qryd_provider import PCZGate
```

### Comparing `qiskit_qryd_provider-0.5.0/pyproject.toml` & `qiskit_qryd_provider-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "qiskit-qryd-provider"
-version = "0.5.0"
+version = "1.0.0"
 description = "Qiskit provider for accessing the emulator and future Rydberg quantum computer of the QRydDemo consortium"
 authors = ["Sebastian Weber"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://thequantumlaend.de/docs/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-qiskit-terra = ">=0.20"
+qiskit = ">=1.0"
 requests = ">=2.27"
 
 [tool.poetry.group.dev.dependencies]
-qiskit-aer = ">=0.10.3"
 pydot = "^1.4.2"
 pillow = "^9.1.0"
 pytest = "^7.1.1"
 pytest-sphinx = "^0.4.0"
 networkx = ">=2.6.3"
 numpy = ">=1.21.6"
 ipykernel = "^6.19.2"
 sphinx = "^5.0.2"
 sphinx-autobuild = "^2021.3.14"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autodoc-typehints = "^1.18.3"
 matplotlib = "^3.6.0"
 pylatexenc = "^2.10"
+qiskit-aer = "^0.14.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.skjold]
 sources = ["gemnasium"]
```

### Comparing `qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/pcp_gate.py` & `qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/pcp_gate.py`

 * *Files identical despite different names*

### Comparing `qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/pcz_gate.py` & `qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/pcz_gate.py`

 * *Files identical despite different names*

### Comparing `qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/qryd_backend.py` & `qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/qryd_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,29 +176,41 @@
             if value is not None:
                 setattr(self.options, key, value)
             else:
                 setattr(self.options, key, getattr(self._default_options(), key))
         else:
             raise NotImplementedError(f'"{key}" is not a valid option.')
 
-    def run(self, circuit: "qiskit.QuantumCircuit", **kwargs) -> QRydJob:
+    def run(
+        self,
+        circuit: Union["qiskit.QuantumCircuit", List["qiskit.QuantumCircuit"]],
+        **kwargs,
+    ) -> QRydJob:
         """Serialize a circuit, submit it to the backend, and create a job.
 
         This method will submit a simulation job and return a Job object that runs the
         circuit on QRydDemo's emulator. This is an async call so that running does not
         block the program.
 
         Args:
             circuit: A QuantumCircuit to run on the backend.
             **kwargs: Any kwarg options to pass to the backend.
 
         Returns:
             A job object.
 
+        Raises:
+            NotImplementedError: If `circuit` is a list with more than one circuit.
+
         """
+        if isinstance(circuit, list):
+            if len(circuit) != 1:
+                raise NotImplementedError("Only a single circuit is supported.")
+            circuit = circuit[0]
+
         for kwarg in kwargs:
             if not hasattr(self.options, kwarg):
                 warnings.warn(
                     "Option %s is not used by this backend." % kwarg,
                     UserWarning,
                     stacklevel=2,
                 )
@@ -751,25 +763,25 @@
     circuits to QRydDemo's infrastructure.
 
     Typical usage example:
 
     .. testcode::
 
         from qiskit_qryd_provider import QRydProvider
-        from qiskit import QuantumCircuit, execute
+        from qiskit import QuantumCircuit, transpile
         import os
 
         provider = QRydProvider(os.getenv("QRYD_API_TOKEN"))
         backend = provider.get_backend("qryd_emulator$square")
 
         qc = QuantumCircuit(2, 2)
         qc.h(0)
         qc.cx(0, 1)
         qc.measure([0, 1], [0, 1])
-        job = execute(qc, backend, shots=200)
+        job = backend.run(transpile(qc, backend), shots=200)
 
     """
 
     def __init__(self, provider: "qiskit_qryd_provider.QRydProvider") -> None:
         """Initialize the backend.
 
         Args:
@@ -804,25 +816,25 @@
     circuits to QRydDemo's infrastructure.
 
     Typical usage example:
 
     .. testcode::
 
         from qiskit_qryd_provider import QRydProvider
-        from qiskit import QuantumCircuit, execute
+        from qiskit import QuantumCircuit, transpile
         import os
 
         provider = QRydProvider(os.getenv("QRYD_API_TOKEN"))
         backend = provider.get_backend("qryd_emulator$triangle")
 
         qc = QuantumCircuit(2, 2)
         qc.h(0)
         qc.cx(0, 1)
         qc.measure([0, 1], [0, 1])
-        job = execute(qc, backend, shots=200)
+        job = backend.run(transpile(qc, backend), shots=200)
 
     """
 
     def __init__(self, provider: "qiskit_qryd_provider.QRydProvider") -> None:
         """Initialize the backend.
 
         Args:
@@ -844,109 +856,59 @@
             if q1 != q2
         ]
 
         # Create target with instructions
         self._create_target(num_qubits, edges)
 
 
-class QecEmulator(QRydBackend):
+class NoisyEmulatorTriangle(QRydBackend):
     """Backend for accessing a specific emulator.
 
-    The emulator is currently under development and aims to simulates
-    *16 qubits* with *all-to-all connectivity* and
-    simple noise models. This emulator is useful for studying quantum error
+    The emulator is currently under development and aims to simulate
+    up to *16 qubits* arranged in a *triangle lattice* with
+    nearest-neighbor connectivity and simple noise models.
+    This emulator is useful for studying quantum error
     correction codes.
 
     Typical usage example:
 
     .. testcode::
 
         from qiskit_qryd_provider import QRydProvider
-        from qiskit import QuantumCircuit, execute
+        from qiskit import QuantumCircuit, transpile
         import os
 
         provider = QRydProvider(os.getenv("QRYD_API_TOKEN"))
-        backend = provider.get_backend("qec_emulator")
+        backend = provider.get_backend("noisy_emulator$triangle")
 
         qc = QuantumCircuit(2, 2)
         qc.h(0)
         qc.cx(0, 1)
         qc.measure([0, 1], [0, 1])
-        job = execute(qc, backend, shots=200, allow_compilation=False)
+        job = backend.run(transpile(qc, backend), shots=200, allow_compilation=True)
 
     """
 
     def __init__(self, provider: "qiskit_qryd_provider.QRydProvider") -> None:
         """Initialize the backend.
 
         Args:
             provider: The provider that this backend comes from.
 
         """
         super().__init__(
             provider=provider,
-            name="qec_emulator",
+            name="noisy_emulator$triangle",
             backend_version="1.0.0",
         )
 
         num_qubits = 16
 
         # Calculate edges
         edges = [
             (q1, q2)
             for q1, q2 in product(range(num_qubits), range(num_qubits))
             if q1 != q2
         ]
-
-        # Create target with instructions
-        self._create_target(num_qubits, edges)
-
-
-class IdealEmulator(QRydBackend):
-    """Backend for accessing a specific emulator.
-
-    The emulator simulates *33 ideal qubits* with *all-to-all connectivity*. This
-    emulator is optimized for speed.
-
-    Typical usage example:
-
-    .. testcode::
-
-        from qiskit_qryd_provider import QRydProvider
-        from qiskit import QuantumCircuit, execute
-        import os
-
-        provider = QRydProvider(os.getenv("QRYD_API_TOKEN"))
-        backend = provider.get_backend("ideal_emulator")
-
-        qc = QuantumCircuit(2, 2)
-        qc.h(0)
-        qc.cx(0, 1)
-        qc.measure([0, 1], [0, 1])
-        job = execute(qc, backend, shots=200)
-
-    """
-
-    def __init__(self, provider: "qiskit_qryd_provider.QRydProvider") -> None:
-        """Initialize the backend.
-
-        Args:
-            provider: The provider that this backend comes from.
-
-        """
-        super().__init__(
-            provider=provider,
-            name="ideal_emulator",
-            backend_version="1.0.0",
-        )
-
-        num_qubits = 33
-
-        # Calculate edges
-        edges = [
-            (q1, q2)
-            for q1, q2 in product(range(num_qubits), range(num_qubits))
-            if q1 != q2
-        ]
 
         # Create target with instructions
         self._create_target(num_qubits, edges)
```

### Comparing `qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/qryd_job.py` & `qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/qryd_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     The job runs asynchronously.
 
     Typical usage example:
 
     .. testcode::
 
         from qiskit_qryd_provider import QRydProvider
-        from qiskit import QuantumCircuit, execute
+        from qiskit import QuantumCircuit, transpile
         import os
 
         provider = QRydProvider(os.getenv("QRYD_API_TOKEN"))
         backend = provider.get_backend("qryd_emulator$square")
 
         qc = QuantumCircuit(2, 2)
         qc.h(0)
         qc.cx(0, 1)
         qc.measure([0, 1], [0, 1])
-        job = execute(qc, backend, shots=200)
+        job = backend.run(transpile(qc, backend), shots=200)
 
         print(job.result().get_counts())
 
     .. testoutput::
         :hide:
 
         ...
@@ -79,16 +79,15 @@
         self._memory = options.memory
         self._shots = options.shots
 
     def submit(self) -> None:
         """Not implemented.
 
         Please use :func:`QRydSimulator.run()
-        <qiskit_qryd_provider.QRydSimulator.run>` or
-        :external+qiskit:py:func:`~qiskit.execute_function.execute` to submit a job.
+        <qiskit_qryd_provider.QRydSimulator.run>` to submit a job.
 
         Raises:
             NotImplementedError: If the method is called.
 
         """
         raise NotImplementedError("Please use QRydSimulator.run() to submit a job.")
```

### Comparing `qiskit_qryd_provider-0.5.0/qiskit_qryd_provider/qryd_provider.py` & `qiskit_qryd_provider-1.0.0/qiskit_qryd_provider/qryd_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List
 
 import requests
 from qiskit.providers import ProviderV1 as Provider
 from qiskit.providers import QiskitBackendNotFoundError
 from qiskit.providers.providerutils import filter_backends
 
-from qiskit_qryd_provider.qryd_backend import IdealEmulator
-from qiskit_qryd_provider.qryd_backend import QecEmulator
+from qiskit_qryd_provider.qryd_backend import NoisyEmulatorTriangle
 from qiskit_qryd_provider.qryd_backend import QRydBackend
 from qiskit_qryd_provider.qryd_backend import QRydEmulatorSquare
 from qiskit_qryd_provider.qryd_backend import QRydEmulatorTriangle
 
 
 class QRydProvider(Provider):
     """Provider for backends from the `QRydDemo`_ consortium.
@@ -34,22 +33,20 @@
       infrastructure.
     * :class:`~qiskit_qryd_provider.QRydEmulatorTriangle`:
       emulator of 30 ideal qubits arranged in a triangle lattice with
       nearest-neighbor connectivity, quantum circuits are compiled to the gate set of
       the Rydberg platform on our servers after submitting the circuits to QRydDemo's
       infrastructure.
 
-    In addition, the following backends are provided that are platform-agnostic and
-    serve special purposes:
+    In addition, the following backends are provided that serve special purposes:
 
-    * :class:`~qiskit_qryd_provider.QecEmulator`:
-      emulator of 16 qubits with all-to-all connectivity and simple noise models,
+    * :class:`~qiskit_qryd_provider.NoisyEmulatorTriangle`:
+      emulator of up to 16 qubits arranged in a triangle lattice with
+      nearest-neighbor connectivity and simple noise models,
       useful for studying quantum error correction codes. Under development.
-    * :class:`~qiskit_qryd_provider.IdealEmulator`:
-      emulator of 33 ideal qubits with all-to-all connectivity, optimized for speed.
 
     Typical usage example:
 
     .. testcode::
 
         from qiskit_qryd_provider import QRydProvider
         import os
@@ -117,13 +114,12 @@
         Returns:
             A list of backends that match the filtering criteria.
 
         """
         backends = [
             QRydEmulatorSquare(provider=self),
             QRydEmulatorTriangle(provider=self),
-            QecEmulator(provider=self),
-            IdealEmulator(provider=self),
+            NoisyEmulatorTriangle(provider=self),
         ]  # type: List[QRydBackend]
         if name:
             backends = [backend for backend in backends if backend.name == name]
         return filter_backends(backends, **kwargs)
```

### Comparing `qiskit_qryd_provider-0.5.0/PKG-INFO` & `qiskit_qryd_provider-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: qiskit-qryd-provider
-Version: 0.5.0
+Version: 1.0.0
 Summary: Qiskit provider for accessing the emulator and future Rydberg quantum computer of the QRydDemo consortium
 License: Apache-2.0
 Author: Sebastian Weber
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: qiskit-terra (>=0.20)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: qiskit (>=1.0)
 Requires-Dist: requests (>=2.27)
 Project-URL: Documentation, https://thequantumlaend.de/docs/
 Description-Content-Type: text/markdown
 
 # Qiskit QRyd Provider
 
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/qiskit_qryd_provider.svg?color=blue)
@@ -56,27 +57,41 @@
 
 ```python
 backend = provider.get_backend("qryd_emulator$triangle")
 ```
 
 If you use these backends, the compilation of quantum circuits happens on our servers. The circuits are compiled to comply with the native gate set and connectivity of the Rydberg platform, using a decomposer developed by [HQS Quantum Simulations](https://quantumsimulations.de/).
 
-After selecting a backend, you can run a circuit on the backend:
+After selecting a backend, you can run a circuit on the backend, using the `transpile` function followed by `backend.run`:
 
 ```python
-from qiskit import QuantumCircuit, execute
+from qiskit import QuantumCircuit, transpile
 
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
-job = execute(qc, backend, shots=200)
+job = backend.run(transpile(qc, backend), shots=200)
 print(job.result().get_counts())
 ```
 
+Alternatively, you can use the `BackendSampler` primitive:
+
+```python
+from qiskit import QuantumCircuit
+from qiskit.primitives import BackendSampler
+
+qc = QuantumCircuit(2, 2)
+qc.h(0)
+qc.cx(0, 1)
+qc.measure([0, 1], [0, 1])
+job = BackendSampler(backend).run(qc, shots=200)
+print(job.result().quasi_dists[0])
+```
+
 ## Expert Options
 
 The provider adds the phase-shifted controlled-Z gate ([PCZGate](https://thequantumlaend.de/docs/gates.html#qiskit_qryd_provider.PCZGate)) and the phase-shifted controlled-phase gate ([PCPGate](https://thequantumlaend.de/docs/gates.html#qiskit_qryd_provider.PCPGate)) to Qiskit. These gates equal the controlled-Z/phase gates up to single-qubit phase gates. The gates can be realized by the Rydberg platform in multiple ways [[1](https://doi.org/10.1103/PhysRevLett.123.170503), [2](https://doi.org/10.1103/PhysRevResearch.4.033019), [3](https://doi.org/10.22331/q-2022-05-13-712)]. The value of the phase shift of the PCZGate can be modified before using the backend via:
 
 ```python
 from qiskit_qryd_provider import PCZGate
```

