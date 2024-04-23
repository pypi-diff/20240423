# Comparing `tmp/sweecrypt-1.0.2.tar.gz` & `tmp/sweecrypt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweecrypt-1.0.2.tar", last modified: Tue Apr  9 00:36:10 2024, max compression
+gzip compressed data, was "sweecrypt-1.0.3.tar", last modified: Tue Apr 23 04:56:44 2024, max compression
```

## Comparing `sweecrypt-1.0.2.tar` & `sweecrypt-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:36:10.001913 sweecrypt-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 00:35:55.000000 sweecrypt-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 00:36:10.001913 sweecrypt-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 00:35:55.000000 sweecrypt-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:36:10.001913 sweecrypt-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-09 00:35:55.000000 sweecrypt-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:36:10.001913 sweecrypt-1.0.2/sweecrypt/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 00:35:55.000000 sweecrypt-1.0.2/sweecrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 00:35:55.000000 sweecrypt-1.0.2/sweecrypt/sweecryptt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:36:10.001913 sweecrypt-1.0.2/sweecrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 00:36:09.000000 sweecrypt-1.0.2/sweecrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 00:36:09.000000 sweecrypt-1.0.2/sweecrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:36:09.000000 sweecrypt-1.0.2/sweecrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 00:36:09.000000 sweecrypt-1.0.2/sweecrypt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:56:44.180912 sweecrypt-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 04:56:40.000000 sweecrypt-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 04:56:44.180912 sweecrypt-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 04:56:40.000000 sweecrypt-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 04:56:44.180912 sweecrypt-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-23 04:56:40.000000 sweecrypt-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:56:44.180912 sweecrypt-1.0.3/sweecrypt/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 04:56:40.000000 sweecrypt-1.0.3/sweecrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-23 04:56:40.000000 sweecrypt-1.0.3/sweecrypt/sweecryptt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:56:44.180912 sweecrypt-1.0.3/sweecrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 04:56:44.000000 sweecrypt-1.0.3/sweecrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-23 04:56:44.000000 sweecrypt-1.0.3/sweecrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:56:44.000000 sweecrypt-1.0.3/sweecrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 04:56:44.000000 sweecrypt-1.0.3/sweecrypt.egg-info/top_level.txt
```

### Comparing `sweecrypt-1.0.2/LICENSE` & `sweecrypt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sweecrypt-1.0.2/setup.py` & `sweecrypt-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2' 
+VERSION = '1.0.3' 
 DESCRIPTION = 'An easy and fun encryption module.'
-readme = "README.md"
 LONG_DESCRIPTION = 'SweeCrypt is an easy and fun encryption module that turn letters and numbers to symbols found on the keyboard.'
 
 setup(
         name="sweecrypt", 
         version=VERSION,
         author="SweeZero",
         author_email="swee@mailfence.com",
+        readme = "README.md",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=[],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
```

### Comparing `sweecrypt-1.0.2/sweecrypt/sweecryptt.py` & `sweecrypt-1.0.3/sweecrypt/sweecryptt.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     "5",
     "6",
     "7",
     "8",
     "9",
     "0",
     "-",
+    "&",
+    ":",
+    ";",
+    "\"",
 ]
 codes = [
     "`",
     "-",
     ")",
     "/",
     "?",
@@ -89,14 +93,18 @@
     "k",
     "l",
     "m",
     "n",
     "o",
     "p",
     "q",
+    "r",
+    "s",
+    "t",
+    "u",
 ]
 
 
 def encrypt(what):
     encoded = ""
     what = what.lower()
     for i in range(len(what)):
```

