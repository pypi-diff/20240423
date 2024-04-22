# Comparing `tmp/tkz-1.0.0.tar.gz` & `tmp/tkz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkz-1.0.0.tar", last modified: Mon Apr 22 22:41:54 2024, max compression
+gzip compressed data, was "tkz-1.0.1.tar", last modified: Mon Apr 22 22:54:59 2024, max compression
```

## Comparing `tkz-1.0.0.tar` & `tkz-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.771881 tkz-1.0.0/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.0/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 22:41:54.771799 tkz-1.0.0/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    14676 2024-04-22 22:41:20.000000 tkz-1.0.0/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.0/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-22 22:41:54.772097 tkz-1.0.0/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.769840 tkz-1.0.0/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.770759 tkz-1.0.0/src/tkz/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.0/src/tkz/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    85841 2024-04-22 21:44:06.000000 tkz-1.0.0/src/tkz/tkz.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.771627 tkz-1.0.0/src/tkz.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:54:59.427324 tkz-1.0.1/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.1/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 22:54:59.427253 tkz-1.0.1/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    14676 2024-04-22 22:41:20.000000 tkz-1.0.1/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.1/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-22 22:54:59.427553 tkz-1.0.1/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:54:59.425631 tkz-1.0.1/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:54:59.426300 tkz-1.0.1/src/tkz/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.1/src/tkz/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    85862 2024-04-22 22:53:54.000000 tkz-1.0.1/src/tkz/tkz.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:54:59.427078 tkz-1.0.1/src/tkz.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 22:54:59.000000 tkz-1.0.1/src/tkz.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-22 22:54:59.000000 tkz-1.0.1/src/tkz.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-22 22:54:59.000000 tkz-1.0.1/src/tkz.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-22 22:54:59.000000 tkz-1.0.1/src/tkz.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-22 22:54:59.000000 tkz-1.0.1/src/tkz.egg-info/top_level.txt
```

### Comparing `tkz-1.0.0/LICENSE.txt` & `tkz-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkz-1.0.0/PKG-INFO` & `tkz-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkz
-Version: 1.0.0
+Version: 1.0.1
 Summary: TikZ Figure Generator
 Home-page: https://gitlab.com/davidwoodburn/tkz
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tkz-1.0.0/README.md` & `tkz-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tkz-1.0.0/setup.cfg` & `tkz-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tkz
-version = 1.0.0
+version = 1.0.1
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = TikZ Figure Generator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/tkz
 classifiers =
```

### Comparing `tkz-1.0.0/src/tkz/tkz.py` & `tkz-1.0.1/src/tkz/tkz.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,18 +616,18 @@
 
         # Ensure some data was defined.
         if (x is None) and (y is None) and (z is None):
             raise ValueError(f"No data was defined for data set {j}.")
 
         # Handle undefined arrays.
         if y is None:
-            if z is not None:
+            if (z is not None) and sets[j].zony:
                 y = z
                 z = None
-            if x is not None:
+            elif x is not None:
                 y = x
                 x = None
         if x is None:
             x = np.arange(y.shape[-1])
 
         # Check for too many dimensions. At this point,
         # `x` and `y` are guaranteed to be arrays.
```

### Comparing `tkz-1.0.0/src/tkz.egg-info/PKG-INFO` & `tkz-1.0.1/src/tkz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkz
-Version: 1.0.0
+Version: 1.0.1
 Summary: TikZ Figure Generator
 Home-page: https://gitlab.com/davidwoodburn/tkz
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

