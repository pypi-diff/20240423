# Comparing `tmp/ansys_pre_commit_hooks-0.3.0.tar.gz` & `tmp/ansys_pre_commit_hooks-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_pre_commit_hooks-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_pre_commit_hooks-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_pre_commit_hooks-0.3.0.tar` & `ansys_pre_commit_hooks-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1098 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/LICENSE
--rw-r--r--   0        0        0    11642 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/README.rst
--rw-r--r--   0        0        0     2928 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1458 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/__init__.py
--rw-r--r--   0        0        0    23610 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/add_license_headers.py
--rw-r--r--   0        0        0     1245 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2
--rw-r--r--   0        0        0     1091 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt
--rw-r--r--   0        0        0    13089 1970-01-01 00:00:00.000000 ansys_pre_commit_hooks-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/LICENSE
+-rw-r--r--   0        0        0    11642 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/README.rst
+-rw-r--r--   0        0        0     2928 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1458 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/__init__.py
+-rw-r--r--   0        0        0    23610 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/add_license_headers.py
+-rw-r--r--   0        0        0     1245 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2
+-rw-r--r--   0        0        0     1091 2024-04-23 07:38:15.787769 ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt
+-rw-r--r--   0        0        0    13089 1970-01-01 00:00:00.000000 ansys_pre_commit_hooks-0.3.1/PKG-INFO
```

### Comparing `ansys_pre_commit_hooks-0.3.0/LICENSE` & `ansys_pre_commit_hooks-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.3.0/README.rst` & `ansys_pre_commit_hooks-0.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 Set custom arguments
 ^^^^^^^^^^^^^^^^^^^^
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-   rev: v0.3.0
+   rev: v0.3.1
    hooks:
    - id: add-license-headers
      args: ["--custom_copyright", "custom copyright phrase", "--custom_template", "template_name", "--custom_license", "license_name", "--ignore_license_check", "--start_year", "2023"]
 
 ``args`` can also be formatted as follows:
 
 .. code:: yaml
@@ -125,28 +125,28 @@
 directories named ``src``, ``examples``, and ``tests``. To specify additional files and/or directories
 the hook should run on, add the necessary regex to the ``files`` line in your
 .pre-commit-config.yaml file:
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-     rev: v0.3.0
+     rev: v0.3.1
      hooks:
      - id: add-license-headers
        files: '(src|examples|tests|newFolder)/.*\.(py|newExtension)|\.(proto|newExtension)'
 
 Ignore specific files or file types
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 In .pre-commit-config.yaml:
 
 .. code:: yaml
 
   - repo: https://github.com/ansys/pre-commit-hooks
-    rev: v0.3.0
+    rev: v0.3.1
     hooks:
     - id: add-license-headers
       exclude: |
           (?x)^(
               path/to/file1.py |
               path/to/.*\.(ts|cpp) |
               (.folder1|folder2)/.* |
```

### Comparing `ansys_pre_commit_hooks-0.3.0/pyproject.toml` & `ansys_pre_commit_hooks-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-pre-commit-hooks"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Python wrapper to create Ansys-tailored pre-commit hooks"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -36,16 +36,16 @@
 tests = [
     "pytest==8.1.1",
     "pytest-cov==5.0.0",
 ]
 doc = [
     "ansys-sphinx-theme[autoapi]==0.15.2",
     "numpydoc==1.7.0",
-    "sphinx==7.2.6",
-    "sphinx-autodoc-typehints==2.0.1",
+    "sphinx==7.3.7",
+    "sphinx-autodoc-typehints==2.1.0",
     "sphinx-copybutton==0.5.1",
 ]
 
 
 [tool.flit.module]
 name = "ansys.pre_commit_hooks"
```

### Comparing `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/__init__.py` & `ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/add_license_headers.py` & `ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/add_license_headers.py`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2` & `ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt` & `ansys_pre_commit_hooks-0.3.1/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.3.0/PKG-INFO` & `ansys_pre_commit_hooks-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-pre-commit-hooks
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper to create Ansys-tailored pre-commit hooks
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -14,16 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata==7.1.0
 Requires-Dist: reuse==3.0.2
 Requires-Dist: GitPython==3.1.43
 Requires-Dist: ansys-sphinx-theme[autoapi]==0.15.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
-Requires-Dist: sphinx==7.2.6 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==2.0.1 ; extra == "doc"
+Requires-Dist: sphinx==7.3.7 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==2.1.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
 Requires-Dist: pytest==8.1.1 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Project-URL: Documentation, https://pre-commit-hooks.docs.ansys.com
 Project-URL: Homepage, https://github.com/ansys/pre-commit-hooks
 Project-URL: Source, https://github.com/ansys/pre-commit-hooks
 Project-URL: Tracker, https://github.com/ansys/pre-commit-hooks/issues
@@ -112,15 +112,15 @@
 
 Set custom arguments
 ^^^^^^^^^^^^^^^^^^^^
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-   rev: v0.3.0
+   rev: v0.3.1
    hooks:
    - id: add-license-headers
      args: ["--custom_copyright", "custom copyright phrase", "--custom_template", "template_name", "--custom_license", "license_name", "--ignore_license_check", "--start_year", "2023"]
 
 ``args`` can also be formatted as follows:
 
 .. code:: yaml
@@ -157,28 +157,28 @@
 directories named ``src``, ``examples``, and ``tests``. To specify additional files and/or directories
 the hook should run on, add the necessary regex to the ``files`` line in your
 .pre-commit-config.yaml file:
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-     rev: v0.3.0
+     rev: v0.3.1
      hooks:
      - id: add-license-headers
        files: '(src|examples|tests|newFolder)/.*\.(py|newExtension)|\.(proto|newExtension)'
 
 Ignore specific files or file types
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 In .pre-commit-config.yaml:
 
 .. code:: yaml
 
   - repo: https://github.com/ansys/pre-commit-hooks
-    rev: v0.3.0
+    rev: v0.3.1
     hooks:
     - id: add-license-headers
       exclude: |
           (?x)^(
               path/to/file1.py |
               path/to/.*\.(ts|cpp) |
               (.folder1|folder2)/.* |
```

