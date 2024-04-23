# Comparing `tmp/mo_dots-9.595.24112.tar.gz` & `tmp/mo_dots-9.596.24113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_dots-9.595.24112.tar", last modified: Sun Apr 21 16:31:48 2024, max compression
+gzip compressed data, was "mo_dots-9.596.24113.tar", last modified: Mon Apr 22 09:12:28 2024, max compression
```

## Comparing `mo_dots-9.595.24112.tar` & `mo_dots-9.596.24113.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 16:31:48.671260 mo_dots-9.595.24112/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.595.24112/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-21 16:31:48.671260 mo_dots-9.595.24112/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.595.24112/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 16:31:48.658317 mo_dots-9.595.24112/mo_dots/
--rw-rw-rw-   0        0        0    13958 2024-04-21 16:31:40.000000 mo_dots-9.595.24112/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16450 2024-04-21 16:31:40.000000 mo_dots-9.595.24112/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4283 2024-04-21 15:00:21.000000 mo_dots-9.595.24112/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10399 2024-04-21 15:00:21.000000 mo_dots-9.595.24112/mo_dots/lists.py
--rw-rw-rw-   0        0        0     6663 2024-04-21 15:00:21.000000 mo_dots-9.595.24112/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5357 2024-04-21 16:31:40.000000 mo_dots-9.595.24112/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1423 2024-04-21 15:00:21.000000 mo_dots-9.595.24112/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:31:48.668743 mo_dots-9.595.24112/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-21 16:31:48.000000 mo_dots-9.595.24112/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-21 16:31:48.000000 mo_dots-9.595.24112/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 16:31:48.000000 mo_dots-9.595.24112/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.595.24112/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-21 16:31:48.000000 mo_dots-9.595.24112/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 16:31:48.000000 mo_dots-9.595.24112/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 16:31:48.671260 mo_dots-9.595.24112/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-21 16:31:43.000000 mo_dots-9.595.24112/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:12:28.106238 mo_dots-9.596.24113/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.596.24113/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-22 09:12:28.105238 mo_dots-9.596.24113/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.596.24113/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 09:12:28.090130 mo_dots-9.596.24113/mo_dots/
+-rw-rw-rw-   0        0        0    14004 2024-04-22 09:12:18.000000 mo_dots-9.596.24113/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16471 2024-04-22 09:12:18.000000 mo_dots-9.596.24113/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4283 2024-04-21 15:00:21.000000 mo_dots-9.596.24113/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10399 2024-04-21 15:00:21.000000 mo_dots-9.596.24113/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     6663 2024-04-21 15:00:21.000000 mo_dots-9.596.24113/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5357 2024-04-21 16:31:40.000000 mo_dots-9.596.24113/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1423 2024-04-21 15:00:21.000000 mo_dots-9.596.24113/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:12:28.101793 mo_dots-9.596.24113/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-22 09:12:28.000000 mo_dots-9.596.24113/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-22 09:12:28.000000 mo_dots-9.596.24113/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 09:12:28.000000 mo_dots-9.596.24113/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.596.24113/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-22 09:12:28.000000 mo_dots-9.596.24113/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 09:12:28.000000 mo_dots-9.596.24113/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 09:12:28.106238 mo_dots-9.596.24113/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-22 09:12:22.000000 mo_dots-9.596.24113/setup.py
```

### Comparing `mo_dots-9.595.24112/LICENSE` & `mo_dots-9.596.24113/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/PKG-INFO` & `mo_dots-9.596.24113/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.595.24112
+Version: 9.596.24113
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.595.24112/README.md` & `mo_dots-9.596.24113/README.md`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/mo_dots/__init__.py` & `mo_dots-9.596.24113/mo_dots/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "is_container",
     "is_data",
     "is_list",
     "is_many",
     "is_missing",
     "is_not_null",
     "is_null",
+    "is_primitive",
     "is_sequence",
     "join_field",
     "last",
     "leaves",
     "leaves_to_data",
     "list_to_data",
     "listwrap",
@@ -51,14 +52,15 @@
     "Null",
     "NullType",
     "object_to_data",
     "PATH_NOT_FOUND",
     "relative_field",
     "register_data",
     "register_many",
+    "register_primitive",
     "set_attr",
     "set_default",
     "split_field",
     "startswith_field",
     "tail_field",
     "to_data",
     "tuplewrap",
```

### Comparing `mo_dots-9.595.24112/mo_dots/datas.py` & `mo_dots-9.596.24113/mo_dots/datas.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 _get = object.__getattribute__
 _set = object.__setattr__
 _new = object.__new__
 
 DEBUG = False
 
 
-
 class Data(object):
     """
     Please see https://github.com/klahnakoski/mo-dots/tree/dev/docs#data-replaces-pythons-dict
     """
 
     __slots__ = [SLOT]
 
@@ -632,13 +631,16 @@
     if hasattr(value, "__iter__"):
         return [_leaves_to_data(v) for v in value]
 
     return value
 
 
 _primitive_types = (str, bytes, int, float, bool, Decimal, datetime, date, time, timedelta)
-_other_primitives = ("Date",)
+
 
 def is_primitive(value):
-    if isinstance(value, _primitive_types):
-        return True
-    return value.__class__.__name__ in _other_primitives
+    return isinstance(value, _primitive_types)
+
+
+def register_primitive(_type):
+    global _primitive_types
+    _primitive_types = tuple(set(_primitive_types + (_type,)))
```

### Comparing `mo_dots-9.595.24112/mo_dots/fields.py` & `mo_dots-9.596.24113/mo_dots/fields.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/mo_dots/lists.py` & `mo_dots-9.596.24113/mo_dots/lists.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/mo_dots/nones.py` & `mo_dots-9.596.24113/mo_dots/nones.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/mo_dots/objects.py` & `mo_dots-9.596.24113/mo_dots/objects.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/mo_dots/utils.py` & `mo_dots-9.596.24113/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.595.24112/mo_dots.egg-info/PKG-INFO` & `mo_dots-9.596.24113/mo_dots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.595.24112
+Version: 9.596.24113
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.595.24112/setup.py` & `mo_dots-9.596.24113/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.595.24112',
+    version='9.596.24113',
     zip_safe=False
 )
```

