# Comparing `tmp/dspy-0.1.4.tar.gz` & `tmp/dspy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspy-0.1.4.tar", max compression
+gzip compressed data, was "dspy-0.1.5.tar", max compression
```

## Comparing `dspy-0.1.4.tar` & `dspy-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-14 21:47:44.135077 dspy-0.1.4/README.md
--rw-r--r--   0        0        0      589 2024-04-14 22:17:57.161255 dspy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 21:47:44.135077 dspy-0.1.4/src/dspy/_init_.py
--rwxr-xr-x   0        0        0       79 2024-04-14 21:56:57.760545 dspy-0.1.4/src/dspy/main.py
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 dspy-0.1.4/setup.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 dspy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-14 21:47:44.135077 dspy-0.1.5/README.md
+-rw-r--r--   0        0        0      368 2024-04-23 15:57:01.708329 dspy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 21:47:44.135077 dspy-0.1.5/src/dspy_dummy/__init__.py
+-rwxr-xr-x   0        0        0       79 2024-04-14 21:56:57.760545 dspy-0.1.5/src/dspy_dummy/main.py
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 dspy-0.1.5/setup.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 dspy-0.1.5/PKG-INFO
```

### Comparing `dspy-0.1.4/setup.py` & `dspy-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['dspy']
+['dspy_dummy']
 
 package_data = \
 {'': ['*']}
 
-entry_points = \
-{'console_scripts': ['ka = kiera.main:main', 'kiera = kiera.main:main']}
+install_requires = \
+['dspy-ai==2.4.5']
 
 setup_kwargs = {
     'name': 'dspy',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Placeholder package for DSPy',
     'long_description': '',
     'author': 'Tom Dörr',
     'author_email': 'tomdoerr96@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'entry_points': entry_points,
+    'install_requires': install_requires,
     'python_requires': '>=3.3,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

