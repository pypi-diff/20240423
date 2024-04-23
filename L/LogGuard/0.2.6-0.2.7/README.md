# Comparing `tmp/logguard-0.2.6.tar.gz` & `tmp/logguard-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logguard-0.2.6.tar", last modified: Mon Apr 22 16:40:52 2024, max compression
+gzip compressed data, was "logguard-0.2.7.tar", last modified: Tue Apr 23 12:02:43 2024, max compression
```

## Comparing `logguard-0.2.6.tar` & `logguard-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 16:40:52.899214 logguard-0.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-22 16:40:52.873154 logguard-0.2.6/LogGuard.egg-info/
--rw-rw-rw-   0        0        0      646 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 16:40:52.000000 logguard-0.2.6/LogGuard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      646 2024-04-22 16:40:52.890865 logguard-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-22 16:40:52.899214 logguard-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-04-22 16:37:57.000000 logguard-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:02:43.026584 logguard-0.2.7/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:02:43.013581 logguard-0.2.7/LogGuard.egg-info/
+-rw-rw-rw-   0        0        0      684 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      684 2024-04-23 12:02:43.020583 logguard-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2024-04-22 14:13:53.000000 logguard-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:02:43.027584 logguard-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      821 2024-04-23 12:00:43.000000 logguard-0.2.7/setup.py
```

### Comparing `logguard-0.2.6/LogGuard.egg-info/PKG-INFO` & `logguard-0.2.7/LogGuard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: LogGuard
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple Python Logger
 Author: Charilaos Karametos
+License: MIT
+Requires-Python: >=3.6
 Requires-Dist: astroid==3.1.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: dill==0.3.8
 Requires-Dist: flake8==7.0.0
 Requires-Dist: flake8-commas==2.1.0
 Requires-Dist: flake8-docstrings==1.7.0
 Requires-Dist: isort==5.13.2
```

### Comparing `logguard-0.2.6/PKG-INFO` & `logguard-0.2.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: LogGuard
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple Python Logger
 Author: Charilaos Karametos
+License: MIT
+Requires-Python: >=3.6
 Requires-Dist: astroid==3.1.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: dill==0.3.8
 Requires-Dist: flake8==7.0.0
 Requires-Dist: flake8-commas==2.1.0
 Requires-Dist: flake8-docstrings==1.7.0
 Requires-Dist: isort==5.13.2
```

### Comparing `logguard-0.2.6/setup.py` & `logguard-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='LogGuard',
-    version='0.2.6',
+    version='0.2.7',
     description='A simple Python Logger',
     author='Charilaos Karametos',
     packages=find_packages(),
     install_requires=[
         "astroid==3.1.0",
         "colorama==0.4.6",
         "dill==0.3.8",
@@ -22,9 +22,13 @@
         "pycodestyle==2.11.1",
         "pydocstyle==6.3.0",
         "pyflakes==3.2.0",
         "pylint==3.1.0",
         "snowballstemmer==2.2.0",
         "tomlkit==0.12.4"
         ],
-    package_data={'': ['log_settings.json','__init__.py']},  
+    package_data={'': ['log_settings.json']},
+    license="MIT",
+    python_requires=">=3.6"
+    
+  
 )
```

