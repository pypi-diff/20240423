# Comparing `tmp/numero_a_letras-0.0.4.tar.gz` & `tmp/numero_a_letras-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numero_a_letras-0.0.4.tar", last modified: Mon Jan 15 13:23:14 2024, max compression
+gzip compressed data, was "numero_a_letras-0.0.5.tar", last modified: Tue Apr 23 20:00:59 2024, max compression
```

## Comparing `numero_a_letras-0.0.4.tar` & `numero_a_letras-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)     1432 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/PKG-INFO
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)      672 2024-01-15 12:16:04.000000 numero_a_letras-0.0.4/README.md
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       38 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/setup.cfg
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)      916 2024-01-15 13:23:03.000000 numero_a_letras-0.0.4/setup.py
-drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/src/
-drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/src/numero_a_letras/
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       65 2024-01-15 13:17:07.000000 numero_a_letras-0.0.4/src/numero_a_letras/__init__.py
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)     4589 2024-01-14 15:16:52.000000 numero_a_letras-0.0.4/src/numero_a_letras/main.py
-drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/src/numero_a_letras.egg-info/
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)     1432 2024-01-15 13:23:14.000000 numero_a_letras-0.0.4/src/numero_a_letras.egg-info/PKG-INFO
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)      321 2024-01-15 13:23:14.000000 numero_a_letras-0.0.4/src/numero_a_letras.egg-info/SOURCES.txt
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)        1 2024-01-15 13:23:14.000000 numero_a_letras-0.0.4/src/numero_a_letras.egg-info/dependency_links.txt
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       20 2024-01-15 13:23:14.000000 numero_a_letras-0.0.4/src/numero_a_letras.egg-info/requires.txt
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       16 2024-01-15 13:23:14.000000 numero_a_letras-0.0.4/src/numero_a_letras.egg-info/top_level.txt
-drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-01-15 13:23:14.330320 numero_a_letras-0.0.4/test/
--rw-rw-r--   0 lugezz    (1000) lugezz    (1000)    13702 2024-01-15 13:13:22.000000 numero_a_letras-0.0.4/test/test_numero_a_letras.py
+drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-04-23 20:00:59.758442 numero_a_letras-0.0.5/
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)     1064 2024-04-23 19:52:58.000000 numero_a_letras-0.0.5/LICENSE
+-rw-r--r--   0 lugezz    (1000) lugezz    (1000)     1227 2024-04-23 20:00:59.758442 numero_a_letras-0.0.5/PKG-INFO
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)      672 2024-04-23 19:52:58.000000 numero_a_letras-0.0.5/README.md
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       38 2024-04-23 20:00:59.758442 numero_a_letras-0.0.5/setup.cfg
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)      916 2024-04-23 19:52:58.000000 numero_a_letras-0.0.5/setup.py
+drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-04-23 20:00:59.754442 numero_a_letras-0.0.5/src/
+drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-04-23 20:00:59.754442 numero_a_letras-0.0.5/src/numero_a_letras/
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       65 2024-04-23 19:52:58.000000 numero_a_letras-0.0.5/src/numero_a_letras/__init__.py
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)     4589 2024-04-23 19:52:58.000000 numero_a_letras-0.0.5/src/numero_a_letras/main.py
+drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-04-23 20:00:59.758442 numero_a_letras-0.0.5/src/numero_a_letras.egg-info/
+-rw-r--r--   0 lugezz    (1000) lugezz    (1000)     1227 2024-04-23 20:00:59.000000 numero_a_letras-0.0.5/src/numero_a_letras.egg-info/PKG-INFO
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)      329 2024-04-23 20:00:59.000000 numero_a_letras-0.0.5/src/numero_a_letras.egg-info/SOURCES.txt
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)        1 2024-04-23 20:00:59.000000 numero_a_letras-0.0.5/src/numero_a_letras.egg-info/dependency_links.txt
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       20 2024-04-23 20:00:59.000000 numero_a_letras-0.0.5/src/numero_a_letras.egg-info/requires.txt
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)       16 2024-04-23 20:00:59.000000 numero_a_letras-0.0.5/src/numero_a_letras.egg-info/top_level.txt
+drwxrwxr-x   0 lugezz    (1000) lugezz    (1000)        0 2024-04-23 20:00:59.758442 numero_a_letras-0.0.5/test/
+-rw-rw-r--   0 lugezz    (1000) lugezz    (1000)    13702 2024-04-23 19:52:58.000000 numero_a_letras-0.0.5/test/test_numero_a_letras.py
```

### Comparing `numero_a_letras-0.0.4/README.md` & `numero_a_letras-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `numero_a_letras-0.0.4/setup.py` & `numero_a_letras-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="numero_a_letras",
-    version="0.0.4",
+    version="0.0.5",
     description="Convierte un número a letras en español",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lugezz/numero_a_letras_literal",
     author="Eugenio",
@@ -23,9 +23,9 @@
     install_requires=[
         # Optional
         # e.g "numpy==1.11.1", "tensorflow>=1.1.0"
     ],
     extras_require={
         "dev": ["twine>=4.0.2"],
     },
-    python_requires=">=3.10, <3.12",
+    python_requires=">=3.10, <3.13",
 )
```

### Comparing `numero_a_letras-0.0.4/src/numero_a_letras/main.py` & `numero_a_letras-0.0.5/src/numero_a_letras/main.py`

 * *Files identical despite different names*

### Comparing `numero_a_letras-0.0.4/test/test_numero_a_letras.py` & `numero_a_letras-0.0.5/test/test_numero_a_letras.py`

 * *Files identical despite different names*

