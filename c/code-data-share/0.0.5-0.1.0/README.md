# Comparing `tmp/code_data_share-0.0.5.tar.gz` & `tmp/code_data_share-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_share-0.0.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "code_data_share-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `code_data_share-0.0.5.tar` & `code_data_share-0.1.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.clang-format
--rw-r--r--   0        0        0     1084 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.devcontainer/3.12.Dockerfile
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.devcontainer/reinstall-cmake.sh
--rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/dependabot.yml
--rw-r--r--   0        0        0     3064 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/workflows/check.yml
--rw-r--r--   0        0        0      698 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/workflows/nightly.yml
--rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/workflows/performance.yml
--rw-r--r--   0        0        0     3045 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.gitignore
--rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 code_data_share-0.0.5/.python-version
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 code_data_share-0.0.5/CMakeLists.txt
--rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 code_data_share-0.0.5/LICENSE
--rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 code_data_share-0.0.5/README.rst
--rw-r--r--   0        0        0     7577 2022-11-09 12:37:21.000000 code_data_share-0.0.5/noxfile.py
--rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 code_data_share-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 code_data_share-0.0.5/requirements-dev.txt
--rwxr-xr-x   0        0        0      839 2022-11-09 12:37:21.000000 code_data_share-0.0.5/scripts/perf_import.sh
--rwxr-xr-x   0        0        0     1247 2022-11-09 12:37:21.000000 code_data_share-0.0.5/scripts/pyperformance.sh
--rw-r--r--   0        0        0    33701 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/_cdsmodule.c
--rw-r--r--   0        0        0    12431 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/_cdsmodule.h
--rw-r--r--   0        0        0     6903 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/clinic/_cdsmodule-b4-312.c.h
--rw-r--r--   0        0        0     9850 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/clinic/_cdsmodule.c.h
--rw-r--r--   0        0        0     3719 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/hashtable.c
--rw-r--r--   0        0        0      801 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/hashtable.h
--rw-r--r--   0        0        0     1607 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/lookup_table.c
--rw-r--r--   0        0        0     1010 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/lookup_table.h
--rw-r--r--   0        0        0    16063 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/_cds/pythoncapi_compat.h
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/artifacts/pycds.pth
--rw-r--r--   0        0        0     5914 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/cds/__init__.py
--rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/cds/_cds.pyi
--rw-r--r--   0        0        0     3966 2022-11-09 12:37:21.000000 code_data_share-0.0.5/src/cds/dump.py
--rw-r--r--   0        0        0     1887 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/.gitignore
--rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/base.toml
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_import/__init__.py
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_import/bm_import_requests.toml
--rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_import/requirements.in
--rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_import/requirements.txt
--rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_import/run_benchmark.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_module_load_attr/__init__.py
--rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_module_load_attr/pyproject.toml
--rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/benchmarks/bm_module_load_attr/run_benchmark.py
--rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds/__init__.py
--rw-r--r--   0        0        0     2563 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds/test_cds.py
--rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds/test_dump.py
--rw-r--r--   0        0        0      716 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds/test_import.py
--rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds_extension/__init__.py
--rw-r--r--   0        0        0     2248 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds_extension/test_archive.py
--rw-r--r--   0        0        0      574 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds_extension/test_base_extension.py
--rw-r--r--   0        0        0     1503 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds_extension/test_flags.py
--rw-r--r--   0        0        0     9756 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/test_cds_extension/test_share_object.py
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/workspace/mod1.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/workspace/mod2/__init__.py
--rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/workspace/mod2/mod2_1.py
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 code_data_share-0.0.5/tests/workspace/mod2/mod2_2/__init__.py
--rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 code_data_share-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.clang-format
+-rw-r--r--   0        0        0     1084 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.devcontainer/3.12.Dockerfile
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.devcontainer/reinstall-cmake.sh
+-rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2997 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/workflows/check.yml
+-rw-r--r--   0        0        0      714 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/workflows/nightly.yml
+-rw-r--r--   0        0        0     1397 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/workflows/performance.yml
+-rw-r--r--   0        0        0     3120 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.gitignore
+-rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 code_data_share-0.1.0/.python-version
+-rw-r--r--   0        0        0     1096 2022-11-09 12:37:21.000000 code_data_share-0.1.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 code_data_share-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 code_data_share-0.1.0/README.rst
+-rw-r--r--   0        0        0     7912 2022-11-09 12:37:21.000000 code_data_share-0.1.0/noxfile.py
+-rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 code_data_share-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 code_data_share-0.1.0/requirements-dev.txt
+-rwxr-xr-x   0        0        0      839 2022-11-09 12:37:21.000000 code_data_share-0.1.0/scripts/perf_import.sh
+-rwxr-xr-x   0        0        0     1247 2022-11-09 12:37:21.000000 code_data_share-0.1.0/scripts/pyperformance.sh
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/_cdscontext.h
+-rw-r--r--   0        0        0    33561 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/_cdsmodule.c
+-rw-r--r--   0        0        0    11479 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/_cdsmodule.h
+-rw-r--r--   0        0        0     6903 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/clinic/_cdsmodule-b4-312.c.h
+-rw-r--r--   0        0        0     9850 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/clinic/_cdsmodule.c.h
+-rw-r--r--   0        0        0     3719 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/hashtable.c
+-rw-r--r--   0        0        0      801 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/hashtable.h
+-rw-r--r--   0        0        0     1607 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/lookup_table.c
+-rw-r--r--   0        0        0     1010 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/lookup_table.h
+-rw-r--r--   0        0        0     3908 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/platforms.c
+-rw-r--r--   0        0        0     1405 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/platforms.h
+-rw-r--r--   0        0        0    16063 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/_cds/pythoncapi_compat.h
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/artifacts/pycds.pth
+-rw-r--r--   0        0        0     5914 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/cds/__init__.py
+-rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/cds/_cds.pyi
+-rw-r--r--   0        0        0     3966 2022-11-09 12:37:21.000000 code_data_share-0.1.0/src/cds/dump.py
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/.gitignore
+-rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/base.toml
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_import/__init__.py
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_import/bm_import_requests.toml
+-rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_import/requirements.in
+-rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_import/requirements.txt
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_import/run_benchmark.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_module_load_attr/__init__.py
+-rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_module_load_attr/pyproject.toml
+-rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/benchmarks/bm_module_load_attr/run_benchmark.py
+-rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds/__init__.py
+-rw-r--r--   0        0        0     2563 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds/test_cds.py
+-rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds/test_dump.py
+-rw-r--r--   0        0        0      716 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds/test_import.py
+-rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds_extension/__init__.py
+-rw-r--r--   0        0        0     2248 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds_extension/test_archive.py
+-rw-r--r--   0        0        0      574 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds_extension/test_base_extension.py
+-rw-r--r--   0        0        0     1503 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds_extension/test_flags.py
+-rw-r--r--   0        0        0     9756 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/test_cds_extension/test_share_object.py
+-rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/workspace/mod1.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/workspace/mod2/__init__.py
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/workspace/mod2/mod2_1.py
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 code_data_share-0.1.0/tests/workspace/mod2/mod2_2/__init__.py
+-rw-r--r--   0        0        0     2700 2022-11-09 12:37:21.000000 code_data_share-0.1.0/PKG-INFO
```

### Comparing `code_data_share-0.0.5/.devcontainer/3.12.Dockerfile` & `code_data_share-0.1.0/.devcontainer/3.12.Dockerfile`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/.devcontainer/devcontainer.json` & `code_data_share-0.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/.devcontainer/reinstall-cmake.sh` & `code_data_share-0.1.0/.devcontainer/reinstall-cmake.sh`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `code_data_share-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `code_data_share-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/.github/PULL_REQUEST_TEMPLATE.md` & `code_data_share-0.1.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/.github/workflows/check.yml` & `code_data_share-0.1.0/.github/workflows/check.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,45 +14,36 @@
   test-cpython:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         # for actions/setup-python:
         # https://raw.githubusercontent.com/actions/python-versions/main/versions-manifest.json
