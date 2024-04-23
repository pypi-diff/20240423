# Comparing `tmp/myst_docutils-2.0.0.tar.gz` & `tmp/myst_docutils-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myst_docutils-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "myst_docutils-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myst_docutils-2.0.0.tar` & `myst_docutils-3.0.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1746 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml
--rw-r--r--   0        0        0      834 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml
--rw-r--r--   0        0        0      692 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml
--rw-r--r--   0        0        0      185 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      598 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/dependabot.yml
--rwxr-xr-x   0        0        0     1711 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/workflows/docutils_setup.py
--rw-r--r--   0        0        0     2219 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/workflows/test-formats.yml
--rw-r--r--   0        0        0     4538 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1846 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.gitignore
--rw-r--r--   0        0        0     1125 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    41106 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/LICENSE
--rw-r--r--   0        0        0     2809 2023-06-13 16:30:47.723699 myst_docutils-2.0.0/README.md
--rw-r--r--   0        0        0      162 2023-06-13 16:30:44.591688 myst_docutils-2.0.0/codecov.yml
--rw-r--r--   0        0        0       71 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/example-include.md
--rw-r--r--   0        0        0      478 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/__init__.py
--rw-r--r--   0        0        0      388 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/_compat.py
--rw-r--r--   0        0        0    13673 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/_docs.py
--rw-r--r--   0        0        0     1373 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/cli.py
--rw-r--r--   0        0        0       84 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/config/__init__.py
--rw-r--r--   0        0        0     5189 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/config/dc_validators.py
--rw-r--r--   0        0        0    19038 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/config/main.py
--rw-r--r--   0        0        0      245 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/docutils_.py
--rw-r--r--   0        0        0    16027 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/inventory.py
--rw-r--r--   0        0        0      302 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/mdit_to_docutils/__init__.py
--rw-r--r--   0        0        0    80426 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/mdit_to_docutils/base.py
--rw-r--r--   0        0        0     4450 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py
--rw-r--r--   0        0        0     9458 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/mdit_to_docutils/sphinx_.py
--rw-r--r--   0        0        0     5705 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/mdit_to_docutils/transforms.py
--rw-r--r--   0        0        0    20648 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/mocking.py
--rw-r--r--   0        0        0       60 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/parsers/__init__.py
--rw-r--r--   0        0        0     8178 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/parsers/directives.py
--rw-r--r--   0        0        0    16236 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/parsers/docutils_.py
--rw-r--r--   0        0        0     4743 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/parsers/mdit.py
--rw-r--r--   0        0        0    13705 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/parsers/parse_html.py
--rw-r--r--   0        0        0     2455 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/parsers/sphinx_.py
--rw-r--r--   0        0        0       26 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/py.typed
--rw-r--r--   0        0        0      256 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/sphinx_.py
--rw-r--r--   0        0        0       40 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/sphinx_ext/__init__.py
--rw-r--r--   0        0        0     4286 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/sphinx_ext/directives.py
--rw-r--r--   0        0        0     3387 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/sphinx_ext/main.py
--rw-r--r--   0        0        0     4730 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/sphinx_ext/mathjax.py
--rw-r--r--   0        0        0    15289 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/sphinx_ext/myst_refs.py
--rw-r--r--   0        0        0     3982 2023-06-13 16:30:44.595688 myst_docutils-2.0.0/myst_parser/warnings_.py
--rw-r--r--   0        0        0     3629 2023-06-13 16:30:47.723699 myst_docutils-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1389 2023-06-13 16:30:44.603688 myst_docutils-2.0.0/tox.ini
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 myst_docutils-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1746 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml
+-rw-r--r--   0        0        0      834 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml
+-rw-r--r--   0        0        0      692 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml
+-rw-r--r--   0        0        0      185 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      598 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     1696 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/workflows/docutils_setup.py
+-rw-r--r--   0        0        0     2219 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/workflows/test-formats.yml
+-rw-r--r--   0        0        0     4590 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1860 2024-04-23 14:36:21.148292 myst_docutils-3.0.0/.gitignore
+-rw-r--r--   0        0        0      896 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      234 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    43261 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2817 2024-04-23 14:36:23.912315 myst_docutils-3.0.0/README.md
+-rw-r--r--   0        0        0      162 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/codecov.yml
+-rw-r--r--   0        0        0       71 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/example-include.md
+-rw-r--r--   0        0        0      479 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/myst_parser/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/myst_parser/_compat.py
+-rw-r--r--   0        0        0    13904 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/myst_parser/_docs.py
+-rw-r--r--   0        0        0     1373 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/myst_parser/cli.py
+-rw-r--r--   0        0        0       84 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/myst_parser/config/__init__.py
+-rw-r--r--   0        0        0     5182 2024-04-23 14:36:21.152292 myst_docutils-3.0.0/myst_parser/config/dc_validators.py
+-rw-r--r--   0        0        0    19244 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/config/main.py
+-rw-r--r--   0        0        0      246 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/docutils_.py
+-rw-r--r--   0        0        0    16017 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/inventory.py
+-rw-r--r--   0        0        0      302 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/mdit_to_docutils/__init__.py
+-rw-r--r--   0        0        0    80773 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/mdit_to_docutils/base.py
+-rw-r--r--   0        0        0     4451 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py
+-rw-r--r--   0        0        0     9459 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/mdit_to_docutils/sphinx_.py
+-rw-r--r--   0        0        0     5706 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/mdit_to_docutils/transforms.py
+-rw-r--r--   0        0        0    22398 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/mocking.py
+-rw-r--r--   0        0        0       60 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/__init__.py
+-rw-r--r--   0        0        0    10854 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/directives.py
+-rw-r--r--   0        0        0    16285 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/docutils_.py
+-rw-r--r--   0        0        0     4744 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/mdit.py
+-rw-r--r--   0        0        0    20982 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/options.py
+-rw-r--r--   0        0        0    13703 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/parse_html.py
+-rw-r--r--   0        0        0     2456 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/parsers/sphinx_.py
+-rw-r--r--   0        0        0       26 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/py.typed
+-rw-r--r--   0        0        0      257 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/sphinx_.py
+-rw-r--r--   0        0        0       40 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/sphinx_ext/__init__.py
+-rw-r--r--   0        0        0     4310 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/sphinx_ext/directives.py
+-rw-r--r--   0        0        0     3384 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/sphinx_ext/main.py
+-rw-r--r--   0        0        0     4745 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/sphinx_ext/mathjax.py
+-rw-r--r--   0        0        0    15298 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/sphinx_ext/myst_refs.py
+-rw-r--r--   0        0        0     4306 2024-04-23 14:36:21.156292 myst_docutils-3.0.0/myst_parser/warnings_.py
+-rw-r--r--   0        0        0     3948 2024-04-23 14:36:23.912315 myst_docutils-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1390 2024-04-23 14:36:21.168292 myst_docutils-3.0.0/tox.ini
+-rw-r--r--   0        0        0     5703 1970-01-01 00:00:00.000000 myst_docutils-3.0.0/PKG-INFO
```

### Comparing `myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml` & `myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml`

 * *Files identical despite different names*

### Comparing `myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml` & `myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml`

 * *Files identical despite different names*

### Comparing `myst_docutils-2.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml` & `myst_docutils-3.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml`

 * *Files identical despite different names*

### Comparing `myst_docutils-2.0.0/.github/dependabot.yml` & `myst_docutils-3.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myst_docutils-2.0.0/.github/workflows/docutils_setup.py` & `myst_docutils-3.0.0/.github/workflows/docutils_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """Script to convert package setup to myst-docutils."""
+
 import sys
 
 import tomlkit
 
 
 def modify_toml(content: str) -> str:
     """Modify `pyproject.toml`."""
@@ -12,15 +13,15 @@
     # change name of package
     doc["project"]["name"] = "myst-docutils"
 
     # move dependency on docutils and sphinx to extra
     dependencies = []
     sphinx_extra = []
     for dep in doc["project"]["dependencies"]:
-        if dep.startswith("docutils") or dep.startswith("sphinx"):
+        if dep.startswith(("docutils", "sphinx")):
             sphinx_extra.append(dep)
         else:
             dependencies.append(dep)
     doc["project"]["dependencies"] = dependencies
     doc["project"]["optional-dependencies"]["sphinx"] = sphinx_extra
 
     return tomlkit.dumps(doc)
```

### Comparing `myst_docutils-2.0.0/.github/workflows/test-formats.yml` & `myst_docutils-3.0.0/.github/workflows/test-formats.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     strategy:
       fail-fast: false
       matrix:
         format: ["man", "text"]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.9
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[linkify,rtd]
     - name: Build docs
@@ -38,17 +38,17 @@
 
     strategy:
       fail-fast: false
       matrix:
         format: ["latex"]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.9
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[linkify,rtd]
     - name: Build docs
```

### Comparing `myst_docutils-2.0.0/.github/workflows/tests.yml` & `myst_docutils-3.0.0/.github/workflows/tests.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,79 +9,80 @@
 
 jobs:
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v4
+    - uses: actions/checkout@v4
+    - name: Set up Python 3.9
+      uses: actions/setup-python@v5
       with:
