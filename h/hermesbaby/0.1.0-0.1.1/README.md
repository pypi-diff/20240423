# Comparing `tmp/hermesbaby-0.1.0.tar.gz` & `tmp/hermesbaby-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermesbaby-0.1.0.tar", max compression
+gzip compressed data, was "hermesbaby-0.1.1.tar", max compression
```

## Comparing `hermesbaby-0.1.0.tar` & `hermesbaby-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      117 2024-04-22 04:05:52.750497 hermesbaby-0.1.0/AUTHORS.rst
--rw-r--r--   0        0        0     1104 2024-04-22 04:07:33.370496 hermesbaby-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1694 2024-04-22 04:07:42.126496 hermesbaby-0.1.0/README.rst
--rw-r--r--   0        0        0      654 2024-04-22 05:16:34.742470 hermesbaby-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-22 04:34:17.510486 hermesbaby-0.1.0/src/hermesbaby/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 04:34:33.114486 hermesbaby-0.1.0/src/hermesbaby/cmd/__init_.py
--rw-r--r--   0        0        0      229 2024-04-22 04:33:29.126486 hermesbaby-0.1.0/src/hermesbaby/cmd/hb.py
--rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 hermesbaby-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-04-22 04:05:52.750497 hermesbaby-0.1.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1104 2024-04-22 04:07:33.370496 hermesbaby-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1694 2024-04-22 04:07:42.126496 hermesbaby-0.1.1/README.rst
+-rw-r--r--   0        0        0      704 2024-04-23 04:02:33.591530 hermesbaby-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-22 04:34:17.510486 hermesbaby-0.1.1/src/hermesbaby/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:34:33.114486 hermesbaby-0.1.1/src/hermesbaby/cmd/__init_.py
+-rw-r--r--   0        0        0      269 2024-04-23 04:02:17.447530 hermesbaby-0.1.1/src/hermesbaby/cmd/hb.py
+-rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 hermesbaby-0.1.1/PKG-INFO
```

### Comparing `hermesbaby-0.1.0/LICENSE.txt` & `hermesbaby-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hermesbaby-0.1.0/README.rst` & `hermesbaby-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `hermesbaby-0.1.0/pyproject.toml` & `hermesbaby-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "hermesbaby"
-version = "0.1.0"
+version = "0.1.1"
 description = "The Software Engineers' Typewriter"
 authors = ["Alexander Mann-Wahrenberg (basejumpa) <alexander.mannwahrenberg@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "^7.3.7"
 
+[tool.poetry.scripts]
+hb = "hermesbaby.cli:main"
+
 [build-system]
 requires = [
     "poetry-core",
     "setuptools>=46.1.0", 
     "setuptools_scm[toml]>=5"
 ]
 
-build-backend = "poetry.core.masonry.api"
-# build-backend = "setuptools.build_meta"
+# build-backend = "poetry.core.masonry.api"
+build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # For smarter version schemes and other configuration options,
 # check out https://github.com/pypa/setuptools_scm
 version_scheme = "no-guess-dev"
```

### Comparing `hermesbaby-0.1.0/PKG-INFO` & `hermesbaby-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermesbaby
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Software Engineers' Typewriter
 License: MIT
 Author: Alexander Mann-Wahrenberg (basejumpa)
 Author-email: alexander.mannwahrenberg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

