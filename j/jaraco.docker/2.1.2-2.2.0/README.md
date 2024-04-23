# Comparing `tmp/jaraco.docker-2.1.2.tar.gz` & `tmp/jaraco_docker-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.docker-2.1.2.tar", last modified: Mon Feb 19 18:41:28 2024, max compression
+gzip compressed data, was "jaraco_docker-2.2.0.tar", last modified: Tue Apr 23 09:45:21 2024, max compression
```

## Comparing `jaraco.docker-2.1.2.tar` & `jaraco_docker-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:41:28.643280 jaraco.docker-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:41:28.639280 jaraco.docker-2.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:41:28.639280 jaraco.docker-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-02-19 18:41:28.643280 jaraco.docker-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:41:28.643280 jaraco.docker-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:41:28.643280 jaraco.docker-2.1.2/jaraco/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/jaraco/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:41:28.643280 jaraco.docker-2.1.2/jaraco.docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-02-19 18:41:28.000000 jaraco.docker-2.1.2/jaraco.docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-19 18:41:28.000000 jaraco.docker-2.1.2/jaraco.docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 18:41:28.000000 jaraco.docker-2.1.2/jaraco.docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-19 18:41:28.000000 jaraco.docker-2.1.2/jaraco.docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 18:41:28.000000 jaraco.docker-2.1.2/jaraco.docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-19 18:41:28.647280 jaraco.docker-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-19 18:41:03.000000 jaraco.docker-2.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.854989 jaraco_docker-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.850989 jaraco_docker-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.850989 jaraco_docker-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 09:45:21.854989 jaraco_docker-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.850989 jaraco_docker-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.846989 jaraco_docker-2.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.854989 jaraco_docker-2.2.0/jaraco/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/jaraco/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/jaraco/docker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.854989 jaraco_docker-2.2.0/jaraco.docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 09:45:21.000000 jaraco_docker-2.2.0/jaraco.docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 09:45:21.000000 jaraco_docker-2.2.0/jaraco.docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:45:21.000000 jaraco_docker-2.2.0/jaraco.docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 09:45:21.000000 jaraco_docker-2.2.0/jaraco.docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 09:45:21.000000 jaraco_docker-2.2.0/jaraco.docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:45:21.854989 jaraco_docker-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:45:21.854989 jaraco_docker-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/tests/mountinfo
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 09:44:56.000000 jaraco_docker-2.2.0/tox.ini
```

### Comparing `jaraco.docker-2.1.2/.github/workflows/main.yml` & `jaraco_docker-2.2.0/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 name: tests
 
 on:
   merge_group:
   push:
     branches-ignore:
-    # disabled for jaraco/skeleton#103
-    # - gh-readonly-queue/**  # Temporary merge queue-related GH-made branches
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
   pull_request:
 
 permissions:
   contents: read
 
 env:
   # Environment variable to support color support (jaraco/skeleton#66)
@@ -24,28 +27,30 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
```

### Comparing `jaraco.docker-2.1.2/LICENSE` & `jaraco_docker-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.docker-2.1.2/PKG-INFO` & `jaraco_docker-2.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: jaraco.docker
-Version: 2.1.2
+Version: 2.2.0
 Summary: Docker facilities
-Home-page: https://github.com/jaraco/jaraco.docker
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.docker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jaraco.functools
 Requires-Dist: jaraco.context
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
+Requires-Dist: importlib_resources; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.docker.svg
    :target: https://pypi.org/project/jaraco.docker
```

### Comparing `jaraco.docker-2.1.2/README.rst` & `jaraco_docker-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.docker-2.1.2/docs/conf.py` & `jaraco_docker-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.docker-2.1.2/jaraco/docker.py` & `jaraco_docker-2.2.0/jaraco/docker/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,40 @@
+import itertools
 import pathlib
+import re
 
 from jaraco.functools import apply
 from jaraco.context import suppress
 
 
 @apply(bool)
 @suppress(FileNotFoundError)
-def text_in_file(text: str, filename: pathlib.Path) -> bool:
+def text_in_file(text: str, filename: pathlib.Path, limit=None) -> bool:
     """
     >>> text_in_file('anything', pathlib.Path(__file__))
     True
     >>> text_in_file('bomb'*2, pathlib.Path(__file__))
     False
     >>> text_in_file('anything', pathlib.Path('/doesnotexist'))
     False
     """
     with filename.open(encoding='utf-8') as lines:
-        return any(text in line for line in lines)
+        return any(re.search(text, line) for line in itertools.islice(lines, limit))
 
 
 dockerenv = pathlib.Path('/.dockerenv')
 cgroup = pathlib.Path('/proc/self/cgroup')
+mountinfo = pathlib.Path('/proc/self/mountinfo')
 
 
 def is_docker() -> bool:
     """
     Is this current environment running in docker?
 
     >>> type(is_docker())
     <class 'bool'>
     """
-    return dockerenv.exists() or text_in_file('docker', cgroup)
+    return (
+        dockerenv.exists()
+        or text_in_file('docker', cgroup)
+        or text_in_file('docker|overlay', mountinfo, limit=1)
+    )
```

### Comparing `jaraco.docker-2.1.2/jaraco.docker.egg-info/PKG-INFO` & `jaraco_docker-2.2.0/jaraco.docker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: jaraco.docker
-Version: 2.1.2
+Version: 2.2.0
 Summary: Docker facilities
-Home-page: https://github.com/jaraco/jaraco.docker
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.docker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jaraco.functools
 Requires-Dist: jaraco.context
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
+Requires-Dist: importlib_resources; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.docker.svg
    :target: https://pypi.org/project/jaraco.docker
```

### Comparing `jaraco.docker-2.1.2/tox.ini` & `jaraco_docker-2.2.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 usedevelop = True
 extras =
 	testing
 
 [testenv:diffcov]
 description = run tests and check that diff from main is covered
 deps =
+	{[testenv]deps}
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
 [testenv:docs]
```

