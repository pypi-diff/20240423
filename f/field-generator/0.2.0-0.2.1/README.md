# Comparing `tmp/field-generator-0.2.0.tar.gz` & `tmp/field-generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "field-generator-0.2.0.tar", last modified: Thu Apr 18 21:11:17 2024, max compression
+gzip compressed data, was "field-generator-0.2.1.tar", last modified: Tue Apr 23 20:01:36 2024, max compression
```

## Comparing `field-generator-0.2.0.tar` & `field-generator-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cs-488-01   (509) staff       (20)        0 2024-04-18 21:11:17.368901 field-generator-0.2.0/
--rw-r--r--   0 cs-488-01   (509) staff       (20)     1056 2024-02-22 21:03:03.000000 field-generator-0.2.0/LICENSE
--rw-r--r--   0 cs-488-01   (509) staff       (20)      518 2024-04-18 21:11:17.368777 field-generator-0.2.0/PKG-INFO
--rw-r--r--   0 cs-488-01   (509) staff       (20)      186 2024-02-22 21:55:33.000000 field-generator-0.2.0/README.md
-drwxr-xr-x   0 cs-488-01   (509) staff       (20)        0 2024-04-18 21:11:17.367930 field-generator-0.2.0/field_generator/
--rw-r--r--   0 cs-488-01   (509) staff       (20)     8114 2024-04-18 21:03:32.000000 field-generator-0.2.0/field_generator/__init__.py
-drwxr-xr-x   0 cs-488-01   (509) staff       (20)        0 2024-04-18 21:11:17.368597 field-generator-0.2.0/field_generator.egg-info/
--rw-r--r--   0 cs-488-01   (509) staff       (20)      518 2024-04-18 21:11:17.000000 field-generator-0.2.0/field_generator.egg-info/PKG-INFO
--rw-r--r--   0 cs-488-01   (509) staff       (20)      248 2024-04-18 21:11:17.000000 field-generator-0.2.0/field_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cs-488-01   (509) staff       (20)        1 2024-04-18 21:11:17.000000 field-generator-0.2.0/field_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cs-488-01   (509) staff       (20)       17 2024-04-18 21:11:17.000000 field-generator-0.2.0/field_generator.egg-info/requires.txt
--rw-r--r--   0 cs-488-01   (509) staff       (20)       16 2024-04-18 21:11:17.000000 field-generator-0.2.0/field_generator.egg-info/top_level.txt
--rw-r--r--   0 cs-488-01   (509) staff       (20)       38 2024-04-18 21:11:17.368939 field-generator-0.2.0/setup.cfg
--rw-r--r--   0 cs-488-01   (509) staff       (20)      540 2024-04-18 21:11:14.000000 field-generator-0.2.0/setup.py
+drwxr-xr-x   0 cs-488-01   (509) staff       (20)        0 2024-04-23 20:01:36.114902 field-generator-0.2.1/
+-rw-r--r--   0 cs-488-01   (509) staff       (20)     1056 2024-02-22 21:03:03.000000 field-generator-0.2.1/LICENSE
+-rw-r--r--   0 cs-488-01   (509) staff       (20)      437 2024-04-23 20:01:36.114792 field-generator-0.2.1/PKG-INFO
+-rw-r--r--   0 cs-488-01   (509) staff       (20)      105 2024-04-23 20:00:33.000000 field-generator-0.2.1/README.md
+drwxr-xr-x   0 cs-488-01   (509) staff       (20)        0 2024-04-23 20:01:36.114023 field-generator-0.2.1/field_generator/
+-rw-r--r--   0 cs-488-01   (509) staff       (20)     8209 2024-04-23 20:00:02.000000 field-generator-0.2.1/field_generator/__init__.py
+drwxr-xr-x   0 cs-488-01   (509) staff       (20)        0 2024-04-23 20:01:36.114623 field-generator-0.2.1/field_generator.egg-info/
+-rw-r--r--   0 cs-488-01   (509) staff       (20)      437 2024-04-23 20:01:36.000000 field-generator-0.2.1/field_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cs-488-01   (509) staff       (20)      248 2024-04-23 20:01:36.000000 field-generator-0.2.1/field_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cs-488-01   (509) staff       (20)        1 2024-04-23 20:01:36.000000 field-generator-0.2.1/field_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cs-488-01   (509) staff       (20)       17 2024-04-23 20:01:36.000000 field-generator-0.2.1/field_generator.egg-info/requires.txt
+-rw-r--r--   0 cs-488-01   (509) staff       (20)       16 2024-04-23 20:01:36.000000 field-generator-0.2.1/field_generator.egg-info/top_level.txt
+-rw-r--r--   0 cs-488-01   (509) staff       (20)       38 2024-04-23 20:01:36.114940 field-generator-0.2.1/setup.cfg
+-rw-r--r--   0 cs-488-01   (509) staff       (20)      540 2024-04-23 20:00:33.000000 field-generator-0.2.1/setup.py
```

### Comparing `field-generator-0.2.0/LICENSE` & `field-generator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `field-generator-0.2.0/field_generator/__init__.py` & `field-generator-0.2.1/field_generator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,25 +43,26 @@
 
     Returns fig, a matplotlib figure object.
     """
     np.seterr(divide='ignore', invalid='ignore')
     x = np.linspace(xmin, xmax, density * 20)
     y = np.linspace(ymin, ymax, density * 20)
     X, Y = np.meshgrid(x, y)
+    ratio = (ymax-ymin)/(xmax-xmin)
     # if hasattr(func, '__call__'):
     #     slopes = func(X, Y)
     # else:
 
     if not (type(func) is str or hasattr(func, '__call__')):
         raise Exception("L, bad argument")
     if type(func) is str:
         slopes = _parseFunc(func, X, Y)
     else:
         slopes = func(X, Y)
-    U = (1 / (1 + slopes ** 2) ** 0.5) * np.ones(X.shape)
+    U = (1 / (1 + slopes ** 2) ** 0.5) * np.ones(X.shape) * ratio
     V = (1 / (1 + slopes ** 2) ** 0.5) * slopes
 
     fig = plt.figure(num=figureNumber)
     plt.title("Slope Field Generator")
     plt.xlabel("X")
     plt.ylabel("Y")
     scale = 50 / lineLength if lineLength is not None else None
@@ -84,21 +85,21 @@
     Returns fig, a matplotlib figure object.
     """
 
     np.seterr(divide='ignore', invalid='ignore')
     x = np.linspace(xmin, xmax, density * 20)
     y = np.linspace(ymin, ymax, density * 20)
     X, Y = np.meshgrid(x, y)
-
+    ratio = (ymax-ymin)/(xmax-xmin)
     if not (type(partialOne) is str or hasattr(partialOne, '__call__')):
         raise Exception("L, bad argument")
     if type(partialOne) is str:
-        U = _parseFunc(partialOne, X, Y)
+        U = _parseFunc(partialOne, X, Y) * ratio
     else:
-        U = partialOne(X, Y)
+        U = partialOne(X, Y) * ratio
 
     if not (type(partialTwo) is str or hasattr(partialTwo, '__call__')):
         raise Exception("L, bad argument")
     if type(partialTwo) is str:
         V = _parseFunc(partialTwo, X, Y)
     else:
         V = partialTwo(X, Y)
```

### Comparing `field-generator-0.2.0/setup.py` & `field-generator-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setuptools.setup(
     name="field-generator",
-    version="0.2.0",
+    version="0.2.1",
     author="EQIKE",
     author_email="lc20-0098@lclark.edu",
     packages=["field_generator"],
     description="A simple slope field generator",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/iamawestruck/Slope-Field-Generator",
```

