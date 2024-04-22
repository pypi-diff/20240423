# Comparing `tmp/infrasys-0.0.2.tar.gz` & `tmp/infrasys-0.0.3.tar.gz`

## Comparing `infrasys-0.0.2.tar` & `infrasys-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,62 @@
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 infrasys-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 infrasys-0.0.2/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 infrasys-0.0.2/.github/workflows/conda_build.yml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 infrasys-0.0.2/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 infrasys-0.0.2/.github/workflows/main_tests.yml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 infrasys-0.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 infrasys-0.0.2/.github/workflows/pull_request_tests.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/Makefile
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/conf.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/make.bat
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/explanation/components.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/explanation/index.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/explanation/location.md
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/explanation/serialization.md
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/explanation/system.md
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/explanation/time_series.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/how_tos/index.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/how_tos/list_time_series.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/index.md
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/system_json.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/api/components.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/api/index.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/api/location.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/api/quantities.md
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/api/system.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/reference/api/time_series.md
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/tutorials/custom_system.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 infrasys-0.0.2/docs/tutorials/index.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/__init__.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/arrow_storage.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/base_quantity.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/common.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/component.py
--rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/component_manager.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/exceptions.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/in_memory_time_series_storage.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/location.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/loggers.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/models.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/normalization.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/parquet_time_series_storage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/py.typed
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/quantities.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/serialization.py
--rw-r--r--   0        0        0    44900 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/system.py
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/time_series_manager.py
--rw-r--r--   0        0        0    21779 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/time_series_metadata_store.py
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/time_series_models.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/time_series_storage_base.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 infrasys-0.0.2/src/infrasys/utils/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/test_arrow_storage.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/test_json.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/test_normalization.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/test_serialization.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/test_single_time_series.py
--rw-r--r--   0        0        0    24907 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/test_system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/models/__init__.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 infrasys-0.0.2/tests/models/simple_system.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 infrasys-0.0.2/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 infrasys-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 infrasys-0.0.2/README.md
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 infrasys-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 infrasys-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 infrasys-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 infrasys-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 infrasys-0.0.3/.github/workflows/conda_build.yml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 infrasys-0.0.3/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 infrasys-0.0.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/explanation/components.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/explanation/index.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/explanation/location.md
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/explanation/serialization.md
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/explanation/system.md
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/explanation/time_series.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/how_tos/index.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/how_tos/list_time_series.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/index.md
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/system_json.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/api/components.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/api/index.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/api/location.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/api/quantities.md
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/api/system.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/reference/api/time_series.md
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/tutorials/custom_system.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 infrasys-0.0.3/docs/tutorials/index.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/__init__.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/arrow_storage.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/base_quantity.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/common.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/component.py
+-rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/component_manager.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/exceptions.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/in_memory_time_series_storage.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/location.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/loggers.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/models.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/normalization.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/parquet_time_series_storage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/py.typed
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/quantities.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/serialization.py
+-rw-r--r--   0        0        0    44823 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/system.py
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/time_series_manager.py
+-rw-r--r--   0        0        0    21779 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/time_series_metadata_store.py
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/time_series_models.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 infrasys-0.0.3/src/infrasys/time_series_storage_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/test_arrow_storage.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/test_normalization.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/test_serialization.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/test_single_time_series.py
+-rw-r--r--   0        0        0    24907 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/test_system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/models/__init__.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 infrasys-0.0.3/tests/models/simple_system.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 infrasys-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 infrasys-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 infrasys-0.0.3/README.md
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 infrasys-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 infrasys-0.0.3/PKG-INFO
```

### Comparing `infrasys-0.0.2/.github/workflows/conda_build.yml` & `infrasys-0.0.3/.github/workflows/conda_build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     types: [published]
 
 jobs:
   build:
     name: Conda
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - uses: conda-incubator/setup-miniconda@v2
       with:
         auto-update-conda: true
         python-version: 3.11
     - name: Build and upload conda package
       shell: bash -l {0}
       env:
```

### Comparing `infrasys-0.0.2/.github/workflows/gh-pages.yml` & `infrasys-0.0.3/.github/workflows/gh-pages.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   push:
     branches: [main]
 
 jobs:
   make-pages:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - name: select python version
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - name: install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install ".[dev]"
       - name: build documentation
```

### Comparing `infrasys-0.0.2/.github/workflows/main_tests.yml` & `infrasys-0.0.3/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-name: Main - CI
+name: CI
 
 on:
