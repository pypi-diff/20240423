# Comparing `tmp/ascnii-0.0.1.dev8.tar.gz` & `tmp/ascnii-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascnii-0.0.1.dev8.tar", last modified: Mon Jan 23 15:06:00 2023, max compression
+gzip compressed data, was "ascnii-0.0.1.dev9.tar", last modified: Mon Jan 23 15:10:12 2023, max compression
```

## Comparing `ascnii-0.0.1.dev8.tar` & `ascnii-0.0.1.dev9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:06:00.810356 ascnii-0.0.1.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:06:00.806356 ascnii-0.0.1.dev8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:06:00.806356 ascnii-0.0.1.dev8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-01-23 15:06:00.810356 ascnii-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:06:00.806356 ascnii-0.0.1.dev8/ascnii/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/ascnii/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/ascnii/ascnii.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:06:00.806356 ascnii-0.0.1.dev8/ascnii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-23 15:06:00.000000 ascnii-0.0.1.dev8/ascnii.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:06:00.810356 ascnii-0.0.1.dev8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   822027 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/examples/example_color.png
--rw-r--r--   0 runner    (1001) docker     (123)   783058 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/examples/example_columns.png
--rw-r--r--   0 runner    (1001) docker     (123)   260771 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/examples/example_default.png
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 15:06:00.810356 ascnii-0.0.1.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-23 15:05:49.000000 ascnii-0.0.1.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:10:12.710511 ascnii-0.0.1.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:10:12.706510 ascnii-0.0.1.dev9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:10:12.706510 ascnii-0.0.1.dev9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-01-23 15:10:12.710511 ascnii-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:10:12.706510 ascnii-0.0.1.dev9/ascnii/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/ascnii/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/ascnii/ascnii.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:10:12.710511 ascnii-0.0.1.dev9/ascnii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-23 15:10:12.000000 ascnii-0.0.1.dev9/ascnii.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 15:10:12.710511 ascnii-0.0.1.dev9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   822027 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/examples/example_color.png
+-rw-r--r--   0 runner    (1001) docker     (123)   783058 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/examples/example_columns.png
+-rw-r--r--   0 runner    (1001) docker     (123)   260771 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/examples/example_default.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 15:10:12.710511 ascnii-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-23 15:09:50.000000 ascnii-0.0.1.dev9/setup.py
```

### Comparing `ascnii-0.0.1.dev8/.github/workflows/pypi.yml` & `ascnii-0.0.1.dev9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/.gitignore` & `ascnii-0.0.1.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/LICENSE` & `ascnii-0.0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/PKG-INFO` & `ascnii-0.0.1.dev9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascnii
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: View brain images in terminal using ASCII characters
 Author: Leonard Sasse
 Author-email: l.sasse@fz-juelich.de
 Project-URL: repository, https://github.com/LeSasse/ascnii
 Keywords: neuroimaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -27,22 +27,29 @@
 you can do so now using the command line tool `ascnii`.
 
 However, for now, `ascnii` assumes that the image is in MNI space, and will
 likely not work for other kinds of inputs (at the moment).
 
 # Set up:
 
+You can simply install from PyPI:
+
+`pip install ascnii`
+
 You may or may not want to set up a virtual environment.
 
 ```sh
 python3 -m venv .examplevenv
 source .examplevenv/bin/activate
 pip install -U pip
 ```
-Then clone the repository to where you would like to install it.
+
+Alternatively, you can install from github.
+Clone the repository to where you would like to install it.
+
 ```
 git clone https://github.com/LeSasse/ascnii.git
 cd ascnii
 pip install -e .
 ```
 
 # How to use:
```

### Comparing `ascnii-0.0.1.dev8/README.md` & `ascnii-0.0.1.dev9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 you can do so now using the command line tool `ascnii`.
 
 However, for now, `ascnii` assumes that the image is in MNI space, and will
 likely not work for other kinds of inputs (at the moment).
 
 # Set up:
 
+You can simply install from PyPI:
+
+`pip install ascnii`
+
 You may or may not want to set up a virtual environment.
 
 ```sh
 python3 -m venv .examplevenv
 source .examplevenv/bin/activate
 pip install -U pip
 ```
-Then clone the repository to where you would like to install it.
+
+Alternatively, you can install from github.
+Clone the repository to where you would like to install it.
+
 ```
 git clone https://github.com/LeSasse/ascnii.git
 cd ascnii
 pip install -e .
 ```
 
 # How to use:
```

### Comparing `ascnii-0.0.1.dev8/ascnii/args.py` & `ascnii-0.0.1.dev9/ascnii/args.py`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/ascnii/ascnii.py` & `ascnii-0.0.1.dev9/ascnii/ascnii.py`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/ascnii.egg-info/PKG-INFO` & `ascnii-0.0.1.dev9/ascnii.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascnii
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: View brain images in terminal using ASCII characters
 Author: Leonard Sasse
 Author-email: l.sasse@fz-juelich.de
 Project-URL: repository, https://github.com/LeSasse/ascnii
 Keywords: neuroimaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -27,22 +27,29 @@
 you can do so now using the command line tool `ascnii`.
 
 However, for now, `ascnii` assumes that the image is in MNI space, and will
 likely not work for other kinds of inputs (at the moment).
 
 # Set up:
 
+You can simply install from PyPI:
+
+`pip install ascnii`
+
 You may or may not want to set up a virtual environment.
 
 ```sh
 python3 -m venv .examplevenv
 source .examplevenv/bin/activate
 pip install -U pip
 ```
-Then clone the repository to where you would like to install it.
+
+Alternatively, you can install from github.
+Clone the repository to where you would like to install it.
+
 ```
 git clone https://github.com/LeSasse/ascnii.git
 cd ascnii
 pip install -e .
 ```
 
 # How to use:
```

### Comparing `ascnii-0.0.1.dev8/examples/example_color.png` & `ascnii-0.0.1.dev9/examples/example_color.png`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/examples/example_columns.png` & `ascnii-0.0.1.dev9/examples/example_columns.png`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/examples/example_default.png` & `ascnii-0.0.1.dev9/examples/example_default.png`

 * *Files identical despite different names*

### Comparing `ascnii-0.0.1.dev8/pyproject.toml` & `ascnii-0.0.1.dev9/pyproject.toml`

 * *Files identical despite different names*

