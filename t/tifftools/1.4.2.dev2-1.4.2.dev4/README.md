# Comparing `tmp/tifftools-1.4.2.dev2.tar.gz` & `tmp/tifftools-1.4.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifftools-1.4.2.dev2.tar", last modified: Thu Feb 29 17:55:57 2024, max compression
+gzip compressed data, was "tifftools-1.4.2.dev4.tar", last modified: Tue Apr 23 12:10:38 2024, max compression
```

## Comparing `tifftools-1.4.2.dev2.tar` & `tifftools-1.4.2.dev4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 17:55:57.599858 tifftools-1.4.2.dev2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 17:55:57.591858 tifftools-1.4.2.dev2/.circleci/
--rw-r--r--   0 root         (0) root         (0)     4031 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      596 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1633 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     3425 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)      549 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      148 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8830 2024-02-29 17:55:57.599858 tifftools-1.4.2.dev2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7969 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/README.rst
--rw-r--r--   0 root         (0) root         (0)      424 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/codecov.yml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 17:55:57.599858 tifftools-1.4.2.dev2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1958 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 17:55:57.591858 tifftools-1.4.2.dev2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 17:55:57.595858 tifftools-1.4.2.dev2/tests/data/
--rw-r--r--   0 root         (0) root         (0)      630 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_datatype.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_double_reference.tif
--rw-r--r--   0 root         (0) root         (0)      653 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_header1.tif
--rw-r--r--   0 root         (0) root         (0)      815 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_header2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_ifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      360 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      616 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_jpeg2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_strip_offset.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_subifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      653 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_tag_offset.tif
--rw-r--r--   0 root         (0) root         (0)      641 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/bad_unicode.tif
--rw-r--r--   0 root         (0) root         (0)      616 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/good_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/data/good_single.tif
--rw-r--r--   0 root         (0) root         (0)     2114 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_constants.py
--rw-r--r--   0 root         (0) root         (0)     4616 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_dump.py
--rw-r--r--   0 root         (0) root         (0)     2608 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)      848 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_options.py
--rw-r--r--   0 root         (0) root         (0)     1603 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_path_or_fobj.py
--rw-r--r--   0 root         (0) root         (0)     1943 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_read_tiff.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_readme.py
--rw-r--r--   0 root         (0) root         (0)     5557 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_set.py
--rw-r--r--   0 root         (0) root         (0)     3992 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)     8478 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tests/test_write_tiff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 17:55:57.595858 tifftools-1.4.2.dev2/tifftools/
--rw-r--r--   0 root         (0) root         (0)     1049 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/__main__.py
--rw-r--r--   0 root         (0) root         (0)    31100 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/commands.py
--rw-r--r--   0 root         (0) root         (0)    67650 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/constants.py
--rw-r--r--   0 root         (0) root         (0)      265 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/path_or_fobj.py
--rwxr-xr-x   0 root         (0) root         (0)    28750 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tifftools/tifftools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 17:55:57.595858 tifftools-1.4.2.dev2/tifftools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8830 2024-02-29 17:55:57.000000 tifftools-1.4.2.dev2/tifftools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1131 2024-02-29 17:55:57.000000 tifftools-1.4.2.dev2/tifftools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 17:55:57.000000 tifftools-1.4.2.dev2/tifftools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-29 17:55:57.000000 tifftools-1.4.2.dev2/tifftools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 17:55:50.000000 tifftools-1.4.2.dev2/tifftools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-29 17:55:57.000000 tifftools-1.4.2.dev2/tifftools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1599 2024-02-29 17:55:34.000000 tifftools-1.4.2.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:10:38.153577 tifftools-1.4.2.dev4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:10:38.141577 tifftools-1.4.2.dev4/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     4029 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      596 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3654 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)      549 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8830 2024-04-23 12:10:38.149577 tifftools-1.4.2.dev4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7969 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/README.rst
+-rw-r--r--   0 root         (0) root         (0)      424 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 12:10:38.153577 tifftools-1.4.2.dev4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:10:38.145577 tifftools-1.4.2.dev4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:10:38.145577 tifftools-1.4.2.dev4/tests/data/
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_datatype.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_double_reference.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_header1.tif
+-rw-r--r--   0 root         (0) root         (0)      815 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_header2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_ifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      360 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_jpeg2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_strip_offset.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_subifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_tag_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/bad_unicode.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/good_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/data/good_single.tif
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_constants.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_dump.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_options.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_path_or_fobj.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_read_tiff.py
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_set.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)     9822 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tests/test_write_tiff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:10:38.149577 tifftools-1.4.2.dev4/tifftools/
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    31419 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/commands.py
+-rw-r--r--   0 root         (0) root         (0)    67608 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/constants.py
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/path_or_fobj.py
+-rwxr-xr-x   0 root         (0) root         (0)    33259 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tifftools/tifftools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:10:38.149577 tifftools-1.4.2.dev4/tifftools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8830 2024-04-23 12:10:38.000000 tifftools-1.4.2.dev4/tifftools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-23 12:10:38.000000 tifftools-1.4.2.dev4/tifftools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:10:38.000000 tifftools-1.4.2.dev4/tifftools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-23 12:10:38.000000 tifftools-1.4.2.dev4/tifftools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:10:30.000000 tifftools-1.4.2.dev4/tifftools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-23 12:10:38.000000 tifftools-1.4.2.dev4/tifftools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-04-23 12:10:13.000000 tifftools-1.4.2.dev4/tox.ini
```

### Comparing `tifftools-1.4.2.dev2/.circleci/config.yml` & `tifftools-1.4.2.dev4/.circleci/config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
       - coverage
   lint_and_docs:
     docker:
       - image: python:3.8
     steps:
       - checkout
       - tox:
