# Comparing `tmp/postbp-1.0.1.tar.gz` & `tmp/postbp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postbp-1.0.1.tar", last modified: Thu Apr  4 15:59:04 2024, max compression
+gzip compressed data, was "postbp-1.0.2.tar", last modified: Tue Apr 23 16:21:39 2024, max compression
```

## Comparing `postbp-1.0.1.tar` & `postbp-1.0.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.161995 postbp-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 15:58:49.000000 postbp-1.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.149994 postbp-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.153994 postbp-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.153994 postbp-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-04 15:58:49.000000 postbp-1.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 15:58:49.000000 postbp-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 15:58:49.000000 postbp-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 15:58:49.000000 postbp-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 15:59:04.157995 postbp-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-04 15:58:49.000000 postbp-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.157995 postbp-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/dailyfirevectors.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/dataloader.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.157995 postbp-1.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/finalfirevectors.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.157995 postbp-1.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/postbp.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/spreadrose.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/tessellation.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 15:58:49.000000 postbp-1.0.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-04 15:58:49.000000 postbp-1.0.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.157995 postbp-1.0.1/postbp/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/dailyfirevectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/finalfirevectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/postbp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/spreadrose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-04 15:58:49.000000 postbp-1.0.1/postbp/tessellation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.157995 postbp-1.0.1/postbp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 15:59:04.000000 postbp-1.0.1/postbp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 15:59:04.000000 postbp-1.0.1/postbp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:59:04.000000 postbp-1.0.1/postbp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 15:59:04.000000 postbp-1.0.1/postbp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 15:59:04.000000 postbp-1.0.1/postbp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 15:59:04.000000 postbp-1.0.1/postbp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 15:58:49.000000 postbp-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 15:58:49.000000 postbp-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 15:58:49.000000 postbp-1.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:59:04.161995 postbp-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:04.157995 postbp-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 15:58:49.000000 postbp-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 15:58:49.000000 postbp-1.0.1/tests/test_postbp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.192233 postbp-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-23 16:21:28.000000 postbp-1.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.180233 postbp-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.184233 postbp-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.184233 postbp-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-23 16:21:28.000000 postbp-1.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-23 16:21:28.000000 postbp-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 16:21:28.000000 postbp-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:21:28.000000 postbp-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-23 16:21:39.192233 postbp-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 16:21:28.000000 postbp-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.188233 postbp-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/dailyfirevectors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/dataloader.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.188233 postbp-1.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/finalfirevectors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.188233 postbp-1.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/postbp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/spreadrose.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/tessellation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 16:21:28.000000 postbp-1.0.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-23 16:21:28.000000 postbp-1.0.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.188233 postbp-1.0.2/postbp/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/dailyfirevectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/finalfirevectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/postbp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/spreadrose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-23 16:21:28.000000 postbp-1.0.2/postbp/tessellation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.188233 postbp-1.0.2/postbp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-23 16:21:39.000000 postbp-1.0.2/postbp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-23 16:21:39.000000 postbp-1.0.2/postbp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:21:39.000000 postbp-1.0.2/postbp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 16:21:39.000000 postbp-1.0.2/postbp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 16:21:39.000000 postbp-1.0.2/postbp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:21:39.000000 postbp-1.0.2/postbp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-23 16:21:28.000000 postbp-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 16:21:28.000000 postbp-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-23 16:21:28.000000 postbp-1.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:21:39.192233 postbp-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:21:39.188233 postbp-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 16:21:28.000000 postbp-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-23 16:21:28.000000 postbp-1.0.2/tests/test_postbp.py
```

### Comparing `postbp-1.0.1/.github/workflows/docs-build.yml` & `postbp-1.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.github/workflows/docs.yml` & `postbp-1.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.github/workflows/installation.yml` & `postbp-1.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.github/workflows/macos.yml` & `postbp-1.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.github/workflows/pypi.yml` & `postbp-1.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.github/workflows/ubuntu.yml` & `postbp-1.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.github/workflows/windows.yml` & `postbp-1.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/.gitignore` & `postbp-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/LICENSE` & `postbp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/PKG-INFO` & `postbp-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postbp
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python Library
 Author-email: Ning Liu <ning.liu@nrcan-rncan.gc.ca>
 License: MIT License
 Project-URL: Homepage, https://github.com/nliu-cfs/postbp
 Keywords: postbp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `postbp-1.0.1/docs/contributing.md` & `postbp-1.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/docs/examples/intro.ipynb` & `postbp-1.0.2/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/docs/installation.md` & `postbp-1.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/mkdocs.yml` & `postbp-1.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/postbp/__init__.py` & `postbp-1.0.2/postbp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Top-level package for postbp."""
 
 __author__ = """Ning Liu"""
 __email__ = "ning.liu@nrcan-rncan.gc.ca"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from .common import (
     prj2hex,  #noqa
     pij_to_shp, #noqa
 )
 from .dataloader import(
     read_fireshp,  #noqa
     read_pointcsv,   #noqa
     read_pointshp,   #noqa
+    validify_fireshp, #noqa
 ) 
 
 from .postbp import (
     generate_ign_prob,  #noqa
     generate_burn_prob,  #noqa
     generate_ssr,  #noqa
     generate_fireshed,   #noqa
```

