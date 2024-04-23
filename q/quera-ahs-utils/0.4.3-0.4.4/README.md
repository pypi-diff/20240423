# Comparing `tmp/quera-ahs-utils-0.4.3.tar.gz` & `tmp/quera_ahs_utils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quera-ahs-utils-0.4.3.tar", last modified: Tue Jun  6 15:53:42 2023, max compression
+gzip compressed data, was "quera_ahs_utils-0.4.4.tar", last modified: Tue Apr 23 18:41:19 2024, max compression
```

## Comparing `quera-ahs-utils-0.4.3.tar` & `quera_ahs_utils-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/quera_ahs_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 15:53:42.000000 quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:53:42.607094 quera-ahs-utils-0.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-06 15:52:54.000000 quera-ahs-utils-0.4.3/test/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:41:19.705712 quera_ahs_utils-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/src/quera_ahs_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/task_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/task_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-23 18:41:19.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-23 18:41:19.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:41:19.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 18:41:19.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 18:41:19.000000 quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:41:19.709712 quera_ahs_utils-0.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/test/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-23 18:40:36.000000 quera_ahs_utils-0.4.4/test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.4.3/LICENSE` & `quera_ahs_utils-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/PKG-INFO` & `quera_ahs_utils-0.4.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: amazon-braket-sdk
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pydantic>=2.0.0
+
+#  :warning: This Package is being Deprecated  :warning:
+
+Thank you for your interest in Aquila and AHS through braket! If you have found these tools useful we know you will love our new [Python SDK for Bloqade](https://github.com/QuEraComputing/bloqade-python). 
+
 
 # quera-ahs-utils
 This python package is a collection of tools that can be used to program QuEra's **neutral atom Analog Hamiltonian Simulator** (**ahs**). These tools are primarily targeted towards the usage of [Amazon's Braket quantum computing service](https://aws.amazon.com/braket/). The Braket Python SDK can be found [here](https://github.com/aws/amazon-braket-sdk-python) along with some examples of how to use their service through a collection of examples from both [Braket](https://github.com/aws/amazon-braket-examples/tree/main/examples/analog_hamiltonian_simulation) and [QuEra](https://github.com/QuEraComputing/QuEra-braket-examples).
 
 Some of the source code contained in this package originates from [this](https://github.com/aws/amazon-braket-examples/blob/main/examples/analog_hamiltonian_simulation/ahs_utils.py) module which was co-authered by the Braket science team.
 
 We would be remiss not to advertise our own [Julia](https://julialang.org/) SDK for programming QuEra's **ahs**, [Bloqade](https://queracomputing.github.io/Bloqade.jl/dev/) as well as modeling neutral atom quantum computing.
```

### Comparing `quera-ahs-utils-0.4.3/README.md` & `quera_ahs_utils-0.4.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#  :warning: This Package is being Deprecated  :warning:
+
+Thank you for your interest in Aquila and AHS through braket! If you have found these tools useful we know you will love our new [Python SDK for Bloqade](https://github.com/QuEraComputing/bloqade-python). 
+
+
 # quera-ahs-utils
 This python package is a collection of tools that can be used to program QuEra's **neutral atom Analog Hamiltonian Simulator** (**ahs**). These tools are primarily targeted towards the usage of [Amazon's Braket quantum computing service](https://aws.amazon.com/braket/). The Braket Python SDK can be found [here](https://github.com/aws/amazon-braket-sdk-python) along with some examples of how to use their service through a collection of examples from both [Braket](https://github.com/aws/amazon-braket-examples/tree/main/examples/analog_hamiltonian_simulation) and [QuEra](https://github.com/QuEraComputing/QuEra-braket-examples).
 
 Some of the source code contained in this package originates from [this](https://github.com/aws/amazon-braket-examples/blob/main/examples/analog_hamiltonian_simulation/ahs_utils.py) module which was co-authered by the Braket science team.
 
 We would be remiss not to advertise our own [Julia](https://julialang.org/) SDK for programming QuEra's **ahs**, [Bloqade](https://queracomputing.github.io/Bloqade.jl/dev/) as well as modeling neutral atom quantum computing.
```

### Comparing `quera-ahs-utils-0.4.3/pyproject.toml` & `quera_ahs_utils-0.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quera-ahs-utils"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 maintainers = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
@@ -22,15 +22,15 @@
 ]
 dependencies = [
   "amazon-braket-sdk",
   "networkx",
   "numpy",
   "scipy",
   "matplotlib",
-  "pydantic",
+  "pydantic>=2.0.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/QuEraComputing/quera-ahs-utils"
 "Bug Tracker" = "https://github.com/QuEraComputing/quera-ahs-utils/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/analysis.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/analysis.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/drive.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/ir.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/parallelize.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/plotting.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/capabilities.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/capabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 
 __all__ = ["QuEraCapabilities"]
 
 
 class RydbergGlobalCapabilities(BaseModel):
     rabi_frequency_min: float
     rabi_frequency_max: float
```

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_results.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/task_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from pydantic import BaseModel, conlist, conint
+from pydantic.v1 import BaseModel, conlist, conint
 from typing import Callable, Optional, List, Tuple
 import numpy as np
 
 __all__ = [
     "QuEraTaskResults",  
     "TaskProbabilities"  
 ]
```

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils/quera_ir/task_specification.py` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils/quera_ir/task_specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 from typing import Optional, List, Tuple, Union
 from decimal import Decimal
 
 from quera_ahs_utils.quera_ir.capabilities import QuEraCapabilities
 
 
 __all__ = [
@@ -151,18 +151,20 @@
         )
             
     
 class QuEraTaskSpecification(BaseModel):
     nshots: int
     lattice: Lattice
     effective_hamiltonian: EffectiveHamiltonian
+    metadata: Optional[str] = None
     
     def __hash__(self):
         return hash((QuEraTaskSpecification, self.nshots, self.lattice, self.effective_hamiltonian))
     
     def discretize(self, task_capabilities: QuEraCapabilities):
         return QuEraTaskSpecification(
             nshots = self.nshots,
             lattice = self.lattice.discretize(task_capabilities),
-            effective_hamiltonian = self.effective_hamiltonian.discretize(task_capabilities)
+            effective_hamiltonian = self.effective_hamiltonian.discretize(task_capabilities),
+            metadata=self.metadata,
         )
```

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/PKG-INFO` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: amazon-braket-sdk
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pydantic>=2.0.0
+
+#  :warning: This Package is being Deprecated  :warning:
+
+Thank you for your interest in Aquila and AHS through braket! If you have found these tools useful we know you will love our new [Python SDK for Bloqade](https://github.com/QuEraComputing/bloqade-python). 
+
 
 # quera-ahs-utils
 This python package is a collection of tools that can be used to program QuEra's **neutral atom Analog Hamiltonian Simulator** (**ahs**). These tools are primarily targeted towards the usage of [Amazon's Braket quantum computing service](https://aws.amazon.com/braket/). The Braket Python SDK can be found [here](https://github.com/aws/amazon-braket-sdk-python) along with some examples of how to use their service through a collection of examples from both [Braket](https://github.com/aws/amazon-braket-examples/tree/main/examples/analog_hamiltonian_simulation) and [QuEra](https://github.com/QuEraComputing/QuEra-braket-examples).
 
 Some of the source code contained in this package originates from [this](https://github.com/aws/amazon-braket-examples/blob/main/examples/analog_hamiltonian_simulation/ahs_utils.py) module which was co-authered by the Braket science team.
 
 We would be remiss not to advertise our own [Julia](https://julialang.org/) SDK for programming QuEra's **ahs**, [Bloqade](https://queracomputing.github.io/Bloqade.jl/dev/) as well as modeling neutral atom quantum computing.
```

### Comparing `quera-ahs-utils-0.4.3/src/quera_ahs_utils.egg-info/SOURCES.txt` & `quera_ahs_utils-0.4.4/src/quera_ahs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/test/test_drive.py` & `quera_ahs_utils-0.4.4/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/test/test_ir.py` & `quera_ahs_utils-0.4.4/test/test_ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/test/test_parallelize.py` & `quera_ahs_utils-0.4.4/test/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.3/test/test_plotting.py` & `quera_ahs_utils-0.4.4/test/test_plotting.py`

 * *Files identical despite different names*

