# Comparing `tmp/ghostwindow-1.0.1.tar.gz` & `tmp/ghostwindow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghostwindow-1.0.1.tar", last modified: Tue Apr  2 02:03:07 2024, max compression
+gzip compressed data, was "ghostwindow-1.1.0.tar", last modified: Tue Apr 23 03:27:27 2024, max compression
```

## Comparing `ghostwindow-1.0.1.tar` & `ghostwindow-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 02:03:07.675202 ghostwindow-1.0.1/
--rw-rw-rw-   0        0        0     3150 2024-04-02 02:03:07.674201 ghostwindow-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2024-04-02 01:27:43.000000 ghostwindow-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 02:03:07.673201 ghostwindow-1.0.1/ghostwindow.egg-info/
--rw-rw-rw-   0        0        0     3150 2024-04-02 02:03:07.000000 ghostwindow-1.0.1/ghostwindow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-04-02 02:03:07.000000 ghostwindow-1.0.1/ghostwindow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 02:03:07.000000 ghostwindow-1.0.1/ghostwindow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 02:03:07.000000 ghostwindow-1.0.1/ghostwindow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2024-04-02 01:27:43.000000 ghostwindow-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 02:03:07.675202 ghostwindow-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      914 2024-04-02 02:01:02.000000 ghostwindow-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 03:27:27.166755 ghostwindow-1.1.0/
+-rw-rw-rw-   0        0        0     3150 2024-04-23 03:27:27.165755 ghostwindow-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2024-04-02 01:27:43.000000 ghostwindow-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 03:27:27.164755 ghostwindow-1.1.0/ghostwindow.egg-info/
+-rw-rw-rw-   0        0        0     3150 2024-04-23 03:27:27.000000 ghostwindow-1.1.0/ghostwindow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-04-23 03:27:27.000000 ghostwindow-1.1.0/ghostwindow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:27:27.000000 ghostwindow-1.1.0/ghostwindow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:27:27.000000 ghostwindow-1.1.0/ghostwindow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2024-04-02 01:27:43.000000 ghostwindow-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 03:27:27.166755 ghostwindow-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      914 2024-04-23 03:11:04.000000 ghostwindow-1.1.0/setup.py
```

### Comparing `ghostwindow-1.0.1/PKG-INFO` & `ghostwindow-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostwindow
-Version: 1.0.1
+Version: 1.1.0
 Summary: A small package with some useful window utility functions
 Home-page: https://github.com/rk767/ghost-window
 Author: rk767
 Author-email: rk8263208@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/rk767/ghost-window
 Project-URL: Source, https://github.com/rk767/ghost-window
```

### Comparing `ghostwindow-1.0.1/README.md` & `ghostwindow-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ghostwindow-1.0.1/ghostwindow.egg-info/PKG-INFO` & `ghostwindow-1.1.0/ghostwindow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostwindow
-Version: 1.0.1
+Version: 1.1.0
 Summary: A small package with some useful window utility functions
 Home-page: https://github.com/rk767/ghost-window
 Author: rk767
 Author-email: rk8263208@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/rk767/ghost-window
 Project-URL: Source, https://github.com/rk767/ghost-window
```

### Comparing `ghostwindow-1.0.1/setup.py` & `ghostwindow-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 import setuptools
 
 setuptools.setup(
     name="ghostwindow",
-    version="1.0.1",
+    version="1.1.0",
     author="rk767",
     author_email="rk8263208@gmail.com",
     description="A small package with some useful window utility functions",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/rk767/ghost-window",
     license="Apache 2.0",
```

