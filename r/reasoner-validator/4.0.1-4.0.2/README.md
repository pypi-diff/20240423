# Comparing `tmp/reasoner_validator-4.0.1.tar.gz` & `tmp/reasoner_validator-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.0.1.tar", max compression
+gzip compressed data, was "reasoner_validator-4.0.2.tar", max compression
```

## Comparing `reasoner_validator-4.0.1.tar` & `reasoner_validator-4.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/LICENSE
--rw-r--r--   0        0        0    13645 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/README.md
--rw-r--r--   0        0        0      131 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/conf.py
--rw-r--r--   0        0        0    20365 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/index.rst
--rw-r--r--   0        0        0      795 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/make.bat
--rw-r--r--   0        0        0      136 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    39468 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2937 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    85875 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    43025 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/message.py
--rw-r--r--   0        0        0    46755 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    14288 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35564 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/validator.py
--rw-r--r--   0        0        0    11943 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      838 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     2407 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/conftest.py
--rw-r--r--   0        0        0   138310 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41247 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    27195 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_validation_report.py
--rw-r--r--   0        0        0     2734 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_workflows.py
--rw-r--r--   0        0        0    15951 1970-01-01 00:00:00.000000 reasoner_validator-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-04-23 02:28:42.039440 reasoner_validator-4.0.2/LICENSE
+-rw-r--r--   0        0        0    13645 2024-04-23 02:28:42.039440 reasoner_validator-4.0.2/README.md
+-rw-r--r--   0        0        0      131 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/conf.py
+-rw-r--r--   0        0        0    20365 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    39468 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2963 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    85875 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    43025 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46755 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    14288 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35564 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    11943 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      838 2024-04-23 02:28:42.043440 reasoner_validator-4.0.2/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     2407 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/conftest.py
+-rw-r--r--   0        0        0   138310 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41247 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    27195 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2734 2024-04-23 02:28:42.047441 reasoner_validator-4.0.2/tests/test_workflows.py
+-rw-r--r--   0        0        0    15948 1970-01-01 00:00:00.000000 reasoner_validator-4.0.2/PKG-INFO
```

### Comparing `reasoner_validator-4.0.1/LICENSE` & `reasoner_validator-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/README.md` & `reasoner_validator-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/docs/Makefile` & `reasoner_validator-4.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/docs/conf.py` & `reasoner_validator-4.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/docs/index.rst` & `reasoner_validator-4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/docs/make.bat` & `reasoner_validator-4.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/docs/validation_codes_dictionary.md` & `reasoner_validator-4.0.2/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/pyproject.toml` & `reasoner_validator-4.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.0.1"
+version = "4.0.2"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -36,17 +36,18 @@
 
 include = [
     { path = "tests" },
     { path = "docs" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-bmt = "^1.1.4"
+python = "^3.10"
+bmt = "^1.4.0"
 #bmt = { git = "https://github.com/biolink/biolink-model-toolkit.git" }
+bioregistry = "^0.11.1"
 
 # jsonschema needs to be pinned to <= 4.18.0 for now,
 # since 4.18.0 appeared to break something for the
 # access and processing of JSON schemata
 jsonschema = "~4.17.3"
 dictdiffer = "^0.9.0"
 PyYAML = "^6.0"
@@ -69,14 +70,15 @@
 # exporting traces for jaeger
 opentelemetry-exporter-otlp-proto-http = {version = "*", optional = true}
 
 # instrumentation for fast api and httpx
 opentelemetry-instrumentation-fastapi = {version = "*", optional = true}
 opentelemetry-instrumentation-httpx = {version = "*", optional = true}
 
+
 [tool.poetry.urls]
 "Change Log" = "https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/NCATSTranslator/reasoner-validator/issues"
 
 [tool.poetry.extras]
 docs = ["numpydoc", "sphinx", "myst-parser", "sphinx-rtd-theme"]
 web = ["fastapi", "uvicorn", "httpx", "opentelemetry-exporter-otlp-proto-http", "opentelemetry-instrumentation-fastapi", "opentelemetry-instrumentation-httpx"]
```

### Comparing `reasoner_validator-4.0.1/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.0.2/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/codes.yaml` & `reasoner_validator-4.0.2/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/github.py` & `reasoner_validator-4.0.2/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/message.py` & `reasoner_validator-4.0.2/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/report.py` & `reasoner_validator-4.0.2/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/sri/util.py` & `reasoner_validator-4.0.2/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.0.2/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.0.2/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/validation_codes.py` & `reasoner_validator-4.0.2/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/validator.py` & `reasoner_validator-4.0.2/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/versioning.py` & `reasoner_validator-4.0.2/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/reasoner_validator/versions.yaml` & `reasoner_validator-4.0.2/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/__init__.py` & `reasoner_validator-4.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.0.2/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.0.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_response_validator.py` & `reasoner_validator-4.0.2/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_semver.py` & `reasoner_validator-4.0.2/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_trapi_versioning.py` & `reasoner_validator-4.0.2/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_validate.py` & `reasoner_validator-4.0.2/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_validation_report.py` & `reasoner_validator-4.0.2/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/tests/test_workflows.py` & `reasoner_validator-4.0.2/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.1/PKG-INFO` & `reasoner_validator-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.0.1
+Version: 4.0.2
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
 Maintainer-email: richard.bruskiewich@delphinai.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: docs
 Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: bmt (>=1.1.4,<2.0.0)
+Requires-Dist: bioregistry (>=0.11.1,<0.12.0)
+Requires-Dist: bmt (>=1.4.0,<2.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
 Requires-Dist: fastapi ; extra == "web"
 Requires-Dist: httpx (>=0.18.2,<0.19.0) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0) ; extra == "docs"
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http ; extra == "web"
```

