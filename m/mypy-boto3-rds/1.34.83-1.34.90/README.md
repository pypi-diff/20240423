# Comparing `tmp/mypy-boto3-rds-1.34.83.tar.gz` & `tmp/mypy_boto3_rds-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rds-1.34.83.tar", last modified: Thu Apr 11 19:18:08 2024, max compression
+gzip compressed data, was "mypy_boto3_rds-1.34.90.tar", last modified: Tue Apr 23 19:34:21 2024, max compression
```

## Comparing `mypy-boto3-rds-1.34.83.tar` & `mypy_boto3_rds-1.34.90.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.467357 mypy-boto3-rds-1.34.83/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-11 19:18:08.467357 mypy-boto3-rds-1.34.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.467357 mypy-boto3-rds-1.34.83/mypy_boto3_rds/
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   164341 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   164338 2024-04-11 19:17:45.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-11 19:17:51.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-11 19:17:50.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-11 19:17:47.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.467357 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-11 19:18:08.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 19:18:08.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:08.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:08.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:08.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 19:18:08.000000 mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:08.467357 mypy-boto3-rds-1.34.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-11 19:17:44.000000 mypy-boto3-rds-1.34.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/mypy_boto3_rds/
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164341 2024-04-23 19:34:01.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164338 2024-04-23 19:34:01.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-04-23 19:34:02.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-23 19:34:07.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-23 19:34:05.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/setup.py
```

### Comparing `mypy-boto3-rds-1.34.83/LICENSE` & `mypy_boto3_rds-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/PKG-INFO` & `mypy_boto3_rds-1.34.90/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.83
-Summary: Type annotations for boto3.RDS 1.34.83 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.RDS 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rds-1.34.83/README.md` & `mypy_boto3_rds-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/__init__.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/__init__.pyi` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/__main__.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDS 1.34.83\n"
-        "Version:         1.34.83\n"
+        "Type annotations for boto3.RDS 1.34.90\n"
+        "Version:         1.34.90\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.83")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/client.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/client.pyi` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/literals.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,14 +541,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/literals.pyi` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -541,14 +541,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/paginator.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/paginator.pyi` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/type_defs.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/type_defs.pyi` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/waiter.py` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds/waiter.pyi` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/PKG-INFO` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.83
-Summary: Type annotations for boto3.RDS 1.34.83 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.RDS 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rds-1.34.83/mypy_boto3_rds.egg-info/SOURCES.txt` & `mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.83/setup.py` & `mypy_boto3_rds-1.34.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds",
-    version="1.34.83",
+    version="1.34.90",
     packages=["mypy_boto3_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.RDS 1.34.83 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.RDS 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