-          env: flake8
+          env: lint
   release:
     docker:
       - image: python:3.8
     steps:
       - checkout
       - run:
           name: Install tox
```

### Comparing `tifftools-1.4.2.dev2/.gitignore` & `tifftools-1.4.2.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/.pre-commit-config.yaml` & `tifftools-1.4.2.dev4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/CHANGELOG.md` & `tifftools-1.4.2.dev4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## Version 1.5.0
+
+### Features
+- Add a deduplicate option to avoid writing all identical data blocks ([#92](../../pull/92))
+- Refactor how ifds-first option emits data so it is closer to the COGs standard ([#92](../../pull/92))
+
 ## Version 1.4.1
 
 ### Improvements
 - Harden writing raw data to ascii format tags ([#90](../../pull/90))
 
 ## Version 1.4.0
```

### Comparing `tifftools-1.4.2.dev2/LICENSE` & `tifftools-1.4.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/PKG-INFO` & `tifftools-1.4.2.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.4.2.dev2
+Version: 1.4.2.dev4
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.4.2.dev2/README.rst` & `tifftools-1.4.2.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/setup.py` & `tifftools-1.4.2.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_datatype.tif` & `tifftools-1.4.2.dev4/tests/data/bad_datatype.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_double_reference.tif` & `tifftools-1.4.2.dev4/tests/data/bad_double_reference.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_header1.tif` & `tifftools-1.4.2.dev4/tests/data/bad_header1.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_header2.tif` & `tifftools-1.4.2.dev4/tests/data/bad_header2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_jpeg2.tif` & `tifftools-1.4.2.dev4/tests/data/bad_jpeg2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_subifd_offset.tif` & `tifftools-1.4.2.dev4/tests/data/bad_subifd_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_tag_offset.tif` & `tifftools-1.4.2.dev4/tests/data/bad_tag_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/bad_unicode.tif` & `tifftools-1.4.2.dev4/tests/data/bad_unicode.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/data/good_jpeg.tif` & `tifftools-1.4.2.dev4/tests/data/good_jpeg.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/datastore.py` & `tifftools-1.4.2.dev4/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_constants.py` & `tifftools-1.4.2.dev4/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_dump.py` & `tifftools-1.4.2.dev4/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_main.py` & `tifftools-1.4.2.dev4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_options.py` & `tifftools-1.4.2.dev4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_path_or_fobj.py` & `tifftools-1.4.2.dev4/tests/test_path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_read_tiff.py` & `tifftools-1.4.2.dev4/tests/test_read_tiff.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_readme.py` & `tifftools-1.4.2.dev4/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_set.py` & `tifftools-1.4.2.dev4/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_split.py` & `tifftools-1.4.2.dev4/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tests/test_write_tiff.py` & `tifftools-1.4.2.dev4/tests/test_write_tiff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import hashlib
 import logging
 import os
 
 import pytest
 
 import tifftools
 
@@ -148,14 +149,38 @@
     }
     destpath = tmp_path / 'sample.tiff'
     tifftools.write_tiff(info, destpath)
     destinfo = tifftools.read_tiff(destpath)
     assert destinfo['bigtiff'] is False
 
 
+def test_write_with_dedup(tmp_path):
+    path = os.path.join(os.path.dirname(__file__), 'data', 'good_single.tif')
+    info = tifftools.read_tiff(path)
+    uniqueString = b'UNIQUESTRING'
+    info['ifds'][0]['tags'][23456] = {
+        'datatype': tifftools.Datatype.UNDEFINED,
+        'data': uniqueString
+    }
+    info['ifds'][0]['tags'][23457] = {
+        'datatype': tifftools.Datatype.UNDEFINED,
+        'data': uniqueString
+    }
+    destpath = tmp_path / 'sample.tiff'
+    tifftools.write_tiff(info, destpath)
+    assert len(open(destpath, 'rb').read().split(uniqueString)) == 3
+    dest2path = tmp_path / 'sample2.tiff'
+    tifftools.write_tiff(info, dest2path, dedup=True)
+    assert len(open(dest2path, 'rb').read().split(uniqueString)) == 2
+    info2 = tifftools.read_tiff(dest2path)
+    dest3path = tmp_path / 'sample3.tiff'
+    tifftools.write_tiff(info2, dest3path)
+    assert open(destpath, 'rb').read() == open(dest3path, 'rb').read()
+
+
 def test_write_bytecount_data(tmp_path):
     path = os.path.join(os.path.dirname(__file__), 'data', 'good_single.tif')
     info = tifftools.read_tiff(path)
     # Just use data from within the file itself; an actual sample file with
     # compression 6 and defined Q, AC, and DC tables would be better.
     info['ifds'][0]['tags'][tifftools.Tag.JPEGQTables.value] = {
         'datatype': tifftools.Datatype.LONG,
@@ -223,9 +248,18 @@
 
 def test_write_ifds_first(tmp_path):
     path = datastore.fetch('d043-200.tif')
     info = tifftools.read_tiff(path)
     destpath = tmp_path / 'sample.tiff'
     tifftools.write_tiff(info, destpath, ifdsFirst=True)
     len = os.path.getsize(destpath)
-    tifftools.write_tiff(info, destpath, allowExisting=True)
-    assert len == os.path.getsize(destpath)
+    destpath2 = tmp_path / 'sample2.tiff'
+    tifftools.write_tiff(info, destpath2)
+    assert len == os.path.getsize(destpath2)
+
+    if hasattr(hashlib, 'file_digest'):
+        info = tifftools.read_tiff(destpath)
+        destpath3 = tmp_path / 'sample3.tiff'
+        tifftools.write_tiff(info, destpath3)
+        assert (
+            hashlib.file_digest(open(destpath2, 'rb'), 'sha512').hexdigest() ==
+            hashlib.file_digest(open(destpath3, 'rb'), 'sha512').hexdigest())
```

### Comparing `tifftools-1.4.2.dev2/tifftools/__init__.py` & `tifftools-1.4.2.dev4/tifftools/__init__.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tifftools/commands.py` & `tifftools-1.4.2.dev4/tifftools/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
     :overwrite: if False, throw an error if the output already exists.
     """
     ifds = []
     for path in source:
         nextInfo = read_tiff(path)
         ifds.extend(nextInfo['ifds'])
     _apply_flags_to_ifd(ifds, **kwargs)
-    write_tiff(ifds, output, allowExisting=overwrite, ifdsFirst=kwargs.get('ifdsfirst', False))
+    write_tiff(ifds, output, allowExisting=overwrite,
+               ifdsFirst=kwargs.get('ifdsfirst', False),
+               dedup=kwargs.get('dedup', False))
 
 
 def _tiff_dump_tag(tag, taginfo, linePrefix, max, dest=None, max_text=None, ifd=None):
     """
     Print a tag to a string.
 
     :param tag: the TiffTag class of the tag that should be printed.
@@ -356,15 +358,16 @@
         outputPath = _make_split_name(prefix, idx, neededChars)
         if subifds and int(Tag.SubIFD) in ifd['tags']:
             ifd = copy.deepcopy(ifd)
             del ifd['tags'][int(Tag.SubIFD)]
         logger.info('Writing %s', outputPath)
         _apply_flags_to_ifd(ifd, **kwargs)
         write_tiff(ifd, outputPath, allowExisting=overwrite,
-                   ifdsFirst=kwargs.get('ifdsfirst', False))
+                   ifdsFirst=kwargs.get('ifdsfirst', False),
+                   dedup=kwargs.get('dedup', False))
 
 
 def _value_to_types_numeric(results):
     """
     Parse a string value into a numeric array of possible different datatypes.
 
     :param results: results dictionary with an entry for Datatype.ASCII.
@@ -523,15 +526,17 @@
             setinfo = read_tiff(tiffpath)
             tag, datatype, ifd, data = _tagspec_to_ifd(tagspec, info)
             if int(tag) not in setinfo['ifds'][0]['tags']:
                 logger.warning('Tag %s is not in %s', tagspec, tiffpath)
             else:
                 ifd['tags'][int(tag)] = setinfo['ifds'][0]['tags'][int(tag)]
     _apply_flags_to_ifd(info, **kwargs)
-    write_tiff(info, output, allowExisting=overwrite, ifdsFirst=kwargs.get('ifdsfirst', False))
+    write_tiff(info, output, allowExisting=overwrite,
+               ifdsFirst=kwargs.get('ifdsfirst', False),
+               dedup=kwargs.get('dedup', False))
 
 
 def tiff_set(source, output=None, overwrite=False, setlist=None, unset=None,
              setfrom=None, **kwargs):
     """
     Set or unset tags in a tiff file.
 
@@ -596,14 +601,17 @@
     }, {
         'args': ('--littleendian', '-L', '--little-endian', '--le'),
         'kwargs': dict(dest='bigendian', action='store_false', help='Output as little-endian.'),
     }, {
         'args': ('--ifdsfirst', '--ifds-first'),
         'kwargs': dict(action='store_true', help='Store IFDs before their related data.'),
     }, {
+        'args': ('--dedup', '--deduplicate'),
+        'kwargs': dict(action='store_true', help='Do not repeat identical data.'),
+    }, {
         'args': ('--stop-on-warning', '-X'),
         'kwargs': dict(
             dest='warningIsError', action='store_true', help='Treat warnings as errors.'),
     }]
     mainParser = argparse.ArgumentParser(description=description, epilog=epilog)
     secondaryParser = argparse.ArgumentParser(description=description, add_help=False)
     subparsers = mainParser.add_subparsers(
```

### Comparing `tifftools-1.4.2.dev2/tifftools/constants.py` & `tifftools-1.4.2.dev4/tifftools/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
     def __str__(self):
         if str(self.name) != str(self.value):
             return '%s %d (0x%X)' % (self.name, self.value, self.value)
         return '%d (0x%X)' % (self.value, self.value)
 
     def __getitem__(self, key):
-        if hasattr(self, str(key)):
+        try:
             return getattr(self, str(key))
-        raise KeyError(key)
+        except AttributeError:
+            raise KeyError(key)
 
     def __int__(self):
         return self.value
 
     def __eq__(self, other):
         if isinstance(other, TiffConstant):
             return self.value == other.value and self.name == other.name
@@ -57,17 +58,15 @@
     def __contains__(self, other):
         return hasattr(self, str(other))
 
     def __hash__(self):
         return hash((type(self).__name__, self.value))
 
     def get(self, key, default=None):
-        if hasattr(self, str(key)):
-            return getattr(self, str(key))
-        return default
+        return getattr(self, str(key), default)
 
 
 class TiffTag(TiffConstant):
     def isOffsetData(self):
         return 'bytecounts' in self
 
     def isIFD(self):
```

### Comparing `tifftools-1.4.2.dev2/tifftools/path_or_fobj.py` & `tifftools-1.4.2.dev4/tifftools/path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tifftools/tifftools.py` & `tifftools-1.4.2.dev4/tifftools/tifftools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 #!/usr/bin/env python3
 
 import functools
+import hashlib
 import logging
 import os
+import shutil
 import struct
+import tempfile
 
 from .constants import Datatype, Tag, get_or_create_tag
 from .exceptions import MustBeBigTiffError, TifftoolsError
 from .path_or_fobj import OpenPathOrFobj, is_filelike_object
 
 logger = logging.getLogger(__name__)
 
+_DEDUP_HASH_METHOD = 'sha256'
+
 
 def check_offset(filelen, offset, length):
     """
     Check if a specific number of bytes can be read from a file at a given
     offset.
 
     :param filelen: the length of the file.
@@ -150,14 +155,15 @@
     :param tiff: the open tiff file object.
     :param info: the total result structure.  Used to track offset locations
         and contains big endian and bigtiff flags.
     :param ifdOffset: byte location in file of this ifd.
     :param ifdList: a list that this ifd will be appended to.
     :param tagSet: the TiffConstantSet class to use for tags.
     """
+    logger.debug(f'read_ifd: {ifdOffset} (0x{ifdOffset:X})')
     bom = info['endianPack']
     if not check_offset(info['size'], ifdOffset, 16 if info['bigtiff'] else 6):
         return
     tiff.seek(ifdOffset)
     # Store the main path here.  This facilitates merging files.
     ifd = {
         'offset': ifdOffset,
@@ -265,15 +271,16 @@
                     nextifd = read_ifd(
                         tiff, info, nextifd, subifdRecord, getattr(tag, 'tagset', None))
                     if subidx + 1 < len(subifdOffsets) and nextifd == subifdOffsets[subidx + 1]:
                         logger.warning('SubIFDs are double referenced')
                         break
 
 
-def write_tiff(ifds, path, bigEndian=None, bigtiff=None, allowExisting=False, ifdsFirst=False):
+def write_tiff(ifds, path, bigEndian=None, bigtiff=None, allowExisting=False,
+               ifdsFirst=False, dedup=False):
     """
     Write a tiff file based on data in a list of ifds.
 
     The ifds or info record that is passed only needs a subset of the fields
     that are populated by read_tiff.  Specifically, if either bigEndian or
     bigtiff are None, their value istaken from either the main info dictionary,
     if passed, or the first IFD if not.  Otherwise, only the 'ifds' key is used
@@ -288,48 +295,83 @@
         use the endian set in the first ifd.
     :param bigtiff: True for bigtiff, False for small tiff, None for use the
         bigtiff value in the first ifd.  If the small tiff is started and the
         file exceeds 4Gb, it is rewritten as bigtiff.  Note that this doesn't
         just convert to bigtiff, but actually rewrites the file to avoid
         unaccounted bytes in the file.
     :param allowExisting: if False, raise an error if the path already exists.
-    :param ifdsFirst: if True, write IFDs before their respective data.
-        Otherwise, IFDs are written after their data.  IFDs are always adjacent
-        to their data.
+    :param ifdsFirst: if True, write IFDs before their respective data.  When
+        this is not set, data is stored (mixed tag and offset data),(ifd),
+        (mixed tag and offset data),(ifd),...  When it is set, data is stored
+        (ifd),(tag data),(ifd),(tag data),...,(offset data),(offset data),...
+        This is not quite the COG specification, as that requires only the
+        strip or tile offset data to be at the end, and that data to be ordered
+        with the smallest image first, but if there are multiple conceptual
+        images, each one in turn (e.g., level0,level1,level2,...,level0,level1,
+        level2,...,...).
+    :param dedup: if False, all data is written.  If True, data blocks that are
+        identical are only written once.
     """
     if isinstance(ifds, dict):
         bigEndian = ifds.get('bigEndian') if bigEndian is None else bigEndian
         bigtiff = ifds.get('bigtiff') if bigtiff is None else bigtiff
         ifds = ifds.get('ifds', [ifds])
     bigEndian = ifds[0].get('bigEndian', False) if bigEndian is None else bigEndian
     bigtiff = ifds[0].get('bigtiff', False) if bigtiff is None else bigtiff
-    if not allowExisting and not is_filelike_object(path) and os.path.exists(path):
-        raise TifftoolsError('File already exists')
+    finalpath = path
+    if not is_filelike_object(path) and os.path.exists(path):
+        if not allowExisting:
+            raise TifftoolsError('File already exists')
+        with tempfile.NamedTemporaryFile(
+                prefix=os.path.basename(path), dir=os.path.dirname(path)) as temppath:
+            path = temppath.name
     rewriteBigtiff = False
-    with OpenPathOrFobj(path, 'wb') as dest:
-        bom = '>' if bigEndian else '<'
-        header = b'II' if not bigEndian else b'MM'
-        if bigtiff:
-            header += struct.pack(bom + 'HHHQ', 0x2B, 8, 0, 0)
-            ifdPtr = len(header) - 8
-        else:
-            header += struct.pack(bom + 'HL', 0x2A, 0)
-            ifdPtr = len(header) - 4
-        dest.write(header)
-        for ifd in ifds:
-            try:
-                ifdPtr = write_ifd(dest, bom, bigtiff, ifd, ifdPtr, ifdsFirst=ifdsFirst)
-            except MustBeBigTiffError:
-                # This can only be raised if bigtiff is false
-                rewriteBigtiff = True
-                break
-        if rewriteBigtiff:
-            dest.seek(0)
-            dest.truncate(0)
-            write_tiff(ifds, dest, bigEndian, True)
+    try:
+        with OpenPathOrFobj(path, 'wb') as dest:
+            bom = '>' if bigEndian else '<'
+            header = b'II' if not bigEndian else b'MM'
+            if bigtiff:
+                header += struct.pack(bom + 'HHHQ', 0x2B, 8, 0, 0)
+                ifdPtr = len(header) - 8
+            else:
+                header += struct.pack(bom + 'HL', 0x2A, 0)
+                ifdPtr = len(header) - 4
+            dest.write(header)
+            origifdPtr = ifdPtr
+            for datadest, ifddest in _ifdsPass(ifdsFirst, dest):
+                ifdPtr = origifdPtr
+                if bool(dedup):
+                    dedup = {'hashes': {}, 'reused': 0}
+                for ifd in ifds:
+                    try:
+                        ifdPtr = write_ifd(
+                            datadest, ifddest, bom, bigtiff, ifd, ifdPtr,
+                            ifdsFirst=ifdsFirst, dedup=dedup)
+                    except MustBeBigTiffError:
+                        # This can only be raised if bigtiff is false
+                        rewriteBigtiff = True
+                        break
+            if rewriteBigtiff:
+                dest.seek(0)
+                dest.truncate(0)
+                write_tiff(ifds, dest, bigEndian, True, ifdsFirst=ifdsFirst, dedup=bool(dedup))
+            elif dedup and dedup['reused']:
+                logger.info('Deduplication reused %d block(s)', dedup['reused'])
+    except Exception:
+        if path != finalpath:
+            os.unlink(path)
+        raise
+    else:
+        if path != finalpath:
+            # By copying the tempfile to the existing destination, the target
+            # path keeps its inode
+            with open(finalpath, 'r+b') as fdest, open(path, 'rb') as fsrc:
+                fdest.truncate(0)
+                shutil.copyfileobj(fsrc, fdest)
+            os.unlink(path)
 
 
 class _WriteTracker():
     """
     Provide a class that simulates enough of a I/O class to track length and
     offset.
     """
@@ -346,43 +388,37 @@
         return self.pos
 
     def seek(self, offset, whence=os.SEEK_SET):
         self.pos = (self.len if whence == os.SEEK_END else (
             self.pos if whence == os.SEEK_CUR else 0)) + offset
 
 
-def _ifdsPass(ifdsFirst, ifdsPass, origdest, ifddest):
+def _ifdsPass(ifdsFirst, dest):
     """
     To handle writing IFDs before or after their associated data, return a
     pair of pointers to handle writing data.  For writing IFDs after the data,
     these are the same.  We write the data, collecting the location of the
     output as we go.  For writing IFDs first, we take three passes.  On the
     first pass, we don't actually write any data, we just collect lengths so
     that we can allocate the appropriate space for the IFD.  For the second
     pass, we write the actual IFD using the correct offsets but don't write the
     data.  Lasttly, we write the actual data.
 
     :param ifdsFirst: if True, ifds are written before data.
-    :param ifdsPass: ignored if idsFirst is False, otherwise a pass number in
-        the set of {0, 1, 2}.
-    :param origdest: the original destination I/O pointer.
-    :param ifddest: the most recent ifd I/O pointer.
+    :param dest: the original destination I/O pointer.
+    :yields: the data destination I/O pointer and the ifd destination I/O
+        pointer.
     """
     if not ifdsFirst:
-        return origdest, origdest
-    if ifdsPass == 0:
-        dest = _WriteTracker(origdest.tell())
-        ifddest = _WriteTracker(0)
-    elif ifdsPass == 1:
-        dest = _WriteTracker(origdest.tell() + ifddest.tell())
-        ifddest = origdest
+        yield dest, dest
     else:
-        dest = origdest
         ifddest = _WriteTracker(0)
-    return dest, ifddest
+        yield _WriteTracker(dest.tell()), ifddest
+        yield _WriteTracker(dest.tell() + ifddest.tell()), dest
+        yield dest, _WriteTracker(0)
 
 
 def _adjustTaginfoForNonBigtiff(bigtiff, taginfo):
     """
     If this isn't a bigtiff, check if a datatype is one that isn't supported
     by non-bigtiff and convert it to the smaller size if possible.
 
@@ -403,15 +439,15 @@
 
 def _checkDataForNonBigtiff(bigtiff, data):
     """
     If this is not a bigtiff, check that all values in the data array can fit
     in a uint32 value.
 
     :param bigtiff: True if this is a bigtiff.
-    :param data: an array of integersto check.
+    :param data: an array of integers to check.
     """
     if not bigtiff and any(val for val in data if val >= 0x100000000):
         raise MustBeBigTiffError('The file is large enough it must be in bigtiff format.')
 
 
 def _writeDeferredData(bigtiff, bom, dest, ifd, ifdrecord, deferredData):
     """
@@ -453,133 +489,160 @@
             opos = dest.tell()
             dest.seek(ddata['offset'])
             dest.write(data)
             dest.seek(opos)
     return ifdrecord
 
 
-def write_ifd(dest, bom, bigtiff, ifd, ifdPtr, tagSet=Tag, ifdsFirst=False):
+def write_ifd(datadest, ifddest, bom, bigtiff, ifd, ifdPtr, tagSet=Tag,
+              ifdsFirst=False, dedup=False):
     """
     Write an IFD to a TIFF file.  This copies image data from other tiff files.
 
-    :param dest: the open file handle to write.
+    :param datadest: the open file handle to write offset data.
+    :param ifddest: the open file handle to write ids and tag data.
     :param bom: either '<' or '>' for using struct to encode values based on
         endian.
     :param bigtiff: True if this is a bigtiff.
     :param ifd: The ifd record.  This requires the tags dictionary and the
         path value.
     :param ifdPtr: a location to write the value of this ifd's start.
     :param tagSet: the TiffConstantSet class to use for tags.
     :param ifdsFirst: if True, write IFDs before their respective data.
         Otherwise, IFDs are written after their data.  IFDs are always adjacent
         to their data.
+    :param dedup: if False, all data is written.  Otherwise, a dictionary with
+        'hashes' and 'reused', where 'hashes' is a dictionary with keys of
+        hashed data that have been written and values of the offsets where it
+        was written, and 'reused' is a count of data blocks that were
+        deduplicated.
     :return: the ifdPtr for the next ifd that could be written.
     """
     ptrpack = 'Q' if bigtiff else 'L'
     tagdatalen = 8 if bigtiff else 4
-    dest.seek(0, os.SEEK_END)
-    origPos = dest.tell()
-    origdest = ifddest = dest
-    for ifdsPass in range(3 if ifdsFirst else 1):
-        dest, ifddest = _ifdsPass(ifdsFirst, ifdsPass, origdest, ifddest)
-        ifdrecord = struct.pack(bom + ('Q' if bigtiff else 'H'), len(ifd['tags']))
-        subifdPtrs = {}
-        deferredData = {}
-        with OpenPathOrFobj(ifd.get('path_or_fobj', False), 'rb') as src:
-            for tag, taginfo in sorted(ifd['tags'].items()):
-                tag = get_or_create_tag(
-                    tag, tagSet, **({'datatype': Datatype[taginfo['datatype']]}
-                                    if taginfo.get('datatype') else {}))
-                if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
-                    data = [0] * len(taginfo['ifds'])
-                    taginfo = taginfo.copy()
-                    taginfo['datatype'] = Datatype.IFD8 if bigtiff else Datatype.IFD
-                else:
-                    data = taginfo['data']
-                count = len(data)
-                if tag.isOffsetData():
-                    taginfo = taginfo.copy()
-                    taginfo['datatype'] = Datatype.LONG8 if bigtiff else Datatype.LONG
-                    if isinstance(tag.bytecounts, str):
-                        if ifdsFirst:
-                            deferredData[int(tagSet[tag.bytecounts])] = {
-                                'tag': tagSet[tag.bytecounts],
-                                'data': ifd['tags'][int(tagSet[tag.bytecounts])]['data'][:],
-                            }
-                            deferredData[int(tag)] = {
-                                'tag': tag,
-                                'data': data[:],
-                                'write': (
-                                    dest, src, data,
-                                    deferredData[int(tagSet[tag.bytecounts])]['data'],
-                                    ifd['size']),
-                                'taginfo': taginfo,
-                            }
-                        else:
-                            data = write_tag_data(
-                                dest, src, data,
-                                ifd['tags'][int(tagSet[tag.bytecounts])]['data'],
-                                ifd['size'])
+    # dest.seek(0, os.SEEK_END)
+    # origPos = dest.tell()
+    # origdest = ifddest = dest
+    nextifdPtr = None
+    ifdrecord = struct.pack(bom + ('Q' if bigtiff else 'H'), len(ifd['tags']))
+    subifdPtrs = {}
+    deferredData = {}
+    ifdpos = ifddest.tell()
+    if ifdsFirst:
+        ifdlen = (
+            len(ifdrecord) + (20 if bigtiff else 12) * len(ifd['tags']) + (8 if bigtiff else 4))
+        ifddest.write(b'\x00' * ifdlen)
+    with OpenPathOrFobj(ifd.get('path_or_fobj', False), 'rb') as src:
+        for tag, taginfo in sorted(ifd['tags'].items()):
+            tag = get_or_create_tag(
+                tag, tagSet, **({'datatype': Datatype[taginfo['datatype']]}
+                                if taginfo.get('datatype') else {}))
+            if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
+                data = [0] * len(taginfo['ifds'])
+                taginfo = taginfo.copy()
+                taginfo['datatype'] = Datatype.IFD8 if bigtiff else Datatype.IFD
+            else:
+                data = taginfo['data']
+            count = len(data)
+            if tag.isOffsetData():
+                taginfo = taginfo.copy()
+                taginfo['datatype'] = Datatype.LONG8 if bigtiff else Datatype.LONG
+                if isinstance(tag.bytecounts, str):
+                    if ifdsFirst:
+                        deferredData[int(tagSet[tag.bytecounts])] = {
+                            'tag': tagSet[tag.bytecounts],
+                            'data': ifd['tags'][int(tagSet[tag.bytecounts])]['data'][:],
+                        }
+                        deferredData[int(tag)] = {
+                            'tag': tag,
+                            'data': data[:],
+                            'write': (
+                                datadest, src, data,
+                                deferredData[int(tagSet[tag.bytecounts])]['data'],
+                                ifd['size'], dedup),
+                            'taginfo': taginfo,
+                        }
                     else:
                         data = write_tag_data(
-                            dest, src, data, [tag.bytecounts] * count, ifd['size'])
-                    _checkDataForNonBigtiff(bigtiff, data)
-                _adjustTaginfoForNonBigtiff(bigtiff, taginfo)
-                if Datatype[taginfo['datatype']].pack:
-                    pack = Datatype[taginfo['datatype']].pack
-                    count //= len(pack)
-                    data = struct.pack(bom + pack * count, *data)
-                elif Datatype[taginfo['datatype']] == Datatype.ASCII:
-                    # Handle null-seperated lists
-                    data = (data if isinstance(data, bytes) else data.encode()) + b'\x00'
-                    count = len(data)
+                            ifddest, src, data,
+                            ifd['tags'][int(tagSet[tag.bytecounts])]['data'],
+                            ifd['size'], dedup)
                 else:
-                    data = taginfo['data']
-                tagrecord = struct.pack(bom + 'HH' + ptrpack, tag, taginfo['datatype'], count)
-                if len(data) <= tagdatalen:
-                    if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
-                        subifdPtrs[tag] = -(len(ifdrecord) + len(tagrecord))
-                    if int(tag) in deferredData:
-                        deferredData[int(tag)]['ifdoffset'] = len(ifdrecord) + len(tagrecord)
-                    tagrecord += data + b'\x00' * (tagdatalen - len(data))
-                else:
-                    # word alignment
-                    if dest.tell() % 2:
-                        dest.write(b'\x00')
-                    if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
-                        subifdPtrs[tag] = dest.tell()
-                    _checkDataForNonBigtiff(bigtiff, [dest.tell()])
-                    tagrecord += struct.pack(bom + ptrpack, dest.tell())
-                    if int(tag) in deferredData:
-                        deferredData[int(tag)]['offset'] = dest.tell()
-                    dest.write(data)
-                ifdrecord += tagrecord
-            ifdrecord = _writeDeferredData(bigtiff, bom, dest, ifd, ifdrecord, deferredData)
-        _checkDataForNonBigtiff(bigtiff, [dest.tell()])
-        pos = dest.tell()
-        # ifds are expected to be on word boundaries
-        if pos % 2:
-            dest.write(b'\x00')
-            pos = dest.tell()
-        dest.seek(ifdPtr)
-        dest.write(struct.pack(bom + ptrpack, origPos if ifdsFirst else pos))
-        dest.seek(0, os.SEEK_END)
-        ifddest.write(ifdrecord)
-        nextifdPtr = dest.tell()
-        ifddest.write(struct.pack(bom + ptrpack, 0))
-    write_sub_ifds(dest, bom, bigtiff, ifd, pos, subifdPtrs, ifdsFirst=ifdsFirst)
+                    data = write_tag_data(
+                        ifddest, src, data, [tag.bytecounts] * count,
+                        ifd['size'], dedup)
+                _checkDataForNonBigtiff(bigtiff, data)
+            _adjustTaginfoForNonBigtiff(bigtiff, taginfo)
+            if Datatype[taginfo['datatype']].pack:
+                pack = Datatype[taginfo['datatype']].pack
+                count //= len(pack)
+                data = struct.pack(bom + pack * count, *data)
+            elif Datatype[taginfo['datatype']] == Datatype.ASCII:
+                # Handle null-seperated lists
+                data = (data if isinstance(data, bytes) else data.encode()) + b'\x00'
+                count = len(data)
+            else:
+                data = taginfo['data']
+            tagrecord = struct.pack(bom + 'HH' + ptrpack, tag, taginfo['datatype'], count)
+            if len(data) <= tagdatalen:
+                if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
+                    subifdPtrs[tag] = -(len(ifdrecord) + len(tagrecord))
+                if int(tag) in deferredData:
+                    deferredData[int(tag)]['ifdoffset'] = len(ifdrecord) + len(tagrecord)
+                tagrecord += data + b'\x00' * (tagdatalen - len(data))
+            else:
+                # word alignment for tag position
+                if ifddest.tell() % 2:
+                    ifddest.write(b'\x00')
+                h = None
+                tpos = ifddest.tell()
+                if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
+                    subifdPtrs[tag] = tpos
+                elif dedup:
+                    h = hashlib.new(_DEDUP_HASH_METHOD, data).digest()
+                    if h in dedup['hashes']:
+                        tpos = dedup['hashes'][h]
+                    else:
+                        dedup['hashes'][h] = tpos
+                        h = None
+                _checkDataForNonBigtiff(bigtiff, [tpos])
+                tagrecord += struct.pack(bom + ptrpack, tpos)
+                if int(tag) in deferredData:
+                    deferredData[int(tag)]['offset'] = tpos
+                if not dedup or h is None:
+                    ifddest.write(data)
+            ifdrecord += tagrecord
+        ifdrecord = _writeDeferredData(bigtiff, bom, ifddest, ifd, ifdrecord, deferredData)
+    _checkDataForNonBigtiff(bigtiff, [ifddest.tell(), datadest.tell()])
+    pos = ifddest.tell()
+    # ifds are expected to be on word boundaries
+    if pos % 2:
+        ifddest.write(b'\x00')
+        pos = ifddest.tell()
+    ifddest.seek(ifdPtr)
+    ifddest.write(struct.pack(bom + ptrpack, ifdpos if ifdsFirst else pos))
+    ifddest.seek(ifdpos if ifdsFirst else 0, os.SEEK_SET if ifdsFirst else os.SEEK_END)
+    ifddest.write(ifdrecord)
+    nextifdPtr = ifddest.tell()
+    ifddest.write(struct.pack(bom + ptrpack, 0))
+    ifddest.seek(0, os.SEEK_END)
+    write_sub_ifds(datadest, ifddest, bom, bigtiff, ifd,
+                   ifdpos if ifdsFirst else pos, subifdPtrs,
+                   ifdsFirst=ifdsFirst, dedup=dedup)
     return nextifdPtr
 
 
-def write_sub_ifds(dest, bom, bigtiff, ifd, parentPos, subifdPtrs, tagSet=Tag, ifdsFirst=False):
+def write_sub_ifds(datadest, ifddest, bom, bigtiff, ifd, parentPos, subifdPtrs,
+                   tagSet=Tag, ifdsFirst=False, dedup=False):
     """
     Write any number of SubIFDs to a TIFF file.  These can be based on tags
     other than the SubIFD tag.
 
-    :param dest: the open file handle to write.
+    :param datadest: the open file handle to write offset data.
+    :param ifddest: the open file handle to write ifd and tag data.
     :param bom: eithter '<' or '>' for using struct to encode values based on
         endian.
     :param bigtiff: True if this is a bigtiff.
     :param ifd: The ifd record.  This requires the tags dictionary and the
         path value.
     :param parentPos: the location of the parent IFD used for relative storage
         locations.
@@ -587,40 +650,51 @@
         either (a) the absolute location to store the location of the first
         subifd, or (b) a negative number whose absolute value is added to
         parentPos to get the absolute location to store the location of the
         first subifd.
     :param ifdsFirst: if True, write IFDs before their respective data.
         Otherwise, IFDs are written after their data.  IFDs are always adjacent
         to their data.
+    :param dedup: if False, all data is written.  Otherwise, a dictionary with
+        'hashes' and 'reused', where 'hashes' is a dictionary with keys of
+        hashed data that have been written and values of the offsets where it
+        was written, and 'reused' is a count of data blocks that were
+        deduplicated.
     """
     tagdatalen = 8 if bigtiff else 4
     for tag, subifdPtr in subifdPtrs.items():
         if subifdPtr < 0:
             subifdPtr = parentPos + (-subifdPtr)
         for subifd in ifd['tags'][int(tag)]['ifds']:
             if not isinstance(subifd, list):
                 subifd = [subifd]
             nextSubifdPtr = subifdPtr
             for ifdInSubifd in subifd:
                 nextSubifdPtr = write_ifd(
-                    dest, bom, bigtiff, ifdInSubifd, nextSubifdPtr,
-                    getattr(tag, 'tagset', None), ifdsFirst=ifdsFirst)
+                    datadest, ifddest, bom, bigtiff, ifdInSubifd,
+                    nextSubifdPtr, getattr(tag, 'tagset', None),
+                    ifdsFirst=ifdsFirst, dedup=dedup)
             subifdPtr += tagdatalen
 
 
-def write_tag_data(dest, src, offsets, lengths, srclen):
+def write_tag_data(dest, src, offsets, lengths, srclen, dedup=False):
     """
     Copy data from a source tiff to a destination tiff, return a list of
     offsets where data was written.
 
     :param dest: the destination file, opened to the location to write.
     :param src: the source file.
     :param offsets: an array of offsets where data will be copied from.
     :param lengths: an array of lengths to copy from each offset.
     :param srclen: the length of the source file.
+    :param dedup: if False, all data is written.  Otherwise, a dictionary with
+        'hashes' and 'reused', where 'hashes' is a dictionary with keys of
+        hashed data that have been written and values of the offsets where it
+        was written, and 'reused' is a count of data blocks that were
+        deduplicated.
     :return: the offsets in the destination file corresponding to the data
         copied.
     """
     COPY_CHUNKSIZE = 1024 ** 2
 
     if len(offsets) != len(lengths):
         raise TifftoolsError('Offsets and byte counts do not correspond.')
@@ -629,30 +703,51 @@
     offsetList = sorted([(offset, idx) for idx, offset in enumerate(offsets)])
     olidx = 0
     lastOffset = lastLength = lastOffsetIdx = None
     while olidx < len(offsetList):
         offset, idx = offsetList[olidx]
         length = lengths[idx]
         if offset and check_offset(srclen, offset, length):
+            # if a block repeats a previous block, continue the pattern
             if lastOffset == offset and lastLength == length:
                 destOffsets[idx] = destOffsets[lastOffsetIdx]
                 olidx += 1
                 continue
             lastOffset, lastLength, lastOffsetIdx = offset, length, idx
             src.seek(offset)
             destOffsets[idx] = dest.tell()
+            tells = {'idx': [idx], 'pos': destOffsets[idx], 'offset': offset}
             # Group reads when possible; the biggest overhead is in the actual
             # read call
-            while (olidx + 1 < len(offsetList) and
+            while (not dedup and olidx + 1 < len(offsetList) and
                    offsetList[olidx + 1][0] == offsetList[olidx][0] + lengths[idx] and
                    check_offset(srclen, offsetList[olidx + 1][0],
                                 lengths[offsetList[olidx + 1][1]])):
                 destOffsets[offsetList[olidx + 1][1]] = destOffsets[idx] + lengths[idx]
+                tells['idx'].append(offsetList[olidx + 1][1])
                 olidx += 1
                 offset, idx = offsetList[olidx]
                 length += lengths[idx]
+            if dedup:
+                readlen = length
+                h = hashlib.new(_DEDUP_HASH_METHOD)
+                while readlen:
+                    data = src.read(min(readlen, COPY_CHUNKSIZE))
+                    h.update(data)
+                    readlen -= len(data)
+                h = h.digest()
+                if h in dedup['hashes']:
+                    hpos = dedup['hashes'][h]
+                    for tidx in tells['idx']:
+                        destOffsets[tidx] = destOffsets[tidx] - tells['pos'] + hpos
+                    dedup['reused'] += 1
+                    logger.debug('Deduplication: %d', dedup['reused'])
+                    length = 0
+                else:
+                    dedup['hashes'][h] = tells['pos']
+                    src.seek(tells['offset'])
             while length:
                 data = src.read(min(length, COPY_CHUNKSIZE))
                 dest.write(data)
                 length -= len(data)
         olidx += 1
     return destOffsets
```

### Comparing `tifftools-1.4.2.dev2/tifftools.egg-info/PKG-INFO` & `tifftools-1.4.2.dev4/tifftools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.4.2.dev2
+Version: 1.4.2.dev4
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.4.2.dev2/tifftools.egg-info/SOURCES.txt` & `tifftools-1.4.2.dev4/tifftools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tifftools-1.4.2.dev2/tox.ini` & `tifftools-1.4.2.dev4/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tox]
 envlist =
   test-py{38,39,310,311,312}
-  flake8
+  lint
 
 [testenv]
 deps =
   argcomplete
   coverage
   pooch
   pytest
   pytest-cov
   pytest-xdist
   pyyaml
 commands =
   pytest --cov {envsitepackagesdir}/tifftools {posargs}
 
-[testenv:flake8]
+[testenv:lint]
 basepython = python3
 skipsdist = true
 skip_install = true
 deps =
   flake8
   flake8-bugbear
   flake8-docstrings
```

