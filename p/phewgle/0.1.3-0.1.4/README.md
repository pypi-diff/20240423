# Comparing `tmp/phewgle-0.1.3.tar.gz` & `tmp/phewgle-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phewgle-0.1.3.tar", max compression
+gzip compressed data, was "phewgle-0.1.4.tar", max compression
```

## Comparing `phewgle-0.1.3.tar` & `phewgle-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      677 2024-04-22 15:23:01.836730 phewgle-0.1.3/README.md
--rw-r--r--   0        0        0      129 2024-04-22 15:23:01.836730 phewgle-0.1.3/phewgle/__init__.py
--rw-r--r--   0        0        0     3935 2024-04-22 15:23:01.836730 phewgle-0.1.3/phewgle/common.py
--rw-r--r--   0        0        0     7297 2024-04-22 15:23:01.840730 phewgle-0.1.3/phewgle/fugle.py
--rw-r--r--   0        0        0     1645 2024-04-22 15:23:01.840730 phewgle-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 phewgle-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      770 2024-04-23 07:54:02.217916 phewgle-0.1.4/README.md
+-rw-r--r--   0        0        0      129 2024-04-23 07:54:02.217916 phewgle-0.1.4/phewgle/__init__.py
+-rw-r--r--   0        0        0     3935 2024-04-23 07:54:02.217916 phewgle-0.1.4/phewgle/common.py
+-rw-r--r--   0        0        0     7297 2024-04-23 07:54:02.217916 phewgle-0.1.4/phewgle/fugle.py
+-rw-r--r--   0        0        0     1624 2024-04-23 07:54:02.217916 phewgle-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 phewgle-0.1.4/PKG-INFO
```

### Comparing `phewgle-0.1.3/README.md` & `phewgle-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # phewgle
 
+[![image](https://img.shields.io/pypi/v/phewgle.svg)](https://pypi.python.org/pypi/phewgle)
+
 **A custom-build version of the Fugle library `fugle-trade-python` with customized features.**
 
 ## Prerequisite
 1. Modify the `User` field in the `.ini` config file by adding `Password` and `CertPassword` sub-items.
     ```
     ...
     [User]
```

### Comparing `phewgle-0.1.3/phewgle/common.py` & `phewgle-0.1.4/phewgle/common.py`

 * *Files identical despite different names*

### Comparing `phewgle-0.1.3/phewgle/fugle.py` & `phewgle-0.1.4/phewgle/fugle.py`

 * *Files identical despite different names*

### Comparing `phewgle-0.1.3/pyproject.toml` & `phewgle-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "phewgle"
-version = "0.1.3"
+version = "0.1.4"
 description = "A custom-build version of the Fugle library `fugle-trade-python` with customized features."
 authors = ["Thomas Lin <thomaslin@tradinglab.app>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.26.4"
 keyring = "^25.1.0"
 keyrings-cryptfile = "^1.3.9"
 fugle-trade-core = "^2.0.0"
 python-dotenv = "^1.0.1"
-mkdocs = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^24.4.0"}
 build = "^1.2.1"
 bump-my-version = "^0.20.1"
 codespell = "^2.2.6"
 wheel = "^0.43.0"
@@ -27,34 +26,34 @@
 pytest-runner = "^6.0.1"
 ipykernel = "^6.29.4"
 livereload = "^2.6.3"
 nbconvert = "^7.16.3"
 nbformat = "^5.10.4"
 sphinx = "^7.3.7"
 watchdog = "^4.0.0"
-mkdocs = "^1.6.0"
-mkdocs-git-revision-date-plugin = "^0.3.2"
-mkdocs-git-revision-date-localized-plugin = "^1.2.4"
-mkdocs-jupyter = ">=0.24.0"
-mkdocs-material = ">=9.1.3"
-mkdocs-pdf-export-plugin = "^0.5.10"
-mkdocstrings = "^0.24.3"
-mkdocstrings-crystal = "^0.3.7"
-mkdocstrings-python-legacy = "^0.2.3"
 pygments = "^2.17.2"
 pymdown-extensions = "^10.8"
 jupyterlab = "^4.1.6"
 python-dotenv = "^1.0.1"
+mkdocs-git-revision-date-plugin = "^0.3.2"
+mkdocs-git-revision-date-localized-plugin = "^1.2.4"
+mkdocstrings-python-legacy = "^0.2.3"
+mkdocstrings-crystal = "^0.3.7"
+mkdocs = "^1.6.0"
+mkdocstrings = "^0.24.3"
+mkdocs-pdf-export-plugin = "^0.5.10"
+mkdocs-material = "9.1.3"
+mkdocs-jupyter = "^0.24.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpversion]
-current_version = "0.1.3"
+current_version = "0.1.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

