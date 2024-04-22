# Comparing `tmp/thick-0.0.4.tar.gz` & `tmp/thick-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thick-0.0.4.tar", last modified: Sun Mar 31 05:05:34 2024, max compression
+gzip compressed data, was "thick-0.0.5.tar", last modified: Mon Apr 22 21:56:46 2024, max compression
```

## Comparing `thick-0.0.4.tar` & `thick-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-03-31 05:05:34.970057 thick-0.0.4/
--rw-r--r--   0 clark     (1000) clark     (1000)    35147 2024-03-30 04:28:52.000000 thick-0.0.4/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)    43623 2024-03-31 05:05:34.970057 thick-0.0.4/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     2729 2024-03-31 04:27:55.000000 thick-0.0.4/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)      538 2024-03-31 02:31:03.000000 thick-0.0.4/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2024-03-31 05:05:34.970057 thick-0.0.4/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-03-31 05:05:34.970057 thick-0.0.4/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-03-31 05:05:34.970057 thick-0.0.4/src/thick/
--rw-r--r--   0 clark     (1000) clark     (1000)       48 2024-03-31 05:05:25.000000 thick-0.0.4/src/thick/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)        2 2024-03-30 04:17:32.000000 thick-0.0.4/src/thick/py.typed
--rw-r--r--   0 clark     (1000) clark     (1000)    12525 2024-03-31 05:05:25.000000 thick-0.0.4/src/thick/thick.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-03-31 05:05:34.970057 thick-0.0.4/src/thick.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)    43623 2024-03-31 05:05:34.000000 thick-0.0.4/src/thick.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      224 2024-03-31 05:05:34.000000 thick-0.0.4/src/thick.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2024-03-31 05:05:34.000000 thick-0.0.4/src/thick.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        6 2024-03-31 05:05:34.000000 thick-0.0.4/src/thick.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-22 21:56:46.383369 thick-0.0.5/
+-rw-r--r--   0 clark     (1000) clark     (1000)    35147 2024-04-22 21:30:59.000000 thick-0.0.5/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)    44009 2024-04-22 21:56:46.383369 thick-0.0.5/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     3115 2024-04-22 21:46:38.000000 thick-0.0.5/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)      538 2024-04-22 21:30:59.000000 thick-0.0.5/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2024-04-22 21:56:46.383369 thick-0.0.5/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-22 21:56:46.383369 thick-0.0.5/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-22 21:56:46.383369 thick-0.0.5/src/thick/
+-rw-r--r--   0 clark     (1000) clark     (1000)       48 2024-04-22 21:56:38.000000 thick-0.0.5/src/thick/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)        2 2024-04-22 21:30:59.000000 thick-0.0.5/src/thick/py.typed
+-rw-r--r--   0 clark     (1000) clark     (1000)    12435 2024-04-22 21:46:38.000000 thick-0.0.5/src/thick/thick.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-22 21:56:46.383369 thick-0.0.5/src/thick.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)    44009 2024-04-22 21:56:46.000000 thick-0.0.5/src/thick.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      224 2024-04-22 21:56:46.000000 thick-0.0.5/src/thick.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2024-04-22 21:56:46.000000 thick-0.0.5/src/thick.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        6 2024-04-22 21:56:46.000000 thick-0.0.5/src/thick.egg-info/top_level.txt
```

### Comparing `thick-0.0.4/LICENSE` & `thick-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thick-0.0.4/PKG-INFO` & `thick-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thick
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python dictionary that gets Thicker rather than longer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -699,25 +699,27 @@
 
 ```py
 foo = {
     "a": ComplexObjectName1,
     "b": ComplexObjectName2,
     "c": ComplexObjectName1,
     ...
-}```
+}
+```
 
 In this case, typing out such a dictionary, especially one with more entries, violates the DRY principle (a personal favorite) and can be quite error-prone.
 
 Perhaps you would try to map a tuple of key to a value:
 ```py
 foo = {
     ("a", "c", ...): ComplexObjectName1,
     ("b", ...): ComplexObjectName2,
     ...
-}```
+}
+```
 
 But, obviously, this breaks on a call like:
 ```py
 "a" in foo
 ```
 
 Enter the Thick dict. Given an iterible (but not a string) of keys, or multiple keys mapped to one value, the Thick automatically deduplicates values, and uses set logic to determine if a given key is a subset of any key.
@@ -790,12 +792,34 @@
 2 in my_thick
 True
 
 2 in my_thick_iterable_key
 False
 ```
 
+### But I just want the normal dictionary!
+Good news! You can use the more-simple, D.R.Y. method for construction, and then get the desired dict directly out!
+```py
+my_thick = Thick({
+    ("a", "b", "c"): foo,
+    ("d", "e", "f"): bar,
+    ...
+    })
+
+normal_dict = my_thick.thin()
+{
+    "a": foo,
+    "b": foo,
+    "c": foo,
+    "d": bar,
+    "e": bar,
+    "f": bar,
+    ...
+}
+```
+
+
 ## Is this really worth it?
 
 Probably not! I intend to use this in a few of my other personal projects, but I also wanted some more experiencing putting up a pip/PyPI package, and I thought the name was fun (and a little risque, to be fair).
 
 I don't expect anyone else to use this, but, if it does end up being useful, please let me know! If you find any bugs or have any feature requests, please create a GitHub issue!
```

