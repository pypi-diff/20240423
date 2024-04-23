# Comparing `tmp/types-boltons-23.1.0.20240331.tar.gz` & `tmp/types-boltons-24.0.0.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-boltons-23.1.0.20240331.tar", last modified: Sun Mar 31 02:17:56 2024, max compression
+gzip compressed data, was "types-boltons-24.0.0.20240423.tar", last modified: Tue Apr 23 02:19:25 2024, max compression
```

## Comparing `types-boltons-23.1.0.20240331.tar` & `types-boltons-24.0.0.20240423.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:56.019530 types-boltons-23.1.0.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-31 02:17:56.019530 types-boltons-23.1.0.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:56.015530 types-boltons-23.1.0.20240331/boltons-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/boltons-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/cacheutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/debugutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/deprutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/dictutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/easterutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/ecoutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/excutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/fileutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/formatutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/funcutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/gcutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/ioutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/iterutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/jsonutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/listutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/mathutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/mboxutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/namedutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/pathutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/boltons-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/queueutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/setutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/socketutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/statsutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/strutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/tableutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/tbutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/timeutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/typeutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-31 02:17:27.000000 types-boltons-23.1.0.20240331/boltons-stubs/urlutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:17:56.019530 types-boltons-23.1.0.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:56.019530 types-boltons-23.1.0.20240331/types_boltons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/types_boltons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/types_boltons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/types_boltons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-31 02:17:55.000000 types-boltons-23.1.0.20240331/types_boltons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:25.076461 types-boltons-24.0.0.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 02:19:24.000000 types-boltons-24.0.0.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:24.000000 types-boltons-24.0.0.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:19:25.076461 types-boltons-24.0.0.20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:25.076461 types-boltons-24.0.0.20240423/boltons-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 02:19:24.000000 types-boltons-24.0.0.20240423/boltons-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/cacheutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/debugutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/deprutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/dictutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/easterutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/ecoutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/excutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/fileutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/formatutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/funcutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/gcutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/ioutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/iterutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/jsonutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/listutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/mathutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/mboxutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/namedutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/pathutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:24.000000 types-boltons-24.0.0.20240423/boltons-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/queueutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/setutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/socketutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/statsutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/strutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/tableutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/tbutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/timeutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/typeutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-23 02:18:48.000000 types-boltons-24.0.0.20240423/boltons-stubs/urlutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:25.076461 types-boltons-24.0.0.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-23 02:19:24.000000 types-boltons-24.0.0.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:25.076461 types-boltons-24.0.0.20240423/types_boltons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:19:25.000000 types-boltons-24.0.0.20240423/types_boltons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 02:19:25.000000 types-boltons-24.0.0.20240423/types_boltons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:25.000000 types-boltons-24.0.0.20240423/types_boltons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 02:19:25.000000 types-boltons-24.0.0.20240423/types_boltons.egg-info/top_level.txt
```

### Comparing `types-boltons-23.1.0.20240331/CHANGELOG.md` & `types-boltons-24.0.0.20240423/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 24.0.0.20240423 (2024-04-23)
+
+Bump boltons to 24.0.* (#11804)
+
 ## 23.1.0.20240331 (2024-03-31)
 
 Remove bare Incomplete annotations in third-party stubs (#11671)
 
 ## 23.1.0.20240310 (2024-03-10)
 
 Bump mypy to 1.9, add to json.encoder, small fixups (#11549)
```

### Comparing `types-boltons-23.1.0.20240331/PKG-INFO` & `types-boltons-24.0.0.20240423/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-boltons
-Version: 23.1.0.20240331
+Version: 24.0.0.20240423
 Summary: Typing stubs for boltons
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boltons.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `boltons`.
 
 This version of `types-boltons` aims to provide accurate annotations
-for `boltons==23.1.*`.
+for `boltons==24.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/boltons. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/cacheutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/cacheutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/dictutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/dictutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/ecoutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/ecoutils.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any
 
 ECO_VERSION: str
-PY_GT_2: bool
 HAVE_URANDOM: bool
 INSTANCE_ID: str
 IS_64BIT: bool
 HAVE_UCS4: bool
 HAVE_READLINE: bool
 SQLITE_VERSION: str
 OPENSSL_VERSION: str
```

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/fileutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/fileutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/formatutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/formatutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/funcutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/funcutils.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 import functools
 from _typeshed import Incomplete
 from functools import total_ordering as total_ordering
 
 NO_DEFAULT: Incomplete
 
+def inspect_formatargspec(
+    args,
+    varargs=None,
+    varkw=None,
+    defaults=None,
+    kwonlyargs=(),
+    kwonlydefaults={},
+    annotations={},
+    formatarg=...,
+    formatvarargs=...,
+    formatvarkw=...,
+    formatvalue=...,
+    formatreturns=...,
+    formatannotation=...,
+): ...
 def get_module_callables(mod, ignore: Incomplete | None = None): ...
 def mro_items(type_obj): ...
 def dir_dict(obj, raise_exc: bool = False): ...
 def copy_function(orig, copy_dict: bool = True): ...
 def partial_ordering(cls): ...
 
 class InstancePartial(functools.partial[Incomplete]):
```

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/ioutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/ioutils.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import abc
 from _typeshed import Incomplete
 from abc import abstractmethod
 
-text_type = str
-binary_type = bytes
 READ_CHUNK_SIZE: int
 EINVAL: Incomplete
 
 class SpooledIOBase(metaclass=abc.ABCMeta):
     __metaclass__: Incomplete
     def __init__(self, max_size: int = 5000000, dir: Incomplete | None = None) -> None: ...
     @abstractmethod
```

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/iterutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/iterutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/jsonutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/jsonutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/listutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/listutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/mathutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/mathutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/setutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/setutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/socketutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/socketutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/statsutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/statsutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/strutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/strutils.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from collections.abc import Callable, Generator, Iterable
 from html.parser import HTMLParser
 from typing import Any, TypeVar
 
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 
-unichr = chr
-
 def camel2under(camel_string: str) -> str: ...
 def under2camel(under_string: str) -> str: ...
 def slugify(text: str, delim: str = "_", lower: bool = True, ascii: bool = False) -> str: ...
 def split_punct_ws(text: str) -> str: ...
 def unit_len(sized_iterable: Iterable[Any], unit_noun: str = "item") -> str: ...
 def ordinalize(number: int | str, ext_only: bool = False) -> str: ...
 def cardinalize(unit_noun: str, count: int) -> str: ...
@@ -45,20 +43,20 @@
 def indent(text: str, margin: str, newline: str = "\n", key: Callable[..., bool] = ...) -> str: ...
 def is_uuid(obj, version: int = 4) -> bool: ...
 def escape_shell_args(args: list[str], sep: str = " ", style: str | None = None) -> str: ...
 def args2sh(args: list[str], sep: str = " ") -> str: ...
 def args2cmd(args: list[str], sep: str = " ") -> str: ...
 def parse_int_list(range_string: str, delim: str = ",", range_delim: str = "-") -> list[int]: ...
 def format_int_list(int_list: list[int], delim: str = ",", range_delim: str = "-", delim_space: bool = False) -> str: ...
+def complement_int_list(
+    range_string: str, range_start: int = 0, range_end: int | None = None, delim: str = ",", range_delim: str = "-"
+) -> str: ...
+def int_ranges_from_int_list(range_string: str, delim: str = ",", range_delim: str = "-") -> tuple[int, int]: ...
 
 class MultiReplace:
     group_map: dict[str, str]
     combined_pattern: str
     def __init__(self, sub_map: dict[str, str], **kwargs) -> None: ...
     def sub(self, text: str) -> str: ...
 
 def multi_replace(text: str, sub_map: dict[str, str], **kwargs) -> str: ...
 def unwrap_text(text: str, ending: str = "\n\n") -> str: ...
-
-# Names in __all__ with no definition:
-#   int_list_complement
-#   int_list_to_int_tuples
```

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/tableutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/tableutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/tbutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/tbutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/timeutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/timeutils.pyi`

 * *Files identical despite different names*

### Comparing `types-boltons-23.1.0.20240331/boltons-stubs/urlutils.pyi` & `types-boltons-24.0.0.20240423/boltons-stubs/urlutils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -76,11 +76,13 @@
 PREV: Incomplete
 NEXT: Incomplete
 KEY: Incomplete
 VALUE: Incomplete
 SPREV: Incomplete
 SNEXT: Incomplete
 
+OMD = OrderedMultiDict
+
 class QueryParamDict(OrderedMultiDict[Incomplete, Incomplete]):
     @classmethod
     def from_text(cls, query_string): ...
     def to_text(self, full_quote: bool = False): ...
```

### Comparing `types-boltons-23.1.0.20240331/setup.py` & `types-boltons-24.0.0.20240423/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `boltons`.
 
 This version of `types-boltons` aims to provide accurate annotations
-for `boltons==23.1.*`.
+for `boltons==24.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/boltons. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="23.1.0.20240331",
+      version="24.0.0.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boltons.md",
```

### Comparing `types-boltons-23.1.0.20240331/types_boltons.egg-info/PKG-INFO` & `types-boltons-24.0.0.20240423/types_boltons.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-boltons
-Version: 23.1.0.20240331
+Version: 24.0.0.20240423
 Summary: Typing stubs for boltons
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/boltons.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `boltons`.
 
 This version of `types-boltons` aims to provide accurate annotations
-for `boltons==23.1.*`.
+for `boltons==24.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/boltons. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-boltons-23.1.0.20240331/types_boltons.egg-info/SOURCES.txt` & `types-boltons-24.0.0.20240423/types_boltons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

