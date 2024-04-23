# Comparing `tmp/nestipy_decorator-0.1.0.tar.gz` & `tmp/nestipy_decorator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_decorator-0.1.0.tar", max compression
+gzip compressed data, was "nestipy_decorator-0.1.1.tar", max compression
```

## Comparing `nestipy_decorator-0.1.0.tar` & `nestipy_decorator-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-23 12:07:02.604929 nestipy_decorator-0.1.0/README.md
--rw-r--r--   0        0        0      388 2024-04-23 12:09:44.728419 nestipy_decorator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2829 2024-04-22 14:32:48.657431 nestipy_decorator-0.1.0/src/nestipy_decorator/__init__.py
--rw-r--r--   0        0        0     1204 2024-04-23 12:09:15.552510 nestipy_decorator-0.1.0/src/nestipy_decorator/method.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 nestipy_decorator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 12:07:02.604929 nestipy_decorator-0.1.1/README.md
+-rw-r--r--   0        0        0      388 2024-04-23 12:22:33.798000 nestipy_decorator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3025 2024-04-23 12:22:26.378023 nestipy_decorator-0.1.1/src/nestipy_decorator/__init__.py
+-rw-r--r--   0        0        0     1204 2024-04-23 12:09:15.552510 nestipy_decorator-0.1.1/src/nestipy_decorator/method.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 nestipy_decorator-0.1.1/PKG-INFO
```

### Comparing `nestipy_decorator-0.1.0/src/nestipy_decorator/__init__.py` & `nestipy_decorator-0.1.1/src/nestipy_decorator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import enum
 from typing import Type, Callable, Union
 
 from nestipy_ioc import NestipyContainer, ModuleProviderDict
 from nestipy_metadata import ModuleMetadata, Reflect, RouteKey
 
+from method import Route, Get, Post, Patch, Put, Delete
+
 
 class Scope(enum.Enum):
     Request = 'Request'
     Transient = 'Transient'
     Singleton = 'Singleton'
 
 
@@ -71,7 +73,20 @@
                              self.controllers + getattr(cls, ModuleMetadata.Controllers, []))
         Reflect.set_metadata(cls, ModuleMetadata.Imports, self.imports + getattr(cls, ModuleMetadata.Imports, []))
         Reflect.set_metadata(cls, ModuleMetadata.Exports, self.exports + getattr(cls, ModuleMetadata.Exports, []))
         Reflect.set_metadata(cls, ModuleMetadata.Global, self.is_global or getattr(cls, ModuleMetadata.Global, False))
         Reflect.set_metadata(cls, ModuleMetadata.Module, True)
         self.container.add_singleton(cls)
         return cls
+
+
+__all__ = [
+    "Module",
+    "Controller",
+    "Injectable",
+    "Route",
+    "Get",
+    "Post",
+    "Put",
+    "Patch",
+    "Delete"
+]
```

### Comparing `nestipy_decorator-0.1.0/src/nestipy_decorator/method.py` & `nestipy_decorator-0.1.1/src/nestipy_decorator/method.py`

 * *Files identical despite different names*

