# Comparing `tmp/python_flux-1.0.8.tar.gz` & `tmp/python_flux-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.0.8.tar", max compression
+gzip compressed data, was "python_flux-1.0.9.tar", max compression
```

## Comparing `python_flux-1.0.8.tar` & `python_flux-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6839 2024-04-22 18:08:08.037611 python_flux-1.0.8/README.rst
--rw-r--r--   0        0        0      741 2024-04-22 18:08:07.618738 python_flux-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.8/python_flux/__init__.py
--rw-r--r--   0        0        0    16467 2024-04-22 18:08:07.619685 python_flux-1.0.8/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.0.8/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1596 2024-04-18 05:35:27.173339 python_flux-1.0.8/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.0.8/python_flux/subscribers.py
--rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 python_flux-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6839 2024-04-22 18:08:08.037611 python_flux-1.0.9/README.rst
+-rw-r--r--   0        0        0      741 2024-04-22 20:53:45.952451 python_flux-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.9/python_flux/__init__.py
+-rw-r--r--   0        0        0    16539 2024-04-22 20:53:45.545182 python_flux-1.0.9/python_flux/flux.py
+-rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.0.9/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-18 05:35:27.173339 python_flux-1.0.9/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.0.9/python_flux/subscribers.py
+-rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 python_flux-1.0.9/PKG-INFO
```

### Comparing `python_flux-1.0.8/README.rst` & `python_flux-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.8/pyproject.toml` & `python_flux-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.0.8"
+version = "1.0.9"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.0.8/python_flux/flux.py` & `python_flux-1.0.9/python_flux/flux.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,24 +222,26 @@
         self.predicate = p
         self.on_mismatch = m
 
     def next(self, context):
         value, e, ctx = super(FFilter, self).next(context)
         if e is not None:
             return value, e, ctx
+
         valid, e = fu.try_or(partial(self.predicate), value, context)
         while e is None and not valid:
             _, e = fu.try_or(partial(self.on_mismatch), value, context)
             if e is not None:
                 return value, e, ctx
             super(FFilter, self).prepare_next()
-            value, e, ctx = super(FFilter, self).next(context)
+            value, e, new_ctx = super(FFilter, self).next(ctx)
             if e is not None:
                 return value, e, ctx
-            valid, e = fu.try_or(partial(self.predicate), value, context)
+            ctx = merge(ctx, new_ctx)
+            valid, e = fu.try_or(partial(self.predicate), value, ctx)
         return value, e, ctx
 
 
 class FTake(Stream):
     def __init__(self, count, flux):
         super().__init__(flux)
         self.count = count
@@ -350,18 +352,18 @@
                     fgen = PFromGenerator(func)
                 self.current = fgen
                 self.current.prepare_next()
 
             cur_value, cur_e, cur_ctx = self.current.next(ctx)
             if cur_e is None:
                 return cur_value, cur_e, cur_ctx
-
             if isinstance(cur_e, StopIteration):
                 self.current = None
                 super(FFlatMap, self).prepare_next()
+            ctx = merge(ctx, cur_ctx)
 
 
 class FOnErrorResume(Stream):
     def __init__(self, f, exceptions, flux):
         super().__init__(flux)
         self.on_error_resume = f
         self.exceptions = exceptions
```

### Comparing `python_flux-1.0.8/python_flux/flux_utilis.py` & `python_flux-1.0.9/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.8/python_flux/producers.py` & `python_flux-1.0.9/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.8/python_flux/subscribers.py` & `python_flux-1.0.9/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.8/PKG-INFO` & `python_flux-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.0.8
+Version: 1.0.9
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

