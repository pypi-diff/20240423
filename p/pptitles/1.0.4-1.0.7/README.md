# Comparing `tmp/pptitles-1.0.4.tar.gz` & `tmp/pptitles-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptitles-1.0.4.tar", last modified: Tue Apr 23 20:09:13 2024, max compression
+gzip compressed data, was "pptitles-1.0.7.tar", last modified: Tue Apr 23 20:13:24 2024, max compression
```

## Comparing `pptitles-1.0.4.tar` & `pptitles-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 20:09:13.231100 pptitles-1.0.4/
--rw-r--r--   0 phx        (501) staff       (20)     1059 2024-04-23 19:47:35.000000 pptitles-1.0.4/LICENSE
--rw-r--r--   0 phx        (501) staff       (20)      713 2024-04-23 20:09:13.230695 pptitles-1.0.4/PKG-INFO
--rw-r--r--   0 phx        (501) staff       (20)      301 2024-04-23 19:52:54.000000 pptitles-1.0.4/README.md
--rwxr-xr-x   0 phx        (501) staff       (20)     2007 2024-04-23 19:44:05.000000 pptitles-1.0.4/pptitles
-drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 20:09:13.230291 pptitles-1.0.4/pptitles.egg-info/
--rw-r--r--   0 phx        (501) staff       (20)      713 2024-04-23 20:09:13.000000 pptitles-1.0.4/pptitles.egg-info/PKG-INFO
--rw-r--r--   0 phx        (501) staff       (20)      163 2024-04-23 20:09:13.000000 pptitles-1.0.4/pptitles.egg-info/SOURCES.txt
--rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 20:09:13.000000 pptitles-1.0.4/pptitles.egg-info/dependency_links.txt
--rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 20:09:13.000000 pptitles-1.0.4/pptitles.egg-info/top_level.txt
--rw-r--r--   0 phx        (501) staff       (20)       38 2024-04-23 20:09:13.231189 pptitles-1.0.4/setup.cfg
--rw-r--r--   0 phx        (501) staff       (20)      785 2024-04-23 20:09:08.000000 pptitles-1.0.4/setup.py
+drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 20:13:24.360233 pptitles-1.0.7/
+-rw-r--r--   0 phx        (501) staff       (20)     1059 2024-04-23 19:47:35.000000 pptitles-1.0.7/LICENSE
+-rw-r--r--   0 phx        (501) staff       (20)      614 2024-04-23 20:13:24.359779 pptitles-1.0.7/PKG-INFO
+-rw-r--r--   0 phx        (501) staff       (20)      202 2024-04-23 20:11:05.000000 pptitles-1.0.7/README.md
+-rwxr-xr-x   0 phx        (501) staff       (20)     2007 2024-04-23 19:44:05.000000 pptitles-1.0.7/pptitles
+drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 20:13:24.359364 pptitles-1.0.7/pptitles.egg-info/
+-rw-r--r--   0 phx        (501) staff       (20)      614 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/PKG-INFO
+-rw-r--r--   0 phx        (501) staff       (20)      163 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/SOURCES.txt
+-rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/dependency_links.txt
+-rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/top_level.txt
+-rw-r--r--   0 phx        (501) staff       (20)       38 2024-04-23 20:13:24.360320 pptitles-1.0.7/setup.cfg
+-rw-r--r--   0 phx        (501) staff       (20)      785 2024-04-23 20:13:19.000000 pptitles-1.0.7/setup.py
```

### Comparing `pptitles-1.0.4/LICENSE` & `pptitles-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pptitles-1.0.4/pptitles` & `pptitles-1.0.7/pptitles`

 * *Files identical despite different names*

### Comparing `pptitles-1.0.4/setup.py` & `pptitles-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pptitles',
-    version='1.0.4',
+    version='1.0.7',
     scripts=['pptitles'],  # Adjust as needed if it's a file or use glob.glob() for multiple files
     author='phx',
     author_email='phx@example.com',
     description='Extract the slide number and title from all slides in a PowerPoint presentation.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/phx/pptitles',
```

