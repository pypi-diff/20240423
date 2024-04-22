# Comparing `tmp/pybunch-1.0.1.tar.gz` & `tmp/pybunch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.1.tar", last modified: Mon Apr 22 13:18:10 2024, max compression
+gzip compressed data, was "pybunch-1.0.2.tar", last modified: Mon Apr 22 16:04:35 2024, max compression
```

## Comparing `pybunch-1.0.1.tar` & `pybunch-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.776661 pybunch-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.772661 pybunch-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.776661 pybunch-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-22 13:18:06.000000 pybunch-1.0.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 13:18:06.000000 pybunch-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 13:18:06.000000 pybunch-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-22 13:18:10.776661 pybunch-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 13:18:06.000000 pybunch-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.776661 pybunch-1.0.1/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 13:18:06.000000 pybunch-1.0.1/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 13:18:06.000000 pybunch-1.0.1/example/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 13:18:06.000000 pybunch-1.0.1/example/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 13:18:06.000000 pybunch-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:18:10.776661 pybunch-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.772661 pybunch-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.776661 pybunch-1.0.1/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:06.000000 pybunch-1.0.1/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-22 13:18:06.000000 pybunch-1.0.1/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-22 13:18:06.000000 pybunch-1.0.1/src/pybunch/packed_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:18:10.776661 pybunch-1.0.1/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-22 13:18:10.000000 pybunch-1.0.1/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 13:18:10.000000 pybunch-1.0.1/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:18:10.000000 pybunch-1.0.1/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 13:18:10.000000 pybunch-1.0.1/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 13:18:10.000000 pybunch-1.0.1/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.127050 pybunch-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.127050 pybunch-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-22 16:04:29.000000 pybunch-1.0.2/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 16:04:29.000000 pybunch-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 16:04:29.000000 pybunch-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 16:04:35.131050 pybunch-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 16:04:29.000000 pybunch-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.127050 pybunch-1.0.2/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 16:04:29.000000 pybunch-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:04:35.131050 pybunch-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/pybunch/packed_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.1/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.2/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.1/LICENSE` & `pybunch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.1/PKG-INFO` & `pybunch-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,11 +15,11 @@
 
 # pybunch
 
 A simple python utility to pack a python project into a single file.
 
 ## Usage
 ```bash
-$ python -m pybunch --root example --entrypoint main -sp example -o packed.py
+$ python -m pybunch --root example --entrypoint main -sp example -so -o packed.py
 $ python packed.py
 21
 ```
```

### Comparing `pybunch-1.0.1/pyproject.toml` & `pybunch-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.1/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.2/src/pybunch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,11 +15,11 @@
 
 # pybunch
 
 A simple python utility to pack a python project into a single file.
 
 ## Usage
 ```bash
-$ python -m pybunch --root example --entrypoint main -sp example -o packed.py
+$ python -m pybunch --root example --entrypoint main -sp example -so -o packed.py
 $ python packed.py
 21
 ```
```

