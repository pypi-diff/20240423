# Comparing `tmp/placeholder_img-0.3.tar.gz` & `tmp/placeholder_img-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "placeholder_img-0.3.tar", last modified: Tue Apr 23 06:05:24 2024, max compression
+gzip compressed data, was "placeholder_img-0.4.tar", last modified: Tue Apr 23 06:30:23 2024, max compression
```

## Comparing `placeholder_img-0.3.tar` & `placeholder_img-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.497777 placeholder_img-0.3/
--rw-r--r--   0 mzs01-search5   (501) staff       (20)       26 2024-04-23 05:57:32.000000 placeholder_img-0.3/MANIFEST.in
--rw-r--r--   0 mzs01-search5   (501) staff       (20)      742 2024-04-23 06:05:24.497197 placeholder_img-0.3/PKG-INFO
--rw-r--r--   0 mzs01-search5   (501) staff       (20)      391 2024-04-23 05:57:32.000000 placeholder_img-0.3/README.rst
-drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.486080 placeholder_img-0.3/placeholder/
--rw-r--r--   0 mzs01-search5   (501) staff       (20)       37 2024-04-23 05:57:32.000000 placeholder_img-0.3/placeholder/__init__.py
--rw-r--r--   0 mzs01-search5   (501) staff       (20)     1893 2024-04-23 05:57:32.000000 placeholder_img-0.3/placeholder/creator.py
-drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.486661 placeholder_img-0.3/placeholder/public/
--rw-r--r--   0 mzs01-search5   (501) staff       (20)  6192764 2024-04-23 05:57:32.000000 placeholder_img-0.3/placeholder/public/NotoSansKR-Regular.ttf
-drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.496548 placeholder_img-0.3/placeholder_img.egg-info/
--rw-r--r--   0 mzs01-search5   (501) staff       (20)      742 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/PKG-INFO
--rw-r--r--   0 mzs01-search5   (501) staff       (20)      320 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/SOURCES.txt
--rw-r--r--   0 mzs01-search5   (501) staff       (20)        1 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/dependency_links.txt
--rw-r--r--   0 mzs01-search5   (501) staff       (20)        7 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/requires.txt
--rw-r--r--   0 mzs01-search5   (501) staff       (20)       12 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/top_level.txt
--rw-r--r--   0 mzs01-search5   (501) staff       (20)      536 2024-04-23 06:05:18.000000 placeholder_img-0.3/pyproject.toml
--rw-r--r--   0 mzs01-search5   (501) staff       (20)       38 2024-04-23 06:05:24.497876 placeholder_img-0.3/setup.cfg
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:30:23.168325 placeholder_img-0.4/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       26 2024-04-23 05:57:32.000000 placeholder_img-0.4/MANIFEST.in
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      881 2024-04-23 06:30:23.163789 placeholder_img-0.4/PKG-INFO
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      391 2024-04-23 05:57:32.000000 placeholder_img-0.4/README.rst
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:30:23.149053 placeholder_img-0.4/placeholder/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       37 2024-04-23 05:57:32.000000 placeholder_img-0.4/placeholder/__init__.py
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)     1925 2024-04-23 06:26:48.000000 placeholder_img-0.4/placeholder/creator.py
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:30:23.150505 placeholder_img-0.4/placeholder/public/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)  6192764 2024-04-23 05:57:32.000000 placeholder_img-0.4/placeholder/public/NotoSansKR-Regular.ttf
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:30:23.163142 placeholder_img-0.4/placeholder_img.egg-info/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      881 2024-04-23 06:30:23.000000 placeholder_img-0.4/placeholder_img.egg-info/PKG-INFO
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      320 2024-04-23 06:30:23.000000 placeholder_img-0.4/placeholder_img.egg-info/SOURCES.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)        1 2024-04-23 06:30:23.000000 placeholder_img-0.4/placeholder_img.egg-info/dependency_links.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)        7 2024-04-23 06:30:23.000000 placeholder_img-0.4/placeholder_img.egg-info/requires.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       12 2024-04-23 06:30:23.000000 placeholder_img-0.4/placeholder_img.egg-info/top_level.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      671 2024-04-23 06:29:22.000000 placeholder_img-0.4/pyproject.toml
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       38 2024-04-23 06:30:23.168441 placeholder_img-0.4/setup.cfg
```

### Comparing `placeholder_img-0.3/PKG-INFO` & `placeholder_img-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: placeholder-img
-Version: 0.3
+Version: 0.4
 Summary: Create a placeholder image to return an image object or save the file
 Author-email: Lee Ji-ho <search5@gmail.com>
 License: BSD-3-Clause
+Project-URL: Repository, https://github.com/search5/placeholder-img
+Project-URL: Issues, https://github.com/search5/placeholder-img/issues
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Requires-Dist: pillow
 
 =================================
```

### Comparing `placeholder_img-0.3/placeholder/creator.py` & `placeholder_img-0.4/placeholder/creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from io import BytesIO
 import os
 import importlib.resources as pkg_resources
 
 from PIL import ImageFont, Image, ImageDraw, ImageColor
 
 
-FONT_PATH = pkg_resources('placeholder.public', 'NotoSansKR-Regular.ttf')
+FONT_PATH = pkg_resources.files('placeholder.public').joinpath('NotoSansKR-Regular.ttf')
+print(FONT_PATH)
 
 
 def _parse_size(size):
     Size = namedtuple('Size', ['width', 'height'])
     try:
         width, height = size.split('x')
     except ValueError:
```

### Comparing `placeholder_img-0.3/placeholder/public/NotoSansKR-Regular.ttf` & `placeholder_img-0.4/placeholder/public/NotoSansKR-Regular.ttf`

 * *Files identical despite different names*

### Comparing `placeholder_img-0.3/placeholder_img.egg-info/PKG-INFO` & `placeholder_img-0.4/placeholder_img.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: placeholder-img
-Version: 0.3
+Version: 0.4
 Summary: Create a placeholder image to return an image object or save the file
 Author-email: Lee Ji-ho <search5@gmail.com>
 License: BSD-3-Clause
+Project-URL: Repository, https://github.com/search5/placeholder-img
+Project-URL: Issues, https://github.com/search5/placeholder-img/issues
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Requires-Dist: pillow
 
 =================================
```

### Comparing `placeholder_img-0.3/pyproject.toml` & `placeholder_img-0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "placeholder-img"
-version = "0.3"
+version = "0.4"
 authors = [
     {name = "Lee Ji-ho", email = "search5@gmail.com"}
 ]
 description = "Create a placeholder image to return an image object or save the file"
 readme = "README.rst"
 requires-python = ">=3.9"
 keywords = ["one", "two"]
@@ -16,9 +16,13 @@
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     "pillow",
 ]
 
+[project.urls]
+Repository = "https://github.com/search5/placeholder-img"
+Issues = "https://github.com/search5/placeholder-img/issues"
+
 [options]
 include-package-data = true
```

