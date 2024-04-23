# Comparing `tmp/idc_index-0.5.1.tar.gz` & `tmp/idc_index-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr 13 01:32:19 2024, max compression
+gzip compressed data, last modified: Tue Apr 23 20:32:50 2024, max compression
```

## Comparing `idc_index-0.5.1.tar` & `idc_index-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      125 2024-04-13 01:32:19.000000 idc_index-0.5.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-13 01:32:19.000000 idc_index-0.5.1/.gitattributes
--rw-r--r--   0        0        0     2357 2024-04-13 01:32:19.000000 idc_index-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-13 01:32:19.000000 idc_index-0.5.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-04-13 01:32:19.000000 idc_index-0.5.1/noxfile.py
--rw-r--r--   0        0        0     2394 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1581 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-04-13 01:32:19.000000 idc_index-0.5.1/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-04-13 01:32:19.000000 idc_index-0.5.1/docs/conf.py
--rw-r--r--   0        0        0      196 2024-04-13 01:32:19.000000 idc_index-0.5.1/docs/index.md
--rw-r--r--   0        0        0      263 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/_version.pyi
--rw-r--r--   0        0        0    27954 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-04-13 01:32:19.000000 idc_index-0.5.1/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     3779 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-04-13 01:32:19.000000 idc_index-0.5.1/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-04-13 01:32:19.000000 idc_index-0.5.1/.gitignore
--rw-r--r--   0        0        0     1077 2024-04-13 01:32:19.000000 idc_index-0.5.1/LICENSE
--rw-r--r--   0        0        0     4290 2024-04-13 01:32:19.000000 idc_index-0.5.1/README.md
--rw-r--r--   0        0        0     6121 2024-04-13 01:32:19.000000 idc_index-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7531 2024-04-13 01:32:19.000000 idc_index-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-23 20:32:50.000000 idc_index-0.5.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-23 20:32:50.000000 idc_index-0.5.2/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-04-23 20:32:50.000000 idc_index-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-23 20:32:50.000000 idc_index-0.5.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-04-23 20:32:50.000000 idc_index-0.5.2/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1581 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-04-23 20:32:50.000000 idc_index-0.5.2/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-04-23 20:32:50.000000 idc_index-0.5.2/docs/index.md
+-rw-r--r--   0        0        0      263 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/_version.pyi
+-rw-r--r--   0        0        0    27954 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     3779 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      437 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-04-23 20:32:50.000000 idc_index-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1077 2024-04-23 20:32:50.000000 idc_index-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4290 2024-04-23 20:32:50.000000 idc_index-0.5.2/README.md
+-rw-r--r--   0        0        0     6121 2024-04-23 20:32:50.000000 idc_index-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7531 2024-04-23 20:32:50.000000 idc_index-0.5.2/PKG-INFO
```

### Comparing `idc_index-0.5.1/.pre-commit-config.yaml` & `idc_index-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/noxfile.py` & `idc_index-0.5.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/.github/CONTRIBUTING.md` & `idc_index-0.5.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/.github/matchers/pylint.json` & `idc_index-0.5.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/.github/workflows/cd.yml` & `idc_index-0.5.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/.github/workflows/ci.yml` & `idc_index-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/docs/conf.py` & `idc_index-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/idc_index/index.py` & `idc_index-0.5.2/idc_index/index.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/tests/idcindex.py` & `idc_index-0.5.2/tests/idcindex.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/.gitignore` & `idc_index-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/LICENSE` & `idc_index-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/README.md` & `idc_index-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.1/pyproject.toml` & `idc_index-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   'duckdb>=0.10.0',
-  "idc-index-data==18.0.0",
+  "idc-index-data==18.0.1",
   "packaging",
   "pandas<2.2",
   "psutil",
   "pyarrow",
   "s5cmd",
 ]
```

### Comparing `idc_index-0.5.1/PKG-INFO` & `idc_index-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: duckdb>=0.10.0
-Requires-Dist: idc-index-data==18.0.0
+Requires-Dist: idc-index-data==18.0.1
 Requires-Dist: packaging
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
 Requires-Dist: pyarrow
 Requires-Dist: s5cmd
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
```

