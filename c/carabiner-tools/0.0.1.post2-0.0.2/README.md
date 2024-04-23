# Comparing `tmp/carabiner-tools-0.0.1.post2.tar.gz` & `tmp/carabiner_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carabiner-tools-0.0.1.post2.tar", last modified: Mon Mar 11 16:43:36 2024, max compression
+gzip compressed data, was "carabiner_tools-0.0.2.tar", last modified: Tue Apr 23 08:52:26 2024, max compression
```

## Comparing `carabiner-tools-0.0.1.post2.tar` & `carabiner_tools-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.841287 carabiner-tools-0.0.1.post2/carabiner/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/cliutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.841287 carabiner-tools-0.0.1.post2/carabiner/io/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/carabiner/mpl/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/mpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/mpl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/carabiner/pd/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/pd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/pd/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/carabiner/tf/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/tf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/carabiner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-03-11 16:43:36.000000 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-11 16:43:36.000000 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 16:43:36.000000 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-11 16:43:36.000000 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-11 16:43:36.000000 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-11 16:43:36.000000 carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:43:36.845287 carabiner-tools-0.0.1.post2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-11 16:43:31.000000 carabiner-tools-0.0.1.post2/test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.187558 carabiner_tools-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-23 08:52:26.187558 carabiner_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.183557 carabiner_tools-0.0.2/carabiner/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/cliutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.183557 carabiner_tools-0.0.2/carabiner/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.183557 carabiner_tools-0.0.2/carabiner/mpl/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/mpl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.183557 carabiner_tools-0.0.2/carabiner/pd/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/pd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/pd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.187558 carabiner_tools-0.0.2/carabiner/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/tf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/carabiner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.187558 carabiner_tools-0.0.2/carabiner_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-23 08:52:26.000000 carabiner_tools-0.0.2/carabiner_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-23 08:52:26.000000 carabiner_tools-0.0.2/carabiner_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:52:26.000000 carabiner_tools-0.0.2/carabiner_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 08:52:26.000000 carabiner_tools-0.0.2/carabiner_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 08:52:26.000000 carabiner_tools-0.0.2/carabiner_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 08:52:26.000000 carabiner_tools-0.0.2/carabiner_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:52:26.187558 carabiner_tools-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:52:26.187558 carabiner_tools-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 08:52:19.000000 carabiner_tools-0.0.2/test/tests.py
```

### Comparing `carabiner-tools-0.0.1.post2/LICENSE` & `carabiner_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/PKG-INFO` & `carabiner_tools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carabiner-tools
-Version: 0.0.1.post2
+Version: 0.0.2
 Summary: Useful utilities.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `carabiner-tools-0.0.1.post2/README.md` & `carabiner_tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/cast.py` & `carabiner_tools-0.0.2/carabiner/cast.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     >>> clist('Hello world')
     ['Hello world']
     >>> clist(('Hello', 'world'))  # doctest: +SKIP
     ['Hello', 'world']
     
     """
 
-    return list(x)
+    try:
+        return list(x)
+    except TypeError:  ## if x is not iterable
+        return [x]
 
 
 @clist.register
 def _(x: str) -> List[str]:
 
     return [x]
```

### Comparing `carabiner-tools-0.0.1.post2/carabiner/cli.py` & `carabiner_tools-0.0.2/carabiner/cli.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/cliutils.py` & `carabiner_tools-0.0.2/carabiner/cliutils.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/collections.py` & `carabiner_tools-0.0.2/carabiner/collections.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/decorators.py` & `carabiner_tools-0.0.2/carabiner/decorators.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/io/utils.py` & `carabiner_tools-0.0.2/carabiner/io/utils.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/itertools.py` & `carabiner_tools-0.0.2/carabiner/itertools.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/mpl/utils.py` & `carabiner_tools-0.0.2/carabiner/mpl/utils.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/pd/utils.py` & `carabiner_tools-0.0.2/carabiner/pd/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses import dataclass, field
 import os
 import sys
 
 try:
     import pandas as pd
 except ImportError:
-    raise ImportError("\Pandas not installed. Try installing with pip:"
+    raise ImportError("Pandas not installed. Try installing with pip:"
                       "\n$ pip install pandas\n"
                       "\nor reinstall carabiner with pandas:\n"
                       "\n$ pip install carabiner[pd]\n")
 
 from ..io import get_lines
 from ..utils import print_err
 
@@ -35,15 +35,15 @@
     out_delim: Optional[str] = field(default=None)
 
     def __post_init__(self):
 
         self.out_delim = self.out_delim or self.in_delim
 
         if self.in_delim == '\t':
-            self.in_delim = '\s+'
+            self.in_delim = r'\s+'
 
 
 _FORMAT: Dict[str, IOFormat] = {'.txt' : IOFormat('\t'), 
                                 '.tsv' : IOFormat('\t'), 
                                 '.csv' : IOFormat(','), 
                                 '.xlsx': IOFormat('xlsx')}
 
@@ -307,17 +307,17 @@
     -------
     pd.DataFrame or iterator of pd.DataFrame
         Pandas DataFrame of the input file.
     
     """
     
     delimiter = resolve_delim(file, format, 
-                              default='\s+')
+                              default='\t')
 
-    if delimiter != 'xlsx':
+    if delimiter.in_delim != 'xlsx':
 
         return read_csv(file, 
                         sep=delimiter.in_delim,
                         encoding='unicode_escape',
                         progress=progress,
                         chunksize=chunksize,
                         *args, **kwargs)
```

### Comparing `carabiner-tools-0.0.1.post2/carabiner/random.py` & `carabiner_tools-0.0.2/carabiner/random.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/tf/utils.py` & `carabiner_tools-0.0.2/carabiner/tf/utils.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner/utils.py` & `carabiner_tools-0.0.2/carabiner/utils.py`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/PKG-INFO` & `carabiner_tools-0.0.2/carabiner_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carabiner-tools
-Version: 0.0.1.post2
+Version: 0.0.2
 Summary: Useful utilities.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `carabiner-tools-0.0.1.post2/carabiner_tools.egg-info/SOURCES.txt` & `carabiner_tools-0.0.2/carabiner_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carabiner-tools-0.0.1.post2/pyproject.toml` & `carabiner_tools-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "carabiner-tools"
-version = "0.0.1.post2"
+version = "0.0.2"
 authors = [
   { name="Eachan Johnson", email="eachan.johnson@crick.ac.uk" },
 ]
 description = "Useful utilities."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