-        python:
-          - "3.8"
-          - "3.9"
-          - "3.10"
-          - "3.11"
-          - "3.12.0-beta - 3.12"
-        os: [ ubuntu-latest, macOS-latest ]
+        python: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
+        os: [ ubuntu-latest, macOS-latest, windows-latest ]
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install nox
       - name: Unit tests
         run: nox -s tests_venv_current
 
   test-conda:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ ubuntu-latest, macOS-latest ]
-        conda-py:
-          - "3.8"
-          - "3.9"
-          - "3.10"
-          - "3.11"
+        os: [ ubuntu-latest, macOS-latest, windows-latest ]
+        conda-py: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
 
     steps:
       - uses: actions/checkout@v4
       - uses: s-weigand/setup-conda@v1
         with:
           conda-channels: conda-forge
       - name: Install dependencies
@@ -71,15 +62,15 @@
 
   test-twine:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install nox twine
       - name: Build sdist to test
         run: |
           nox -s build_sdist
@@ -89,15 +80,15 @@
 
   check-format:
     name: Formatting Check
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install flake8
       - name: Lint with flake8
         run: |
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
```

### Comparing `code_data_share-0.0.5/.github/workflows/nightly.yml` & `code_data_share-0.1.0/.github/workflows/nightly.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-name: check
+name: nightly
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
   schedule:
     # 6:00 of UTF+8 every day
     - cron: '0 22 * * *'
   workflow_dispatch:
 
 jobs:
   test-nightly:
