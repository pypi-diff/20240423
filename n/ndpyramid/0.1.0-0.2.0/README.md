# Comparing `tmp/ndpyramid-0.1.0.tar.gz` & `tmp/ndpyramid-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndpyramid-0.1.0.tar", last modified: Tue Aug 29 20:34:22 2023, max compression
+gzip compressed data, was "ndpyramid-0.2.0.tar", last modified: Tue Apr 23 16:28:10 2024, max compression
```

## Comparing `ndpyramid-0.1.0.tar` & `ndpyramid-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.747268 ndpyramid-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (999)      119 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     1358 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2196 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/.github/workflows/pypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1821 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      736 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (999)     1067 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     3511 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2740 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/ci/
--rw-r--r--   0 runner    (1001) docker     (999)      354 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (999)      277 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/ndpyramid/
--rw-r--r--   0 runner    (1001) docker     (999)      138 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/ndpyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       21 2023-08-29 20:34:22.000000 ndpyramid-0.1.0/ndpyramid/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)     1863 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/ndpyramid/common.py
--rw-r--r--   0 runner    (1001) docker     (999)     5089 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/ndpyramid/core.py
--rw-r--r--   0 runner    (1001) docker     (999)     9722 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/ndpyramid/regrid.py
--rw-r--r--   0 runner    (1001) docker     (999)     4414 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/ndpyramid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/ndpyramid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3511 2023-08-29 20:34:22.000000 ndpyramid-0.1.0/ndpyramid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      569 2023-08-29 20:34:22.000000 ndpyramid-0.1.0/ndpyramid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 20:34:22.000000 ndpyramid-0.1.0/ndpyramid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       77 2023-08-29 20:34:22.000000 ndpyramid-0.1.0/ndpyramid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       10 2023-08-29 20:34:22.000000 ndpyramid-0.1.0/ndpyramid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (999)    11165 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)     2386 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:22.751268 ndpyramid-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3218 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/tests/test_pyramids.py
--rw-r--r--   0 runner    (1001) docker     (999)      721 2023-08-29 20:34:05.000000 ndpyramid-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.384500 ndpyramid-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.376500 ndpyramid-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.376500 ndpyramid-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.github/workflows/codspeed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-23 16:28:10.384500 ndpyramid-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.376500 ndpyramid-0.2.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ci/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.376500 ndpyramid-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.376500 ndpyramid-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/_static/monogram-dark-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/_static/monogram-light-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/generate-pyramids.md
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/quick-start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/docs/schema.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.380499 ndpyramid-0.2.0/ndpyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 16:28:10.000000 ndpyramid-0.2.0/ndpyramid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/coarsen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/reproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/ndpyramid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.380499 ndpyramid-0.2.0/ndpyramid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-23 16:28:10.000000 ndpyramid-0.2.0/ndpyramid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-23 16:28:10.000000 ndpyramid-0.2.0/ndpyramid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:28:10.000000 ndpyramid-0.2.0/ndpyramid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 16:28:10.000000 ndpyramid-0.2.0/ndpyramid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:28:10.000000 ndpyramid-0.2.0/ndpyramid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.380499 ndpyramid-0.2.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:28:10.384500 ndpyramid-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:28:10.380499 ndpyramid-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/tests/test_pyramids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-23 16:27:56.000000 ndpyramid-0.2.0/tests/test_utils.py
```

### Comparing `ndpyramid-0.1.0/.github/workflows/main.yaml` & `ndpyramid-0.2.0/.github/workflows/main.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -5,51 +5,55 @@
     branches:
       - main
   pull_request:
     branches:
       - main
   workflow_dispatch:
   schedule:
-    - cron: '0 0 * * *' # Daily “At 00:00”
+    - cron: "0 0 * * *" # Daily “At 00:00”
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   test:
     if: github.repository == 'carbonplan/ndpyramid'
     name: ${{ matrix.python-version }}-build
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10'] #TODO: add 3.11 once sparse/numba support it
+        python-version: ["3.9", "3.10", "3.11"]
     timeout-minutes: 20
     defaults:
       run:
         shell: bash -l {0}
     steps:
-      - uses: actions/checkout@v3
+      - name: Checkout
+        uses: actions/checkout@v4
+
       - name: Install Conda environment from environment.yml
-        uses: mamba-org/provision-with-micromamba@main
+        uses: mamba-org/setup-micromamba@v1
         with:
+          # environment-file is not assumed anymore
           environment-file: ci/environment.yml
-          cache-downloads: true
-          extra-specs: |
+          create-args: >-
             python=${{ matrix.python-version }}
+          # now called cache-environment
+          cache-environment: true
 
       - name: Install package
         run: |
           python -m pip install -e . --no-deps
       - name: Conda list information
         run: |
           conda env list
           conda list
       - name: Run tests
         run: |
           python -m pytest
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           file: ./coverage.xml
           fail_ci_if_error: false
```

### Comparing `ndpyramid-0.1.0/.github/workflows/pypi-release.yaml` & `ndpyramid-0.2.0/.github/workflows/pypi-release.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
   push:
 
 jobs:
   build-artifacts:
     runs-on: ubuntu-latest
     if: github.repository == 'carbonplan/ndpyramid'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: 3.9
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
@@ -35,28 +35,28 @@
           pwd
           if [ -f dist/ndpyramid-unknown.tar.gz ]; then
             echo "❌ INVALID VERSION NUMBER"
             exit 1
           else
             echo "✅ Looks good"
           fi
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: releases
           path: dist
 
   test-built-dist:
     needs: build-artifacts
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: 3.9
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: releases
           path: dist
       - name: List contents of built dist
         run: |
           ls -ltrh
           ls -ltrh dist
@@ -69,17 +69,17 @@
           python -c "import ndpyramid; print(ndpyramid.__version__)"
 
   upload-to-pypi:
     needs: test-built-dist
     if: github.event_name == 'release'
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.8
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
           verbose: true