### Comparing `postbp-1.0.1/postbp/common.py` & `postbp-1.0.2/postbp/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """The common module contains common functions and classes used by the other modules.
 """
 import geopandas as gpd
 from shapely.geometry import LineString #, Polygon, Point
+from tqdm import tqdm
 
 def prj2hex(shp0, hexagons, threshold=0):
-    """Generate intersection shape by overlaying shapefile shp0 and the hexagon shapefile
+    """Generate a geometric intersection of shp0 and the hexagon shapefile.
     option to set threshold
 
     Args:
-        shp0 (type:GeoDataFrame): _description_
+        shp0 (GeoDataFrame): GeoDataFrame to be identified by hexagon shape
         hexagons (GeoDataFrame): hexagonal patches
-        threshold (int, optional): _description_. Defaults to 0.
+        threshold (float, optional): Value between 0 and 1. The proportion for classifying hexagon as intersecting with shp0. Defaults to 0.
 
     Returns:
-        GeoDataFrame: _description_
+        GeoDataFrame: Return a GeoDataFrame of the intersection with hexagon ID field as attributes
     """    
-    
-    shp1 = gpd.overlay(shp0, hexagons, how='intersection') 
+    thresholdArea = hexagons.at[1,'geometry'].area * threshold
+    try:
+        shp1 = gpd.overlay(shp0, hexagons, how='intersection') 
+    except:
+        pass    
     shp1['areaFire'] = shp1.geometry.area
-    shp1 = shp1.loc[shp1['areaFire'] > threshold]
+    shp1 = shp1.loc[shp1['areaFire'] > thresholdArea]
     shp1.drop(labels='areaFire', axis=1, inplace=True)
     return shp1
 
 def pij_to_shp(pij_input, nodes, **kwargs):
-    """Generate shapefile of lines connecting i and j, with column indicating probability of spread
+    """Adding geometry to pij vectors file
 
     Args:
-        pij_input (_type_): _description_
-        nodes (_type_): _description_
+        pij_input (DataFrame): pij dataframe
+        nodes (GeoDataFrame): centroid of the hexagonal patches
 
     Returns:
-        _type_: _description_
+        GeoDataFrame: pij value with geometry of lines connecting node-i and node-j
     """    
     
     pij = pij_input.copy()
     node = nodes.copy()
     if 'Node_ID' in kwargs:
         node = node.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     if 'column_i' in kwargs:
```

### Comparing `postbp-1.0.1/postbp/dailyfirevectors.py` & `postbp-1.0.2/postbp/dailyfirevectors.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 warnings.filterwarnings("ignore")
 from tqdm import tqdm
 
 def angle(record):
     """Calculate angle from three points: ignition point and the points where fire spread from and to.  
 
     Args:
-        record (_type_): _description_
+        record (dataframe): a row of the output from generate_daily_vectors function
 
     Returns:
