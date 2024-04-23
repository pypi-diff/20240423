# Comparing `tmp/waylay_sdk_core-0.2.0.tar.gz` & `tmp/waylay_sdk_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_core-0.2.0.tar", last modified: Mon Apr 15 07:40:21 2024, max compression
+gzip compressed data, was "waylay_sdk_core-0.2.1.tar", last modified: Tue Apr 23 12:34:40 2024, max compression
```

## Comparing `waylay_sdk_core-0.2.0.tar` & `waylay_sdk_core-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.099580 waylay_sdk_core-0.2.0/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-03-26 14:02:35.000000 waylay_sdk_core-0.2.0/LICENSE.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     3967 2024-04-15 07:40:21.098954 waylay_sdk_core-0.2.0/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1710 2024-04-10 15:11:43.000000 waylay_sdk_core-0.2.0/README.md
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1541 2024-04-12 12:21:48.000000 waylay_sdk_core-0.2.0/pyproject.toml
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-15 07:40:21.099674 waylay_sdk_core-0.2.0/setup.cfg
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:20.999483 waylay_sdk_core-0.2.0/src/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:20.996684 waylay_sdk_core-0.2.0/src/waylay/
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.044374 waylay_sdk_core-0.2.0/src/waylay/sdk/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      754 2024-03-28 08:55:26.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       65 2024-04-12 12:21:48.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/_version.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.065377 waylay_sdk_core-0.2.0/src/waylay/sdk/api/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      661 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     6130 2024-04-11 14:02:19.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/_models.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4423 2024-04-10 15:17:36.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       40 2024-04-12 12:21:10.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/constants.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2298 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/exceptions.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2299 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/http.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    14116 2024-04-12 12:21:10.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/api/serialization.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.078570 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      523 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/exceptions.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     5972 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/interactive.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    11539 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/model.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/parse.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4243 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/auth/provider.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1880 2024-04-08 08:02:45.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/client.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.083365 waylay_sdk_core-0.2.0/src/waylay/sdk/config/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      341 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/config/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     3106 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/config/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)    13667 2024-03-08 11:24:03.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/config/model.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2809 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/exceptions.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.090961 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      229 2024-03-15 11:31:35.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/__init__.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4401 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/base.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2373 2024-03-21 16:22:46.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/client.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      206 2024-04-08 08:02:45.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/loader.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     2480 2024-03-28 11:04:55.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/type_stubs.py
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       80 2024-02-13 14:44:08.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/py.typed
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.092512 waylay_sdk_core-0.2.0/src/waylay/sdk/services/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     4887 2024-04-08 08:02:45.000000 waylay_sdk_core-0.2.0/src/waylay/sdk/services/gateway.py
-drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:40:21.097642 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     3967 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 simonschoonjans   (501) staff       (20)     1133 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)       64 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/entry_points.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)      365 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/requires.txt
--rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-04-15 07:40:20.000000 waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.241704 waylay_sdk_core-0.2.1/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-03-26 09:30:45.000000 waylay_sdk_core-0.2.1/LICENSE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     3967 2024-04-23 12:34:40.241327 waylay_sdk_core-0.2.1/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1710 2024-04-08 12:34:55.000000 waylay_sdk_core-0.2.1/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1541 2024-04-23 12:31:12.000000 waylay_sdk_core-0.2.1/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-23 12:34:40.241761 waylay_sdk_core-0.2.1/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.209468 waylay_sdk_core-0.2.1/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.208408 waylay_sdk_core-0.2.1/src/waylay/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.212743 waylay_sdk_core-0.2.1/src/waylay/sdk/
+-rw-r--r--   0 thomas     (502) staff       (20)      754 2024-03-27 11:50:39.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)       65 2024-04-23 12:31:08.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/_version.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.220746 waylay_sdk_core-0.2.1/src/waylay/sdk/api/
+-rw-r--r--   0 thomas     (502) staff       (20)      661 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     6901 2024-04-23 12:29:35.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/_models.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4423 2024-03-27 11:50:39.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/client.py
+-rw-r--r--   0 thomas     (502) staff       (20)       40 2024-04-16 11:19:13.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/constants.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2298 2024-03-15 07:16:26.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/exceptions.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2299 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/http.py
+-rw-r--r--   0 thomas     (502) staff       (20)    14265 2024-04-22 09:24:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/api/serialization.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.223438 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/
+-rw-r--r--   0 thomas     (502) staff       (20)      523 2024-03-14 11:07:10.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)      882 2024-03-14 10:54:52.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/exceptions.py
+-rw-r--r--   0 thomas     (502) staff       (20)     5972 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/interactive.py
+-rw-r--r--   0 thomas     (502) staff       (20)    11539 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/model.py
+-rw-r--r--   0 thomas     (502) staff       (20)      832 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/parse.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4243 2024-03-07 17:25:15.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/auth/provider.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1880 2024-04-08 09:44:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/client.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.228040 waylay_sdk_core-0.2.1/src/waylay/sdk/config/
+-rw-r--r--   0 thomas     (502) staff       (20)      341 2024-03-14 11:07:10.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/config/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     3106 2024-03-26 17:17:35.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/config/client.py
+-rw-r--r--   0 thomas     (502) staff       (20)    13577 2024-04-22 09:24:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/config/model.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2809 2024-03-15 07:16:26.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/exceptions.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.230028 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/
+-rw-r--r--   0 thomas     (502) staff       (20)      229 2024-03-14 11:07:10.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4401 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/base.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2373 2024-03-25 07:17:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/client.py
+-rw-r--r--   0 thomas     (502) staff       (20)      206 2024-04-08 09:44:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/loader.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2480 2024-04-08 09:44:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/type_stubs.py
+-rw-r--r--   0 thomas     (502) staff       (20)       80 2024-02-08 12:59:42.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/py.typed
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.233856 waylay_sdk_core-0.2.1/src/waylay/sdk/services/
+-rw-r--r--   0 thomas     (502) staff       (20)     4853 2024-04-22 09:24:30.000000 waylay_sdk_core-0.2.1/src/waylay/sdk/services/gateway.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-23 12:34:40.240311 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     3967 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1133 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       64 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      365 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        7 2024-04-23 12:34:40.000000 waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/top_level.txt
```

### Comparing `waylay_sdk_core-0.2.0/LICENSE.txt` & `waylay_sdk_core-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/PKG-INFO` & `waylay_sdk_core-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2020, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay_sdk_core-0.2.0/README.md` & `waylay_sdk_core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/pyproject.toml` & `waylay_sdk_core-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-core"
-version = "0.2.0"
+version = "0.2.1"
 description = "Waylay Python SDK."
 requires-python = ">=3.9"
 keywords = ["waylay", "sdk"]
 readme = "README.md"
 authors = [{name = "Waylay", email = "info@waylay.io"}]
 license={file = "LICENSE.txt"}
 dependencies = [
```

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/__init__.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/api/__init__.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/api/_models.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/api/_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 from abc import ABC
+import contextlib
+from copy import deepcopy
 from datetime import date, datetime
 from decimal import Decimal
 from inspect import isclass
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Union, get_type_hints
 
 from typing_extensions import (
     Annotated,  # >=3.9
@@ -62,15 +64,29 @@
             return handler(value)
         except ValidationError:
             context = info.context or {}
             if context.get("skip_validation", False):
                 model = cls.model_construct(**value)
                 if not model.model_fields_set:
                     raise
-                for field_name in model.model_fields_set:
+
+                # set missing fields to None
+                model_fields_set = deepcopy(model.model_fields_set)
+                model_fields_missing = [
+                    field_name
+                    for [field_name, field_info] in model.model_fields.items()
+                    if field_name not in model_fields_set and field_info.is_required()
+                ]
+                for field_name in model_fields_missing:
+                    with contextlib.suppress(ValueError, TypeError):
+                        setattr(model, field_name, None)
+
+                model.__pydantic_fields_set__ = model_fields_set
+                # recursively validate set fields
+                for field_name in model_fields_set:
                     field_value = getattr(model, field_name)
                     strict = (info.config or {}).get("strict")
                     try:
                         cls.__pydantic_validator__.validate_assignment(
                             model,
                             field_name,
                             field_value,
@@ -113,19 +129,19 @@
                     except ValidationError:
                         return value
             else:
                 raise
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert the model instance to dict."""
-        return self.model_dump()
+        return self.model_dump(by_alias=True, exclude_none=True)
 
     def to_json(self) -> str:
         """Convert the model instance to a JSON-encoded string."""
-        return self.model_dump_json()
+        return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
         """Create a model instance from a dict."""
         return cls.model_validate(obj)
 
     @classmethod
```

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/api/client.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/api/client.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/api/exceptions.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/api/http.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/api/http.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/api/serialization.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/api/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,22 +377,26 @@
         return return_data
 
 
 async def _iter_event_stream(
     response: Response,
     response_type: type[T],
     select_path: str = "",
+    *,
+    _ignore_retry_events: bool = True,
 ) -> AsyncIterator[T]:
     _response_type = _response_type_for_status_code(response.status_code, response_type)
     content_type = response.headers.get("content-type", "")
     try:
         async for event_str in __iter_events_response(response, content_type):
             event = __parse_event(event_str, content_type)
             if not event:
                 continue
+            if _ignore_retry_events and "retry" in event and len(event) == 1:
+                continue
             _deserialized_event = _deserialize(
                 _extract_selected(event, select_path), _response_type
             )
             yield _deserialized_event
     finally:
         await response.aclose()
```

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/__init__.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/exceptions.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/interactive.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/interactive.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/model.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/model.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/parse.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/parse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/auth/provider.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/auth/provider.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/client.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/client.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/config/client.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/config/client.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/config/model.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/config/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,14 @@
 
     profile: str
     _auth: WaylayTokenAuth
     _local_settings: Settings
     _tenant_settings: Optional[TenantSettings] = None
     _token_auth_provider: Type[WaylayTokenAuth] = WaylayTokenAuth
 
-    client_side_validation: bool = True
-    """Enable/disable client side validation."""
-
     def __init__(
         self,
         credentials: Optional[WaylayCredentials] = None,
         profile: str = DEFAULT_PROFILE,
         settings: Optional[TenantSettings] = None,
         fetch_tenant_settings=True,
         credentials_callback: Optional[CredentialsCallback] = None,
```

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/exceptions.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/base.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/base.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/client.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/client.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/plugin/type_stubs.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/plugin/type_stubs.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_core-0.2.0/src/waylay/sdk/services/gateway.py` & `waylay_sdk_core-0.2.1/src/waylay/sdk/services/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,11 +150,10 @@
 
     name: str
     version: str
     health: str
 
     model_config = ConfigDict(
         populate_by_name=True,
-        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
     )
```

### Comparing `waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/PKG-INFO` & `waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2020, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay_sdk_core-0.2.0/src/waylay_sdk_core.egg-info/SOURCES.txt` & `waylay_sdk_core-0.2.1/src/waylay_sdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

