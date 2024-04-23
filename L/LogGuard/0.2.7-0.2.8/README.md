# Comparing `tmp/logguard-0.2.7.tar.gz` & `tmp/logguard-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logguard-0.2.7.tar", last modified: Tue Apr 23 12:02:43 2024, max compression
+gzip compressed data, was "logguard-0.2.8.tar", last modified: Tue Apr 23 12:17:50 2024, max compression
```

## Comparing `logguard-0.2.7.tar` & `logguard-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 12:02:43.026584 logguard-0.2.7/
-drwxrwxrwx   0        0        0        0 2024-04-23 12:02:43.013581 logguard-0.2.7/LogGuard.egg-info/
--rw-rw-rw-   0        0        0      684 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:02:42.000000 logguard-0.2.7/LogGuard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      684 2024-04-23 12:02:43.020583 logguard-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      901 2024-04-22 14:13:53.000000 logguard-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 12:02:43.027584 logguard-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      821 2024-04-23 12:00:43.000000 logguard-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:17:50.205459 logguard-0.2.8/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:17:50.188909 logguard-0.2.8/LogGuard.egg-info/
+-rw-rw-rw-   0        0        0      751 2024-04-23 12:17:50.000000 logguard-0.2.8/LogGuard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-23 12:17:50.000000 logguard-0.2.8/LogGuard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:17:50.000000 logguard-0.2.8/LogGuard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2024-04-23 12:17:50.000000 logguard-0.2.8/LogGuard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:17:50.000000 logguard-0.2.8/LogGuard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      751 2024-04-23 12:17:50.198905 logguard-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2024-04-22 14:13:53.000000 logguard-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:17:50.205459 logguard-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-04-23 12:17:39.000000 logguard-0.2.8/setup.py
```

### Comparing `logguard-0.2.7/LogGuard.egg-info/PKG-INFO` & `logguard-0.2.8/LogGuard.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: LogGuard
-Version: 0.2.7
+Version: 0.2.8
 Summary: A simple Python Logger
+Home-page: https://github.com/chariskar/LogGuard/tree/LogGuard-PY
 Author: Charilaos Karametos
 License: MIT
 Requires-Python: >=3.6
 Requires-Dist: astroid==3.1.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: dill==0.3.8
 Requires-Dist: flake8==7.0.0
```

### Comparing `logguard-0.2.7/PKG-INFO` & `logguard-0.2.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: LogGuard
-Version: 0.2.7
+Version: 0.2.8
 Summary: A simple Python Logger
+Home-page: https://github.com/chariskar/LogGuard/tree/LogGuard-PY
 Author: Charilaos Karametos
 License: MIT
 Requires-Python: >=3.6
 Requires-Dist: astroid==3.1.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: dill==0.3.8
 Requires-Dist: flake8==7.0.0
```

### Comparing `logguard-0.2.7/README.md` & `logguard-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `logguard-0.2.7/setup.py` & `logguard-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='LogGuard',
-    version='0.2.7',
+    version='0.2.8',
     description='A simple Python Logger',
     author='Charilaos Karametos',
     packages=find_packages(),
     install_requires=[
         "astroid==3.1.0",
         "colorama==0.4.6",
         "dill==0.3.8",
@@ -24,11 +24,12 @@
         "pyflakes==3.2.0",
         "pylint==3.1.0",
         "snowballstemmer==2.2.0",
         "tomlkit==0.12.4"
         ],
     package_data={'': ['log_settings.json']},
     license="MIT",
-    python_requires=">=3.6"
-    
+    python_requires=">=3.6",
+    url='https://github.com/chariskar/LogGuard/tree/LogGuard-PY'
+
   
 )
```