+    if: false
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python: [ "3.12-dev" ]
+        python: [ "3.13-dev" ]
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python }}
-        uses: deadsnakes/action@v3.0.1
+        uses: deadsnakes/action@v3.1.0
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install nox
       - name: Unit tests
```

### Comparing `code_data_share-0.0.5/.github/workflows/performance.yml` & `code_data_share-0.1.0/.github/workflows/performance.yml`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 concurrency:
   group: "workflow = ${{ github.workflow }}, ref = ${{ github.event.ref }}, pr = ${{ github.event.pull_request.id }}"
   cancel-in-progress: ${{ github.event_name == 'pull_request' || github.repository != 'alibaba/code-data-share-for-python' }}
 
 jobs:
   perf-import:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ ubuntu-latest, macOS-latest, windows-latest ]
 
     steps:
       - uses: actions/checkout@v4
       - uses: s-weigand/setup-conda@v1
         with:
           conda-channels: conda-forge
       - name: Install dependencies
@@ -24,15 +27,18 @@
           python -m pip install --upgrade pip
           python -m pip install nox pyperf
       - name: Perf importing third-party packages
         run: |
           sh scripts/perf_import.sh
 
   pyperformance:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ ubuntu-latest, macOS-latest, windows-latest ]
 
     steps:
       - uses: actions/checkout@v4
       - uses: s-weigand/setup-conda@v1
         with:
           conda-channels: conda-forge
       - name: Install dependencies
```

### Comparing `code_data_share-0.0.5/.github/workflows/release.yml` & `code_data_share-0.1.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,69 +6,70 @@
 
 jobs:
   build_sdist:
     name: Build sdist
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
 
       - name: Install nox
         run: python -m pip install nox
       - name: Build sdist
         run: nox -s build_sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: dist
