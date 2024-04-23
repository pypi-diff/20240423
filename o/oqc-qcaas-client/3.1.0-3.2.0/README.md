# Comparing `tmp/oqc_qcaas_client-3.1.0.tar.gz` & `tmp/oqc_qcaas_client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqc_qcaas_client-3.1.0.tar", max compression
+gzip compressed data, was "oqc_qcaas_client-3.2.0.tar", max compression
```

## Comparing `oqc_qcaas_client-3.1.0.tar` & `oqc_qcaas_client-3.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1453 2024-03-28 12:45:33.997614 oqc_qcaas_client-3.1.0/LICENSE
--rw-r--r--   0        0        0      350 2024-03-28 12:45:33.969615 oqc_qcaas_client-3.1.0/client/README.md
--rw-r--r--   0        0        0       89 2024-03-28 12:45:33.969615 oqc_qcaas_client-3.1.0/client/qcaas_client/__init__.py
--rw-r--r--   0        0        0    36050 2024-03-28 12:45:33.969615 oqc_qcaas_client-3.1.0/client/qcaas_client/client.py
--rw-r--r--   0        0        0     4981 2024-03-28 12:45:33.969615 oqc_qcaas_client-3.1.0/client/qcaas_client/commandline.py
--rw-r--r--   0        0        0      142 2024-03-28 12:45:33.969615 oqc_qcaas_client-3.1.0/client/qcaas_client/config.py
--rw-r--r--   0        0        0    16375 2024-03-28 12:45:33.973615 oqc_qcaas_client-3.1.0/client/scc/compiler/config.py
--rw-r--r--   0        0        0        0 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/__init__.py
--rw-r--r--   0        0        0      745 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/config.py
--rw-r--r--   0        0        0     3915 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/enums.py
--rw-r--r--   0        0        0      539 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/json_utils.py
--rw-r--r--   0        0        0      831 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/log_reduct.py
--rw-r--r--   0        0        0     3202 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/logger.py
--rw-r--r--   0        0        0     3368 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/metrics.py
--rw-r--r--   0        0        0     2207 2024-03-28 12:45:33.993615 oqc_qcaas_client-3.1.0/common/qcaas_common/type_conversions.py
--rw-r--r--   0        0        0     1827 2024-03-28 12:45:44.489517 oqc_qcaas_client-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 oqc_qcaas_client-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1453 2024-04-23 10:55:04.228104 oqc_qcaas_client-3.2.0/LICENSE
+-rw-r--r--   0        0        0      350 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/README.md
+-rw-r--r--   0        0        0       89 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/__init__.py
+-rw-r--r--   0        0        0    36050 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/client.py
+-rw-r--r--   0        0        0     4981 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/commandline.py
+-rw-r--r--   0        0        0      142 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/config.py
+-rw-r--r--   0        0        0    16377 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/scc/compiler/config.py
+-rw-r--r--   0        0        0        0 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/config.py
+-rw-r--r--   0        0        0     3915 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/enums.py
+-rw-r--r--   0        0        0      539 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/json_utils.py
+-rw-r--r--   0        0        0      831 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/log_reduct.py
+-rw-r--r--   0        0        0     3202 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/logger.py
+-rw-r--r--   0        0        0     3368 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/metrics.py
+-rw-r--r--   0        0        0     2207 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/type_conversions.py
+-rw-r--r--   0        0        0     1827 2024-04-23 10:55:12.878618 oqc_qcaas_client-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 oqc_qcaas_client-3.2.0/PKG-INFO
```

### Comparing `oqc_qcaas_client-3.1.0/LICENSE` & `oqc_qcaas_client-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/client/qcaas_client/client.py` & `oqc_qcaas_client-3.2.0/client/qcaas_client/client.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/client/qcaas_client/commandline.py` & `oqc_qcaas_client-3.2.0/client/qcaas_client/commandline.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/client/scc/compiler/config.py` & `oqc_qcaas_client-3.2.0/client/scc/compiler/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,17 @@
     def __repr__(self):
         return self.name
 
 
 class QuantumResultsFormat:
     def __init__(self):
         self.format: Optional[InlineResultsProcessing] = None
-        self.transforms: Optional[
-            ResultsFormatting
-        ] = ResultsFormatting.DynamicStructureReturn
+        self.transforms: Optional[ResultsFormatting] = (
+            ResultsFormatting.DynamicStructureReturn
+        )
 
     def raw(self) -> QuantumResultsFormat:
         self.format = InlineResultsProcessing.Raw
         return self
 
     def binary(self) -> QuantumResultsFormat:
         self.format = InlineResultsProcessing.Binary
```

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/config.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/config.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/enums.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/enums.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/json_utils.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/json_utils.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/log_reduct.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/log_reduct.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/logger.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/logger.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/metrics.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/metrics.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/common/qcaas_common/type_conversions.py` & `oqc_qcaas_client-3.2.0/common/qcaas_common/type_conversions.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.1.0/pyproject.toml` & `oqc_qcaas_client-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oqc_qcaas_client"
-version = "3.1.0"
+version = "3.2.0"
 description = "OQC Quantum Computing as a Service (QCaaS)"
 authors = [ "OQC <oqc_qcaas_support@oxfordquantumcircuits.com>",]
 readme = "client/README.md"
 exclude = [ ".env",]
 license = "BSD-3-Clause"
 source = []
 [[tool.poetry.packages]]
@@ -35,15 +35,15 @@
 toml = "0.10.2"
 pamqp = "2.3.0"
 attrs = "21.2.0"
 bidict = "0.23.1"
 certifi = "2024.2.2"
 charset-normalizer = "3.3.2"
 h11 = "0.14.0"
-idna = "3.6"
+idna = "3.7"
 markupsafe = "2.1.5"
 python-dotenv = "1.0.1"
 python-engineio = "4.9.0"
 python-socketio = "5.5.2"
 requests = "2.31.0"
 simple-websocket = "1.0.0"
 urllib3 = "2.2.1"
```

### Comparing `oqc_qcaas_client-3.1.0/PKG-INFO` & `oqc_qcaas_client-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oqc-qcaas-client
-Version: 3.1.0
+Name: oqc_qcaas_client
+Version: 3.2.0
 Summary: OQC Quantum Computing as a Service (QCaaS)
 License: BSD-3-Clause
 Author: OQC
 Author-email: oqc_qcaas_support@oxfordquantumcircuits.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: pip-licenses
 Requires-Dist: attrs (==21.2.0)
 Requires-Dist: bidict (==0.23.1)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: charset-normalizer (==3.3.2)
 Requires-Dist: h11 (==0.14.0)
-Requires-Dist: idna (==3.6)
+Requires-Dist: idna (==3.7)
 Requires-Dist: markupsafe (==2.1.5)
 Requires-Dist: pamqp (==2.3.0)
 Requires-Dist: pip-licenses (>=3.5.3,<4.0.0) ; extra == "pip-licenses"
 Requires-Dist: python-dotenv (==1.0.1)
 Requires-Dist: python-engineio (==4.9.0)
 Requires-Dist: python-socketio (==5.5.2)
 Requires-Dist: requests (==2.31.0)
```