-  schedule:
-  - cron: "0 0 * * 1-5"
   push:
     branches:
       - main
+  pull_request:
 
 jobs:
-  test:
-    runs-on: ubuntu-latest
+  pytest:
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.11", "3.12"]
+        os: [ubuntu-latest, windows-latest]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install ".[dev]"
-    - name: Run pytest
+    - name: Run pytest with coverage
       run: |
-        python -m pytest -v --disable-warnings tests
+        pytest -v --cov --cov-report=xml
+    - name: codecov
+      uses: codecov/codecov-action@v4.2.0
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
+        name: infrasys-tests
+        fail_ci_if_error: false
+        verbose: true
   mypy:
     runs-on: ubuntu-latest
     name: "mypy"
     steps:
       - uses: davidslusser/actions_python_mypy@v1.0.0
         with:
           src: "src"
```

### Comparing `infrasys-0.0.2/.github/workflows/publish_to_pypi.yml` & `infrasys-0.0.3/.github/workflows/publish_to_pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [published]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: 3.11
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
         pip install setuptools wheel twine
```

### Comparing `infrasys-0.0.2/docs/Makefile` & `infrasys-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/conf.py` & `infrasys-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/index.md` & `infrasys-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/make.bat` & `infrasys-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/explanation/components.md` & `infrasys-0.0.3/docs/explanation/components.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/explanation/serialization.md` & `infrasys-0.0.3/docs/explanation/serialization.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/explanation/system.md` & `infrasys-0.0.3/docs/explanation/system.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/explanation/time_series.md` & `infrasys-0.0.3/docs/explanation/time_series.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/how_tos/list_time_series.md` & `infrasys-0.0.3/docs/how_tos/list_time_series.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/reference/system_json.md` & `infrasys-0.0.3/docs/reference/system_json.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/docs/tutorials/custom_system.md` & `infrasys-0.0.3/docs/tutorials/custom_system.md`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/arrow_storage.py` & `infrasys-0.0.3/src/infrasys/arrow_storage.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/base_quantity.py` & `infrasys-0.0.3/src/infrasys/base_quantity.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/component.py` & `infrasys-0.0.3/src/infrasys/component.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,19 @@
     name: Annotated[str, Field(frozen=True)]
 
     def check_component_addition(self) -> None:
         """Perform checks on the component before adding it to a system."""
 
     def model_dump_custom(self, *args, **kwargs) -> dict[str, Any]:
         """Custom serialization for this package"""
-        refs = {x: self._model_dump_field(x) for x in self.model_fields}
+        refs = {}
+        for x in self.model_fields:
+            val = self._model_dump_field(x)
+            if val is not None:
+                refs[x] = val
         exclude = kwargs.get("exclude", [])
         exclude += list(set(exclude).union(refs))
         kwargs["exclude"] = exclude
         data = serialize_value(self, *args, **kwargs)
         data.update(refs)
         return data
 
@@ -48,14 +52,16 @@
             data[TYPE_METADATA] = SerializedTypeMetadata(
                 fields=SerializedQuantityType(
                     module=val.__module__,
                     type=val.__class__.__name__,
                 ),
             ).model_dump()
             val = data
+        else:
+            val = None
         # TODO: other composite types may need handling.
         # Parent packages can always implement a field_serializer themselves.
         return val
 
     def pprint(self):
         return _pprint(self)
```

### Comparing `infrasys-0.0.2/src/infrasys/component_manager.py` & `infrasys-0.0.3/src/infrasys/component_manager.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/exceptions.py` & `infrasys-0.0.3/src/infrasys/exceptions.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/in_memory_time_series_storage.py` & `infrasys-0.0.3/src/infrasys/in_memory_time_series_storage.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/loggers.py` & `infrasys-0.0.3/src/infrasys/loggers.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/models.py` & `infrasys-0.0.3/src/infrasys/models.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/normalization.py` & `infrasys-0.0.3/src/infrasys/normalization.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/parquet_time_series_storage.py` & `infrasys-0.0.3/src/infrasys/parquet_time_series_storage.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/quantities.py` & `infrasys-0.0.3/src/infrasys/quantities.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/serialization.py` & `infrasys-0.0.3/src/infrasys/serialization.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/system.py` & `infrasys-0.0.3/src/infrasys/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     SerializedComponentReference,
     SerializedQuantityType,
     SerializedType,
     TYPE_METADATA,
 )
 from infrasys.time_series_manager import TimeSeriesManager, TIME_SERIES_KWARGS
 from infrasys.time_series_models import SingleTimeSeries, TimeSeriesData, TimeSeriesMetadata
