# Comparing `tmp/dioptic.profileparser-0.2.1.tar.gz` & `tmp/dioptic_profileparser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptic.profileparser-0.2.1.tar", last modified: Wed Feb  7 17:36:14 2024, max compression
+gzip compressed data, was "dioptic_profileparser-0.3.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `dioptic.profileparser-0.2.1.tar` & `dioptic_profileparser-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.530697 dioptic.profileparser-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.526697 dioptic.profileparser-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.526697 dioptic.profileparser-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/.github/workflows/pypi-packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-07 17:36:14.530697 dioptic.profileparser-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.526697 dioptic.profileparser-0.2.1/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)   154785 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/cpp/peglib.h
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/cpp/processprofile.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.530697 dioptic.profileparser-0.2.1/dioptic.profileparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-07 17:36:14.000000 dioptic.profileparser-0.2.1/dioptic.profileparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-07 17:36:14.000000 dioptic.profileparser-0.2.1/dioptic.profileparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 17:36:14.000000 dioptic.profileparser-0.2.1/dioptic.profileparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 17:36:14.000000 dioptic.profileparser-0.2.1/dioptic.profileparser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.530697 dioptic.profileparser-0.2.1/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/js/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/js/profile_parser_js.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:36:14.530697 dioptic.profileparser-0.2.1/python/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/python/pyprofileparser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 17:36:14.530697 dioptic.profileparser-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-07 17:36:05.000000 dioptic.profileparser-0.2.1/setup.py
+-rw-r--r--   0        0        0     1747 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/.github/workflows/pypi-packages.yml
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/.github/workflows/web-package.yml
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/LICENSE
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/README.md
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/include/profileparser/types.hpp
+-rw-r--r--   0        0        0     5633 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/include/profileparser/utils.hpp
+-rw-r--r--   0        0        0     1874 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/include/profileparser.hpp
+-rw-r--r--   0        0        0      620 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/lineinfo.cpp
+-rw-r--r--   0        0        0    17677 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/parser.cpp
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/parser.hpp
+-rw-r--r--   0        0        0   154785 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/peglib.h
+-rw-r--r--   0        0        0     9760 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/printers.cpp
+-rw-r--r--   0        0        0     4502 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/cpp/validation.cpp
+-rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1510 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/python/CMakeLists.txt
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/python/__init__.py
+-rw-r--r--   0        0        0     7192 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/python/pyprofileparser.cpp
+-rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/web/CMakeLists.txt
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/web/README.md
+-rw-r--r--   0        0        0     6309 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/web/binding_api.hpp
+-rw-r--r--   0        0        0     9441 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/web/binding_ast.hpp
+-rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/web/binding_helpers.hpp
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/web/profile_parser_js.cpp
+-rw-r--r--   0        0        0      399 2022-11-09 12:37:21.000000 dioptic_profileparser-0.3.0/PKG-INFO
```

### Comparing `dioptic.profileparser-0.2.1/.github/workflows/pypi-packages.yml` & `dioptic_profileparser-0.3.0/.github/workflows/pypi-packages.yml`

 * *Files 27% similar despite different names*

```diff
@@ -7,56 +7,57 @@
     tags:
       - v[0-9]+.**
 
 jobs:
   build-sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Build sdist package
         run: |
           python -m pip install pip build --upgrade
           python -m build --sdist
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: packages
+          name: packages-src
           path: "dist/*.tar.gz"
 
   build-win64-wheels:
     runs-on: windows-latest
     strategy:
       matrix:
         python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: ilammy/msvc-dev-cmd@v1
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Build wheel for py${{ matrix.python-version }}
         run: |
           python -m pip install pip build --upgrade
           python -m build --wheel
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: packages
+          name: packages-win-py${{ matrix.python-version }}
           path: "dist/*.whl"
 
   pypi-publish:
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs: [build-sdist, build-win64-wheels]
     runs-on: ubuntu-latest
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
-        name: packages
         path: dist
+        pattern: packages-*
+        merge-multiple: true
     - name: Test PyPI publish
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
         skip-existing: true
     - name: PyPI publish
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dioptic.profileparser-0.2.1/LICENSE` & `dioptic_profileparser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dioptic.profileparser-0.2.1/cpp/peglib.h` & `dioptic_profileparser-0.3.0/cpp/peglib.h`

 * *Files identical despite different names*

