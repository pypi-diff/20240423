# Comparing `tmp/cnes_pylint_extension-7.0.0.tar.gz` & `tmp/cnes-pylint-extension-7.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnes_pylint_extension-7.0.0.tar", last modified: Tue Apr 23 12:15:44 2024, max compression
+gzip compressed data, was "cnes-pylint-extension-7.0.0rc1.tar", last modified: Fri Mar 22 13:52:08 2024, max compression
```

## Comparing `cnes_pylint_extension-7.0.0.tar` & `cnes-pylint-extension-7.0.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:15:44.388965 cnes_pylint_extension-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-23 12:15:40.000000 cnes_pylint_extension-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-23 12:15:44.388965 cnes_pylint_extension-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-23 12:15:40.000000 cnes_pylint_extension-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:15:44.384965 cnes_pylint_extension-7.0.0/checkers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:15:44.384965 cnes_pylint_extension-7.0.0/checkers/cnes_checker/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 12:15:40.000000 cnes_pylint_extension-7.0.0/checkers/cnes_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28807 2024-04-23 12:15:40.000000 cnes_pylint_extension-7.0.0/checkers/cnes_checker/cnes_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:15:44.388965 cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-23 12:15:44.000000 cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 12:15:44.000000 cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:15:44.000000 cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 12:15:44.000000 cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 12:15:44.000000 cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:15:44.388965 cnes_pylint_extension-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 12:15:40.000000 cnes_pylint_extension-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:15:44.388965 cnes_pylint_extension-7.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-23 12:15:40.000000 cnes_pylint_extension-7.0.0/test/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:52:08.585538 cnes-pylint-extension-7.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-22 13:52:01.000000 cnes-pylint-extension-7.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-03-22 13:52:08.585538 cnes-pylint-extension-7.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-22 13:52:01.000000 cnes-pylint-extension-7.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:52:08.581538 cnes-pylint-extension-7.0.0rc1/checkers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:52:08.585538 cnes-pylint-extension-7.0.0rc1/checkers/cnes_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 13:52:01.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28807 2024-03-22 13:52:01.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_checker/cnes_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:52:08.585538 cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-03-22 13:52:08.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-22 13:52:08.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:52:08.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-22 13:52:08.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-22 13:52:08.000000 cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 13:52:08.585538 cnes-pylint-extension-7.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-22 13:52:01.000000 cnes-pylint-extension-7.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:52:08.585538 cnes-pylint-extension-7.0.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-22 13:52:01.000000 cnes-pylint-extension-7.0.0rc1/test/test_functional.py
```

### Comparing `cnes_pylint_extension-7.0.0/LICENSE` & `cnes-pylint-extension-7.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnes_pylint_extension-7.0.0/PKG-INFO` & `cnes-pylint-extension-7.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnes-pylint-extension
-Version: 7.0.0
+Version: 7.0.0rc1
 Summary: A PyLint plugin to add CNES specific checks
 Home-page: https://github.com/cnescatlab/cnes-pylint-extension
 Author: CNES CatLab
 Project-URL: Bug Reports, https://github.com/cnescatlab/cnes-pylint-extension/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cnes_pylint_extension-7.0.0/README.md` & `cnes-pylint-extension-7.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `cnes_pylint_extension-7.0.0/checkers/cnes_checker/cnes_checker.py` & `cnes-pylint-extension-7.0.0rc1/checkers/cnes_checker/cnes_checker.py`

 * *Files identical despite different names*

### Comparing `cnes_pylint_extension-7.0.0/checkers/cnes_pylint_extension.egg-info/PKG-INFO` & `cnes-pylint-extension-7.0.0rc1/checkers/cnes_pylint_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnes-pylint-extension
-Version: 7.0.0
+Version: 7.0.0rc1
 Summary: A PyLint plugin to add CNES specific checks
 Home-page: https://github.com/cnescatlab/cnes-pylint-extension
 Author: CNES CatLab
 Project-URL: Bug Reports, https://github.com/cnescatlab/cnes-pylint-extension/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `cnes_pylint_extension-7.0.0/setup.py` & `cnes-pylint-extension-7.0.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cnes-pylint-extension",
-    version="7.0.0",
+    version="7.0.0rc1",
     author="CNES CatLab",
     description="A PyLint plugin to add CNES specific checks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cnescatlab/cnes-pylint-extension",
     packages=setuptools.find_packages(where='checkers'),
     package_dir={'': 'checkers'},
```

### Comparing `cnes_pylint_extension-7.0.0/test/test_functional.py` & `cnes-pylint-extension-7.0.0rc1/test/test_functional.py`

 * *Files identical despite different names*

