# Comparing `tmp/qiskit-ionq-0.5.1.tar.gz` & `tmp/qiskit-ionq-0.5.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ionq-0.5.1.tar", last modified: Tue Apr 23 16:58:03 2024, max compression
+gzip compressed data, was "qiskit-ionq-0.5.1.dev0.tar", last modified: Fri Apr 12 19:37:12 2024, max compression
```

## Comparing `qiskit-ionq-0.5.1.tar` & `qiskit-ionq-0.5.1.dev0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.856700 qiskit-ionq-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.852700 qiskit-ionq-0.5.1/.eggs/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 16:58:02.000000 qiskit-ionq-0.5.1/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.848700 qiskit-ionq-0.5.1/.eggs/pytest_runner-6.0.1-py3.11.egg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.852700 qiskit-ionq-0.5.1/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-23 16:58:03.856700 qiskit-ionq-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.852700 qiskit-ionq-0.5.1/qiskit_ionq/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_equivalence_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/ionq_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/qiskit_ionq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.856700 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 16:58:03.000000 qiskit-ionq-0.5.1/qiskit_ionq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 16:58:03.856700 qiskit-ionq-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:58:03.856700 qiskit-ionq-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-23 16:57:44.000000 qiskit-ionq-0.5.1/test/test_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.409914 qiskit-ionq-0.5.1.dev0/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 19:37:11.000000 qiskit-ionq-0.5.1.dev0/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.405914 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.409914 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.409914 qiskit-ionq-0.5.1.dev0/qiskit_ionq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/test/test_mock.py
```

### Comparing `qiskit-ionq-0.5.1/LICENSE.txt` & `qiskit-ionq-0.5.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/PKG-INFO` & `qiskit-ionq-0.5.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.5.1
+Version: 0.5.1.dev0
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
```

### Comparing `qiskit-ionq-0.5.1/README.md` & `qiskit-ionq-0.5.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/__init__.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,8 +36,7 @@
         "Qiskit is not installed. Please install the latest version of Qiskit."
     ) from exc
 
 from .ionq_provider import IonQProvider
 from .version import __version__
 from .ionq_gates import GPIGate, GPI2Gate, MSGate, ZZGate
 from .constants import ErrorMitigation
-from .ionq_equivalence_library import add_equivalences
```

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/constants.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/exceptions.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/helpers.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/helpers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/ionq_backend.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import warnings
 
 from qiskit.providers import BackendV1 as Backend
 from qiskit.providers.models import BackendConfiguration
 from qiskit.providers.models.backendstatus import BackendStatus
 from qiskit.providers import Options
 
-from . import exceptions, ionq_client, ionq_job, ionq_equivalence_library
+from . import exceptions, ionq_client, ionq_job
 from .helpers import GATESET_MAP
 
 
 class Calibration:
     """
     IonQ backend calibration data.
 
@@ -128,19 +128,14 @@
 
 
 class IonQBackend(Backend):
     """IonQ Backend base class."""
 
     _client = None
 
-    def __init__(self, *args, **kwargs):
-        # Add IonQ equivalences
-        ionq_equivalence_library.add_equivalences()
-        super().__init__(*args, **kwargs)
-
     @classmethod
     def _default_options(cls):
         return Options(
             shots=1024,
             job_settings=None,
             error_mitigation=None,
             extra_query_params={},
```

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/ionq_client.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/ionq_gates.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/ionq_job.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/ionq_provider.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/ionq_result.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq/version.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import pathlib
 import subprocess
 from typing import List
 
 pkg_parent = pathlib.Path(__file__).parent.parent.absolute()
 
 # major, minor, patch
-VERSION_INFO = ".".join(map(str, (0, 5, 1)))
+VERSION_INFO = ".".join(map(str, (0, 5, 1, "dev0")))
 
 
 def _minimal_ext_cmd(cmd: List[str]) -> bytes:
     # construct minimal environment
     env = {
         "LANGUAGE": "C",  # LANGUAGE is used on win32
         "LANG": "C",
```

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq.egg-info/PKG-INFO` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.5.1
+Version: 0.5.1.dev0
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
```

### Comparing `qiskit-ionq-0.5.1/qiskit_ionq.egg-info/SOURCES.txt` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 ./qiskit_ionq.egg-info/top_level.txt
 qiskit_ionq/__init__.py
 qiskit_ionq/constants.py
 qiskit_ionq/exceptions.py
 qiskit_ionq/helpers.py
 qiskit_ionq/ionq_backend.py
 qiskit_ionq/ionq_client.py
-qiskit_ionq/ionq_equivalence_library.py
 qiskit_ionq/ionq_gates.py
 qiskit_ionq/ionq_job.py
 qiskit_ionq/ionq_provider.py
 qiskit_ionq/ionq_result.py
 qiskit_ionq/version.py
 qiskit_ionq.egg-info/PKG-INFO
 qiskit_ionq.egg-info/SOURCES.txt
```

### Comparing `qiskit-ionq-0.5.1/setup.py` & `qiskit-ionq-0.5.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/test/test_exceptions.py` & `qiskit-ionq-0.5.1.dev0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.1/test/test_mock.py` & `qiskit-ionq-0.5.1.dev0/test/test_mock.py`

 * *Files identical despite different names*