-        _type_: _description_
+        degree value: the value of beta angle, i.e. the angle between the line connecting ignition point and starting point of fire, and the line connecting the hexagon nodes that a fire spreading from and to. 
     """    
     x0, y0 = record['geometry_x'].x, record['geometry_x'].y
     x1, y1 = record['geometry'].x, record['geometry'].y
     x2, y2 = record['geometry_y'].x, record['geometry_y'].y
     xv1, yv1 = x1-x0, y1-y0
     xv2, yv2 = x2-x0, y2-y0
     deg1 = (360 + degrees(atan2(xv1, yv1))) % 360
     deg2 = (360 + degrees(atan2(xv2, yv2))) % 360
     return deg2 - deg1 if deg1 <= deg2 else 360 - (deg1 - deg2)
 
 
 
 def generate_daily_vectors(fireshp, ignition, hexagons, bufferFactor=10, **kwargs):
-    """_summary_
+    """Generate fire spreading vectors from the daily fire spread perimeters
 
     Args:
-        fireshp (_type_): _description_
-        ignition (_type_): _description_
-        hexagons (_type_): _description_
+        fireshp (GeoDataFrame): the daily fire perimeter geometry with fire ID and day of spread as attributes
+        ignition (GeoDataFrame): ignition point shapes with fire ID field in attributes
+        hexagons (GeoDataFrame): geometry of hexagonal patches with ID field
         bufferFactor (int, optional): convert ignition point into a circle polygon of the diameter of bufferFactor
 it shall be small enough so as not to have ignition point locates in more than one hexagons it also defines threshold for the minimum area of fire perimeter to be in a hexagon to be regarded as burned. Defaults to 10.
 
     Returns:
-        _type_: _description_
+        DataFrame: a dataframe table containing fire starting hexagon ID (i), destination hexagon ID (j), 'day', fire ID, and ignition hexagon ID 
     """    
     hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
         hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     
     threshold = 3.1415926*bufferFactor**2 - 1 
     SRID = fireshp.crs
@@ -102,22 +102,22 @@
             df = pd.concat([df, dfMore], sort = True)
         except Exception as e:
             with open("errorlog_dailyfire.txt", "w+") as f:
                 f.write(f'{e} occurs for fire ID # {i} \n')    
     return df
 
 def calc_angles(vectors, nodes, **kwargs):
-    """_summary_
+    """Calculate beta angle for every pair of vectors of fire spread
 
     Args:
-        vectors (_type_): _description_
-        nodes (_type_): _description_
+        vectors (dataframe): outputs from generate_daily_vectors function
+        nodes (GeoDataFrame): centroid points of the hexagonal patch network
 
     Returns:
-        _type_: _description_
+        dataframe: a dataframe containing geometry of i, j, ignition point and beta angle value of each vector
     """    
     node = nodes.copy()
     if 'Node_ID' in kwargs:
         node = node.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
 
     vectorsW = vectors.copy()
     vectorsW = node.merge(vectors, left_on='Node_ID', right_on='column_i', how='right')
@@ -133,27 +133,27 @@
         except:
             vectorsW.at[index, 'angle'] = 181  # when origin is identical to ignition
     vectorsW.loc[vectorsW['day'] == 999, 'angle'] = 361  # from ignition to all hexes in perimeter
     vectorsW.loc[vectorsW['day'] == 1, 'angle'] = 181  # in day 1: origin is identical to ignition
     vectorsW.drop_duplicates(subset = ['day', 'column_j', 'fire', 'ignPt', 'column_i'], keep = 'first', inplace = True)
     return vectorsW
 
-def select_angle(vectors, alpha):
-    """_summary_
+def select_angle(vectors_with_angle, alpha):
+    """Select intended angle of fire spread sector
 
     Args:
-        vectors (_type_): _description_
-        alpha (_type_): _description_
+        vectors_with_angle (dataframe): outputs from calc_angles function
+        alpha (degree): fire spread sector angle (alpha angle), value from 0 to 360
 
     Returns:
-        _type_: _description_
+        dataframe: a dataframe containing geometry of i, j, ignition point and beta angle value of each vector
     """    
     maxAngle = alpha/2+180
     minAngle = 180-alpha/2
-    vectorsV = vectors.copy()
+    vectorsV = vectors_with_angle.copy()
     vectorsV.drop(vectorsV.loc[vectorsV['angle'] > maxAngle].index, inplace = True)
     vectorsV.drop(vectorsV.loc[vectorsV['angle'] < minAngle].index, inplace = True)
     vectorsV.sort_values(by = ['fire','day'], inplace = True)
     vectorsV.reset_index(drop = True, inplace = True)
     return vectorsV