+          name: dist-sdist
           path: |
             dist/*.tar.gz
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ ubuntu-latest, macOS-latest ]
+        os: [ ubuntu-latest, macOS-latest, windows-latest ]
 
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
       - name: Set up QEMU
         if: runner.os == 'Linux'
         uses: docker/setup-qemu-action@v3
         with:
           platforms: all
 
       - name: Install cibuildwheel
         run: python -m pip install cibuildwheel
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir dist
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: dist
+          name: dist-${{ matrix.os }}
           path: |
             dist/*.whl
   publish:
     name: Publish
     needs: [ build_wheels, build_sdist ]
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
 
       - name: Download artifact
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
-          name: dist
+          pattern: dist-*
           path: dist
+          merge-multiple: true
 
       - name: Upload wheels to Github release
-        uses: actions/github-script@v6
+        uses: actions/github-script@v7
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           script: |
             const fs = require('fs').promises;
             const { repo: { owner, repo }, sha } = context;
             
             // GITHUB_REF would be refs/tags/<tag_name>
```

### Comparing `code_data_share-0.0.5/.gitignore` & `code_data_share-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/CMakeLists.txt` & `code_data_share-0.1.0/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 cmake_minimum_required(VERSION 3.20)
 project(pycds)
 
 set(CMAKE_C_STANDARD 11)
-set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Werror=implicit-function-declaration")
+if (MSVC)
+    set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} /we4013")
+else ()
+    set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Werror=implicit-function-declaration")
+endif ()
 
 # Only for IDE linting, skbuild will handle wheel dependencies.
 if (NOT SKBUILD)
     #set(Python_ROOT_DIR "")
 endif ()
 
 find_package(Python 3.8 REQUIRED COMPONENTS Interpreter Development.Module)
 
-add_compile_definitions(Py_BUILD_CORE)  # for sizeof(PyGC_Head)
+add_compile_definitions(Py_BUILD_CORE Py_BUILD_CORE_MODULE)  # for sizeof(PyGC_Head)
 add_compile_definitions(NEED_OPCODE_TABLES)  # for _PyOpcode_Caches and _PyOpcode_Deopt
 
-python_add_library(_cds MODULE WITH_SOABI src/_cds/_cdsmodule.c src/_cds/lookup_table.c src/_cds/hashtable.c)
+python_add_library(_cds MODULE WITH_SOABI src/_cds/_cdsmodule.c src/_cds/lookup_table.c src/_cds/hashtable.c src/_cds/platforms.c)
 # clinic-generated files access core header.
 target_include_directories(_cds PRIVATE "${Python_INCLUDE_DIRS}/internal")
 
 # todo: if find cpython repo, run clinic
 # currently we manually run `python3 ../cpython/Tools/clinic/clinic.py --make --srcdir src/_cds`
 
-install(TARGETS _cds DESTINATION .)
+install(TARGETS _cds LIBRARY DESTINATION .)
 
 install(FILES src/artifacts/pycds.pth DESTINATION .)
```

### Comparing `code_data_share-0.0.5/LICENSE` & `code_data_share-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/README.rst` & `code_data_share-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/noxfile.py` & `code_data_share-0.1.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,36 @@
 
 import nox
 from nox.command import CommandFailed
 from nox.virtualenv import CondaEnv
 
 nox.options.default_venv_backend = 'conda'
 
-SUPPORTED_PYTHONS = ['3.8', '3.9', '3.10', '3.11']
+SUPPORTED_PYTHONS = ['3.8', '3.9', '3.10', '3.11', '3.12']
 
 OS = platform.system()
 RELEASE = platform.release()
 PYCDS_ROOT = os.path.dirname(__file__)
 
-DISABLE_SITE_HOOK_KEY = 'DISABLE_SITE_HOOK'
+GA = os.environ.get('GITHUB_ACTIONS') == 'true'
+
 CDS_PYPERFORMANCE = 'git+https://github.com/oraluben/pyperformance.git@cds'
 
 
+def _clean_nox():
+    from nox.virtualenv import shutil
+
+    shutil.rmtree(os.path.join(PYCDS_ROOT, '.nox'), ignore_errors=True)
+
+
+def ci_session_cleanup():
+    if OS == 'Windows' and GA:
+        _clean_nox()
+
+
 def _py_version(session: nox.Session):
     """
     :return: "3.9", "3.10", ...
     """
     out: str = session.run('python', '-c', 'import sys; print(f"{sys.version_info[0]}.{sys.version_info[1]}")',
                            silent=True)
     out = out.strip()
@@ -89,15 +101,15 @@
 PACKAGES = (
     Package('boto3'),
     Package('requests'),
     Package('numpy'),
     Package('pyparsing'),
     Package('sqlalchemy'),
     Package('werkzeug'),
-    Package('aiohttp'),
+    Package('aiohttp', skip=lambda _py: _py in ('3.12',)),
     Package('google-cloud-storage', module='google.cloud.storage'),
     Package('flask'),
     Package('azure-core', module='azure.core'),
     Package('jsonschema'),
 
     # Pillow is a package with C extension, and do not involve much CPython's internal library.
     # So this should be a good test for cds'ing C extensions.
@@ -129,17 +141,19 @@
 
         tmp = session.create_tmp()
 
         lst = os.path.join(tmp, 'test.lst')
         img = os.path.join(tmp, 'test.img')
 
         session.run('python', '-c', package.import_stmt, env={'PYCDSMODE': 'TRACE', 'PYCDSLIST': lst})
-        session.run('python', '-c', f'import cds.dump; cds.dump.run_dump("{lst}", "{img}")')
+        session.run('python', '-c', f'import cds.dump; cds.dump.run_dump({repr(lst)}, {repr(img)})')
         session.run('python', '-c', package.import_stmt, env={'PYCDSMODE': 'SHARE', 'PYCDSARCHIVE': img})
 
+        ci_session_cleanup()
+
 
     @nox.session(name=f'test_import_third_party_perf-{py}', tags=['test_import_third_party_perf'], python=py)
     @nox.parametrize('package', [package for package in PACKAGES if not package.should_skip(py)])
     def test_import_third_party_perf(session: nox.Session, package):
         """
         Benchmark import statements w./w.o. CDS.
 
@@ -155,28 +169,30 @@
         tmp = session.create_tmp()
 
         lst = os.path.join(tmp, 'test.lst')
         img = os.path.join(tmp, 'test.img')
 
         logger.info(f'start generating CDS archive for {package.name}')
         session.run('python', '-c', package.import_stmt, env={'PYCDSMODE': 'TRACE', 'PYCDSLIST': lst}, log=False)
-        session.run('python', '-c', f'import cds.dump; cds.dump.run_dump("{lst}", "{img}")', log=False)
+        session.run('python', '-c', f'import cds.dump; cds.dump.run_dump({repr(lst)}, {repr(img)})', log=False)
         session.run('python', '-c', package.import_stmt, env={'PYCDSMODE': 'SHARE', 'PYCDSARCHIVE': img}, log=False)
         logger.info(f'finish generating CDS archive for {package.name}')
 
         raw_out = f'perf-import-{session.python}-raw'
         cds_out = f'perf-import-{session.python}-cds'
 
         session.run('pyperf', 'command', '--fast', f'--append={raw_out}.json', f'--name={package.name}',
                     'python', '-c', package.import_stmt)
         session.run('pyperf', 'command', '--fast', f'--append={cds_out}.json', f'--name={package.name}',
                     '--inherit-environ=PYCDSMODE,PYCDSARCHIVE',
                     'python', '-c', package.import_stmt,
                     env={'PYCDSMODE': 'SHARE', 'PYCDSARCHIVE': img})
 
+        ci_session_cleanup()
+
 
 def _pyperformance(session: nox.Session, pyperformance_args=None):
     session.install(CDS_PYPERFORMANCE)
 
     configs = [
         (os.path.realpath(f'pyperformance-{_py_version(session)}-{config_name}.json'), config_args)
         for (config_name, config_args) in [
```

### Comparing `code_data_share-0.0.5/pyproject.toml` & `code_data_share-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "code-data-share"
-version = "0.0.5"
+version = "0.1.0"
 readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     'Operating System :: MacOS :: MacOS X',
-    # 'Operating System :: Microsoft :: Windows',
+    'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX :: Linux',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Programming Language :: Python :: Implementation :: CPython',
@@ -29,9 +29,13 @@
 [tool.cibuildwheel.linux]
 archs = ["x86_64", "aarch64"]
 skip = "*-musllinux*"
 
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "universal2", "arm64"]
 
+[tool.cibuildwheel.windows]
+archs = ["AMD64", "ARM64"]
+test-skip = "*-win_arm64"
+
 [tool.scikit-build]
 wheel.packages = ["src/cds"]
```

### Comparing `code_data_share-0.0.5/scripts/perf_import.sh` & `code_data_share-0.1.0/scripts/perf_import.sh`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/scripts/pyperformance.sh` & `code_data_share-0.1.0/scripts/pyperformance.sh`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/_cdsmodule.c` & `code_data_share-0.1.0/src/_cds/_cdsmodule.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 #include "_cdsmodule.h"
 
 #include <stddef.h>
-#include <sys/fcntl.h>
-#include <sys/mman.h>
-
-#ifdef MAP_POPULATE
-#define M_POPULATE MAP_POPULATE
-#else
-#define M_POPULATE 0
-#endif
 
 /*[clinic input]
 module _cds
 [clinic start generated code]*/
 /*[clinic end generated code: output=da39a3ee5e6b4b0d input=4970e54eebac52d1]*/
 
 // clang-format off