-        python-version: "3.8"
-    - uses: pre-commit/action@v3.0.0
+        python-version: "3.9"
+    - uses: pre-commit/action@v3.0.1
 
   tests:
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         sphinx: [">=7,<8"]
         os: [ubuntu-latest]
         include:
         - os: ubuntu-latest
           python-version: "3.8"
           sphinx: ">=6,<7"
         - os: windows-latest
           python-version: "3.8"
           sphinx: ">=6,<7"
 
     runs-on: ${{ matrix.os }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e ".[linkify,testing]" "sphinx${{ matrix.sphinx }}"
     - name: Run pytest
       run: |
         pytest --cov=myst_parser --cov-report=xml --cov-report=term-missing
         coverage xml
     - name: Upload to Codecov
       if: github.repository == 'executablebooks/MyST-Parser' && matrix.python-version == 3.8 && matrix.os == 'ubuntu-latest'
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
+        token: ${{ secrets.CODECOV_TOKEN }}
         name: myst-parser-pytests
         flags: pytests
         file: ./coverage.xml
         fail_ci_if_error: true
 
   check-myst-docutils:
 
     name: Check myst-docutils install
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        docutils-version: ["0.17", "0.18", "0.19", "0.20"]
+        docutils-version: ["0.18", "0.19", "0.20", "0.21"]
 
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v4
+      uses: actions/checkout@v4
+    - name: Set up Python 3.9
+      uses: actions/setup-python@v5
       with:
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Install setup
       run: |
         python -m pip install --upgrade pip
         pip install tomlkit
     - name: Modify setup
       run: python .github/workflows/docutils_setup.py pyproject.toml README.md
     - name: Install dependencies
@@ -124,17 +125,17 @@
     name: Publish myst-parser to PyPi
     needs:
     - check
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
     - name: Set up Python 3.8
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.8"
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
@@ -147,17 +148,17 @@
 
     name: Publish myst-docutils to PyPi
     needs: [publish]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
     - name: Set up Python 3.8
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.8"
     - name: install flit and tomlkit
       run: |
         pip install flit~=3.4 tomlkit
     - name: Modify setup
       run: python .github/workflows/docutils_setup.py pyproject.toml README.md
```

### Comparing `myst_docutils-2.0.0/.gitignore` & `myst_docutils-3.0.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -129,7 +129,9 @@
 # Pyre type checker
 .pyre/
 
 _archive/
 
 .vscode/
 .DS_Store
+
+docs/apidocs
```

### Comparing `myst_docutils-2.0.0/.pre-commit-config.yaml` & `myst_docutils-3.0.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -2,55 +2,42 @@
 # pre-commit install
 
 exclude: >
     (?x)^(
       \.vscode/settings\.json|
       tests/test_commonmark/commonmark\.json|
       .*\.xml|
-      tests/.*/.*\.md
+      tests/.*/.*\.md|
+      tests/.*/.*\.yaml
     )$
 
 repos:
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     - id: check-json
     - id: check-yaml
     - id: end-of-file-fixer
     - id: trailing-whitespace
 
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
-    hooks:
-    - id: pyupgrade
-      args: [--py38-plus]
-
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-    - id: isort
-
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-    - id: black
-
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.1
     hooks:
     - id: ruff
+      args: [--fix]
+    - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.9.0
     hooks:
     - id: mypy
       args: [--config-file=pyproject.toml]
       additional_dependencies:
-      - sphinx~=5.0
       - types-urllib3
+      - sphinx~=7.3
       - markdown-it-py~=3.0
       - mdit-py-plugins~=0.4.0
       files: >
         (?x)^(
             myst_parser/.*py|
         )$
```

### Comparing `myst_docutils-2.0.0/CHANGELOG.md` & `myst_docutils-3.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,51 @@
 # Changelog
 
+## 3.0.0 - 2024-04-23
+
+### Upgraded dependencies
+
+- ⬆️ Add support for Python 3.12 by <gh-user:hugovk> in <gh-pr:848>
+- ⬆️ Update docutils requirement from >=0.16,<0.21 to >=0.18,<0.22 by <gh-user:chrisjsewell> in <gh-pr:916>
+
+### New features
+
+- ✨ Allow for use of the `line-block` directive by <gh-user:chrisjsewell> in <gh-pr:900>
+- ✨ Emits sphinx include-read event by <gh-user:sumezulike> in <gh-pr:887>
+
+### Improvements
+
+- 👌 Nested parse attribution in `attr_block` by <gh-user:chrisjsewell> in <gh-pr:831>
+- 👌 Directive option parsing by <gh-user:chrisjsewell> in <gh-pr:796
+- 👌 Improve directive parsing warnings by <gh-user:chrisjsewell> in <gh-pr:893>
+- 👌 Allow for opening external links in new tabs (#856) by <gh-user:marjus45> in <gh-pr:857>
+
+### Internal
+
+- 🔧 Replace black, isort, pyupgrade with ruff formatter by <gh-user:chrisjsewell> in <gh-pr:833>
+- 🔧 remove redundant mypy config by <gh-user:danieleades> in <gh-pr:866>
+- 🔧 Add additional Ruff lints (and fix issues) by <gh-user:danieleades> in <gh-pr:862>
+- 🔧 mypy- disallow 'any generics' by <gh-user:danieleades> in <gh-pr:865>
+- 🔧 Fix docutils deprecation in option parsing by <gh-user:agoose77> in <gh-pr:842>
+
+### Documentation
+
+- 📚 Fix a broken link in configuration.md by <gh-user:zupo> in <gh-pr:907>
+- 📚 Add linkify dependency to contributing docs. by <gh-user:jhcole> in <gh-pr:792>
+- 📚 Fix the double `used` in docs/syntax/math.md by <gh-user:ice-tong> in <gh-pr:810>
+- 📚 Also add linkify to pip install command in README by <gh-user:n-peugnet> in <gh-pr:851>
+- 📚 Fix the code section title in live preview by <gh-user:BoboTiG> in <gh-pr:875>
+- 📚 Fix admonition example by <gh-user:72757373656c6c> in <gh-pr:904>
+- 📚 Fix url for jupyter book gallery by <gh-user:72757373656c6c> in <gh-pr:905>
+- 📚 Update theme version by <gh-user:chrisjsewell> in <gh-pr:918>
+- 📚 Fix typo by <gh-user:blakeNaccarato> in <gh-pr:911>
+- 📚 Fix architecture typo (#855) by <gh-user:72757373656c6c> in <gh-pr:910>
+
+**Full Changelog**: [v2.0.0...v3.0.0](https://github.com/executablebooks/MyST-Parser/compare/v2.0.0...v3.0.0)
+
 ## 2.0.0 - 2023-06-13
 
 This release primarily updates core myst-parser dependencies,
 with some minor changes to parsing behaviour:
 
 * ⬆️ UPGRADE: `markdown-it-py` to v3 (<gh-pr:773>)
   * This is mainly a non-breaking change, fixing some edge cases in parsing
```

### Comparing `myst_docutils-2.0.0/LICENSE` & `myst_docutils-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myst_docutils-2.0.0/README.md` & `myst_docutils-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 Or for package development:
 
 ```bash
 git clone https://github.com/executablebooks/MyST-Parser
 cd MyST-Parser
 git checkout master
-pip install -e .[code_style,testing,rtd]
+pip install -e .[code_style,linkify,testing,rtd]
 ```
 
 To use the MyST parser in Sphinx, simply add: `extensions = ["myst_parser"]` to your `conf.py`.
 
 ## Contributing
 
 We welcome all contributions!
```

### Comparing `myst_docutils-2.0.0/myst_parser/_docs.py` & `myst_docutils-3.0.0/myst_parser/_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Code to use internally, for documentation."""
+
 from __future__ import annotations
 
+import contextlib
 import io
 from typing import Sequence, Union, get_args, get_origin
 
 from docutils import nodes
-from docutils.frontend import OptionParser
+from docutils.core import Publisher
 from docutils.parsers.rst import directives
 from sphinx.directives import other
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective
 
 from myst_parser.parsers.docutils_ import to_html5_demo
+
 from .config.main import MdParserConfig
 from .parsers.docutils_ import Parser as DocutilsParser
 from .warnings_ import MystWarnings
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -90,15 +93,15 @@
     @staticmethod
     def field_type(field):
         ftypes: Sequence[str]
         ftypes = (
             get_args(field.type) if get_origin(field.type) is Union else [field.type]
         )
         ctype = " | ".join(
-            str("None" if ftype == type(None) else ftype)  # type: ignore
+            str("None" if ftype == type(None) else ftype)  # type: ignore[comparison-overlap]
             for ftype in ftypes
         )
         ctype = " ".join(ctype.splitlines())
         ctype = ctype.replace("typing.", "")
         ctype = ctype.replace("typing_extensions.", "")
         for tname in ("str", "int", "float", "bool"):
             ctype = ctype.replace(f"<class '{tname}'>", tname)
@@ -170,19 +173,26 @@
     has_content = False
     required_arguments = 0
     optional_arguments = 0
     final_argument_whitespace = False
 
     def run(self):
         """Run the directive."""
+
         stream = io.StringIO()
-        OptionParser(
-            components=(DocutilsParser,),
-            usage="myst-docutils-<writer> [options] [<source> [<destination>]]",
-        ).print_help(stream)
+
+        pub = Publisher(parser=DocutilsParser())
+        with contextlib.redirect_stdout(stream):
+            try:
+                pub.process_command_line(
+                    ["--help"],
+                    usage="myst-docutils-<writer> [options] [<source> [<destination>]]",
+                )
+            except SystemExit as exc:
+                assert not exc.code
         return [nodes.literal_block("", stream.getvalue())]
 
 
 class DirectiveDoc(SphinxDirective):
     """Load and document a directive."""
 
     required_arguments = 1  # name of the directive
```

### Comparing `myst_docutils-2.0.0/myst_parser/cli.py` & `myst_docutils-3.0.0/myst_parser/cli.py`

 * *Files identical despite different names*

### Comparing `myst_docutils-2.0.0/myst_parser/config/dc_validators.py` & `myst_docutils-3.0.0/myst_parser/config/dc_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Validators for dataclasses, mirroring those of https://github.com/python-attrs/attrs."""
+
 from __future__ import annotations
 
 import dataclasses as dc
 from typing import Any, Protocol, Sequence
 
 
 def validate_field(inst: Any, field: dc.Field, value: Any) -> None:
@@ -33,16 +34,15 @@
     for field in dc.fields(inst):
         validate_field(inst, field, getattr(inst, field.name))
 
 
 class ValidatorType(Protocol):
     def __call__(
         self, inst: Any, field: dc.Field, value: Any, suffix: str = ""
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
 def any_(inst, field, value, suffix=""):
     """
     A validator that does not perform any validation.
     """
```

### Comparing `myst_docutils-2.0.0/myst_parser/config/main.py` & `myst_docutils-3.0.0/myst_parser/config/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The configuration for the myst parser."""
+
 import dataclasses as dc
 from importlib import import_module
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
@@ -13,14 +14,15 @@
     Set,
     Tuple,
     TypedDict,
     Union,
 )
 
 from myst_parser.warnings_ import MystWarnings
+
 from .dc_validators import (
     any_,
     deep_iterable,
     deep_mapping,
     in_,
     instance_of,
     optional,
@@ -99,15 +101,15 @@
                 "classes" in val
                 and not isinstance(val["classes"], list)
                 and not all(isinstance(c, str) for c in val["classes"])
             ):
                 raise TypeError(
                     f"'{field.name}[{key}][classes]' is not a list of str: {val['classes']!r}"
                 )
-            new_dict[key] = val  # type: ignore
+            new_dict[key] = val  # type: ignore[assignment]
         else:
             raise TypeError(
                 f"'{field.name}[{key}]' value is not a string or dict: {val!r}"
             )
 
     setattr(inst, field.name, new_dict)
 
@@ -228,14 +230,22 @@
         default=False,
         metadata={
             "validator": instance_of(bool),
             "help": "Parse all links as simple hyperlinks",
         },
     )
 
+    links_external_new_tab: bool = dc.field(
+        default=False,
+        metadata={
+            "validator": instance_of(bool),
+            "help": "Open all external links in a new tab",
+        },
+    )
+
     url_schemes: Dict[str, Optional[UrlSchemeType]] = dc.field(
         default_factory=lambda: {
             "http": None,
             "https": None,
             "mailto": None,
             "ftp": None,
         },
@@ -572,15 +582,15 @@
     try:
         if not next(text).startswith("---"):
             return None
     except StopIteration:
         return None
     top_matter = []
     for line in text:
-        if line.startswith("---") or line.startswith("..."):
+        if line.startswith(("---", "...")):
             break
         top_matter.append(line.rstrip() + "\n")
     try:
         metadata = yaml.safe_load("".join(top_matter))
     except (yaml.parser.ParserError, yaml.scanner.ScannerError) as err:
         raise TopmatterReadError("Malformed YAML") from err
     if not isinstance(metadata, dict):
```

### Comparing `myst_docutils-2.0.0/myst_parser/inventory.py` & `myst_docutils-3.0.0/myst_parser/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Logic for dealing with sphinx style inventories (e.g. `objects.inv`).
 
 These contain mappings of reference names to ids, scoped by domain and object type.
 
 This is adapted from the Sphinx inventory.py module.
 We replicate it here, so that it can be used without Sphinx.
 """
+
 from __future__ import annotations
 
 import argparse
 import functools
 import json
 import re
 import zlib
@@ -227,15 +228,15 @@
             while pos != -1:
                 yield buf[:pos].decode()
                 buf = buf[pos + 1 :]
                 pos = buf.find(b"\n")
 
 
 @functools.lru_cache(maxsize=256)
-def _create_regex(pat: str) -> re.Pattern:
+def _create_regex(pat: str) -> re.Pattern[str]:
     r"""Create a regex from a pattern, that can include `*` wildcards,
     to match 0 or more characters.
 
     `\*` is translated as a literal `*`.
     """
     regex = ""
     backslash_last = False
@@ -400,15 +401,15 @@
     return delimiter.join(str_items)
 
 
 def fetch_inventory(
     uri: str, *, timeout: None | float = None, base_url: None | str = None
 ) -> InventoryType:
     """Fetch an inventory from a URL or local path."""
-    if uri.startswith("http://") or uri.startswith("https://"):
+    if uri.startswith(("http://", "https://")):
         with urlopen(uri, timeout=timeout) as stream:
             return load(stream, base_url=base_url)
     with open(uri, "rb") as stream:
         return load(stream, base_url=base_url)
 
 
 def inventory_cli(inputs: None | list[str] = None):
```

### Comparing `myst_docutils-2.0.0/myst_parser/mdit_to_docutils/base.py` & `myst_docutils-3.0.0/myst_parser/mdit_to_docutils/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convert Markdown-it tokens to docutils nodes."""
+
 from __future__ import annotations
 
 import inspect
 import json
 import os
 import posixpath
 import re
@@ -18,27 +19,26 @@
     Iterator,
     MutableMapping,
     Sequence,
     cast,
 )
 from urllib.parse import urlparse
 
+import docutils
 import jinja2
 import yaml
 from docutils import nodes
-from docutils.frontend import OptionParser
 from docutils.languages import get_language
-from docutils.parsers.rst import Directive, DirectiveError
+from docutils.parsers.rst import Directive, DirectiveError, directives, roles
 from docutils.parsers.rst import Parser as RSTParser
-from docutils.parsers.rst import directives, roles
 from docutils.parsers.rst.directives.misc import Include
 from docutils.parsers.rst.languages import get_language as get_language_rst
 from docutils.statemachine import StringList
 from docutils.transforms.components import Filter
-from docutils.utils import Reporter, new_document
+from docutils.utils import Reporter, SystemMessage, new_document
 from docutils.utils.code_analyzer import Lexer, LexerError, NumberLines
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml
 from markdown_it.renderer import RendererProtocol
 from markdown_it.token import Token
 from markdown_it.tree import SyntaxTreeNode
 
@@ -51,23 +51,31 @@
     MockInliner,
     MockRSTParser,
     MockState,
     MockStateMachine,
 )
 from myst_parser.parsers.directives import MarkupError, parse_directive_text
 from myst_parser.warnings_ import MystWarnings, create_warning
+
 from .html_to_nodes import html_to_nodes
 
 if TYPE_CHECKING:
     from sphinx.environment import BuildEnvironment
 
 
 def make_document(source_path="notset", parser_cls=RSTParser) -> nodes.document:
     """Create a new docutils document, with the parser classes' default settings."""
-    settings = OptionParser(components=(parser_cls,)).get_default_values()
+    if docutils.__version_info__[:2] >= (0, 19):
+        from docutils.frontend import get_default_settings
+
+        settings = get_default_settings(parser_cls)
+    else:
+        from docutils.frontend import OptionParser
+
+        settings = OptionParser(components=(parser_cls,)).get_default_values()
     return new_document(source_path, settings=settings)
 
 
 REGEX_SCHEME = re.compile(r"^([a-zA-Z][a-zA-Z0-9+.-]*):")
 """RFC 7595: A non-empty scheme component followed by a colon (:),
 consisting of a sequence of characters beginning with a letter
 and followed by any combination of letters, digits, plus (+), period (.), or hyphen (-).
@@ -249,17 +257,17 @@
 
     def _render_finalise(self) -> None:
         """Finalise the render of the document."""
 
         # save for later reference resolution
         self.document.myst_slugs = self._heading_slugs
         if self._heading_slugs and self.sphinx_env:
-            self.sphinx_env.metadata[self.sphinx_env.docname][
-                "myst_slugs"
-            ] = self._heading_slugs
+            self.sphinx_env.metadata[self.sphinx_env.docname]["myst_slugs"] = (
+                self._heading_slugs
+            )
 
         # log warnings for duplicate reference definitions
         # "duplicate_refs": [{"href": "ijk", "label": "B", "map": [4, 5], "title": ""}],
         for dup_ref in self.md_env.get("duplicate_refs", []):
             self.create_warning(
                 f"Duplicate reference definition: {dup_ref['label']}",
                 MystWarnings.MD_DEF_DUPE,
@@ -368,15 +376,15 @@
 
         with _restore():
             self._render_tokens(tokens)
 
     @contextmanager
     def current_node_context(
         self, node: nodes.Element, append: bool = False
-    ) -> Iterator:
+    ) -> Iterator[None]:
         """Context manager for temporarily setting the current node."""
         if append:
             self.current_node.append(node)
         current_node = self.current_node
         self.current_node = node
         yield
         self.current_node = current_node
@@ -578,20 +586,23 @@
 
     def render_blockquote(self, token: SyntaxTreeNode) -> None:
         quote = nodes.block_quote()
         self.copy_attributes(token, quote, keys=("class", "id"))
         self.add_line_and_source_path(quote, token)
         with self.current_node_context(quote, append=True):
             self.render_children(token)
-        if "attribution" in token.attrs:
-            attribution = nodes.attribution(
-                token.attrs["attribution"], "", nodes.Text(token.attrs["attribution"])
-            )
-            self.add_line_and_source_path(attribution, token)
-            quote.append(attribution)
+            if "attribution" in token.attrs:
+                attribution = nodes.attribution(token.attrs["attribution"], "")
+                self.add_line_and_source_path(attribution, token)
+                with self.current_node_context(attribution, append=True):
+                    self.nested_render_text(
+                        str(token.attrs["attribution"]),
+                        token_line(token, 0),
+                        inline=True,
+                    )
 
     def render_hr(self, token: SyntaxTreeNode) -> None:
         node = nodes.transition()
         self.add_line_and_source_path(node, token)
         self.current_node.append(node)
 
     def render_code_inline(self, token: SyntaxTreeNode) -> None:
@@ -938,16 +949,20 @@
         self, token: SyntaxTreeNode, conversion: None | UrlSchemeType = None
     ) -> None:
         """Render link token (including autolink and linkify),
         where the link has been identified as an external URL.
         """
         ref_node = nodes.reference()
         self.add_line_and_source_path(ref_node, token)
+        attribute_keys = ["class", "id", "reftitle", "target", "rel"]
+        if self.md_config.links_external_new_tab:
+            token.attrs["target"] = "_blank"
+            token.attrs["rel"] = "noreferer noopener"
         self.copy_attributes(
-            token, ref_node, ("class", "id", "reftitle"), aliases={"title": "reftitle"}
+            token, ref_node, attribute_keys, aliases={"title": "reftitle"}
         )
         uri = cast(str, token.attrGet("href") or "")
         implicit_text: str | None = None
 
         if conversion is not None:
             # implicit_template: str | None = None
             # if isinstance(conversion, (list, tuple)):
@@ -1575,20 +1590,20 @@
                         self.add_line_and_source_path(term, child)
                         with self.current_node_context(term):
                             self.render_children(child)
                         if make_terms:
                             from sphinx.domains.std import make_glossary_term
 
                             term = make_glossary_term(
-                                self.sphinx_env,  # type: ignore
+                                self.sphinx_env,  # type: ignore[arg-type]
                                 term.children,
-                                None,  # type: ignore
+                                None,  # type: ignore[arg-type]
                                 term.source,
                                 term.line,
-                                node_id=None,  # type: ignore
+                                node_id=None,
                                 document=self.document,
                             )
                         self.current_node.append(term)
                 elif child.type == "dd":
                     if item is None:
                         error = self.reporter.error(
                             (
@@ -1710,15 +1725,15 @@
         :param additional_options: Additional options to add to the directive,
             above those parsed from the content.
 
         """
         self.document.current_line = position
 
         # get directive class
-        output: tuple[Directive | None, list] = directives.directive(
+        output: tuple[Directive | None, list[SystemMessage]] = directives.directive(
             name, self.language_module_rst, self.document
         )
         directive_class, messages = output
         if not directive_class:
             warn_node = self.create_warning(
                 f"Unknown directive type: {name!r}",
                 MystWarnings.UNKNOWN_DIRECTIVE,
@@ -1734,29 +1749,29 @@
             directive_class.option_spec["heading-offset"] = directives.nonnegative_int
 
         try:
             parsed = parse_directive_text(
                 directive_class,
                 first_line,
                 content,
+                line=position,
                 additional_options=additional_options,
             )
         except MarkupError as error:
             error = self.reporter.error(
                 f"Directive '{name}': {error}",
                 line=position,
             )
             return [error]
 
-        if parsed.warnings:
-            _errors = ",\n".join(parsed.warnings)
+        for _warning in parsed.warnings:
             self.create_warning(
-                f"{name!r}: {_errors}",
-                MystWarnings.DIRECTIVE_PARSING,
-                line=position,
+                f"{name!r}: {_warning.msg}",
+                _warning.type,
+                line=_warning.lineno if _warning.lineno is not None else position,
                 append_to=self.current_node,
             )
 
         # initialise directive
         if issubclass(directive_class, Include):
             directive_instance = MockIncludeDirective(
                 self,
@@ -1795,31 +1810,27 @@
             msg_node = self.reporter.system_message(
                 error.level, error.msg, line=position
             )
             msg_node += nodes.literal_block(content, content)
             result = [msg_node]
         except MockingError as exc:
             error_msg = self.reporter.error(
-                "Directive '{}' cannot be mocked: {}: {}".format(
-                    name, exc.__class__.__name__, exc
-                ),
+                f"Directive '{name}' cannot be mocked: {exc.__class__.__name__}: {exc}",
                 nodes.literal_block(content, content),
                 line=position,
             )
             return [error_msg]
 
         assert isinstance(
             result, list
         ), f'Directive "{name}" must return a list of nodes.'
         for i in range(len(result)):
             assert isinstance(
                 result[i], nodes.Node
-            ), 'Directive "{}" returned non-Node object (index {}): {}'.format(
-                name, i, result[i]
-            )
+            ), f'Directive "{name}" returned non-Node object (index {i}): {result[i]}'
         return result
 
     def render_substitution_inline(self, token: SyntaxTreeNode) -> None:
         """Render inline substitution {{key}}."""
         self.render_substitution(token, inline=True)
 
     def render_substitution_block(self, token: SyntaxTreeNode) -> None:
@@ -1903,27 +1914,19 @@
 
     See:
     https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#html-metadata
     """
     if not data:
         return []
 
-    try:
-        meta_cls = nodes.meta
-    except AttributeError:
-        # docutils-0.17 or older
-        from docutils.parsers.rst.directives.html import MetaBody
-
-        meta_cls = MetaBody.meta
-
     output = []
 
     for key, value in data.items():
         content = str(value or "")
-        meta_node = meta_cls(content)
+        meta_node = nodes.meta(content)
         meta_node.source = document["source"]
         meta_node.line = line
         meta_node["content"] = content
         try:
             if not content:
                 raise ValueError("No content")
             for i, key_part in enumerate(key.split()):
```

### Comparing `myst_docutils-2.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py` & `myst_docutils-3.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convert HTML to docutils nodes."""
+
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING
 
 from docutils import nodes
```

### Comparing `myst_docutils-2.0.0/myst_parser/mdit_to_docutils/sphinx_.py` & `myst_docutils-3.0.0/myst_parser/mdit_to_docutils/sphinx_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convert Markdown-it tokens to docutils nodes, including sphinx specific elements."""
+
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from typing import cast
 from uuid import uuid4
```

### Comparing `myst_docutils-2.0.0/myst_parser/mdit_to_docutils/transforms.py` & `myst_docutils-3.0.0/myst_parser/mdit_to_docutils/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Directives that can be applied to both Sphinx and docutils."""
+
 from __future__ import annotations
 
 import typing as t
 
 from docutils import nodes
 from docutils.transforms import Transform
 from markdown_it.common.normalize_url import normalizeLink
```

### Comparing `myst_docutils-2.0.0/myst_parser/mocking.py` & `myst_docutils-3.0.0/myst_parser/mocking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module provides classes to Mock the core components of the docutils.RSTParser,
 the key difference being that nested parsing treats the text as Markdown not rST.
 """
+
 from __future__ import annotations
 
 import os
 import re
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
@@ -80,17 +81,15 @@
 
     def __getattr__(self, name: str):
         """This method is only be called if the attribute requested has not
         been defined. Defined attributes will not be overridden.
         """
         # TODO use document.reporter mechanism?
         if hasattr(Inliner, name):
-            msg = "{cls} has not yet implemented attribute '{name}'".format(
-                cls=type(self).__name__, name=name
-            )
+            msg = f"{type(self).__name__} has not yet implemented attribute '{name}'"
             raise MockingError(msg).with_traceback(sys.exc_info()[2])
         msg = f"{type(self).__name__} has no attribute {name}"
         raise MockingError(msg).with_traceback(sys.exc_info()[2])
 
 
 class MockState:
     """A mock version of `docutils.parsers.rst.states.RSTState`.
@@ -125,28 +124,28 @@
         self.memo = Struct
 
     def parse_directive_block(
         self,
         content: StringList,
         line_offset: int,
         directive: type[Directive],
-        option_presets: dict,
-    ) -> tuple[list, dict, StringList, int]:
+        option_presets: dict[str, Any],
+    ) -> tuple[list[str], dict[str, Any], StringList, int]:
         """Parse the full directive text
 
         :raises MarkupError: for errors in parsing the directive
         :returns: (arguments, options, content, content_offset)
         """
         # note this is essentially only used by the docutils `role` directive
         if option_presets:
             raise MockingError("parse_directive_block: option_presets not implemented")
         # TODO should argument_str always be ""?
         parsed = parse_directive_text(directive, "", "\n".join(content))
         if parsed.warnings:
-            raise MarkupError(",".join(parsed.warnings))
+            raise MarkupError(",".join(w.msg for w in parsed.warnings))
         return (
             parsed.arguments,
             parsed.options,
             StringList(parsed.body, source=content.source),
             line_offset + parsed.body_offset,
         )
 
@@ -260,14 +259,43 @@
 
     def build_table(self, tabledata, tableline, stub_columns: int = 0, widths=None):
         return Body.build_table(self, tabledata, tableline, stub_columns, widths)
 
     def build_table_row(self, rowdata, tableline):
         return Body.build_table_row(self, rowdata, tableline)
 
+    def nest_line_block_lines(self, block: nodes.line_block):
+        """Modify the line block element in-place, to nest line block segments.
+
+        Line nodes are placed into child line block containers, based on their indentation.
+        """
+        for index in range(1, len(block)):
+            if getattr(block[index], "indent", None) is None:
+                block[index].indent = block[index - 1].indent
+        self._nest_line_block_segment(block)
+
+    def _nest_line_block_segment(self, block: nodes.line_block):
+        indents = [item.indent for item in block]
+        least = min(indents)
+        new_items = []
+        new_block = nodes.line_block()
+        for item in block:
+            if item.indent > least:
+                new_block.append(item)
+            else:
+                if len(new_block):
+                    self._nest_line_block_segment(new_block)
+                    new_items.append(new_block)
+                    new_block = nodes.line_block()
+                new_items.append(item)
+        if len(new_block):
+            self._nest_line_block_segment(new_block)
+            new_items.append(new_block)
+        block[:] = new_items
+
     def __getattr__(self, name: str):
         """This method is only be called if the attribute requested has not
         been defined. Defined attributes will not be overridden.
         """
         cls = type(self).__name__
         msg = (
             f"{cls} has not yet implemented attribute '{name}'. "
@@ -303,17 +331,15 @@
         return self.document["source"], lineno or self._lineno
 
     def __getattr__(self, name: str):
         """This method is only be called if the attribute requested has not
         been defined. Defined attributes will not be overridden.
         """
         if hasattr(RSTStateMachine, name):
-            msg = "{cls} has not yet implemented attribute '{name}'".format(
-                cls=type(self).__name__, name=name
-            )
+            msg = f"{type(self).__name__} has not yet implemented attribute '{name}'"
             raise MockingError(msg).with_traceback(sys.exc_info()[2])
         msg = f"{type(self).__name__} has no attribute {name}"
         raise MockingError(msg).with_traceback(sys.exc_info()[2])
 
 
 class MockIncludeDirective:
     """This directive uses a lot of statemachine logic that is not yet mocked.
@@ -324,16 +350,16 @@
     """
 
     def __init__(
         self,
         renderer: DocutilsRenderer,
         name: str,
         klass: Include,
-        arguments: list,
-        options: dict,
+        arguments: list[str],
+        options: dict[str, Any],
         body: list[str],
         lineno: int,
     ):
         self.renderer = renderer
         self.document = renderer.document
         self.name = name
         self.klass = klass
@@ -371,39 +397,53 @@
 
         # read file
         encoding = self.options.get("encoding", self.document.settings.input_encoding)
         error_handler = self.document.settings.input_encoding_error_handler
         # tab_width = self.options.get("tab-width", self.document.settings.tab_width)
         try:
             file_content = path.read_text(encoding=encoding, errors=error_handler)
-        except FileNotFoundError:
+        except FileNotFoundError as error:
             raise DirectiveError(
                 4, f'Directive "{self.name}": file not found: {str(path)!r}'
-            )
+            ) from error
         except Exception as error:
             raise DirectiveError(
                 4, f'Directive "{self.name}": error reading file: {path}\n{error}.'
+            ) from error
+
+        if self.renderer.sphinx_env is not None:
+            # Emit the "include-read" event
+            # see: https://github.com/sphinx-doc/sphinx/commit/ff18318613db56d0000db47e5c8f0140556cef0c
+            arg = [file_content]
+            relative_path = Path(
+                os.path.relpath(path, start=self.renderer.sphinx_env.srcdir)
+            )
+            parent_docname = Path(self.renderer.document["source"]).stem
+            self.renderer.sphinx_env.app.events.emit(
+                "include-read",
+                relative_path,
+                parent_docname,
+                arg,
             )
+            file_content = arg[0]
 
         # get required section of text
         startline = self.options.get("start-line", None)
         endline = self.options.get("end-line", None)
         file_content = "\n".join(file_content.splitlines()[startline:endline])
         startline = startline or 0
         for split_on_type in ["start-after", "end-before"]:
             split_on = self.options.get(split_on_type, None)
             if not split_on:
                 continue
             split_index = file_content.find(split_on)
             if split_index < 0:
                 raise DirectiveError(
                     4,
-                    'Directive "{}"; option "{}": text not found "{}".'.format(
-                        self.name, split_on_type, split_on
-                    ),
+                    f'Directive "{self.name}"; option "{split_on_type}": text not found "{split_on}".',
                 )
             if split_on_type == "start-after":
                 startline += split_index + len(split_on)
                 file_content = file_content[split_index + len(split_on) :]
             else:
                 file_content = file_content[:split_index]
 
@@ -412,18 +452,18 @@
                 file_content, source=str(path), classes=self.options.get("class", [])
             )
             literal_block.line = 1  # TODO don;t think this should be 1?
             self.add_name(literal_block)
             if "number-lines" in self.options:
                 try:
                     startline = int(self.options["number-lines"] or 1)
-                except ValueError:
+                except ValueError as err:
                     raise DirectiveError(
                         3, ":number-lines: with non-integer start value"
-                    )
+                    ) from err
                 endline = startline + len(file_content.splitlines())
                 if file_content.endswith("\n"):
                     file_content = file_content[:-1]
                 tokens = NumberLines([([], file_content)], startline, endline)
                 for classes, value in tokens:
                     if classes:
                         literal_block += nodes.inline(value, value, classes=classes)
```

### Comparing `myst_docutils-2.0.0/myst_parser/parsers/directives.py` & `myst_docutils-3.0.0/myst_parser/parsers/directives.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,194 +29,285 @@
     ```
 
 If the first line of a directive's content is blank, this will be stripped
 from the content.
 This is to allow for separation between the option block and content.
 
 """
+
 from __future__ import annotations
 
-import datetime
 import re
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import Any, Callable
 
 import yaml
 from docutils.parsers.rst import Directive
+from docutils.parsers.rst.directives import flag
 from docutils.parsers.rst.directives.misc import TestDirective
 from docutils.parsers.rst.states import MarkupError
 
+from myst_parser.warnings_ import MystWarnings
+
+from .options import TokenizeError
+from .options import to_items as options_to_items
+
+
+@dataclass
+class ParseWarnings:
+    msg: str
+    lineno: int | None = None
+    type: MystWarnings = MystWarnings.DIRECTIVE_PARSING
+
 
 @dataclass
 class DirectiveParsingResult:
     arguments: list[str]
     """The arguments parsed from the first line."""
     options: dict
     """Options parsed from the YAML block."""
     body: list[str]
     """The lines of body content"""
     body_offset: int
     """The number of lines to the start of the body content."""
-    warnings: list[str]
-    """List of non-fatal errors encountered during parsing."""
+    warnings: list[ParseWarnings]
+    """List of non-fatal errors encountered during parsing.
+    (message, line_number)
+    """
 
 
 def parse_directive_text(
     directive_class: type[Directive],
     first_line: str,
     content: str,
     *,
+    line: int | None = None,
     validate_options: bool = True,
     additional_options: dict[str, str] | None = None,
 ) -> DirectiveParsingResult:
     """Parse (and validate) the full directive text.
 
     :param first_line: The text on the same line as the directive name.
         May be an argument or body text, dependent on the directive
     :param content: All text after the first line. Can include options.
     :param validate_options: Whether to validate the values of options
+        This is actually only here to be used by myst-nb cells,
+        which converts options directly to JSON metadata, using the full YAML spec.
     :param additional_options: Additional options to add to the directive,
         above those parsed from the content (content options take priority).
 
     :raises MarkupError: if there is a fatal parsing/validation error
     """
-    parse_errors: list[str] = []
+    parse_warnings: list[ParseWarnings]
+    options: dict[str, Any]
+    body_lines: list[str]
+    content_offset: int
+    has_options_block: bool
+
     if directive_class.option_spec:
-        body, options, option_errors = parse_directive_options(
+        # only look for an option block if there are possible options
+        # body, options, option_errors = _parse_directive_options(
+        result = _parse_directive_options(
             content,
             directive_class,
-            validate=validate_options,
+            line=line,
+            as_yaml=not validate_options,
             additional_options=additional_options,
         )
-        parse_errors.extend(option_errors)
-        body_lines = body.splitlines()
+        parse_warnings = result.warnings
+        has_options_block = result.has_options
+        options = result.options
+        body_lines = result.content.splitlines()
         content_offset = len(content.splitlines()) - len(body_lines)
     else:
-        # If there are no possible options, we do not look for a YAML block
+        parse_warnings = []
+        has_options_block = False
         options = {}
         body_lines = content.splitlines()
         content_offset = 0
 
     if not (directive_class.required_arguments or directive_class.optional_arguments):
-        # If there are no possible arguments, then the body starts on the argument line
-        if first_line:
+        # If there are no possible arguments, then the body can start on the argument line
+        if first_line.strip():
+            if has_options_block and any(body_lines):
+                parse_warnings.append(
+                    ParseWarnings(
+                        "Splitting content across first line and body, "
+                        "when an options block is present, is not recommended"
+                    )
+                )
             body_lines.insert(0, first_line)
+            content_offset = 0
         arguments = []
     else:
         arguments = parse_directive_arguments(directive_class, first_line)
 
     # remove first line of body if blank
     # this is to allow space between the options and the content
     if body_lines and not body_lines[0].strip():
         body_lines = body_lines[1:]
         content_offset += 1
 
     # check for body content
     if body_lines and not directive_class.has_content:
-        parse_errors.append("Has content, but none permitted")
+        parse_warnings.append(ParseWarnings("Has content, but none permitted"))
 
     return DirectiveParsingResult(
-        arguments, options, body_lines, content_offset, parse_errors
+        arguments, options, body_lines, content_offset, parse_warnings
     )
 
 
-def parse_directive_options(
+@dataclass
+class _DirectiveOptions:
+    content: str
+    options: dict[str, Any]
+    warnings: list[ParseWarnings]
+    has_options: bool
+
+
+def _parse_directive_options(
     content: str,
     directive_class: type[Directive],
-    validate: bool = True,
+    as_yaml: bool,
+    line: int | None,
     additional_options: dict[str, str] | None = None,
-) -> tuple[str, dict, list[str]]:
+) -> _DirectiveOptions:
     """Parse (and validate) the directive option section.
 
     :returns: (content, options, validation_errors)
     """
-    options: dict[str, Any] = {}
-    validation_errors: list[str] = []
+    yaml_block: None | str = None
     if content.startswith("---"):
+        line = None if line is None else line + 1
         content = "\n".join(content.splitlines()[1:])
         match = re.search(r"^-{3,}", content, re.MULTILINE)
         if match:
             yaml_block = content[: match.start()]
             content = content[match.end() + 1 :]  # TODO advance line number
         else:
             yaml_block = content
             content = ""
         yaml_block = dedent(yaml_block)
-        try:
-            options = yaml.safe_load(yaml_block) or {}
-        except (yaml.parser.ParserError, yaml.scanner.ScannerError):
-            validation_errors.append("Invalid options format (bad YAML)")
-    elif content.lstrip().startswith(":"):
-        content_lines = content.splitlines()  # type: list
+    elif content.startswith(":"):
+        content_lines = content.splitlines()
         yaml_lines = []
         while content_lines:
-            if not content_lines[0].lstrip().startswith(":"):
+            if not content_lines[0].startswith(":"):
                 break
-            yaml_lines.append(content_lines.pop(0).lstrip()[1:])
+            yaml_lines.append(content_lines.pop(0)[1:])
         yaml_block = "\n".join(yaml_lines)
         content = "\n".join(content_lines)
+
+    has_options_block = yaml_block is not None
+
+    if as_yaml:
+        yaml_errors: list[ParseWarnings] = []
         try:
-            options = yaml.safe_load(yaml_block) or {}
+            yaml_options = yaml.safe_load(yaml_block or "") or {}
         except (yaml.parser.ParserError, yaml.scanner.ScannerError):
-            validation_errors.append("Invalid options format (bad YAML)")
+            yaml_options = {}
+            yaml_errors.append(
+                ParseWarnings(
+                    "Invalid options format (bad YAML)",
+                    line,
+                    MystWarnings.DIRECTIVE_OPTION,
+                )
+            )
+        if not isinstance(yaml_options, dict):
+            yaml_options = {}
+            yaml_errors.append(
+                ParseWarnings(
+                    "Invalid options format (not a dict)",
+                    line,
+                    MystWarnings.DIRECTIVE_OPTION,
+                )
+            )
+        return _DirectiveOptions(content, yaml_options, yaml_errors, has_options_block)
 
-    if not isinstance(options, dict):
-        options = {}
-        validation_errors.append("Invalid options format (not a dict)")
+    validation_errors: list[ParseWarnings] = []
 
-    if validation_errors:
-        return content, options, validation_errors
+    options: dict[str, str] = {}
+    if yaml_block is not None:
+        try:
+            _options, state = options_to_items(yaml_block)
+            options = dict(_options)
+        except TokenizeError as err:
+            return _DirectiveOptions(
+                content,
+                options,
+                [
+                    ParseWarnings(
+                        f"Invalid options format: {err.problem}",
+                        line,
+                        MystWarnings.DIRECTIVE_OPTION,
+                    )
+                ],
+                has_options_block,
+            )
+        if state.has_comments:
+            validation_errors.append(
+                ParseWarnings(
+                    "Directive options has # comments, which may not be supported in future versions.",
+                    line,
+                    MystWarnings.DIRECTIVE_OPTION_COMMENTS,
+                )
+            )
 
-    if (not validate) or issubclass(directive_class, TestDirective):
+    if issubclass(directive_class, TestDirective):
         # technically this directive spec only accepts one option ('option')
         # but since its for testing only we accept all options
-        return content, options, validation_errors
+        return _DirectiveOptions(content, options, [], has_options_block)
 
     if additional_options:
-        # The YAML block takes priority over additional options
+        # The options block takes priority over additional options
         options = {**additional_options, **options}
 
     # check options against spec
     options_spec: dict[str, Callable] = directive_class.option_spec
     unknown_options: list[str] = []
     new_options: dict[str, Any] = {}
+    value: str | None
     for name, value in options.items():
         try:
             convertor = options_spec[name]
         except KeyError:
             unknown_options.append(name)
             continue
-        if not isinstance(value, str):
-            if value is True or value is None:
-                value = None  # flag converter requires no argument
-            elif isinstance(value, (int, float, datetime.date, datetime.datetime)):
-                # convertor always requires string input
-                value = str(value)
-            else:
-                validation_errors.append(
-                    f'option "{name}" value not string (enclose with ""): {value}'
-                )
-                continue
+        if not value:
+            # restructured text parses empty option values as None
+            value = None
+        if convertor is flag:
+            # flag will error if value is not empty,
+            # but to be more permissive we allow any value
+            value = None
         try:
             converted_value = convertor(value)
         except (ValueError, TypeError) as error:
             validation_errors.append(
-                f"Invalid option value for {name!r}: {value}: {error}"
+                ParseWarnings(
+                    f"Invalid option value for {name!r}: {value}: {error}",
+                    line,
+                    MystWarnings.DIRECTIVE_OPTION,
+                )
             )
         else:
             new_options[name] = converted_value
 
     if unknown_options:
         validation_errors.append(
-            f"Unknown option keys: {sorted(unknown_options)} "
-            f"(allowed: {sorted(options_spec)})"
+            ParseWarnings(
+                f"Unknown option keys: {sorted(unknown_options)} "
+                f"(allowed: {sorted(options_spec)})",
+                line,
+                MystWarnings.DIRECTIVE_OPTION,
+            )
         )
 
-    return content, new_options, validation_errors
+    return _DirectiveOptions(content, new_options, validation_errors, has_options_block)
 
 
 def parse_directive_arguments(
     directive_cls: type[Directive], arg_text: str
 ) -> list[str]:
     """Parse (and validate) the directive argument section."""
     required = directive_cls.required_arguments
```

### Comparing `myst_docutils-2.0.0/myst_parser/parsers/docutils_.py` & `myst_docutils-3.0.0/myst_parser/parsers/docutils_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MyST Markdown parser for docutils."""
+
 from dataclasses import Field
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -93,16 +94,16 @@
     ):
         """Check/normalize a key-value pair setting.
 
         Items delimited by `,`, and key-value pairs delimited by `=`.
         """
         try:
             output = yaml.safe_load(value)
-        except Exception:
-            raise ValueError("Invalid YAML string")
+        except Exception as err:
+            raise ValueError("Invalid YAML string") from err
         if not isinstance(output, dict):
             raise ValueError("Expecting a YAML dictionary")
         return output
 
     return _validate_yaml
 
 
@@ -111,24 +112,24 @@
 ):
     """Validate a url_schemes setting.
 
     This is a tricky one, because it can be either a comma-separated list or a YAML dictionary.
     """
     try:
         output = yaml.safe_load(value)
-    except Exception:
-        raise ValueError("Invalid YAML string")
+    except Exception as err:
+        raise ValueError("Invalid YAML string") from err
     if isinstance(output, str):
         output = {k: None for k in output.split(",")}
     if not isinstance(output, dict):
         raise ValueError("Expecting a comma-delimited str or YAML dictionary")
     return output
 
 
-def _attr_to_optparse_option(at: Field, default: Any) -> Tuple[dict, str]:
+def _attr_to_optparse_option(at: Field, default: Any) -> Tuple[Dict[str, Any], str]:
     """Convert a field into a Docutils optparse options dict.
 
     :returns: (option_dict, default)
     """
     if at.name == "url_schemes":
         return {
             "metavar": "<comma-delimited>|<yaml-dict>",
@@ -334,15 +335,15 @@
     settings_spec = filter_settings_spec(
         Writer.settings_spec,
         "template",
     )
 
     def apply_template(self):
         subs = self.interpolation_dict()
-        return "%(body)s\n" % subs
+        return "{body}\n".format(**subs)
 
     def __init__(self):
         self.parts = {}
         self.translator_class = SimpleTranslator
 
 
 def _run_cli(writer_name: str, writer_description: str, argv: Optional[List[str]]):
```

### Comparing `myst_docutils-2.0.0/myst_parser/parsers/mdit.py` & `myst_docutils-3.0.0/myst_parser/parsers/mdit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module holds the ``create_md_parser`` function,
 which creates a parser from the config.
 """
+
 from __future__ import annotations
 
 from typing import Callable
 
 from markdown_it import MarkdownIt
 from markdown_it.renderer import RendererProtocol
 from mdit_py_plugins.amsmath import amsmath_plugin
```

### Comparing `myst_docutils-2.0.0/myst_parser/parsers/parse_html.py` & `myst_docutils-3.0.0/myst_parser/parsers/parse_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     >> str(ast[0][0])
     '<p>text</p>'
 
 Note: optional tags are not accounted for
 (see https://html.spec.whatwg.org/multipage/syntax.html#optional-tags)
 
 """
+
 from __future__ import annotations
 
 import inspect
 import itertools
 from collections import abc, deque
 from html.parser import HTMLParser
 from typing import Any, Callable, Iterable, Iterator
@@ -358,15 +359,15 @@
             count = count + 1
             if ind.name == name:
                 break
         else:
             count = 0
 
         # It pops all the items which do not match with the closing tag.
-        for _ in range(0, count):
+        for _ in range(count):
             self.stack.pop()
 
 
 class HtmlToAst(HTMLParser):
     """The tokenizer class."""
 
     # see https://html.spec.whatwg.org/multipage/syntax.html#void-elements
```

### Comparing `myst_docutils-2.0.0/myst_parser/parsers/sphinx_.py` & `myst_docutils-3.0.0/myst_parser/parsers/sphinx_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MyST Markdown parser for sphinx."""
+
 from __future__ import annotations
 
 from docutils import nodes
 from docutils.parsers.rst import Parser as RstParser
 from sphinx.parsers import Parser as SphinxParser
 from sphinx.util import logging
```

### Comparing `myst_docutils-2.0.0/myst_parser/sphinx_ext/directives.py` & `myst_docutils-3.0.0/myst_parser/sphinx_ext/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """MyST specific directives"""
+
+from __future__ import annotations
+
 from copy import copy
-from typing import List, Tuple, cast
+from typing import cast
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.directives import SphinxDirective
 from sphinx.util.docutils import SphinxRole
 
 from myst_parser.mocking import MockState
@@ -23,15 +26,15 @@
 
 class SubstitutionReferenceRole(SphinxRole):
     """Implement substitution references as a role.
 
     Note, in ``docutils/parsers/rst/roles.py`` this is left unimplemented.
     """
 
-    def run(self) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
+    def run(self) -> tuple[list[nodes.Node], list[nodes.system_message]]:
         subref_node = nodes.substitution_reference(self.rawtext, self.text)
         self.set_source_info(subref_node, self.lineno)
         subref_node["refname"] = nodes.fully_normalize_name(self.text)
         return [subref_node], []
 
 
 class FigureMarkdown(SphinxDirective):
@@ -55,15 +58,15 @@
     option_spec = {
         "width": figwidth_value,
         "class": directives.class_option,
         "align": align,
         "name": directives.unchanged,
     }
 
-    def run(self) -> List[nodes.Node]:
+    def run(self) -> list[nodes.Node]:
         figwidth = self.options.pop("width", None)
         figclasses = self.options.pop("class", None)
         align = self.options.pop("align", None)
 
         if not isinstance(self.state, MockState):
             return [self.figure_error("Directive is only supported in myst parser")]
         state = cast(MockState, self.state)
```

### Comparing `myst_docutils-2.0.0/myst_parser/sphinx_ext/main.py` & `myst_docutils-3.0.0/myst_parser/sphinx_ext/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The setup for the sphinx extension."""
+
 from typing import Any
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
 from myst_parser.parsers.docutils_ import (
     depart_container_html,
@@ -52,26 +53,26 @@
         override=True,
         html=(visit_container_html, depart_container_html),
     )
 
     for name, default, field in MdParserConfig().as_triple():
         if "sphinx" not in field.metadata.get("omit", []):
             # TODO add types?
-            app.add_config_value(f"myst_{name}", default, "env", types=Any)
+            app.add_config_value(f"myst_{name}", default, "env", types=Any)  # type: ignore[arg-type]
 
     app.connect("builder-inited", create_myst_config)
     app.connect("builder-inited", override_mathjax)
 
 
 def create_myst_config(app):
     """Create the myst config object and add it to the sphinx environment."""
     from sphinx.util import logging
 
     # Ignore type checkers because the attribute is dynamically assigned
-    from sphinx.util.console import bold  # type: ignore[attr-defined]
+    from sphinx.util.console import bold
 
     from myst_parser import __version__
     from myst_parser.config.main import MdParserConfig
 
     logger = logging.getLogger(__name__)
 
     values = {
```

### Comparing `myst_docutils-2.0.0/myst_parser/sphinx_ext/mathjax.py` & `myst_docutils-3.0.0/myst_parser/sphinx_ext/mathjax.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 1. Mathjax should not search for ``$`` delimiters, nor LaTeX amsmath environments,
    since we already achieve this with the dollarmath and amsmath mrakdown-it-py plugins
 2. amsmath math blocks should be wrapped in mathjax delimiters (default ``\\[...\\]``),
    and assigned an equation number
 
 """
+
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.ext import mathjax
 from sphinx.locale import _
 from sphinx.util import logging
 from sphinx.util.math import get_node_equation_number
 from sphinx.writers.html import HTMLTranslator
@@ -43,28 +44,28 @@
     This is accompanied by setting the `ignoreClass` on the top-level section of each MyST document.
     """
     if (
         "amsmath" in app.config["myst_enable_extensions"]
         and "mathjax" in app.registry.html_block_math_renderers
     ):
         app.registry.html_block_math_renderers["mathjax"] = (
-            html_visit_displaymath,  # type: ignore[assignment]
+            html_visit_displaymath,
             None,
         )
 
     if "dollarmath" not in app.config["myst_enable_extensions"]:
         return
-    if not app.env.myst_config.update_mathjax:  # type: ignore
+    if not app.env.myst_config.update_mathjax:  # type: ignore[attr-defined]
         return
 
-    mjax_classes = app.env.myst_config.mathjax_classes  # type: ignore
+    mjax_classes = app.env.myst_config.mathjax_classes  # type: ignore[attr-defined]
 
     if "mathjax3_config" in app.config:
         # sphinx 4 + mathjax 3
-        app.config.mathjax3_config = app.config.mathjax3_config or {}  # type: ignore
+        app.config.mathjax3_config = app.config.mathjax3_config or {}  # type: ignore[attr-defined]
         app.config.mathjax3_config.setdefault("options", {})
         if (
             "processHtmlClass" in app.config.mathjax3_config["options"]
             and app.config.mathjax3_config["options"]["processHtmlClass"]
             != mjax_classes
         ):
             log_override_warning(
```

### Comparing `myst_docutils-2.0.0/myst_parser/sphinx_ext/myst_refs.py` & `myst_docutils-3.0.0/myst_parser/sphinx_ext/myst_refs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A post-transform for overriding the behaviour of sphinx reference resolution.
 
 This is applied to MyST type references only, such as ``[text](target)``,
 and allows for nested syntax
 """
+
 from __future__ import annotations
 
 import re
 from typing import Any, cast
 
 from docutils import nodes
 from docutils.nodes import Element, document
@@ -223,15 +224,15 @@
             stddomain = cast(StandardDomain, self.env.get_domain("std"))
             for objtype in stddomain.object_types:
                 key = (objtype, target)
                 if objtype == "term":
                     key = (objtype, target.lower())
                 if key in stddomain.objects:
                     docname, labelid = stddomain.objects[key]
-                    domain_role = "std:" + stddomain.role_for_objtype(objtype)
+                    domain_role = "std:" + (stddomain.role_for_objtype(objtype) or "")
                     ref_node = make_refnode(
                         self.app.builder, refdoc, docname, labelid, contnode
                     )
                     results.append((domain_role, ref_node))
 
         # finally resolve for any other type of allowed reference domain
         for domain in self.env.domains.values():
```

### Comparing `myst_docutils-2.0.0/myst_parser/warnings_.py` & `myst_docutils-3.0.0/myst_parser/warnings_.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Central handling of warnings for the myst extension."""
+
 from __future__ import annotations
 
 from enum import Enum
 from typing import Sequence
 
 from docutils import nodes
 
@@ -20,21 +21,27 @@
 
     MD_TOPMATTER = "topmatter"
     """Issue reading front-matter."""
     MD_DEF_DUPE = "duplicate_def"
     """Duplicate Markdown reference definition."""
     MD_FOOTNOTE_DUPE = "footnote"
     """Duplicate Markdown footnote definition."""
-    MD_FOOTNOTE_MISSING = "footnote"
+    MD_FOOTNOTE_MISSING = "footnote"  # noqa: PIE796
     """Missing Markdown footnote definition."""
     MD_HEADING_NON_CONSECUTIVE = "header"
     """Non-consecutive heading levels."""
 
     DIRECTIVE_PARSING = "directive_parse"
     """Issue parsing directive."""
+    DIRECTIVE_OPTION = "directive_option"
+    """Issue parsing directive options."""
+    DIRECTIVE_OPTION_COMMENTS = "directive_comments"
+    """Directive options has # comments, which may not be supported in future versions."""
+    DIRECTIVE_BODY = "directive_body"
+    """Issue parsing directive body."""
     UNKNOWN_DIRECTIVE = "directive_unknown"
     """Unknown directive."""
     UNKNOWN_ROLE = "role_unknown"
     """Unknown role."""
 
     # cross-reference resolution
     XREF_AMBIGUOUS = "xref_ambiguous"
```

### Comparing `myst_docutils-2.0.0/pyproject.toml` & `myst_docutils-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup",
 ]
 keywords = [
     "markdown",
@@ -41,43 +42,44 @@
 
 [project.optional-dependencies]
 code_style = ["pre-commit~=3.0"]
 # for use with "linkify" extension
 linkify = ["linkify-it-py~=2.0"]
 # Note: This is only required for internal use
 rtd = [
+    "sphinx>=7",
     "ipython",
-    "sphinx-book-theme==1.0.0rc2",
-    "pydata-sphinx-theme==v0.13.0rc4",
-    "sphinx-design2",
+    "sphinx-book-theme~=1.1",
+    "sphinx-design",
     "sphinx-copybutton",
     "sphinxext-rediraffe~=0.2.7",
     # TODO this can uncommented once https://github.com/mgaitan/sphinxcontrib-mermaid/issues/109 is fixed
     # "sphinxcontrib.mermaid~=0.7.1",
-    "sphinxext-opengraph~=0.8.2",
+    "sphinxext-opengraph~=0.9.0",
     "sphinx-pyscript",
-    "sphinx-tippy>=0.3.1",
-    "sphinx-autodoc2~=0.4.2",
+    "sphinx-tippy>=0.4.3",
+    "sphinx-autodoc2~=0.5.0",
     "sphinx-togglebutton",
 ]
 testing = [
     "beautifulsoup4",
     "coverage[toml]",
-    "pytest>=7,<8",
+    "defusedxml",  # required by sphinx 7.3 testing utils
+    "pytest>=8,<9",
     "pytest-cov",
     "pytest-regressions",
-    "pytest-param-files~=0.3.4",
+    "pytest-param-files~=0.6.0",
     "sphinx-pytest",
 ]
 testing-docutils = [
     "pygments",
-    "pytest>=7,<8",
-    "pytest-param-files~=0.3.4",
+    "pytest>=8,<9",
+    "pytest-param-files~=0.6.0",
 ]
-sphinx = ["docutils>=0.16,<0.21", "sphinx>=6,<8"]
+sphinx = ["docutils>=0.18,<0.22", "sphinx>=6,<8"]
 
 [project.scripts]
 myst-anchors = "myst_parser.cli:print_anchors"
 myst-inv = "myst_parser.inventory:inventory_cli"
 myst-docutils-html = "myst_parser.parsers.docutils_:cli_html"
 myst-docutils-html5 = "myst_parser.parsers.docutils_:cli_html5"
 myst-docutils-demo = "myst_parser.parsers.docutils_:cli_html5_demo"
@@ -90,37 +92,45 @@
 
 [tool.flit.sdist]
 exclude = [
     "docs/",
     "tests/",
 ]
 
-[tool.isort]
-profile = "black"
-known_first_party = ["myst_parser", "tests"]
-known_third_party = ["docutils", "markdown_it", "sphinx"]
-# Group first party and local folder imports together
-no_lines_before = "LOCALFOLDER"
-
-[tool.ruff]
-line-length = 100
-extend-select = ["B0", "C4", "ICN", "ISC", "N", "RUF", "SIM"]
-extend-ignore = ["RUF005"]
+[tool.ruff.lint]
+extend-select = ["B", "C4", "FA", "FURB", "I", "ICN", "ISC", "N", "PERF", "PGH", "PIE", "RUF", "SIM", "UP"]
+extend-ignore = ["ISC001", "RUF005", "RUF012"]
+
+[tool.ruff.lint.per-file-ignores]
+"myst_parser/parsers/docutils_.py" = ["FA"]
+"myst_parser/config/main.py" = ["FA"]
 
 [tool.mypy]
 show_error_codes = true
 check_untyped_defs = true
 strict_equality = true
-no_implicit_optional = true
 warn_unused_ignores = true
+disallow_any_generics = true
 
 [[tool.mypy.overrides]]
 module = ["docutils.*", "yaml.*", "pygments.*"]
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+# shrink me
+module = [
+    "myst_parser.config.dc_validators",
+    "myst_parser.config.main",
+    "myst_parser.inventory",
+    "myst_parser.parsers.directives",
+    "myst_parser.parsers.docutils_",
+    "myst_parser.parsers.parse_html",
+]
+disallow_any_generics = false
+
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:.*The default for the setting.*:FutureWarning",
 ]
 
 [tool.coverage.run]
 omit = ["*/_docs.py"]
```

### Comparing `myst_docutils-2.0.0/tox.ini` & `myst_docutils-3.0.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 # To rebuild the tox environment, for example when dependencies change, use
 # `tox -r`
 
 # Note: if the following error is encountered: `ImportError while loading conftest`
 # then then deleting compiled files has been found to fix it: `find . -name \*.pyc -delete`
 
 [tox]
-envlist = py38-sphinx7
+envlist = py39-sphinx7
 
 [testenv]
 usedevelop = true
 
-[testenv:py{37,38,39,310,311}-sphinx{6,7}]
+[testenv:py{38,39,310,311,312}-sphinx{6,7}]
 deps =
     sphinx6: sphinx>=6,<7
     sphinx7: sphinx>=7,<8
 extras =
     linkify
     testing
 commands = pytest {posargs}
```

### Comparing `myst_docutils-2.0.0/PKG-INFO` & `myst_docutils-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myst-docutils
-Version: 2.0.0
+Version: 3.0.0
 Summary: An extended [CommonMark](https://spec.commonmark.org/) compliant parser,
 Keywords: markdown,lexer,parser,development,docutils,sphinx
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
@@ -12,47 +12,49 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Dist: jinja2
 Requires-Dist: markdown-it-py~=3.0
 Requires-Dist: mdit-py-plugins~=0.4
 Requires-Dist: pyyaml
 Requires-Dist: pre-commit~=3.0 ; extra == "code_style"
 Requires-Dist: linkify-it-py~=2.0 ; extra == "linkify"
+Requires-Dist: sphinx>=7 ; extra == "rtd"
 Requires-Dist: ipython ; extra == "rtd"
-Requires-Dist: sphinx-book-theme==1.0.0rc2 ; extra == "rtd"
-Requires-Dist: pydata-sphinx-theme==v0.13.0rc4 ; extra == "rtd"
-Requires-Dist: sphinx-design2 ; extra == "rtd"
+Requires-Dist: sphinx-book-theme~=1.1 ; extra == "rtd"
+Requires-Dist: sphinx-design ; extra == "rtd"
 Requires-Dist: sphinx-copybutton ; extra == "rtd"
 Requires-Dist: sphinxext-rediraffe~=0.2.7 ; extra == "rtd"
-Requires-Dist: sphinxext-opengraph~=0.8.2 ; extra == "rtd"
+Requires-Dist: sphinxext-opengraph~=0.9.0 ; extra == "rtd"
 Requires-Dist: sphinx-pyscript ; extra == "rtd"
-Requires-Dist: sphinx-tippy>=0.3.1 ; extra == "rtd"
-Requires-Dist: sphinx-autodoc2~=0.4.2 ; extra == "rtd"
+Requires-Dist: sphinx-tippy>=0.4.3 ; extra == "rtd"
+Requires-Dist: sphinx-autodoc2~=0.5.0 ; extra == "rtd"
 Requires-Dist: sphinx-togglebutton ; extra == "rtd"
-Requires-Dist: docutils>=0.16,<0.21 ; extra == "sphinx"
+Requires-Dist: docutils>=0.18,<0.22 ; extra == "sphinx"
 Requires-Dist: sphinx>=6,<8 ; extra == "sphinx"
 Requires-Dist: beautifulsoup4 ; extra == "testing"
 Requires-Dist: coverage[toml] ; extra == "testing"
-Requires-Dist: pytest>=7,<8 ; extra == "testing"
+Requires-Dist: defusedxml ; extra == "testing"
+Requires-Dist: pytest>=8,<9 ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
-Requires-Dist: pytest-param-files~=0.3.4 ; extra == "testing"
+Requires-Dist: pytest-param-files~=0.6.0 ; extra == "testing"
 Requires-Dist: sphinx-pytest ; extra == "testing"
 Requires-Dist: pygments ; extra == "testing-docutils"
-Requires-Dist: pytest>=7,<8 ; extra == "testing-docutils"
-Requires-Dist: pytest-param-files~=0.3.4 ; extra == "testing-docutils"
+Requires-Dist: pytest>=8,<9 ; extra == "testing-docutils"
+Requires-Dist: pytest-param-files~=0.6.0 ; extra == "testing-docutils"
 Project-URL: Documentation, https://myst-parser.readthedocs.io
 Project-URL: Homepage, https://github.com/executablebooks/MyST-Parser
 Provides-Extra: code_style
 Provides-Extra: linkify
 Provides-Extra: rtd
 Provides-Extra: sphinx
 Provides-Extra: testing
@@ -96,15 +98,15 @@
 
 Or for package development:
 
 ```bash
 git clone https://github.com/executablebooks/MyST-Parser
 cd MyST-Parser
 git checkout master
-pip install -e .[code_style,testing,rtd]
+pip install -e .[code_style,linkify,testing,rtd]
 ```
 
 To use the MyST parser in Sphinx, simply add: `extensions = ["myst_parser"]` to your `conf.py`.
 
 ## Contributing
 
 We welcome all contributions!
```

