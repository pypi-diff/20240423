# Comparing `tmp/placeholder_img-0.2.tar.gz` & `tmp/placeholder_img-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "placeholder_img-0.2.tar", last modified: Sat Apr 13 18:59:58 2024, max compression
+gzip compressed data, was "placeholder_img-0.3.tar", last modified: Tue Apr 23 06:05:24 2024, max compression
```

## Comparing `placeholder_img-0.2.tar` & `placeholder_img-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jiho      (1000) jiho      (1000)        0 2024-04-13 18:59:58.987718 placeholder_img-0.2/
--rw-rw-r--   0 jiho      (1000) jiho      (1000)       26 2024-04-13 18:59:52.000000 placeholder_img-0.2/MANIFEST.in
--rw-r--r--   0 jiho      (1000) jiho      (1000)      742 2024-04-13 18:59:58.983718 placeholder_img-0.2/PKG-INFO
--rw-rw-r--   0 jiho      (1000) jiho      (1000)      391 2024-04-13 17:22:59.000000 placeholder_img-0.2/README.rst
-drwxrwxr-x   0 jiho      (1000) jiho      (1000)        0 2024-04-13 18:59:58.979718 placeholder_img-0.2/placeholder/
--rw-rw-r--   0 jiho      (1000) jiho      (1000)       37 2024-04-13 17:03:40.000000 placeholder_img-0.2/placeholder/__init__.py
--rw-rw-r--   0 jiho      (1000) jiho      (1000)     2176 2024-04-13 17:06:40.000000 placeholder_img-0.2/placeholder/creator.py
-drwxrwxr-x   0 jiho      (1000) jiho      (1000)        0 2024-04-13 18:59:58.979718 placeholder_img-0.2/placeholder/public/
--rw-rw-r--   0 jiho      (1000) jiho      (1000)  6192764 2023-08-17 23:53:04.000000 placeholder_img-0.2/placeholder/public/NotoSansKR-Regular.ttf
-drwxrwxr-x   0 jiho      (1000) jiho      (1000)        0 2024-04-13 18:59:58.983718 placeholder_img-0.2/placeholder_img.egg-info/
--rw-r--r--   0 jiho      (1000) jiho      (1000)      742 2024-04-13 18:59:58.000000 placeholder_img-0.2/placeholder_img.egg-info/PKG-INFO
--rw-rw-r--   0 jiho      (1000) jiho      (1000)      320 2024-04-13 18:59:58.000000 placeholder_img-0.2/placeholder_img.egg-info/SOURCES.txt
--rw-rw-r--   0 jiho      (1000) jiho      (1000)        1 2024-04-13 18:59:58.000000 placeholder_img-0.2/placeholder_img.egg-info/dependency_links.txt
--rw-rw-r--   0 jiho      (1000) jiho      (1000)        7 2024-04-13 18:59:58.000000 placeholder_img-0.2/placeholder_img.egg-info/requires.txt
--rw-rw-r--   0 jiho      (1000) jiho      (1000)       12 2024-04-13 18:59:58.000000 placeholder_img-0.2/placeholder_img.egg-info/top_level.txt
--rw-rw-r--   0 jiho      (1000) jiho      (1000)      539 2024-04-13 18:58:36.000000 placeholder_img-0.2/pyproject.toml
--rw-rw-r--   0 jiho      (1000) jiho      (1000)       38 2024-04-13 18:59:58.987718 placeholder_img-0.2/setup.cfg
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.497777 placeholder_img-0.3/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       26 2024-04-23 05:57:32.000000 placeholder_img-0.3/MANIFEST.in
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      742 2024-04-23 06:05:24.497197 placeholder_img-0.3/PKG-INFO
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      391 2024-04-23 05:57:32.000000 placeholder_img-0.3/README.rst
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.486080 placeholder_img-0.3/placeholder/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       37 2024-04-23 05:57:32.000000 placeholder_img-0.3/placeholder/__init__.py
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)     1893 2024-04-23 05:57:32.000000 placeholder_img-0.3/placeholder/creator.py
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.486661 placeholder_img-0.3/placeholder/public/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)  6192764 2024-04-23 05:57:32.000000 placeholder_img-0.3/placeholder/public/NotoSansKR-Regular.ttf
+drwxr-xr-x   0 mzs01-search5   (501) staff       (20)        0 2024-04-23 06:05:24.496548 placeholder_img-0.3/placeholder_img.egg-info/
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      742 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/PKG-INFO
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      320 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/SOURCES.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)        1 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/dependency_links.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)        7 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/requires.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       12 2024-04-23 06:05:24.000000 placeholder_img-0.3/placeholder_img.egg-info/top_level.txt
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)      536 2024-04-23 06:05:18.000000 placeholder_img-0.3/pyproject.toml
+-rw-r--r--   0 mzs01-search5   (501) staff       (20)       38 2024-04-23 06:05:24.497876 placeholder_img-0.3/setup.cfg
```

### Comparing `placeholder_img-0.2/PKG-INFO` & `placeholder_img-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placeholder-img
-Version: 0.2
+Version: 0.3
 Summary: Create a placeholder image to return an image object or save the file
 Author-email: Lee Ji-ho <search5@gmail.com>
 License: BSD-3-Clause
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `placeholder_img-0.2/placeholder/creator.py` & `placeholder_img-0.3/placeholder/creator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 from collections import namedtuple
 from io import BytesIO
 import os
-import sys
-import importlib
+import importlib.resources as pkg_resources
 
 from PIL import ImageFont, Image, ImageDraw, ImageColor
-import importlib._bootstrap
 
 
-def get_abs_filepath(package, path):
-    spec = importlib.util.find_spec(package)
-    mod = (sys.modules.get(package) or importlib._bootstrap._load(spec))
-    parts = path.split("/")
-    parts.insert(0, os.path.dirname(mod.__file__))
-    return os.path.join(*parts)
-
-
-FONT_PATH = get_abs_filepath('placeholder', 'public/NotoSansKR-Regular.ttf')
+FONT_PATH = pkg_resources('placeholder.public', 'NotoSansKR-Regular.ttf')
 
 
 def _parse_size(size):
     Size = namedtuple('Size', ['width', 'height'])
     try:
         width, height = size.split('x')
     except ValueError:
```

### Comparing `placeholder_img-0.2/placeholder/public/NotoSansKR-Regular.ttf` & `placeholder_img-0.3/placeholder/public/NotoSansKR-Regular.ttf`

 * *Files identical despite different names*

### Comparing `placeholder_img-0.2/placeholder_img.egg-info/PKG-INFO` & `placeholder_img-0.3/placeholder_img.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placeholder-img
-Version: 0.2
+Version: 0.3
 Summary: Create a placeholder image to return an image object or save the file
 Author-email: Lee Ji-ho <search5@gmail.com>
 License: BSD-3-Clause
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `placeholder_img-0.2/pyproject.toml` & `placeholder_img-0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "placeholder-img"
-version = "0.2"
+version = "0.3"
 authors = [
-    {name = "Lee Ji-ho", email = "search5@gmail.com"},
+    {name = "Lee Ji-ho", email = "search5@gmail.com"}
 ]
 description = "Create a placeholder image to return an image object or save the file"
 readme = "README.rst"
 requires-python = ">=3.9"
 keywords = ["one", "two"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3"
 ]
 dependencies = [
     "pillow",
 ]
 
 [options]
 include-package-data = true
-
```