@@ -173,17 +165,17 @@
     }
     PyCDS_InitMoveIn();
 
     PyCDS_MoveInRec(obj, &cds_status.archive_header->obj, &obj);
 
     PyCDS_FinalizeMoveIn();
 
-    ftruncate(cds_status.archive_fd, cds_status.archive_header->used);
-    close(cds_status.archive_fd);
-    cds_status.archive_fd = 0;
+    finalize_map(cds_status, cds_status.archive_header->used,
+                 cds_status.archive_header);
+
     if (cds_status.traverse_error) {
         return NULL;
     }
 
     return Py_NewRef(Py_None);
 }
 
@@ -265,41 +257,43 @@
     if (cds_status.archive != NULL || cds_status.archive_fd != 0 ||
         cds_status.archive_header != NULL) {
         PyErr_SetString(CDSException, "archive already initialized.");
         return NULL;
     }
 
     cds_status.archive = archive;
-    cds_status.archive_fd = open(archive, O_RDWR | O_CREAT | O_TRUNC, 0666);
-    if (cds_status.archive_fd < 0) {
+    cds_status.archive_fd =
+        create_archive_preallocate(archive, CDS_MAX_IMG_SIZE);
+    if (cds_status.archive_fd <= 0) {
         PyErr_SetString(CDSException, "create mmap file failed.");
-        return NULL;
+        goto fail;
     }
-    ftruncate(cds_status.archive_fd, CDS_MAX_IMG_SIZE);
-    void *shm =
-        mmap(CDS_REQUESTING_ADDR, CDS_MAX_IMG_SIZE, PROT_READ | PROT_WRITE,
-             MAP_SHARED | MAP_FIXED, cds_status.archive_fd, 0);
-    if (shm == MAP_FAILED) {
-        PyErr_SetString(CDSException, "mmap failed.");
-        return NULL;
+    void *shm = create_map_from_archive(CDS_REQUESTING_ADDR, CDS_MAX_IMG_SIZE,
+                                        cds_status);
+    if (shm == NULL) {
+        PyErr_SetString(CDSException, "mmap failed during dump.");
+        goto fail;
     }
     else if (shm != CDS_REQUESTING_ADDR) {
         PyErr_SetString(CDSException, "unexpected mapping.");
-        return NULL;
+        goto fail;
     }
     cds_status.archive_header = (struct CDSArchiveHeader *)shm;
     cds_status.archive_header->mapped_addr = shm;
     cds_status.archive_header->none_addr = Py_None;
     cds_status.archive_header->true_addr = Py_True;
     cds_status.archive_header->false_addr = Py_False;
     cds_status.archive_header->ellipsis_addr = Py_Ellipsis;
     cds_status.archive_header->used =
         ALIEN_TO(sizeof(struct CDSArchiveHeader), 8);
     cds_status.archive_header->all_string_ref = NULL;
     return shm;
+fail:
+    close_archive(&cds_status.archive_fd);
+    return NULL;
 }
 
 void *
 PyCDS_Malloc(size_t size)
 {
     cds_status.move_in_ctx->n_alloc++;
     if (!size)
@@ -312,15 +306,15 @@
     void *res =
         ((char *)cds_status.archive_header) + cds_status.archive_header->used;
     if ((cds_status.archive_header->used += size_aligned) > CDS_MAX_IMG_SIZE) {
         cds_status.archive_header->used -= sizeof(PyGC_Head);
         cds_status.archive_header->used -= size_aligned;
         return NULL;
     }
-    PyCDS_Verbose(2, "Malloc: [%p, %p)", res, res + size_aligned);
+    PyCDS_Verbose(2, "Malloc: [%p, %p)", res, P(res) + size_aligned);
     return res;
 }
 
 void
 PyCDS_Free(void *p)
 {
     // do nothing for now.
@@ -328,16 +322,16 @@
     PyCDS_Verbose(2, "Free: %p", p);
 }
 bool
 PyCDS_InHeap(void *p)
 {
     if (cds_status.archive_header) {
         if (p > cds_status.archive_header->mapped_addr &&
-            p < cds_status.archive_header->mapped_addr +
-                    cds_status.archive_header->used)
+            P(p) < P(cds_status.archive_header->mapped_addr) +
+                       cds_status.archive_header->used)
             return true;
     }
     return false;
 }
 
 void *
 PyCDS_LoadArchive(const char *archive)