```

### Comparing `ndpyramid-0.1.0/.gitignore` & `ndpyramid-0.2.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/generated/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
@@ -124,7 +125,9 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+docs/generated/
```

### Comparing `ndpyramid-0.1.0/LICENSE` & `ndpyramid-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ndpyramid-0.1.0/PKG-INFO` & `ndpyramid-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,24 @@
-Metadata-Version: 2.1
-Name: ndpyramid
-Version: 0.1.0
-Summary: A small utility for generating ND array pyramids using Xarray and Zarr
-Author-email: CarbonPlan <tech@carbonplan.org>
-License: MIT
-Project-URL: repository, https://github.com/carbonplan/ndpyramid
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align='left'>
-  <a href='https://carbonplan.org/#gh-light-mode-only'>
-    <img
-      src='https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png'
-      height='48px'
-    />
-  </a>
-  <a href='https://carbonplan.org/#gh-dark-mode-only'>
-    <img
-      src='https://carbonplan-assets.s3.amazonaws.com/monogram/light-small.png'
-      height='48px'
-    />
-  </a>
+<p align="left" >
+<a href='https://carbonplan.org'>
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="https://carbonplan-assets.s3.amazonaws.com/monogram/light-small.png">
+  <img alt="CarbonPlan monogram." height="48" src="https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png">
+</picture>
+</a>
 </p>
 
 # ndpyramid
 
 A small utility for generating ND array pyramids using Xarray and Zarr.
 
 [![CI](https://github.com/carbonplan/ndpyramid/actions/workflows/main.yaml/badge.svg)](https://github.com/carbonplan/ndpyramid/actions/workflows/main.yaml)
-![MIT License](https://badgen.net/badge/license/MIT/blue)
+![PyPI](https://img.shields.io/pypi/v/ndpyramid)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/ndpyramid.svg)](https://anaconda.org/conda-forge/ndpyramid)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 # installation
 
 Ndpyramid can be installed in three ways:
 
 Using the [conda](https://conda.io) package manager that comes with the Anaconda/Miniconda distribution:
 
@@ -90,12 +66,12 @@
 pyramid.to_zarr('./path/to/write')
 ```
 
 See the docstrings for more details about input parameters and options.
 
 ## license
 
-All the code in this repository is [MIT](https://choosealicense.com/licenses/mit/) licensed, but we request that you please provide attribution if reusing any of our digital content (graphics, logo, articles, etc.).
+All the code in this repository is [MIT](https://choosealicense.com/licenses/mit/)-licensed, but we request that you please provide attribution if reusing any of our digital content (graphics, logo, articles, etc.).
 
 ## about us
 
-CarbonPlan is a non-profit organization working on the science and data of carbon removal. We aim to improve the transparency and scientific integrity of carbon removal and climate solutions through open data and tools. Find out more at [carbonplan.org](https://carbonplan.org/) or get in touch by [opening an issue](https://github.com/carbonplan/ndpyramid/issues/new) or [sending us an email](mailto:hello@carbonplan.org).
+CarbonPlan is a nonprofit organization that uses data and science for climate action. We aim to improve the transparency and scientific integrity of climate solutions with open data and tools. Find out more at [carbonplan.org](https://carbonplan.org/) or get in touch by [opening an issue](https://github.com/carbonplan/ndpyramid/issues/new) or [sending us an email](mailto:hello@carbonplan.org).
```

#### html2text {}

```diff
@@ -1,26 +1,17 @@
-Metadata-Version: 2.1 Name: ndpyramid Version: 0.1.0 Summary: A small utility
-for generating ND array pyramids using Xarray and Zarr Author-email: CarbonPlan
-carbonplan.org> License: MIT Project-URL: repository, https://github.com/
-carbonplan/ndpyramid Classifier: Development Status :: 4 - Beta Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Science/Research Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE
-_[_h_t_t_p_s_:_/_/_c_a_r_b_o_n_p_l_a_n_-_a_s_s_e_t_s_._s_3_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_o_n_o_g_r_a_m_/_d_a_r_k_-_s_m_a_l_l_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_c_a_r_b_o_n_p_l_a_n_-_a_s_s_e_t_s_._s_3_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_o_n_o_g_r_a_m_/_l_i_g_h_t_-_s_m_a_l_l_._p_n_g_]
+_[_C_a_r_b_o_n_P_l_a_n_ _m_o_n_o_g_r_a_m_._]
 # ndpyramid A small utility for generating ND array pyramids using Xarray and
 Zarr. [![CI](https://github.com/carbonplan/ndpyramid/actions/workflows/
 main.yaml/badge.svg)](https://github.com/carbonplan/ndpyramid/actions/
-workflows/main.yaml) ![MIT License](https://badgen.net/badge/license/MIT/blue)
-# installation Ndpyramid can be installed in three ways: Using the [conda]
-(https://conda.io) package manager that comes with the Anaconda/Miniconda
+workflows/main.yaml) ![PyPI](https://img.shields.io/pypi/v/ndpyramid) [![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/ndpyramid.svg)](https://
+anaconda.org/conda-forge/ndpyramid) [![License: MIT](https://img.shields.io/
+badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) #
+installation Ndpyramid can be installed in three ways: Using the [conda](https:
+//conda.io) package manager that comes with the Anaconda/Miniconda
 distribution: ```shell conda install ndpyramid --channel conda-forge ``` Using
 the [pip](https://pypi.org/project/pip/) package manager: ```shell python -
 m pip install ndpyramid ``` To install a development version from source:
 ```python git clone https://github.com/carbonplan/ndpyramid cd ndpyramid python
 -m pip install -e . ``` # usage Ndpyramid provides a set of utilities for
 creating pyramids with standardized metadata. The example below demonstrates
 the usage of the `pyramid_coarsen` and `pyramid_reproject` utilities. Check out
@@ -30,15 +21,15 @@
 load a sample xarray.Dataset ds = xr.tutorial.load_dataset('air_temperature') #
 make a coarsened pyramid pyramid = pyramid_coarsen(ds, factors=[16, 8, 4, 3, 2,
 1], dims=['lat', 'lon'], boundary='trim') # make a reprojected (EPSG:3857)
 pyramid ds = ds.rio.write_crs('EPSG:4326') pyramid = pyramid_reproject(ds,
 levels=2) # write the pyramid to zarr pyramid.to_zarr('./path/to/write') ```
 See the docstrings for more details about input parameters and options. ##
 license All the code in this repository is [MIT](https://choosealicense.com/
-licenses/mit/) licensed, but we request that you please provide attribution if
+licenses/mit/)-licensed, but we request that you please provide attribution if
 reusing any of our digital content (graphics, logo, articles, etc.). ## about
-us CarbonPlan is a non-profit organization working on the science and data of
-carbon removal. We aim to improve the transparency and scientific integrity of
-carbon removal and climate solutions through open data and tools. Find out more
-at [carbonplan.org](https://carbonplan.org/) or get in touch by [opening an
-issue](https://github.com/carbonplan/ndpyramid/issues/new) or [sending us an
-email](mailto:hello@carbonplan.org).
+us CarbonPlan is a nonprofit organization that uses data and science for
+climate action. We aim to improve the transparency and scientific integrity of
+climate solutions with open data and tools. Find out more at [carbonplan.org]
+(https://carbonplan.org/) or get in touch by [opening an issue](https://
+github.com/carbonplan/ndpyramid/issues/new) or [sending us an email](mailto:
+hello@carbonplan.org).
```

### Comparing `ndpyramid-0.1.0/ndpyramid/common.py` & `ndpyramid-0.2.0/ndpyramid/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import typing
 
 import pydantic
 import pyproj
 import rasterio.transform
 
+ProjectionOptions = typing.Literal['web-mercator', 'equidistant-cylindrical']
+
 
 class Projection(pydantic.BaseModel):
-    name: typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator'
+    name: ProjectionOptions = 'web-mercator'
     _crs: str = pydantic.PrivateAttr()
     _proj = pydantic.PrivateAttr()
 
     def __init__(self, **data) -> None:
 
         super().__init__(**data)
         epsg_codes = {'web-mercator': 'EPSG:3857', 'equidistant-cylindrical': 'EPSG:4326'}
         self._crs = epsg_codes[self.name]
         self._proj = pyproj.Proj(self._crs)
 
-    @pydantic.validate_arguments
-    def transform(self, *, dim:int) -> rasterio.transform.Affine:
-
+    @pydantic.validate_call
+    def transform(self, *, dim: int) -> rasterio.transform.Affine:
 
         if self.name == 'web-mercator':
             # set up the transformation matrix for the web-mercator projection such that the data conform
             # to the slippy-map tiles assumed boundaries. See https://github.com/carbonplan/ndpyramid/pull/70
             # for detailed on calculating the parameters.
-            return rasterio.transform.Affine.translation(-20037508.342789244, 20037508.342789248) * rasterio.transform.Affine.scale((20037508.342789244 * 2) / dim, -(20037508.342789248 * 2) / dim)
+            return rasterio.transform.Affine.translation(
+                -20037508.342789244, 20037508.342789248
+            ) * rasterio.transform.Affine.scale(
+                (20037508.342789244 * 2) / dim, -(20037508.342789248 * 2) / dim
+            )
         elif self.name == 'equidistant-cylindrical':
             # set up the transformation matrix that maps between the Equidistant Cylindrical projection
             # and the latitude-longitude projection. The Affine.translation function moves the origin
             # of the grid from (0, 0) to (-180, 90) in latitude-longitude coordinates,
             # and the Affine.scale function scales the grid coordinates to match the size of the grid
             # in latitude-longitude coordinates. The resulting transformation matrix maps grid coordinates to
             # latitude-longitude coordinates.
-            return rasterio.transform.Affine.translation(-180, 90) * rasterio.transform.Affine.scale(360 / dim, -180 / dim)
+            return rasterio.transform.Affine.translation(
+                -180, 90
+            ) * rasterio.transform.Affine.scale(360 / dim, -180 / dim)
```

### Comparing `ndpyramid-0.1.0/ndpyramid/core.py` & `ndpyramid-0.2.0/ndpyramid/reproject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,147 @@
 from __future__ import annotations  # noqa: F401
 
-import typing
 from collections import defaultdict
 
 import datatree as dt
+import numpy as np
 import xarray as xr
+from rasterio.warp import Resampling
 
-from .common import Projection
-from .utils import add_metadata_and_zarr_encoding, get_version, multiscales_template
+from .common import Projection, ProjectionOptions
+from .utils import (
+    add_metadata_and_zarr_encoding,
+    get_levels,
+    get_version,
+    multiscales_template,
+)
+
+
+def _da_reproject(da, *, dim, crs, resampling, transform):
+    if da.encoding.get('_FillValue') is None and np.issubdtype(da.dtype, np.floating):
+        da.encoding['_FillValue'] = np.nan
+    return da.rio.reproject(
+        crs,
+        resampling=resampling,
+        shape=(dim, dim),
+        transform=transform,
+    )
 
 
-def pyramid_coarsen(
-    ds: xr.Dataset, *, factors: list[int], dims: list[str], **kwargs
-) -> dt.DataTree:
-    """Create a multiscale pyramid via coarsening of a dataset by given factors
+def level_reproject(
+    ds: xr.Dataset,
+    *,
+    projection: ProjectionOptions = 'web-mercator',
+    level: int,
+    pixels_per_tile: int = 128,
+    resampling: str | dict = 'average',
+    extra_dim: str = None,
+    clear_attrs: bool = False,
+) -> xr.Dataset:
+    """Create a level of a multiscale pyramid of a dataset via reprojection.
 
     Parameters
     ----------
     ds : xarray.Dataset
-        The dataset to coarsen.
-    factors : list[int]
-        The factors to coarsen by.
-    dims : list[str]
-        The dimensions to coarsen.
-    kwargs : dict
-        Additional keyword arguments to pass to xarray.Dataset.coarsen.
-    """
+        The dataset to create a multiscale pyramid of.
+    projection : str, optional
+        The projection to use. Default is 'web-mercator'.
+    level : int
+        The level of the pyramid to create.
+    pixels_per_tile : int, optional
+        Number of pixels per tile
+    resampling : dict
+        Rasterio warp resampling method to use. Keys are variable names and values are warp resampling methods.
+    extra_dim : str, optional
+        The name of the extra dimension to iterate over. Default is None.
+    clear_attrs : bool, False
+        Clear the attributes of the DataArrays within the multiscale level. Default is False.
+
+    Returns
+    -------
+    xr.Dataset
+        The multiscale pyramid level.
 
-    # multiscales spec
-    save_kwargs = locals()
-    del save_kwargs['ds']
+    Warning
+    -------
+    Pyramid generation by level is experimental and subject to change.
+    """
+    projection_model = Projection(name=projection)
+    dim = 2**level * pixels_per_tile
+    dst_transform = projection_model.transform(dim=dim)
+    save_kwargs = {
+        'level': level,
+        'pixels_per_tile': pixels_per_tile,
+        'projection': projection,
+        'resampling': resampling,
+        'extra_dim': extra_dim,
+        'clear_attrs': clear_attrs,
+    }
 
     attrs = {
         'multiscales': multiscales_template(
-            datasets=[{'path': str(i)} for i in range(len(factors))],
+            datasets=[{'path': '.', 'level': level, 'crs': projection_model._crs}],
             type='reduce',
-            method='pyramid_coarsen',
+            method='pyramid_reproject',
             version=get_version(),
             kwargs=save_kwargs,
         )
     }
 
-    # set up pyramid
-    plevels = {}
-
-    # pyramid data
-    for key, factor in enumerate(factors):
-        # merge dictionary via union operator
-        kwargs |= {d: factor for d in dims}
-        plevels[str(key)] = ds.coarsen(**kwargs).mean()
+    # Convert resampling from string to dictionary if necessary
+    if isinstance(resampling, str):
+        resampling_dict: dict = defaultdict(lambda: resampling)
+    else:
+        resampling_dict = resampling
 
-    plevels['/'] = xr.Dataset(attrs=attrs)
-    return dt.DataTree.from_dict(plevels)
+    # create the data array for each level
+    ds_level = xr.Dataset(attrs=ds.attrs)
+    for k, da in ds.items():
+        if clear_attrs:
+            da.attrs.clear()
+        if len(da.shape) == 4:
+            # if extra_dim is not specified, raise an error
+            if extra_dim is None:
+                raise ValueError("must specify 'extra_dim' to iterate over 4d data")
+            da_all = []
+            for index in ds[extra_dim]:
+                # reproject each index of the 4th dimension
+                da_reprojected = _da_reproject(
+                    da.sel({extra_dim: index}),
+                    dim=dim,
+                    crs=projection_model._crs,
+                    resampling=Resampling[resampling_dict[k]],
+                    transform=dst_transform,
+                )
+                da_all.append(da_reprojected)
+            ds_level[k] = xr.concat(da_all, ds[extra_dim])
+        else:
+            # if the data array is not 4D, just reproject it
+            ds_level[k] = _da_reproject(
+                da,
+                dim=dim,
+                crs=projection_model._crs,
+                resampling=Resampling[resampling_dict[k]],
+                transform=dst_transform,
+            )
+    ds_level.attrs['multiscales'] = attrs['multiscales']
+    return ds_level
 
 
 def pyramid_reproject(
     ds: xr.Dataset,
     *,
-    projection:typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator',
+    projection: ProjectionOptions = 'web-mercator',
     levels: int = None,
     pixels_per_tile: int = 128,
     other_chunks: dict = None,
     resampling: str | dict = 'average',
     extra_dim: str = None,
+    clear_attrs: bool = False,
 ) -> dt.DataTree:
-
     """Create a multiscale pyramid of a dataset via reprojection.
 
     Parameters
     ----------
     ds : xarray.Dataset
         The dataset to create a multiscale pyramid of.
     projection : str, optional
@@ -81,80 +154,67 @@
     other_chunks : dict
         Chunks for non-spatial dims to pass to :py:meth:`~xr.Dataset.chunk`. Default is None
     resampling : str or dict, optional
         Rasterio warp resampling method to use. Default is 'average'.
         If a dict, keys are variable names and values are warp resampling methods.
     extra_dim : str, optional
         The name of the extra dimension to iterate over. Default is None.
+    clear_attrs : bool, False
+        Clear the attributes of the DataArrays within the multiscale pyramid. Default is False.
 
     Returns
     -------
     dt.DataTree
         The multiscale pyramid.
 
     """
-
-    import rioxarray  # noqa: F401
-    from rasterio.warp import Resampling
-
-    # multiscales spec
-    save_kwargs = {'levels': levels, 'pixels_per_tile': pixels_per_tile}
+    if not levels:
+        levels = get_levels(ds)
+    projection_model = Projection(name=projection)
+    save_kwargs = {
+        'levels': levels,
+        'pixels_per_tile': pixels_per_tile,
+        'projection': projection,
+        'other_chunks': other_chunks,
+        'resampling': resampling,
+        'extra_dim': extra_dim,
+        'clear_attrs': clear_attrs,
+    }
     attrs = {
         'multiscales': multiscales_template(
-            datasets=[{'path': str(i)} for i in range(levels)],
+            datasets=[
+                {'path': str(i), 'level': i, 'crs': projection_model._crs} for i in range(levels)
+            ],
             type='reduce',
             method='pyramid_reproject',
             version=get_version(),
             kwargs=save_kwargs,
         )
     }
 
-    # Convert resampling from string to dictionary if necessary
-    if isinstance(resampling, str):
-        resampling_dict = defaultdict(lambda: resampling)
-    else:
-        resampling_dict = resampling
-
-    projection_model = Projection(name=projection)
-
     # set up pyramid
     plevels = {}
 
     # pyramid data
     for level in range(levels):
-        lkey = str(level)
-        dim = 2**level * pixels_per_tile
-        dst_transform = projection_model.transform(dim=dim)
-
-        def reproject(da, var):
-            return da.rio.reproject(
-                projection_model._crs,
-                resampling=Resampling[resampling_dict[var]],
-                shape=(dim, dim),
-                transform=dst_transform,
-            )
-
-        # create the data array for each level
-        plevels[lkey] = xr.Dataset(attrs=ds.attrs)
-        for k, da in ds.items():
-            if len(da.shape) == 4:
-                # if extra_dim is not specified, raise an error
-                if extra_dim is None:
-                    raise ValueError("must specify 'extra_dim' to iterate over 4d data")
-                da_all = []
-                for index in ds[extra_dim]:
-                    # reproject each index of the 4th dimension
-                    da_reprojected = reproject(da.sel({extra_dim: index}), k)
-                    da_all.append(da_reprojected)
-                plevels[lkey][k] = xr.concat(da_all, ds[extra_dim])
-            else:
-                # if the data array is not 4D, just reproject it
-                plevels[lkey][k] = reproject(da, k)
+        plevels[str(level)] = level_reproject(
+            ds,
+            projection=projection,
+            level=level,
+            pixels_per_tile=pixels_per_tile,
+            resampling=resampling,
+            extra_dim=extra_dim,
+            clear_attrs=clear_attrs,
+        )
 
     # create the final multiscale pyramid
     plevels['/'] = xr.Dataset(attrs=attrs)
     pyramid = dt.DataTree.from_dict(plevels)
 
     pyramid = add_metadata_and_zarr_encoding(
-        pyramid, levels=levels, pixels_per_tile=pixels_per_tile, other_chunks=other_chunks, projection=projection_model
+        pyramid,
+        levels=levels,
+        pixels_per_tile=pixels_per_tile,
+        other_chunks=other_chunks,
+        projection=projection_model,
     )
     return pyramid
```

### Comparing `ndpyramid-0.1.0/ndpyramid/regrid.py` & `ndpyramid-0.2.0/ndpyramid/regrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,19 @@
     n_out, n_in = ds_w.attrs['n_out'], ds_w.attrs['n_in']
     crds = np.stack([row, col])
     return xr.DataArray(
         sparse.COO(crds, s, (n_out, n_in)), dims=('out_dim', 'in_dim'), name='weights'
     )
 
 
-def make_grid_ds(level: int, pixels_per_tile: int = 128, projection:typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator') -> xr.Dataset:
+def make_grid_ds(
+    level: int,
+    pixels_per_tile: int = 128,
+    projection: typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator',
+) -> xr.Dataset:
     """Make a dataset representing a target grid
 
     Parameters
     ----------
     level : int
         The zoom level to compute the grid for. Level zero is the furthest out zoom level
     pixels_per_tile : int, optional
@@ -67,22 +71,21 @@
     projection_model = Projection(name=projection)
 
     dim = (2**level) * pixels_per_tile
 
     transform = projection_model.transform(dim=dim)
 
     if projection_model.name == 'equidistant-cylindrical':
-        title='Equidistant Cylindrical Grid'
+        title = 'Equidistant Cylindrical Grid'
 
     elif projection_model.name == 'web-mercator':
-        title='Web Mercator Grid'
+        title = 'Web Mercator Grid'
 
     p = projection_model._proj
 
-
     grid_shape = (dim, dim)
     bounds_shape = (dim + 1, dim + 1)
 
     xs = np.empty(grid_shape)
     ys = np.empty(grid_shape)
     lat = np.empty(grid_shape)
     lon = np.empty(grid_shape)
@@ -112,15 +115,18 @@
             'lat_b': xr.DataArray(lat_b, dims=['y_b', 'x_b']),
             'lon_b': xr.DataArray(lon_b, dims=['y_b', 'x_b']),
         },
         attrs=dict(title=title, Conventions='CF-1.8'),
     )
 
 
-def make_grid_pyramid(levels: int = 6, projection:typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator') -> dt.DataTree:
+def make_grid_pyramid(
+    levels: int = 6,
+    projection: typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator',
+) -> dt.DataTree:
     """helper function to create a grid pyramid for use with xesmf
 
     Parameters
     ----------
     levels : int, optional
         Number of levels in pyramid, by default 6
 
@@ -132,17 +138,19 @@
     plevels = {
         str(level): make_grid_ds(level, projection=projection).chunk(-1) for level in range(levels)
     }
     return dt.DataTree.from_dict(plevels)
 
 
 def generate_weights_pyramid(
-    ds_in: xr.Dataset, levels: int, method: str = 'bilinear', regridder_kws: dict = None,
-    projection:typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator'
-
+    ds_in: xr.Dataset,
+    levels: int,
+    method: str = 'bilinear',
+    regridder_kws: dict = None,
+    projection: typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator',
 ) -> dt.DataTree:
     """helper function to generate weights for a multiscale regridder
 
     Parameters
     ----------
     ds_in : xr.Dataset
         Input dataset to regrid
@@ -176,24 +184,23 @@
     root = xr.Dataset(attrs={'levels': levels, 'regrid_method': method})
     plevels['/'] = root
     return dt.DataTree.from_dict(plevels)
 
 
 def pyramid_regrid(
     ds: xr.Dataset,
-    projection:typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator',
+    projection: typing.Literal['web-mercator', 'equidistant-cylindrical'] = 'web-mercator',
     target_pyramid: dt.DataTree = None,
     levels: int = None,
     weights_pyramid: dt.DataTree = None,
     method: str = 'bilinear',
     regridder_kws: dict = None,
     regridder_apply_kws: dict = None,
     other_chunks: dict = None,
     pixels_per_tile: int = 128,
-
 ) -> dt.DataTree:
     """Make a pyramid using xesmf's regridders
 
     Parameters
     ----------
     ds : xr.Dataset
         Input dataset
@@ -232,29 +239,38 @@
     if levels is None:
         levels = len(target_pyramid.keys())  # TODO: get levels from the pyramid metadata
 
     regridder_kws = {} if regridder_kws is None else regridder_kws
     regridder_kws = {'periodic': True, **regridder_kws}
 
     # multiscales spec
-    save_kwargs = locals()
-    del save_kwargs['ds']
-    del save_kwargs['target_pyramid']
-    del save_kwargs['xe']
-    del save_kwargs['weights_pyramid']
+    projection_model = Projection(name=projection)
+    save_kwargs = {
+        'levels': levels,
+        'pixels_per_tile': pixels_per_tile,
+        'projection': projection,
+        'other_chunks': other_chunks,
+        'method': method,
+        'regridder_kws': regridder_kws,
+        'regridder_apply_kws': regridder_apply_kws,
+    }
 
     attrs = {
         'multiscales': multiscales_template(
-            datasets=[{'path': str(i)} for i in range(levels)],
+            datasets=[
+                {'path': str(i), 'level': i, 'crs': projection_model._crs} for i in range(levels)
+            ],
             type='reduce',
             method='pyramid_regrid',
             version=get_version(),
             kwargs=save_kwargs,
         )
     }
+    save_kwargs.pop('levels')
+    save_kwargs.pop('other_chunks')
 
     # set up pyramid
 
     plevels = {}
 
     # pyramid data
     for level in range(levels):
@@ -273,17 +289,31 @@
                 ds, grid, method, reuse_weights=True, weights=weights, **regridder_kws
             )
         # regrid
         if regridder_apply_kws is None:
             regridder_apply_kws = {}
         regridder_apply_kws = {**{'keep_attrs': True}, **regridder_apply_kws}
         plevels[str(level)] = regridder(ds, **regridder_apply_kws)
+        level_attrs = {
+            'multiscales': multiscales_template(
+                datasets=[{'path': '.', 'level': level, 'crs': projection_model._crs}],
+                type='reduce',
+                method='pyramid_regrid',
+                version=get_version(),
+                kwargs=save_kwargs,
+            )
+        }
+        plevels[str(level)].attrs['multiscales'] = level_attrs['multiscales']
 
     root = xr.Dataset(attrs=attrs)
     plevels['/'] = root
     pyramid = dt.DataTree.from_dict(plevels)
 
     pyramid = add_metadata_and_zarr_encoding(
-        pyramid, levels=levels, other_chunks=other_chunks, pixels_per_tile=pixels_per_tile, projection=Projection(name=projection)
+        pyramid,
+        levels=levels,
+        other_chunks=other_chunks,
+        pixels_per_tile=pixels_per_tile,
+        projection=Projection(name=projection),
     )
 
     return pyramid
```

### Comparing `ndpyramid-0.1.0/ndpyramid/utils.py` & `ndpyramid-0.2.0/ndpyramid/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 }
 
 
 def get_version() -> str:
     return __version__
 
 
+def get_levels(ds: xr.Dataset) -> int:
+    raise NotImplementedError('Automatic determination of number of levels is not yet implemented')
+
+
 def multiscales_template(
     *,
     datasets: list = None,
     type: str = '',
     method: str = '',
     version: str = '',
     args: list = None,
@@ -57,71 +61,96 @@
 
 
 def set_zarr_encoding(
     ds: xr.Dataset,
     codec_config: dict | None = None,
     float_dtype: npt.DTypeLike | None = None,
     int_dtype: npt.DTypeLike | None = None,
+    datetime_dtype: npt.DTypeLike | None = None,
+    object_dtype: npt.DTypeLike | None = None,
 ) -> xr.Dataset:
     """Set zarr encoding for each variable in the dataset
 
     Parameters
     ----------
     ds : xr.Dataset
         Input dataset
     codec_config : dict, optional
         Dictionary of parameters to pass to numcodecs.get_codec.
         The default is {'id': 'zlib', 'level': 1}
     float_dtype : str or dtype, optional
         Dtype to cast floating point variables to
+    int_dtype : str or dtype, optional
+        Dtype to cast integer variables to
+    object_dtype : str or dtype, optional
+        Dtype to cast object variables to.
+    datetime_dtype : str or dtype, optional
+        Dtype to encode numpy.datetime64 variables as.
+        Time coordinates are encoded as 'int32' if cf_xarray
+        is able to identify the coordinates representing time,
+        even if `datetime_dtype` is None.
+
 
     Returns
     -------
     ds : xr.Dataset
         Output dataset with updated variable encodings
+
+    Notes
+    -----
+    The *_dtype parameters can be used to coerce variables into data types
+    readable by Zarr implementations in other languages.
     """
     import numcodecs
 
     ds = ds.copy()
 
     if codec_config is None:
         codec_config = {'id': 'zlib', 'level': 1}
     compressor = numcodecs.get_codec(codec_config)
 
     time_vars = ds.cf.axes.get('T', []) + ds.cf.bounds.get('T', [])
     for varname, da in ds.variables.items():
-        # maybe cast float type
+        # remove old encoding
+        da.encoding.clear()
+
+        # maybe cast data type
         if np.issubdtype(da.dtype, np.floating) and float_dtype is not None:
             da = da.astype(float_dtype)
-
-        if np.issubdtype(da.dtype, np.integer) and int_dtype is not None:
+            da.encoding['dtype'] = str(float_dtype)
+        elif np.issubdtype(da.dtype, np.integer) and int_dtype is not None:
             da = da.astype(int_dtype)
-
-        # remove old encoding
-        da.encoding.clear()
+            da.encoding['dtype'] = str(int_dtype)
+        elif da.dtype == 'O' and object_dtype is not None:
+            da = da.astype(object_dtype)
+            da.encoding['dtype'] = str(object_dtype)
+        elif np.issubdtype(da.dtype, np.datetime64) and datetime_dtype is not None:
+            da.encoding['dtype'] = str(datetime_dtype)
+        elif varname in time_vars:
+            da.encoding['dtype'] = 'int32'
 
         # update with new encoding
         da.encoding['compressor'] = compressor
         with contextlib.suppress(KeyError):
             del da.attrs['_FillValue']
         da.encoding['_FillValue'] = default_fillvals.get(da.dtype.str[-2:], None)
 
-        # TODO: handle date/time types
-        # set encoding for time and time_bnds
-        if varname in time_vars:
-            da.encoding['dtype'] = 'int32'
         ds[varname] = da
 
     return ds
 
 
 def add_metadata_and_zarr_encoding(
-    pyramid: dt.DataTree, *, levels: int, other_chunks: dict = None, pixels_per_tile: int = 128, projection: Projection = None
+    pyramid: dt.DataTree,
+    *,
+    levels: int,
+    other_chunks: dict = None,
+    pixels_per_tile: int = 128,
+    projection: Projection = None,
 ) -> dt.DataTree:
-
     '''Postprocess data pyramid. Adds multiscales metadata and sets Zarr encoding
 
     Parameters
     ----------
     pyramid : dt.DataTree
         Input data pyramid
     levels : int
@@ -133,14 +162,21 @@
     projection: Projection
         Projection model of the pyramids
 
     Returns
     -------
     dt.DataTree
         Updated data pyramid with metadata / encoding set
+
+    Notes
+    -----
+    The variables within the pyramid are coerced into data types readable by
+    `@carbonplan/maps`. See https://ndpyramid.readthedocs.io/en/latest/schema.html
+    for more information. Raise an issue in https://github.com/carbonplan/ndpyramid
+    if more flexibility is needed.
     '''
     chunks = {'x': pixels_per_tile, 'y': pixels_per_tile}
     if other_chunks is not None:
         chunks |= other_chunks
 
     for level in range(levels):
         slevel = str(level)
@@ -148,13 +184,18 @@
         if projection:
             pyramid.ds.attrs['multiscales'][0]['datasets'][level]['crs'] = projection._crs
         # set dataset chunks
         pyramid[slevel].ds = pyramid[slevel].ds.chunk(chunks)
 
         # set dataset encoding
         pyramid[slevel].ds = set_zarr_encoding(
-            pyramid[slevel].ds, codec_config={'id': 'zlib', 'level': 1}, float_dtype='float32'
+            pyramid[slevel].ds,
+            codec_config={'id': 'zlib', 'level': 1},
+            float_dtype='float32',
+            int_dtype='int32',
+            datetime_dtype='int32',
+            object_dtype='str',
         )
 
     # set global metadata
     pyramid.ds.attrs.update({'title': 'multiscale data pyramid', 'version': __version__})
     return pyramid
```

### Comparing `ndpyramid-0.1.0/ndpyramid.egg-info/SOURCES.txt` & `ndpyramid-0.2.0/ndpyramid.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 .gitignore
 .pre-commit-config.yaml
 .prettierrc.toml
+.readthedocs.yaml
 LICENSE
 README.md
 codecov.yml
 pyproject.toml
 .github/dependabot.yml
+.github/workflows/codspeed.yml
 .github/workflows/main.yaml
 .github/workflows/pypi-release.yaml
+ci/doc.yml
 ci/environment.yml
+docs/Makefile
+docs/api.rst
+docs/conf.py
+docs/generate-pyramids.md
+docs/index.rst
+docs/make.bat
+docs/quick-start.md
+docs/schema.md
+docs/_static/monogram-dark-cropped.png
+docs/_static/monogram-light-cropped.png
 ndpyramid/__init__.py
 ndpyramid/_version.py
+ndpyramid/coarsen.py
 ndpyramid/common.py
-ndpyramid/core.py
+ndpyramid/create.py
 ndpyramid/regrid.py
+ndpyramid/reproject.py
+ndpyramid/testing.py
 ndpyramid/utils.py
 ndpyramid.egg-info/PKG-INFO
 ndpyramid.egg-info/SOURCES.txt
 ndpyramid.egg-info/dependency_links.txt
 ndpyramid.egg-info/requires.txt
 ndpyramid.egg-info/top_level.txt
 notebooks/demo.ipynb
```

### Comparing `ndpyramid-0.1.0/notebooks/demo.ipynb` & `ndpyramid-0.2.0/notebooks/demo.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9187804864861688%*

 * *Differences: {"'cells'": '{0: {\'id\': \'0\', \'source\': {insert: [(0, \'<p align="left" >\\n\'), (1, "<a '*

 * *            'href=\'https://carbonplan.org\'>\\n"), (2, \'<picture>\\n\'), (3, \'  <source '*

 * *            'media="(prefers-color-scheme: dark)" '*

 * *            'srcset="https://carbonplan-assets.s3.amazonaws.com/monogram/light-small.png">\\n\'), '*

 * *            '(4, \'  <img alt="CarbonPlan monogram." width="48" '*

 * *            'src="https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png">\\n\'), (5, '*

 * *      […]*

```diff
@@ -1,125 +1,129 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "270cab20",
+            "id": "0",
             "metadata": {},
             "source": [
-                "<img width=\"50\" src=\"https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png\" style=\"margin-left:0px;margin-top:20px\"/>\n",
+                "<p align=\"left\" >\n",
+                "<a href='https://carbonplan.org'>\n",
+                "<picture>\n",
+                "  <source media=\"(prefers-color-scheme: dark)\" srcset=\"https://carbonplan-assets.s3.amazonaws.com/monogram/light-small.png\">\n",
+                "  <img alt=\"CarbonPlan monogram.\" width=\"48\" src=\"https://carbonplan-assets.s3.amazonaws.com/monogram/dark-small.png\">\n",
+                "</picture>\n",
+                "</a>\n",
+                "</p>\n",
                 "\n",
                 "# Demo map data preparation\n",
                 "\n",
-                "_by Joe Hamman & Jeremy Freeman (CarbonPlan), September 27, 2021_\n",
+                "_by Joe Hamman & Jeremy Freeman (CarbonPlan), September 27, 2021, Updated by Max Jones (CarbonPlan), February 8, 2024_\n",
                 "\n",
                 "This notebook demonstrates the production of Zarr data pyramids for use with\n",
                 "[`@carbonplan/maps`](https://github.com/carbonplan/maps), an api for interactive\n",
                 "multi-dimensional data-driven web maps.\n",
                 "\n",
                 "Some of the libraries used here are in pre-release condition. Specifically\n",
                 "`ndpyramid` and `datatree` are currently udergoing rapid development. Use the\n",
-                "pattern below but expect changes to the specific apis.\n"
+                "pattern below but expect changes to the specific apis.\n",
+                "\n",
+                "All of the libraries used in this demonstration are included in [this conda environment file](https://github.com/carbonplan/ndpyramid/blob/main/ci/environment.yml).\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "076c0441",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import xarray as xr\n",
                 "import pandas as pd\n",
-                "import rioxarray\n",
-                "from ndpyramid import pyramid_reproject\n",
-                "from carbonplan_data.utils import set_zarr_encoding\n",
-                "from carbonplan_data.metadata import get_cf_global_attrs"
+                "import xarray as xr\n",
+                "\n",
+                "from ndpyramid import pyramid_reproject"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f8de434a",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "VERSION = 2\n",
                 "LEVELS = 6\n",
                 "PIXELS_PER_TILE = 128\n",
-                "\n",
-                "input_path = f\"gs://carbonplan-maps/v{VERSION}/demo/raw\"\n",
-                "save_path = f\"gs://carbonplan-maps/v{VERSION}/demo/\""
+                "S3 = False\n",
+                "input_path = f\"s3://carbonplan-maps/v{VERSION}/demo/raw\"\n",
+                "if S3:\n",
+                "    base = f\"s3://carbonplan-maps/v{VERSION}/demo/\"\n",
+                "    store_2d = base + \"2d/tavg\"\n",
+                "    store_3d = base + \"3d/tavg-prec\"\n",
+                "    store_3d_1var = base + \"3d/tavg-month\"\n",
+                "    store_4d = base + \"4d/tavg-prec-month\"\n",
+                "else:\n",
+                "    import zarr\n",
+                "\n",
+                "    store_2d = zarr.storage.MemoryStore()\n",
+                "    store_3d = zarr.storage.MemoryStore()\n",
+                "    store_3d_1var = zarr.storage.MemoryStore()\n",
+                "    store_4d = zarr.storage.MemoryStore()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9a2af554",
+            "id": "3",
             "metadata": {},
             "source": [
                 "## 2d (tavg)\n",
                 "\n",
                 "In this example we open a single 2d image (GeoTIFF) and create a Zarr pyramid.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e8629d34",
+            "id": "4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%time\n",
                 "# input dataset\n",
                 "path = f\"{input_path}/wc2.1_2.5m_tavg_10.tif\"\n",
-                "\n",
                 "# open and extract the input dataset\n",
                 "ds = (\n",
                 "    xr.open_dataarray(path, engine=\"rasterio\")\n",
                 "    .to_dataset(name=\"tavg\")\n",
                 "    .squeeze()\n",
                 "    .reset_coords([\"band\"], drop=True)\n",
                 ")\n",
                 "\n",
                 "# create the pyramid\n",
-                "dt = pyramid_reproject(ds, levels=LEVELS)\n",
-                "\n",
-                "# modify the data in the pyramid\n",
-                "for child in dt.children.values():\n",
-                "    child.ds = set_zarr_encoding(\n",
-                "        child.ds, codec_config={\"id\": \"zlib\", \"level\": 1}, float_dtype=\"float32\"\n",
-                "    )\n",
-                "    child.ds = child.ds.chunk({\"x\": PIXELS_PER_TILE, \"y\": PIXELS_PER_TILE})\n",
-                "    child.ds[\"tavg\"].attrs.clear()\n",
-                "dt.attrs = get_cf_global_attrs(version=VERSION)\n",
-                "\n",
-                "for level in range(LEVELS):\n",
-                "    slevel = str(level)\n",
-                "    dt.ds.attrs['multiscales'][0]['datasets'][level]['pixels_per_tile'] = PIXELS_PER_TILE\n",
-                "dt.ds.attrs['multiscales'][0]['metadata']['version'] = VERSION\n",
+                "dt = pyramid_reproject(ds, levels=LEVELS, clear_attrs=True)\n",
                 "\n",
                 "# write the pyramid to zarr\n",
-                "dt.to_zarr(save_path + \"2d/tavg\", consolidated=True)"
+                "dt.to_zarr(store_2d, consolidated=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f845a5db",
+            "id": "5",
             "metadata": {},
             "source": [
                 "## 3d, two variables (tavg and prec)\n",
                 "\n",
                 "In this example, we open two 2d images (temperature and precipitation), combine\n",
                 "them into a single array (along the `band` dimension), and create a Zarr\n",
                 "pyramid.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "28e45eb9",
+            "id": "6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%time\n",
                 "# input datasets\n",
                 "path1 = f\"{input_path}/wc2.1_2.5m_tavg_10.tif\"\n",
                 "path2 = f\"{input_path}/wc2.1_2.5m_prec_10.tif\"\n",
@@ -133,59 +137,42 @@
                 ")\n",
                 "ds2 = (\n",
                 "    xr.open_dataarray(path2, engine=\"rasterio\")\n",
                 "    .to_dataset(name=\"climate\")\n",
                 "    .squeeze()\n",
                 "    .reset_coords([\"band\"], drop=True)\n",
                 ")\n",
-                "ds2[\"climate\"] = ds2[\"climate\"].astype(\"float32\")\n",
                 "ds2[\"climate\"].values[ds2[\"climate\"].values == ds2[\"climate\"].values[0, 0]] = ds1[\"climate\"].values[\n",
                 "    0, 0\n",
                 "]\n",
                 "ds = xr.concat([ds1, ds2], pd.Index([\"tavg\", \"prec\"], name=\"band\"))\n",
-                "ds[\"band\"] = ds[\"band\"].astype(\"str\")\n",
                 "\n",
                 "# create the pyramid\n",
-                "dt = pyramid_reproject(ds, levels=LEVELS)\n",
-                "\n",
-                "# modify the data in the pyramid\n",
-                "for child in dt.children.values():\n",
-                "    child.ds = set_zarr_encoding(\n",
-                "        child.ds, codec_config={\"id\": \"zlib\", \"level\": 1}, float_dtype=\"float32\"\n",
-                "    )\n",
-                "    child.ds = child.ds.chunk({\"x\": PIXELS_PER_TILE, \"y\": PIXELS_PER_TILE, \"band\": 2})\n",
-                "    child.ds[\"climate\"].attrs.clear()\n",
-                "dt.attrs = get_cf_global_attrs(version=VERSION)\n",
-                "\n",
-                "for level in range(LEVELS):\n",
-                "    slevel = str(level)\n",
-                "    dt.ds.attrs['multiscales'][0]['datasets'][level]['pixels_per_tile'] = PIXELS_PER_TILE\n",
-                "dt.ds.attrs['multiscales'][0]['metadata']['version'] = VERSION\n",
+                "dt = pyramid_reproject(ds, levels=LEVELS, other_chunks={'band': 2}, clear_attrs=True)\n",
                 "\n",
                 "# write the pyramid to zarr\n",
-                "dt.to_zarr(save_path + \"3d/tavg-prec\", consolidated=True)\n",
-                "dt.ds.attrs"
+                "dt.to_zarr(store_3d, consolidated=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cccd8513",
+            "id": "7",
             "metadata": {},
             "source": [
                 "## 3d, one variable, multiple time points\n",
                 "\n",
                 "In this example, we open 12 2d images (one map of temperature for each month),\n",
                 "combine them into a single array (along the `month` dimension), and create a\n",
                 "Zarr pyramid.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c6408ef2",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%time\n",
                 "# open and extract the input datasets\n",
                 "ds_all = []\n",
                 "months = list(map(lambda d: d + 1, range(12)))\n",
@@ -195,55 +182,38 @@
                 "        xr.open_dataarray(path, engine=\"rasterio\")\n",
                 "        .to_dataset(name=\"tavg\")\n",
                 "        .squeeze()\n",
                 "        .reset_coords([\"band\"], drop=True)\n",
                 "    )\n",
                 "    ds_all.append(ds)\n",
                 "ds = xr.concat(ds_all, pd.Index(months, name=\"month\"))\n",
-                "ds[\"month\"] = ds[\"month\"].astype(\"int32\")\n",
                 "\n",
                 "# create the pyramid\n",
-                "dt = pyramid_reproject(ds, levels=LEVELS)\n",
-                "\n",
-                "# modify the data in the pyramid\n",
-                "for child in dt.children.values():\n",
-                "    child.ds = set_zarr_encoding(\n",
-                "        child.ds, codec_config={\"id\": \"zlib\", \"level\": 1}, float_dtype=\"float32\"\n",
-                "    )\n",
-                "    child.ds = child.ds.chunk({\"x\": PIXELS_PER_TILE, \"y\": PIXELS_PER_TILE, \"month\": 12})\n",
-                "    child.ds[\"tavg\"].attrs.clear()\n",
-                "dt.attrs = get_cf_global_attrs(version=VERSION)\n",
-                "\n",
-                "for level in range(LEVELS):\n",
-                "    slevel = str(level)\n",
-                "    dt.ds.attrs['multiscales'][0]['datasets'][level]['pixels_per_tile'] = PIXELS_PER_TILE\n",
-                "dt.ds.attrs['multiscales'][0]['metadata']['version'] = VERSION\n",
-                "\n",
+                "dt = pyramid_reproject(ds, levels=LEVELS, other_chunks={'month': 12}, clear_attrs=True)\n",
                 "\n",
                 "# write the pyramid to zarr\n",
-                "dt.to_zarr(save_path + \"3d/tavg-month\", consolidated=True)\n",
-                "dt.ds.attrs"
+                "dt.to_zarr(store_3d_1var, consolidated=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a9c778b7",
+            "id": "9",
             "metadata": {},
             "source": [
                 "## 4d, multiple variables, multiple time points\n",
                 "\n",
                 "In this example, we open 12 2d images for 2 variables (one map of temperature\n",
                 "and precipitation for each month), combine them into a single array (along the\n",
                 "`month` and `band` dimensions), and create a Zarr pyramid.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d456314d",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%time\n",
                 "# open and extract the input datasets\n",
                 "ds1_all = []\n",
                 "ds2_all = []\n",
@@ -264,68 +234,48 @@
                 "        xr.open_dataarray(path, engine=\"rasterio\")\n",
                 "        .to_dataset(name=\"climate\")\n",
                 "        .squeeze()\n",
                 "        .reset_coords([\"band\"], drop=True)\n",
                 "    )\n",
                 "    ds2_all.append(ds)\n",
                 "ds2 = xr.concat(ds2_all, pd.Index(months, name=\"month\"))\n",
-                "ds1[\"month\"] = ds1[\"month\"].astype(\"int32\")\n",
-                "ds2[\"month\"] = ds2[\"month\"].astype(\"int32\")\n",
-                "ds2[\"climate\"] = ds2[\"climate\"].astype(\"float32\")\n",
                 "ds2[\"climate\"].values[ds2[\"climate\"].values == ds2[\"climate\"].values[0, 0, 0]] = ds1[\n",
                 "    \"climate\"\n",
                 "].values[0, 0, 0]\n",
                 "ds = xr.concat([ds1, ds2], pd.Index([\"tavg\", \"prec\"], name=\"band\"))\n",
-                "ds[\"band\"] = ds[\"band\"].astype(\"str\")\n",
                 "\n",
                 "# create the pyramid\n",
-                "dt = pyramid_reproject(ds, levels=LEVELS, extra_dim=\"band\")\n",
-                "for child in dt.children.values():\n",
-                "    child.ds = set_zarr_encoding(\n",
-                "        child.ds, codec_config={\"id\": \"zlib\", \"level\": 1}, float_dtype=\"float32\"\n",
-                "    )\n",
-                "    child.ds = child.ds.chunk({\"x\": PIXELS_PER_TILE, \"y\": PIXELS_PER_TILE, \"band\": 2, \"month\": 12})\n",
-                "    child.ds[\"climate\"].attrs.clear()\n",
-                "dt.attrs = get_cf_global_attrs(version=VERSION)\n",
-                "\n",
-                "for level in range(LEVELS):\n",
-                "    slevel = str(level)\n",
-                "    dt.ds.attrs['multiscales'][0]['datasets'][level]['pixels_per_tile'] = PIXELS_PER_TILE\n",
-                "dt.ds.attrs['multiscales'][0]['metadata']['version'] = VERSION\n",
-                "\n",
+                "dt = pyramid_reproject(\n",
+                "    ds, levels=LEVELS, extra_dim=\"band\", other_chunks={'band': 2, 'month': 12}, clear_attrs=True\n",
+                ")\n",
+                "dt.ds.attrs\n",
                 "\n",
                 "# write the pyramid to zarr\n",
-                "dt.to_zarr(save_path + \"4d/tavg-prec-month\", consolidated=True)\n",
-                "dt.ds.attrs"
+                "dt.to_zarr(store_4d, consolidated=True, mode=\"w\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a934685a",
+            "id": "11",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3",
-            "language": "python",
-            "name": "python3"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.12"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ndpyramid-0.1.0/pyproject.toml` & `ndpyramid-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,31 @@
     "xarray-datatree >= 0.0.11",
     "zarr",
     "pydantic>=1.10",
     "rasterio",
     "pyproj",
 ]
 
+
+[project.optional-dependencies]
+test = [
+    "dask",
+    "mercantile",
+    "pooch",
+    "pre-commit",
+    "pytest-benchmark",
+    "pytest-codspeed",
+    "pytest-cov",
+    "pytest-mypy",
+    "pytest",
+    "rioxarray",
+    "scipy",
+]
+
+
 [project.urls]
 repository = "https://github.com/carbonplan/ndpyramid"
 
 [tool.setuptools.packages.find]
 include = ["ndpyramid*"]
 
 [tool.setuptools_scm]
@@ -78,14 +95,16 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
+
+[tool.ruff.lint]
 per-file-ignores = {}
 # E402: module level import not at top of file
 # E501: line too long - let black worry about that
 # E731: do not assign a lambda expression, use a def
 ignore = ["E402", "E501", "E731"]
 select = [
     # Pyflakes
@@ -96,16 +115,20 @@
     # isort
     "I",
     # Pyupgrade
     "UP",
 ]
 
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 18
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["ndpyramid"]
 
 [tool.pytest.ini_options]
 console_output_style = "count"
 addopts = "--cov=./ --cov-report=xml --verbose"
+
+[tool.mypy]
+ignore_missing_imports = true
+no_implicit_optional = false
```

### Comparing `ndpyramid-0.1.0/tests/test_utils.py` & `ndpyramid-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