-from infrasys.utils.json import ExtendedJSONEncoder
 
 
 class System:
     """Implements behavior for systems"""
 
     def __init__(
         self,
@@ -153,15 +152,15 @@
         if data is None:
             data = system_data
         else:
             if "system" in data:
                 raise ISConflictingArguments("data contains the key 'system'")
             data["system"] = system_data
         with open(filename, "w", encoding="utf-8") as f_out:
-            json.dump(data, f_out, indent=indent, cls=ExtendedJSONEncoder)
+            json.dump(data, f_out, indent=indent)
             logger.info("Wrote system data to {}", filename)
 
         self._time_series_mgr.serialize(self._make_time_series_directory(filename))
 
     @classmethod
     def from_json(
         cls, filename: Path | str, upgrade_handler: Callable | None = None, **kwargs
```

### Comparing `infrasys-0.0.2/src/infrasys/time_series_manager.py` & `infrasys-0.0.3/src/infrasys/time_series_manager.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/time_series_metadata_store.py` & `infrasys-0.0.3/src/infrasys/time_series_metadata_store.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/time_series_models.py` & `infrasys-0.0.3/src/infrasys/time_series_models.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/src/infrasys/time_series_storage_base.py` & `infrasys-0.0.3/src/infrasys/time_series_storage_base.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/conftest.py` & `infrasys-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/test_arrow_storage.py` & `infrasys-0.0.3/tests/test_arrow_storage.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/test_normalization.py` & `infrasys-0.0.3/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/test_serialization.py` & `infrasys-0.0.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/test_single_time_series.py` & `infrasys-0.0.3/tests/test_single_time_series.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/test_system.py` & `infrasys-0.0.3/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/tests/models/simple_system.py` & `infrasys-0.0.3/tests/models/simple_system.py`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/.gitignore` & `infrasys-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `infrasys-0.0.2/LICENSE.txt` & `infrasys-0.0.3/LICENSE.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Alliance for Sustainable Energy LLC, All rights reserved.
+Copyright (c) 2024, Alliance for Sustainable Energy LLC, All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `infrasys-0.0.2/README.md` & `infrasys-0.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # infrasys
 
-[![Main - CI](https://github.com/NREL/infrasys/workflows/Main%20-%20CI/badge.svg)](https://github.com/NREL/infrasys/actions/workflows/main_tests.yml)
+[![CI](https://github.com/NREL/infrasys/workflows/CI/badge.svg)](https://github.com/NREL/infrasys/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/NREL/infrasys/branch/main/graph/badge.svg)](https://codecov.io/gh/NREL/infrasys)
 
 This package implements a data store for components and time series in support of Python-based
 modeling packages. While it is designed to support teams modeling transmission and distribution
 systems for electrical grids, it can be used by any package that needs to store components
 (e.g., generators and buses) that have quantities (e.g., power and voltage) which may vary over
 time.
@@ -35,7 +35,14 @@
 $ pip install -e ".[dev]"
 ```
 
 Please install `pre-commit` so that your code is checked before making commits.
 ```
 $ pre-commit install
 ```
+
+## License
+infrasys is released under a BSD 3-Clause
+[License](https://github.com/NREL/infrasys/blob/main/LICENSE.txt).
+
+infrasys was developed under software record SWR-24-42 at the National Renewable Energy Laboratory
+([NREL](https://www.nrel.gov)).
```

### Comparing `infrasys-0.0.2/pyproject.toml` & `infrasys-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "infrasys"
-version = "0.0.2"
+version = "0.0.3"
 description = ''
 readme = "README.md"
 requires-python = ">=3.10, <3.13"
 license = "BSD-3-Clause"
 keywords = []
 authors = [
-  { name = "Aadil Latif", email = "aadil.latif@nrel.gov" },
-  { name = "Daniel Thom", email = "daniel.thom@nrel.gov" },
-  { name = "Kapil Duwadi", email = "kapil.duwadi@nrel.gov" },
-  { name = "Pedro Andres Sanchez Perez", email = "pedroandres.sanchezperez@nrel.gov" },
-  { name = "Tarek Elgindy", email = "tarek.elgindy@nrel.gov" },
+    { name = "Aadil Latif", email = "aadil.latif@nrel.gov" },
+    { name = "Daniel Thom", email = "daniel.thom@nrel.gov" },
+    { name = "Kapil Duwadi", email = "kapil.duwadi@nrel.gov" },
+    { name = "Pedro Andres Sanchez Perez", email = "pedroandres.sanchezperez@nrel.gov" },
+    { name = "Tarek Elgindy", email = "tarek.elgindy@nrel.gov" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "numpy",
-    "pyarrow",
-    "pint",
-    "loguru",
-    "rich",
+    "numpy~=1.26.4",
+    "pyarrow~=15.0.2",
+    "pint~=0.23",
+    "loguru~=0.7.2",
+    "rich~=13.7.1",
     "pydantic >= 2.4, <= 3",
 ]
 [project.optional-dependencies]
 dev = [
     "furo",
     "mypy",
     "myst_parser",
@@ -53,19 +53,18 @@
 
 [project.urls]
 Documentation = "https://github.com/NREL/infrasys#readme"
 Issues = "https://github.com/NREL/infrasys/issues"
 Source = "https://github.com/NREL/infrasys"
 
 [tool.pytest.ini_options]
+pythonpath = "src"
 minversion = "6.0"
 addopts = "-ra"
-testpaths = [
-    "tests",
-]
+testpaths = ["tests"]
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     ".ruff_cache",
     ".venv",
@@ -80,20 +79,20 @@
 indent-width = 4
 
 target-version = "py311"
 
 [tool.ruff.lint]
 # Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
 select = [
-    "C901",  # McCabe complexity
-    "E4",  # Subset of pycodestyle (E)
+    "C901", # McCabe complexity
+    "E4",   # Subset of pycodestyle (E)
     "E7",
     "E9",
-    "F",  # Pyflakes
-    "W",  # pycodestyle warnings
+    "F",    # Pyflakes
+    "W",    # pycodestyle warnings
 ]
 ignore = []
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
```

### Comparing `infrasys-0.0.2/PKG-INFO` & `infrasys-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.3
 Name: infrasys
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/NREL/infrasys#readme
 Project-URL: Issues, https://github.com/NREL/infrasys/issues
 Project-URL: Source, https://github.com/NREL/infrasys
 Author-email: Aadil Latif <aadil.latif@nrel.gov>, Daniel Thom <daniel.thom@nrel.gov>, Kapil Duwadi <kapil.duwadi@nrel.gov>, Pedro Andres Sanchez Perez <pedroandres.sanchezperez@nrel.gov>, Tarek Elgindy <tarek.elgindy@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.13,>=3.10
-Requires-Dist: loguru
-Requires-Dist: numpy
-Requires-Dist: pint
-Requires-Dist: pyarrow
+Requires-Dist: loguru~=0.7.2
+Requires-Dist: numpy~=1.26.4
+Requires-Dist: pint~=0.23
+Requires-Dist: pyarrow~=15.0.2
 Requires-Dist: pydantic<=3,>=2.4
-Requires-Dist: rich
+Requires-Dist: rich~=13.7.1
 Provides-Extra: dev
 Requires-Dist: autodoc-pydantic~=2.0; extra == 'dev'
 Requires-Dist: furo; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: myst-parser; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyarrow-stubs; extra == 'dev'
@@ -35,15 +35,15 @@
 Requires-Dist: sphinx-click; extra == 'dev'
 Requires-Dist: sphinx-copybutton; extra == 'dev'
 Requires-Dist: sphinx-tabs~=3.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # infrasys
 
-[![Main - CI](https://github.com/NREL/infrasys/workflows/Main%20-%20CI/badge.svg)](https://github.com/NREL/infrasys/actions/workflows/main_tests.yml)
+[![CI](https://github.com/NREL/infrasys/workflows/CI/badge.svg)](https://github.com/NREL/infrasys/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/NREL/infrasys/branch/main/graph/badge.svg)](https://codecov.io/gh/NREL/infrasys)
 
 This package implements a data store for components and time series in support of Python-based
 modeling packages. While it is designed to support teams modeling transmission and distribution
 systems for electrical grids, it can be used by any package that needs to store components
 (e.g., generators and buses) that have quantities (e.g., power and voltage) which may vary over
 time.
@@ -74,7 +74,14 @@
 $ pip install -e ".[dev]"
 ```
 
 Please install `pre-commit` so that your code is checked before making commits.
 ```
 $ pre-commit install
 ```
+
+## License
+infrasys is released under a BSD 3-Clause
+[License](https://github.com/NREL/infrasys/blob/main/LICENSE.txt).
+
+infrasys was developed under software record SWR-24-42 at the National Renewable Energy Laboratory
+([NREL](https://www.nrel.gov)).
```

