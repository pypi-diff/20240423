# Comparing `tmp/precommend-0.2.2.tar.gz` & `tmp/precommend-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precommend-0.2.2.tar", last modified: Fri Apr 19 08:50:28 2024, max compression
+gzip compressed data, was "precommend-0.3.0.tar", last modified: Tue Apr 23 13:21:01 2024, max compression
```

## Comparing `precommend-0.2.2.tar` & `precommend-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 08:50:23.000000 precommend-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-19 08:50:23.000000 precommend-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-19 08:50:23.000000 precommend-0.2.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-19 08:50:23.000000 precommend-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 08:50:23.000000 precommend-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 08:50:23.000000 precommend-0.2.2/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 08:50:23.000000 precommend-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 08:50:23.000000 precommend-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-19 08:50:28.472251 precommend-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 08:50:23.000000 precommend-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/precommend/
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/precommend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 08:50:23.000000 precommend-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:50:28.472251 precommend-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 08:50:23.000000 precommend-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 08:50:23.000000 precommend-0.2.2/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/cpp/test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/generic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/generic/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/generic/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/generic/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/generic/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/generic/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/python/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.229344 precommend-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.221344 precommend-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:20:54.000000 precommend-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.221344 precommend-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 13:20:54.000000 precommend-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 13:20:54.000000 precommend-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 13:20:54.000000 precommend-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-23 13:20:54.000000 precommend-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 13:20:54.000000 precommend-0.3.0/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-23 13:20:54.000000 precommend-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 13:20:54.000000 precommend-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-23 13:21:01.229344 precommend-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 13:20:54.000000 precommend-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-23 13:20:54.000000 precommend-0.3.0/bump_identify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/precommend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/precommend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-23 13:20:54.000000 precommend-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:21:01.229344 precommend-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 13:20:54.000000 precommend-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 13:20:54.000000 precommend-0.3.0/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.221344 precommend-0.3.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/cpp/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/generic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/generic/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/generic/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/generic/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/generic/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/generic/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/python/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/test_core.py
```

### Comparing `precommend-0.2.2/.github/workflows/ci.yml` & `precommend-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/.github/workflows/pypi.yml` & `precommend-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/.gitignore` & `precommend-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/.pre-commit-config.yaml` & `precommend-0.3.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     hooks:
       - id: synchronize-files
         name: Synchronize files within the repository
         entry: python sync.py
         language: system
         always_run: true
         pass_filenames: false
+      - id: bump-precommit-and-identify
+        name: Bump versions of pre-commit and identify
+        entry: python bump_identify.py
+        language: system
+        always_run: true
+        pass_filenames: false
 
   - repo: https://github.com/psf/black
     rev: 24.4.0
     hooks:
       - id: black  # Run Black - the uncompromising Python code formatter
       - id: black-jupyter  # Run Black - the uncompromising Python code formatter (Jupyter version)
 
@@ -53,15 +59,15 @@
     hooks:
       - id: cmake-format  # Apply formatting to CMake files
         additional_dependencies:
           - pyyaml
       - id: cmake-lint  # Apply linting to CMake files
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.3
+    rev: v18.1.4
     hooks:
       - id: clang-format  # Format C++ code with Clang-Format - automatically applying the changes
         types_or: [c++, c, c#, cuda, objective-c]
         args:
         - --style=Mozilla
 
   - repo: https://github.com/asottile/setup-cfg-fmt
```

### Comparing `precommend-0.2.2/LICENSE.md` & `precommend-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/PKG-INFO` & `precommend-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.2.2
+Version: 0.3.0
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.md
 Requires-Dist: click
-Requires-Dist: identify>=2.5.35
-Requires-Dist: pre-commit>=3.6.2
+Requires-Dist: identify>=2.5.36
+Requires-Dist: pre-commit>=3.7.0
 Requires-Dist: ruamel.yaml
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 # Welcome to precommend
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `precommend-0.2.2/README.md` & `precommend-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/precommend/.pre-commit-config.yaml` & `precommend-0.3.0/precommend/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     hooks:
       - id: synchronize-files
         name: Synchronize files within the repository
         entry: python sync.py
         language: system
         always_run: true
         pass_filenames: false
+      - id: bump-precommit-and-identify
+        name: Bump versions of pre-commit and identify
+        entry: python bump_identify.py
+        language: system
+        always_run: true
+        pass_filenames: false
 
   - repo: https://github.com/psf/black
     rev: 24.4.0
     hooks:
       - id: black  # Run Black - the uncompromising Python code formatter
       - id: black-jupyter  # Run Black - the uncompromising Python code formatter (Jupyter version)
 
@@ -53,15 +59,15 @@
     hooks:
       - id: cmake-format  # Apply formatting to CMake files
         additional_dependencies:
           - pyyaml
       - id: cmake-lint  # Apply linting to CMake files
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.3
+    rev: v18.1.4
     hooks:
       - id: clang-format  # Format C++ code with Clang-Format - automatically applying the changes
         types_or: [c++, c, c#, cuda, objective-c]
         args:
         - --style=Mozilla
 
   - repo: https://github.com/asottile/setup-cfg-fmt
```

### Comparing `precommend-0.2.2/precommend/__main__.py` & `precommend-0.3.0/precommend/__main__.py`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/precommend/core.py` & `precommend-0.3.0/precommend/core.py`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/precommend/rules.py` & `precommend-0.3.0/precommend/rules.py`

 * *Files identical despite different names*

### Comparing `precommend-0.2.2/precommend.egg-info/PKG-INFO` & `precommend-0.3.0/precommend.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.2.2
+Version: 0.3.0
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.md
 Requires-Dist: click
-Requires-Dist: identify>=2.5.35
-Requires-Dist: pre-commit>=3.6.2
+Requires-Dist: identify>=2.5.36
+Requires-Dist: pre-commit>=3.7.0
 Requires-Dist: ruamel.yaml
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 # Welcome to precommend
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `precommend-0.2.2/precommend.egg-info/SOURCES.txt` & `precommend-0.3.0/precommend.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 COPYING.md
 LICENSE.md
 MANIFEST.in
 README.md
+bump_identify.py
 pyproject.toml
 setup.py
 sync.py
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/pypi.yml
 precommend/.pre-commit-config.yaml
```

### Comparing `precommend-0.2.2/pyproject.toml` & `precommend-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "click",
-    "identify >= 2.5.35",
-    "pre-commit >= 3.6.2",
+    "identify >= 2.5.36",
+    "pre-commit >= 3.7.0",
     "ruamel.yaml",
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest",
 ]
```

### Comparing `precommend-0.2.2/tests/test_core.py` & `precommend-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