### Comparing `thick-0.0.4/README.md` & `thick-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 
 ```py
 foo = {
     "a": ComplexObjectName1,
     "b": ComplexObjectName2,
     "c": ComplexObjectName1,
     ...
-}```
+}
+```
 
 In this case, typing out such a dictionary, especially one with more entries, violates the DRY principle (a personal favorite) and can be quite error-prone.
 
 Perhaps you would try to map a tuple of key to a value:
 ```py
 foo = {
     ("a", "c", ...): ComplexObjectName1,
     ("b", ...): ComplexObjectName2,
     ...
-}```
+}
+```
 
 But, obviously, this breaks on a call like:
 ```py
 "a" in foo
 ```
 
 Enter the Thick dict. Given an iterible (but not a string) of keys, or multiple keys mapped to one value, the Thick automatically deduplicates values, and uses set logic to determine if a given key is a subset of any key.
@@ -105,12 +107,34 @@
 2 in my_thick
 True
 
 2 in my_thick_iterable_key
 False
 ```
 
+### But I just want the normal dictionary!
+Good news! You can use the more-simple, D.R.Y. method for construction, and then get the desired dict directly out!
+```py
+my_thick = Thick({
+    ("a", "b", "c"): foo,
+    ("d", "e", "f"): bar,
+    ...
+    })
+
+normal_dict = my_thick.thin()
+{
+    "a": foo,
+    "b": foo,
+    "c": foo,
+    "d": bar,
+    "e": bar,
+    "f": bar,
+    ...
+}
+```
+
+
 ## Is this really worth it?
 
 Probably not! I intend to use this in a few of my other personal projects, but I also wanted some more experiencing putting up a pip/PyPI package, and I thought the name was fun (and a little risque, to be fair).
 
 I don't expect anyone else to use this, but, if it does end up being useful, please let me know! If you find any bugs or have any feature requests, please create a GitHub issue!
```

### Comparing `thick-0.0.4/pyproject.toml` & `thick-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thick-0.0.4/src/thick/thick.py` & `thick-0.0.5/src/thick/thick.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Mapping, Any, Iterator, Iterable
 from collections import UserDict
 from collections.abc import Set, KeysView, ItemsView, ValuesView
 
 
 class ThickKey(Set):
-    """A custom \"key\" for a Thick dict. Effectively a frozenset implementation
+    """A custom "key" for a Thick dict. Effectively a frozenset implementation
     with a custom repr."""
 
     def __init__(self, d: Any) -> None:
         """wraps around a frozenset, the input data can be
         any type, will be cast to a Collection"""
         if (isinstance(d, str) and len(d) > 1) or not isinstance(d, Iterable):
             d = (d,)
@@ -262,36 +262,33 @@
             del self.data[whole_key]
             return
 
         raise KeyError(key)
 
     def reverse(self) -> Thick:
         """Because the Thick is required to have exactly one
-        instance of each value, it is easy to create a \"reversed\"
+        instance of each value, it is easy to create a "reversed"
         Thick, where the values become keys, and keys values
         """
         new: Thick = Thick()
         key: ThickKey
         value: Any
         for key, value in self.items():
             new[value] = key
 
         return new
 
-    def get_dict(self) -> dict[Any, Any]:
-        """Get something like the underlying dict of the Thick,
-        though cast any ThickKey items to tuples."""
-        return_dict: dict[Any, Any] = {}
+    def thin(self) -> dict[Any, Any]:
+        """Get the "thin" (i.e., not Thick) dictionary from the Thick. In essence, this "reduplicates" the dictionary."""
+        thin_dict: dict[Any, Any] = {}
         for key, value in self.items():
-            if len(key) > 1:
-                return_dict[tuple(key)] = value
-            else:
-                return_dict[tuple(key)[0]] = value
+            for k in key:
+                thin_dict[k] = value
 
-        return return_dict
+        return thin_dict
 
     def values(self) -> ThickValuesView:
         return ThickValuesView(self)
 
     def keys(self) -> ThickKeysView:
         return ThickKeysView(self)
```

### Comparing `thick-0.0.4/src/thick.egg-info/PKG-INFO` & `thick-0.0.5/src/thick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thick
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python dictionary that gets Thicker rather than longer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -699,25 +699,27 @@
 
 ```py
 foo = {
     "a": ComplexObjectName1,
     "b": ComplexObjectName2,
     "c": ComplexObjectName1,
     ...
-}```
+}
+```
 
 In this case, typing out such a dictionary, especially one with more entries, violates the DRY principle (a personal favorite) and can be quite error-prone.
 
 Perhaps you would try to map a tuple of key to a value:
 ```py
 foo = {
     ("a", "c", ...): ComplexObjectName1,
     ("b", ...): ComplexObjectName2,
     ...
-}```
+}
+```
 
 But, obviously, this breaks on a call like:
 ```py
 "a" in foo
 ```
 
 Enter the Thick dict. Given an iterible (but not a string) of keys, or multiple keys mapped to one value, the Thick automatically deduplicates values, and uses set logic to determine if a given key is a subset of any key.
@@ -790,12 +792,34 @@
 2 in my_thick
 True
 
 2 in my_thick_iterable_key
 False
 ```
 
+### But I just want the normal dictionary!
+Good news! You can use the more-simple, D.R.Y. method for construction, and then get the desired dict directly out!
+```py
+my_thick = Thick({
+    ("a", "b", "c"): foo,
+    ("d", "e", "f"): bar,
+    ...
+    })
+
+normal_dict = my_thick.thin()
+{
+    "a": foo,
+    "b": foo,
+    "c": foo,
+    "d": bar,
+    "e": bar,
+    "f": bar,
+    ...
+}
+```
+
+
 ## Is this really worth it?
 
 Probably not! I intend to use this in a few of my other personal projects, but I also wanted some more experiencing putting up a pip/PyPI package, and I thought the name was fun (and a little risque, to be fair).
 
 I don't expect anyone else to use this, but, if it does end up being useful, please let me know! If you find any bugs or have any feature requests, please create a GitHub issue!
```

