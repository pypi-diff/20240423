# Comparing `tmp/mutwo.common-0.9.0.tar.gz` & `tmp/mutwo.common-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.common-0.9.0.tar", last modified: Sun Aug 14 08:01:37 2022, max compression
+gzip compressed data, was "mutwo.common-0.9.1.tar", last modified: Sun Aug 14 12:40:46 2022, max compression
```

## Comparing `mutwo.common-0.9.0.tar` & `mutwo.common-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1238 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:37.530614 mutwo.common-0.9.0/mutwo/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/mutwo/common_generators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      446 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2611 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/brown.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2736 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/brun.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7093 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/chomksy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1652 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2921 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/edwards.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1882 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/gray.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4245 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/koenig.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7961 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/lehmer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/schillinger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4270 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_generators/toussaint.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/mutwo/common_utilities/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       95 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_utilities/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2208 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_utilities/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/mutwo/common_version/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       96 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/mutwo/common_version/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/mutwo.common.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1238 2022-08-14 08:01:37.000000 mutwo.common-0.9.0/mutwo.common.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2022-08-14 08:01:37.000000 mutwo.common-0.9.0/mutwo.common.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-14 08:01:37.000000 mutwo.common-0.9.0/mutwo.common.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2022-08-14 08:01:37.000000 mutwo.common-0.9.0/mutwo.common.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-08-14 08:01:37.000000 mutwo.common-0.9.0/mutwo.common.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      104 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-08-14 08:01:37.534614 mutwo.common-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2022-08-14 08:01:27.000000 mutwo.common-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:46.170156 mutwo.common-0.9.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1238 2022-08-14 12:40:46.170156 mutwo.common-0.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:46.166156 mutwo.common-0.9.1/mutwo/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:46.166156 mutwo.common-0.9.1/mutwo/common_generators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      446 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2611 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/brown.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2736 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/brun.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7093 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/chomksy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1652 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2921 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/edwards.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1882 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/gray.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4245 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/koenig.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7961 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/lehmer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/schillinger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4270 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_generators/toussaint.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:46.166156 mutwo.common-0.9.1/mutwo/common_utilities/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       95 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_utilities/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2208 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_utilities/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:46.166156 mutwo.common-0.9.1/mutwo/common_version/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      144 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/mutwo/common_version/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-14 12:40:46.166156 mutwo.common-0.9.1/mutwo.common.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1238 2022-08-14 12:40:46.000000 mutwo.common-0.9.1/mutwo.common.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2022-08-14 12:40:46.000000 mutwo.common-0.9.1/mutwo.common.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-14 12:40:46.000000 mutwo.common-0.9.1/mutwo.common.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2022-08-14 12:40:46.000000 mutwo.common-0.9.1/mutwo.common.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-08-14 12:40:46.000000 mutwo.common-0.9.1/mutwo.common.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      104 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-08-14 12:40:46.170156 mutwo.common-0.9.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1369 2022-08-14 12:40:36.000000 mutwo.common-0.9.1/setup.py
```

### Comparing `mutwo.common-0.9.0/LICENSE` & `mutwo.common-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/PKG-INFO` & `mutwo.common-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.common
-Version: 0.9.0
+Version: 0.9.1
 Summary: Common extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.common
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
 Requires-Python: >=3.9, <4
```

### Comparing `mutwo.common-0.9.0/README.md` & `mutwo.common-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/brown.py` & `mutwo.common-0.9.1/mutwo/common_generators/brown.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/brun.py` & `mutwo.common-0.9.1/mutwo/common_generators/brun.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/chomksy.py` & `mutwo.common-0.9.1/mutwo/common_generators/chomksy.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/constants.py` & `mutwo.common-0.9.1/mutwo/common_generators/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/edwards.py` & `mutwo.common-0.9.1/mutwo/common_generators/edwards.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/gray.py` & `mutwo.common-0.9.1/mutwo/common_generators/gray.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/koenig.py` & `mutwo.common-0.9.1/mutwo/common_generators/koenig.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/lehmer.py` & `mutwo.common-0.9.1/mutwo/common_generators/lehmer.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_generators/toussaint.py` & `mutwo.common-0.9.1/mutwo/common_generators/toussaint.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo/common_utilities/exceptions.py` & `mutwo.common-0.9.1/mutwo/common_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/mutwo.common.egg-info/PKG-INFO` & `mutwo.common-0.9.1/mutwo.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.common
-Version: 0.9.0
+Version: 0.9.1
 Summary: Common extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.common
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
 Requires-Python: >=3.9, <4
```

### Comparing `mutwo.common-0.9.0/mutwo.common.egg-info/SOURCES.txt` & `mutwo.common-0.9.1/mutwo.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutwo.common-0.9.0/setup.py` & `mutwo.common-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools  # type: ignore
 
 version = {}
 with open("mutwo/common_version/__init__.py") as fp:
     exec(fp.read(), version)
 
-VERSION = version["__version__"]
+VERSION = version["VERSION"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 extras_require = {"testing": ["nose", "coveralls"]}
 
 setuptools.setup(
```

