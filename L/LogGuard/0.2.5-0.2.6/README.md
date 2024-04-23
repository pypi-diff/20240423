# Comparing `tmp/logguard-0.2.5.tar.gz` & `tmp/logguard-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logguard-0.2.5.tar", last modified: Mon Apr 22 16:32:38 2024, max compression
+gzip compressed data, was "logguard-0.2.6.tar", last modified: Mon Apr 22 16:40:52 2024, max compression
```

## Comparing `logguard-0.2.5.tar` & `logguard-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 16:32:37.990177 logguard-0.2.5/
-drwxrwxrwx   0        0        0        0 2024-04-22 16:32:37.976634 logguard-0.2.5/LogGuard.egg-info/
--rw-rw-rw-   0        0        0      646 2024-04-22 16:32:37.000000 logguard-0.2.5/LogGuard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-22 16:32:37.000000 logguard-0.2.5/LogGuard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 16:32:37.000000 logguard-0.2.5/LogGuard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2024-04-22 16:32:37.000000 logguard-0.2.5/LogGuard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 16:32:37.000000 logguard-0.2.5/LogGuard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      646 2024-04-22 16:32:37.982620 logguard-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-22 16:32:37.990177 logguard-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-04-22 16:32:02.000000 logguard-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 16:40:52.899214 logguard-0.2.6/
+drwxrwxrwx   0        0        0        0 2024-04-22 16:40:52.873154 logguard-0.2.6/LogGuard.egg-info/
+-rw-rw-rw-   0        0        0      646 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      646 2024-04-22 16:40:52.890865 logguard-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-22 16:40:52.899214 logguard-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      778 2024-04-22 16:37:57.000000 logguard-0.2.6/setup.py
```

### Comparing `logguard-0.2.5/LogGuard.egg-info/PKG-INFO` & `logguard-0.2.6/LogGuard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogGuard
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple Python Logger
 Author: Charilaos Karametos
 Requires-Dist: astroid==3.1.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: dill==0.3.8
 Requires-Dist: flake8==7.0.0
 Requires-Dist: flake8-commas==2.1.0
```

### Comparing `logguard-0.2.5/PKG-INFO` & `logguard-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogGuard
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple Python Logger
 Author: Charilaos Karametos
 Requires-Dist: astroid==3.1.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: dill==0.3.8
 Requires-Dist: flake8==7.0.0
 Requires-Dist: flake8-commas==2.1.0
```

### Comparing `logguard-0.2.5/setup.py` & `logguard-0.2.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='LogGuard',
-    version='0.2.5',
+    version='0.2.6',
     description='A simple Python Logger',
     author='Charilaos Karametos',
     packages=find_packages(),
     install_requires=[
         "astroid==3.1.0",
         "colorama==0.4.6",
         "dill==0.3.8",
```