@@ -346,52 +340,55 @@
         PyErr_SetString(CDSException, "archive already loaded.");
         return NULL;
     }
 
     PyCDS_Verbose(1, "opening archive %s", archive);
 
     cds_status.archive = archive;
-    cds_status.archive_fd = open(archive, O_RDWR);
-    if (cds_status.archive_fd < 0) {
-        PyErr_SetString(CDSException, "open mmap file failed.");
+    struct CDSArchiveHeader h;
+    struct CDSArchiveHeader *header = read_header_from_archive(
+        cds_status.archive, &cds_status.archive_fd, &h, sizeof(h));
+    if (header == NULL) {
+        if (cds_status.archive_fd == NULL_FD) {
+            PyErr_SetString(CDSException, "open mmap file failed.");
+        }
+        else {
+            PyErr_SetString(CDSException, "read archive header failed.");
+        }
         goto fail;
     }
 
-    struct CDSArchiveHeader h;
-    if (read(cds_status.archive_fd, &h, sizeof(h)) != sizeof(h)) {
-        PyErr_SetString(CDSException, "read archive header failed.");
+    if (CDS_REQUESTING_ADDR != h.mapped_addr) {
+        PyErr_SetString(CDSException, "Archive address changed.");
         goto fail;
     }
 
-    PyCDS_Verbose(2, "requesting %p...", h.mapped_addr);
     size_t aligned_size = ALIEN_TO(h.used, 4096);
-    void *shm =
-        mmap(h.mapped_addr, aligned_size, PROT_READ | PROT_WRITE,
-             MAP_PRIVATE | MAP_FIXED | M_POPULATE, cds_status.archive_fd, 0);
-    if (shm == MAP_FAILED) {
+    void *shm = map_archive(cds_status, aligned_size, h.mapped_addr);
+    if (shm == NULL) {
         PyErr_SetString(CDSException, "mmap failed.");
         goto fail;
     }
     else if (shm != h.mapped_addr) {
         PyErr_SetString(CDSException, "mmap relocated.");
         goto fail;
     }
+
     cds_status.archive_header = (struct CDSArchiveHeader *)shm;
-    close(cds_status.archive_fd);
-    cds_status.archive_fd = 0;
+    close_archive(&cds_status.archive_fd);
 
 #if M_POPULATE == 0
     for (size_t i = 0; i < cds_status.archive_header->used; i += 4096) {
         ((char volatile *)shm)[i] += 0;
     }
 #endif
 
     if (cds_status.archive_header->none_addr) {
         cds_status.shift =
-            (void *)Py_None - (void *)cds_status.archive_header->none_addr;
+            P(Py_None) - P(cds_status.archive_header->none_addr);
     }
     if (cds_status.archive_header->obj != NULL) {
         assert(!cds_status.traverse_error);
         PyCDS_PatchPyObject(&cds_status.archive_header->obj);
         // if patch failed, Python exception is set
         if (cds_status.traverse_error) {
             return NULL;
@@ -450,16 +447,15 @@
             str_refs = str_refs->next;
         }
     }
 
     return shm;
 
 fail:
-    close(cds_status.archive_fd);
-    cds_status.archive_fd = 0;
+    close_archive(&cds_status.archive_fd);
     return NULL;
 }
 
 void
 PyCDS_InitMoveIn()
 {
     assert(cds_status.move_in_ctx == NULL);
@@ -573,19 +569,20 @@
 #if PY_MINOR_VERSION >= 12
         if (size == 0) {
             UNEXPECTED_SINGLETON(op);
         }
         else if (size == 1) {
             // not static single byte
             // maybe from marshal?
-#define BS(...) (&_Py_SINGLETON(bytes_characters __VA_OPT__([) __VA_ARGS__ __VA_OPT__(])))
-            assert((void *)BS(256) == (void *)(BS() + 1));
-            *target = (PyObject *)BS((Py_UCS1)PyBytes_AS_STRING(op)[0]);
-            assert(*target >= (PyObject *)BS());
-            assert(*target < (PyObject *)(BS() + 1));
+#define BS (&_Py_SINGLETON(bytes_characters))
+#define BSi(i) (&_Py_SINGLETON(bytes_characters[i]))
+            assert((void *)BSi(256) == (void *)(BS + 1));
+            *target = (PyObject *)BSi((Py_UCS1)PyBytes_AS_STRING(op)[0]);
+            assert(*target >= (PyObject *)BS);
+            assert(*target < (PyObject *)(BS + 1));
 #undef BS
             goto _return;
         }
 #endif
 
         PyBytesObject *res = (PyBytesObject *)PyCDS_Malloc(
             offsetof(PyBytesObject, ob_sval) + 1 + size);
```

### Comparing `code_data_share-0.0.5/src/_cds/_cdsmodule.h` & `code_data_share-0.1.0/src/_cds/_cdsmodule.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #ifndef PYCDS__CDSMODULE_H
 #define PYCDS__CDSMODULE_H
 
 #include <Python.h>
 
+#include "_cdscontext.h"
+#include "platforms.h"
+#include "pythoncapi_compat.h"
+
 // immortal & static objects
 #if PY_MINOR_VERSION >= 12
 #include <internal/pycore_long.h>
 #include <internal/pycore_object.h>
 #include <internal/pycore_runtime.h>
 #endif
 
@@ -24,64 +28,25 @@
 #include <objimpl.h>
 #endif
 
 #if PY_MINOR_VERSION < 8
 #error Requires CPython 3.8+.
 #endif
 
-#include <stdbool.h>
-
 #if PY_MINOR_VERSION >= 12
 #include "clinic/_cdsmodule.c.h"
 #else
 #include "clinic/_cdsmodule-b4-312.c.h"
 #endif
-#include "lookup_table.h"
-#include "pythoncapi_compat.h"
 
 #define CDS_MAX_IMG_SIZE (1024 * 1024 * 1024)
-#define CDS_REQUESTING_ADDR ((void *)0x280000000L)
+#define CDS_REQUESTING_ADDR ((void *)0x0000280000000000L)
 
 #define FAST_PATCH
 
-struct StringRefItem {
-    PyObject **ref;
-    struct StringRefItem *next;
-};
-
-struct StringRefList {
-    PyObject *str;
-    struct StringRefItem *refs;
-    struct StringRefList *next;
-};
-
-struct CDSArchiveHeader {
-    void *mapped_addr;
-    void *none_addr;
-    void *true_addr;
-    void *false_addr;
-    void *ellipsis_addr;
-    size_t used;
-
-    PyObject *obj;
-
-    struct StringRefList *all_string_ref;
-};
-
-struct MoveInContext {
-    int n_alloc;
-
-    table *orig_pyobject_to_in_heap_pyobject_map;
-    table *in_heap_str_to_string_ref_list_map;
-
-#if PY_MINOR_VERSION >= 12
-    PyObject *static_strings;
-#endif
-};
-
 /*
  * Internal representation of PYCDSMODE.
  * See `config_read_env_vars` for detail.
  *
  * 0: disable
  * 1: dumped name list (from PYDUMPMODULELIST)
  * 2: dumped archive from name list (PYCDSMODE=DUMP, from PYCDSLIST &
@@ -93,36 +58,17 @@
 
 #define CDS_MODE_DISABLED (0)
 #define CDS_MODE_DUMP_LIST (1)
 #define CDS_MODE_DUMP_ARCHIVE (2)
 #define CDS_MODE_SHARE (3)
 #define CDS_MODE_MANUALLY (-1)
 
+#define P(p) ((p_type)(p))
 #define ALIEN_TO(size, align) (((size) + ((align)-1)) & ~((align)-1))
-#define UNSHIFT(p, shift, ty) ((ty *)((void *)(p) + (shift)))
-
-struct CDSStatus {
-    int verbose;
-    int mode;
-
-    // Prevent re-entry of cds.init_from_env()
-    bool initialized;
-
-    long shift;
-    bool traverse_error;
-
-    const char *archive;
-    int archive_fd;
-
-    struct CDSArchiveHeader *archive_header;
-
-    PyObject *flags;
-
-    struct MoveInContext *move_in_ctx;
-};
+#define UNSHIFT(p, shift, ty) ((ty *)(P(p) + (shift)))
 
 void *PyCDS_Malloc(size_t);
 
 void
 PyCDS_Free(void *);
 
 bool
@@ -137,16 +83,14 @@
 
 void *
 PyCDS_AllocatorRealloc(void *, void *, size_t);
 
 void
 PyCDS_AllocatorFree(void *, void *);
 
-PyAPI_DATA(struct CDSStatus) cds_status;
-
 PyMODINIT_FUNC
 PyInit__cds(void);
 
 void *
 PyCDS_CreateArchive(const char *archive);
 
 void *
```

### Comparing `code_data_share-0.0.5/src/_cds/clinic/_cdsmodule-b4-312.c.h` & `code_data_share-0.1.0/src/_cds/clinic/_cdsmodule-b4-312.c.h`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/clinic/_cdsmodule.c.h` & `code_data_share-0.1.0/src/_cds/clinic/_cdsmodule.c.h`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/hashtable.c` & `code_data_share-0.1.0/src/_cds/hashtable.c`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/hashtable.h` & `code_data_share-0.1.0/src/_cds/hashtable.h`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/lookup_table.c` & `code_data_share-0.1.0/src/_cds/lookup_table.c`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/lookup_table.h` & `code_data_share-0.1.0/src/_cds/lookup_table.h`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/_cds/pythoncapi_compat.h` & `code_data_share-0.1.0/src/_cds/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/cds/__init__.py` & `code_data_share-0.1.0/src/cds/__init__.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/src/cds/dump.py` & `code_data_share-0.1.0/src/cds/dump.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/__init__.py` & `code_data_share-0.1.0/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import logging
 import os
 import random
 
 from test.support.script_helper import assert_python_ok, assert_python_failure
 
 import typing as t
@@ -11,20 +12,30 @@
     return assert_python_ok('-c', src, **env_vars)
 
 
 def assert_python_source_failure(src, **env_vars):
     return assert_python_failure('-c', src, **env_vars)
 
 
+def utf8_wrap(f):
+    @functools.wraps(f)
+    def inner(*args, **kwargs):
+        if 'PYTHONUTF8' not in kwargs:
+            kwargs['PYTHONUTF8'] = '1'
+        return f(*args, **kwargs)
+
+    return inner
+
+
 class UtilMixin:
     exists = staticmethod(os.path.exists)
-    assert_python_ok = staticmethod(assert_python_ok)
-    assert_python_failure = staticmethod(assert_python_failure)
-    assert_python_source_ok = staticmethod(assert_python_source_ok)
-    assert_python_source_failure = staticmethod(assert_python_source_failure)
+    assert_python_ok = staticmethod(utf8_wrap(assert_python_ok))
+    assert_python_failure = staticmethod(utf8_wrap(assert_python_failure))
+    assert_python_source_ok = staticmethod(utf8_wrap(assert_python_source_ok))
+    assert_python_source_failure = staticmethod(utf8_wrap(assert_python_source_failure))
 
     assertExists = lambda self, file: self.assertTrue(self.exists(file), f'{file} should exists but not.')
     assertNotExists = lambda self, file: self.assertFalse(self.exists(file), f'{file} should not exists but present.')
 
     @staticmethod
     def hook_installed():
         try:
@@ -60,11 +71,11 @@
         f = 1 / f
     return f
 
 
 def is_shared(address: t.Union[str, int]):
     if isinstance(address, int):
         address = hex(address)
-    return len(address) == len('0x280000000') and address.startswith('0x28')
+    return len(address) == len('0x280000000000') and address.startswith('0x28')
 
 
 logging.getLogger().setLevel(logging.DEBUG)
```

### Comparing `code_data_share-0.0.5/tests/benchmarks/bm_import/run_benchmark.py` & `code_data_share-0.1.0/tests/benchmarks/bm_import/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/benchmarks/bm_module_load_attr/run_benchmark.py` & `code_data_share-0.1.0/tests/benchmarks/bm_module_load_attr/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds/__init__.py` & `code_data_share-0.1.0/tests/test_cds/__init__.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds/test_cds.py` & `code_data_share-0.1.0/tests/test_cds/test_cds.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds/test_dump.py` & `code_data_share-0.1.0/tests/test_cds/test_dump.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds/test_import.py` & `code_data_share-0.1.0/tests/test_cds/test_import.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds_extension/test_archive.py` & `code_data_share-0.1.0/tests/test_cds_extension/test_archive.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds_extension/test_base_extension.py` & `code_data_share-0.1.0/tests/test_cds_extension/test_base_extension.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds_extension/test_flags.py` & `code_data_share-0.1.0/tests/test_cds_extension/test_flags.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/tests/test_cds_extension/test_share_object.py` & `code_data_share-0.1.0/tests/test_cds_extension/test_share_object.py`

 * *Files identical despite different names*

### Comparing `code_data_share-0.0.5/PKG-INFO` & `code_data_share-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: code-data-share
-Version: 0.0.5
-Classifier: Development Status :: 3 - Alpha
+Version: 0.1.0
+Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

