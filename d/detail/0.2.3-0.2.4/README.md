# Comparing `tmp/detail-0.2.3.tar.gz` & `tmp/detail-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detail-0.2.3.tar", max compression
+gzip compressed data, was "detail-0.2.4.tar", max compression
```

## Comparing `detail-0.2.3.tar` & `detail-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1456 2024-04-18 12:09:29.055768 detail-0.2.3/LICENSE
--rw-r--r--   0        0        0     1786 2024-04-18 12:09:29.055768 detail-0.2.3/README.md
--rw-r--r--   0        0        0      256 2024-04-18 12:09:29.055768 detail-0.2.3/detail/__init__.py
--rw-r--r--   0        0        0     3456 2024-04-18 12:09:29.055768 detail-0.2.3/detail/cli.py
--rw-r--r--   0        0        0    19842 2024-04-18 12:09:29.055768 detail-0.2.3/detail/core.py
--rw-r--r--   0        0        0      678 2024-04-18 12:09:29.055768 detail-0.2.3/detail/exceptions.py
--rw-r--r--   0        0        0     4590 2024-04-18 12:09:29.055768 detail-0.2.3/detail/github.py
--rw-r--r--   0        0        0        0 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/__init__.py
--rw-r--r--   0        0        0     3833 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_cli.py
--rw-r--r--   0        0        0     3116 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_core.py
--rw-r--r--   0        0        0     7142 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_github.py
--rw-r--r--   0        0        0    12860 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_integration.py
--rw-r--r--   0        0        0     1164 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_utils.py
--rw-r--r--   0        0        0       66 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_version.py
--rw-r--r--   0        0        0     1106 2024-04-18 12:09:29.055768 detail-0.2.3/detail/utils.py
--rw-r--r--   0        0        0       73 2024-04-18 12:09:29.055768 detail-0.2.3/detail/version.py
--rw-r--r--   0        0        0     2194 2024-04-18 12:09:50.400089 detail-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 detail-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-23 00:02:44.551489 detail-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1785 2024-04-23 00:02:44.551489 detail-0.2.4/README.md
+-rw-r--r--   0        0        0      256 2024-04-23 00:02:44.551489 detail-0.2.4/detail/__init__.py
+-rw-r--r--   0        0        0     3456 2024-04-23 00:02:44.551489 detail-0.2.4/detail/cli.py
+-rw-r--r--   0        0        0    19842 2024-04-23 00:02:44.551489 detail-0.2.4/detail/core.py
+-rw-r--r--   0        0        0      678 2024-04-23 00:02:44.551489 detail-0.2.4/detail/exceptions.py
+-rw-r--r--   0        0        0     4590 2024-04-23 00:02:44.551489 detail-0.2.4/detail/github.py
+-rw-r--r--   0        0        0        0 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/__init__.py
+-rw-r--r--   0        0        0     3833 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/test_cli.py
+-rw-r--r--   0        0        0     3116 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/test_core.py
+-rw-r--r--   0        0        0     7142 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/test_github.py
+-rw-r--r--   0        0        0    12860 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/test_integration.py
+-rw-r--r--   0        0        0     1164 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/test_utils.py
+-rw-r--r--   0        0        0       66 2024-04-23 00:02:44.551489 detail-0.2.4/detail/tests/test_version.py
+-rw-r--r--   0        0        0     1106 2024-04-23 00:02:44.551489 detail-0.2.4/detail/utils.py
+-rw-r--r--   0        0        0       73 2024-04-23 00:02:44.551489 detail-0.2.4/detail/version.py
+-rw-r--r--   0        0        0     2223 2024-04-23 00:03:06.127557 detail-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 detail-0.2.4/PKG-INFO
```

### Comparing `detail-0.2.3/LICENSE` & `detail-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/README.md` & `detail-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 ## Installation
 
 Install detail with:
 
     pip3 install detail
 
-
 ## Contributing Guide
 
 For information on setting up detail for development and contributing changes, view [CONTRIBUTING.rst](CONTRIBUTING.rst).
 
 ## Creators
 
 - @wesleykendall (Wes Kendall)
```

### Comparing `detail-0.2.3/detail/cli.py` & `detail-0.2.4/detail/cli.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/core.py` & `detail-0.2.4/detail/core.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/exceptions.py` & `detail-0.2.4/detail/exceptions.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/github.py` & `detail-0.2.4/detail/github.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/tests/test_cli.py` & `detail-0.2.4/detail/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/tests/test_core.py` & `detail-0.2.4/detail/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/tests/test_github.py` & `detail-0.2.4/detail/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/tests/test_integration.py` & `detail-0.2.4/detail/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/tests/test_utils.py` & `detail-0.2.4/detail/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/detail/utils.py` & `detail-0.2.4/detail/utils.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.3/pyproject.toml` & `detail-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 fail_under = 100
 
 [tool.poetry]
 name = "detail"
 packages = [
   { include = "detail" },
 ]
-version = "0.2.3"
+version = "0.2.4"
 description = "Build automations off of structured notes in your project"
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
@@ -66,14 +66,15 @@
 mkdocs = "1.5.3"
 black = "24.4.0"
 mkdocs-material = "9.5.18"
 mkdocstrings-python = "1.9.2"
 footing = "*"
 setuptools = "*"
 poetry-core = "*"
+typing-extensions = "4.11.0"
 
 [tool.poetry.scripts]
 detail = 'detail.cli:main'
 
 [tool.pytest.ini_options]
 xfail_strict = true
 testpaths = "detail/tests"
```

### Comparing `detail-0.2.3/PKG-INFO` & `detail-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detail
-Version: 0.2.3
+Version: 0.2.4
 Summary: Build automations off of structured notes in your project
 Home-page: https://github.com/Opus10/detail
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.8.0,<4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -52,15 +52,14 @@
 
 ## Installation
 
 Install detail with:
 
     pip3 install detail
 
-
 ## Contributing Guide
 
 For information on setting up detail for development and contributing changes, view [CONTRIBUTING.rst](CONTRIBUTING.rst).
 
 ## Creators
 
 - @wesleykendall (Wes Kendall)
```