```

### Comparing `postbp-1.0.1/postbp/tessellation.py` & `postbp-1.0.2/postbp/tessellation.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 3. projection of the hexagon network to be the same as that of the fire shapefile.
 4. generate the centroid of the hexes as nodes shapefile
 5. generate arcs connecting neighbouring nodes
 
 '''
 
 import geopandas as gpd
+import pandas as pd
 from shapely.geometry import Polygon, Point, LineString
 import warnings
 warnings.filterwarnings("ignore")
 import math
 from tqdm import tqdm
 
-def create_hexnodes(area, xmin, ymin, xmax, ymax):
+def _create_hexnodes(area, xmin, ymin, xmax, ymax):
     nodes = []
     
     side = 3**0.25 * math.sqrt(2 * area / 9)
     v_step = math.sqrt(3) * side
     h_step = 1.5 * side
 
 
@@ -48,116 +49,123 @@
             c_y += v_step
         c_x += h_step
         c_y = v_start_array[v_start_idx]
         v_start_idx = (v_start_idx + 1) % 2
         
     return nodes
 
-def create_hexgrids(area, x, y):
+def _create_hexgrids(area, x, y):
     """
     Create a hexagon centered on (x, y)
     :param x: x-coordinate of the hexagon's center
     :param y: y-coordinate of the hexagon's center
     :return: The polygon containing the hexagon's coordinates
     """
     # l: length of the hexagon's side
     l = 3**0.25 * math.sqrt(2 * area / 9)
     c = [[x + math.cos(math.radians(angle)) * l, y + math.sin(math.radians(angle)) * l] for angle in range(0, 360, 60)]
     return Polygon(c)
 
 def create_hexagons_nodes(boundaryShp, **kwargs):
-    """_summary_
-
+    """Creat geodataframe of hexagonal patches and the nodes (centroids) of the hexagons of defined size and range.
+       Hexagon size can be defined in area, side length, or long diameter. Must input one parameter out of the three options.
     Args:
-        boundaryShp (_type_): _description_
+        boundaryShp (GeoDataFrame): the geodataframe defines the range that the hexagonal patches covers
+        area (float, OPTIONAL): define the size of each hexagon by area in cubic meters
+        side (float, OPTIONAL): define the size of each hexagon by side length in meter
+        diameter (float, OPTIONAL): define the size of each hexagon by long diameter in meter
 
     Returns:
-        _type_: _description_
+        GeoDataFrame: return geodataframes of hexagons and nodes of the defined size and covering the defined range.
+                      Note to give two variable names when using this function.
     """    
     if 'area' in kwargs:
         area = kwargs['area']
 
     if "side" in kwargs:
         area = kwargs["side"]**2*3/2*math.sqrt(3)
 
     if "diameter" in kwargs:
         area = kwargs["diameter"]**2*3/8*math.sqrt(3)
     
     myCRS = boundaryShp.crs
     xmin,ymin,xmax,ymax =  boundaryShp.total_bounds
-    nodes = create_hexnodes(area, xmin, ymin, xmax, ymax)
-    hexagons = [create_hexgrids(area, node[0], node[1]) for node in nodes]
+    nodes = _create_hexnodes(area, xmin, ymin, xmax, ymax)
+    hexagons = [_create_hexgrids(area, node[0], node[1]) for node in nodes]
     
     nodes = [Point(node) for node in nodes]
     nodes = gpd.GeoDataFrame({'geometry': nodes})
     nodes['Node_ID'] = nodes.index + 1
     nodes.crs = myCRS
     hexagons = gpd.GeoDataFrame({'geometry':hexagons})
     hexagons['Node_ID'] = hexagons.index + 1
     hexagons.crs = myCRS
 
     return hexagons, nodes
 
 def create_hexagons(boundaryShp, **kwargs):
-    """_summary_
-
+    """Creat geodataframe of hexagonal patches of defined size and range.
+       Hexagon size can be defined in area, side length, or long diameter. Must input one parameter out of the three options.
     Args:
-        boundaryShp (_type_): _description_
+        boundaryShp (GeoDataFrame): the geodataframe defines the range that the hexagonal patches covers
+        area (float, OPTIONAL): define the size of each hexagon by area in cubic meters
+        side (float, OPTIONAL): define the size of each hexagon by side length in meter
+        diameter (float, OPTIONAL): define the size of each hexagon by long diameter in meter
 
     Returns:
-        _type_: _description_
-    """    
+        GeoDataFrame: return a geodataframe of hexagonal network of the defined size and covering the defined range.
+    """   
     if 'area' in kwargs:
         area = kwargs['area']
 
     if "side" in kwargs:
         area = kwargs["side"]**2*3/2*math.sqrt(3)
 
     if "diameter" in kwargs:
         area = kwargs["diameter"]**2*3/8*math.sqrt(3)
     
     myCRS = boundaryShp.crs
     xmin,ymin,xmax,ymax =  boundaryShp.total_bounds
-    nodes = create_hexnodes(area, xmin, ymin, xmax, ymax)
-    hexagons = [create_hexgrids(area, node[0], node[1]) for node in nodes]
+    nodes = _create_hexnodes(area, xmin, ymin, xmax, ymax)
+    hexagons = [_create_hexgrids(area, node[0], node[1]) for node in nodes]
     
     nodes = [Point(node) for node in nodes]
     nodes = gpd.GeoDataFrame({'geometry': nodes})
     nodes['Node_ID'] = nodes.index + 1
     nodes.crs = myCRS
     hexagons = gpd.GeoDataFrame({'geometry':hexagons})
     hexagons['Node_ID'] = hexagons.index + 1
     hexagons.crs = myCRS
 
     return hexagons
 
 def nodes_from_hexagons(hexagons):
-    """_summary_
+    """Generate nodes geometry from hexagons
 
     Args:
-        hexagons (_type_): _description_
+        hexagons (GeoDataFrame): geometry and ID of hexagonal patches
 
     Returns:
-        _type_: _description_
+        GeoDataFrame: return nodes geometry with ID attributes same as the hexagons.
     """    
     nodes = hexagons.copy()
     nodes['centroid'] = nodes.geometry.centroid
     nodes.drop(labels='geometry', axis=1, inplace=True)
     nodes.rename(columns={'centroid':'geometry'}, inplace=True)
     nodes = nodes.set_geometry('geometry')
     return nodes
 
 def create_arcs(hexagons, **kwargs):
-    """_summary_
+    """Create geometry of arcs connecting each neighbouring hexagons.
 
     Args:
-        hexagons (_type_): _description_
+        hexagons (GeoDataFrame): geometry and ID of hexagonal patches
 
     Returns:
-        _type_: _description_
+        GeoDataFrame: return arcs geometry with attributes indicating IDs of the two hexagons it connects.
     """    
     hexagon = hexagons.copy()
     if 'Node_ID' in kwargs:
         hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
         
     nodes = nodes_from_hexagons(hexagon)
     nodes = nodes.set_index('Node_ID')
@@ -170,12 +178,13 @@
         nnnn = hexagon[~hexagon.geometry.disjoint(hexagon.at[index,'geometry'])].index.tolist()
         nnnn = [i for i in nnnn if index != i]
         mmmm = [index] * len(nnnn)
         mmnn = [LineString(xy) for xy in zip(nodes.loc[mmmm].geometry, nodes.loc[nnnn].geometry)]
         mmnn = gpd.GeoDataFrame(df, crs = SRID, geometry = mmnn )
         mmnn['Node_1'] = mmmm
         mmnn['Node_2'] = nnnn
-        arcs = arcs.append(mmnn)
+        arcs = pd.concat([arcs,mmnn])
+
     arcs['Node_1'] = arcs['Node_1'].astype(int)
     arcs['Node_2'] = arcs['Node_2'].astype(int)
 
     return arcs
```

### Comparing `postbp-1.0.1/postbp.egg-info/PKG-INFO` & `postbp-1.0.2/postbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postbp
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python Library
 Author-email: Ning Liu <ning.liu@nrcan-rncan.gc.ca>
 License: MIT License
 Project-URL: Homepage, https://github.com/nliu-cfs/postbp
 Keywords: postbp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `postbp-1.0.1/postbp.egg-info/SOURCES.txt` & `postbp-1.0.2/postbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postbp-1.0.1/pyproject.toml` & `postbp-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "postbp"
-version = "1.0.1"
+version = "1.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "A Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "1.0.1"
+current_version = "1.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

