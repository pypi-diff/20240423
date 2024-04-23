# Comparing `tmp/pydantic_changedetect-0.6.7.tar.gz` & `tmp/pydantic_changedetect-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_changedetect-0.6.7.tar", max compression
+gzip compressed data, was "pydantic_changedetect-0.7.0.tar", max compression
```

## Comparing `pydantic_changedetect-0.6.7.tar` & `pydantic_changedetect-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/LICENSE
--rw-r--r--   0        0        0     5584 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/README.md
--rw-r--r--   0        0        0       71 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/_compat.py
--rw-r--r--   0        0        0    31972 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/changedetect.py
--rw-r--r--   0        0        0        0 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/py.typed
--rw-r--r--   0        0        0     2654 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/utils.py
--rw-r--r--   0        0        0     1052 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     6402 1970-01-01 00:00:00.000000 pydantic_changedetect-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-23 16:57:04.283765 pydantic_changedetect-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5584 2024-04-23 16:57:04.283765 pydantic_changedetect-0.7.0/README.md
+-rw-r--r--   0        0        0       71 2024-04-23 16:57:04.283765 pydantic_changedetect-0.7.0/pydantic_changedetect/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-23 16:57:04.283765 pydantic_changedetect-0.7.0/pydantic_changedetect/_compat.py
+-rw-r--r--   0        0        0    32782 2024-04-23 16:57:04.287766 pydantic_changedetect-0.7.0/pydantic_changedetect/changedetect.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:57:04.287766 pydantic_changedetect-0.7.0/pydantic_changedetect/py.typed
+-rw-r--r--   0        0        0     2654 2024-04-23 16:57:04.287766 pydantic_changedetect-0.7.0/pydantic_changedetect/utils.py
+-rw-r--r--   0        0        0     1052 2024-04-23 16:57:04.287766 pydantic_changedetect-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6402 1970-01-01 00:00:00.000000 pydantic_changedetect-0.7.0/PKG-INFO
```

### Comparing `pydantic_changedetect-0.6.7/LICENSE` & `pydantic_changedetect-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.7/README.md` & `pydantic_changedetect-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.7/pydantic_changedetect/_compat.py` & `pydantic_changedetect-0.7.0/pydantic_changedetect/_compat.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.7/pydantic_changedetect/changedetect.py` & `pydantic_changedetect-0.7.0/pydantic_changedetect/changedetect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import decimal
 import warnings
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -28,14 +29,22 @@
         from pydantic.typing import DictStrAny, SetStr
     if PYDANTIC_V2:
         from pydantic.main import IncEx
 
     Model = TypeVar("Model", bound="ChangeDetectionMixin")
 
 NO_VALUE = object()
+COMPARABLE_TYPES = (
+    str,
+    int, float,
+    bool,
+    decimal.Decimal,
+    datetime.datetime, datetime.date, datetime.time, datetime.timedelta,
+    pydantic.BaseModel,
+)
 
 
 class ChangeDetectionMixin(pydantic.BaseModel):
     """
     Utility mixin to allow pydantic models to detect changes to fields.
 
     Example:
@@ -217,19 +226,38 @@
             if original is NO_VALUE:
                 self.model_original[name] = self.__dict__[name]
             else:
                 self.model_original[name] = original
             self.model_self_changed_fields.add(name)
 
     def _model_value_is_comparable_type(self, value: Any) -> bool:
+        if isinstance(value, (list, set, tuple)):
+            return all(
+                self._model_value_is_comparable_type(i)
+                for i
+                in value
+            )
+        elif isinstance(value, dict):
+            return all(
+                (
+                    self._model_value_is_comparable_type(k)
+                    and self._model_value_is_comparable_type(v)
+                )
+                for k, v
+                in value.items()
+            )
+
         return (
             value is None
-            or isinstance(value, (str, int, float, bool, decimal.Decimal))
+            or isinstance(value, COMPARABLE_TYPES)
         )
 
+    def _model_value_is_actually_unchanged(self, value1: Any, value2: Any) -> bool:
+        return value1 == value2
+
     @no_type_check
     def __setattr__(self, name, value) -> None:  # noqa: ANN001
         self_compat = PydanticCompat(self)
 
         # Private attributes need not to be handled
         if (
             self.__private_attributes__  # may be None
@@ -253,15 +281,15 @@
             original_value = original_update.get(name, None)
             # Don't use value parameter directly, as pydantic validation might have changed it
             # (when validate_assignment == True)
             current_value = self.__dict__[name]
             if (
                 self._model_value_is_comparable_type(original_value)
                 and self._model_value_is_comparable_type(current_value)
-                and original_value == current_value
+                and self._model_value_is_actually_unchanged(original_value, current_value)
             ):
                 has_changed = False
 
         # Store changed state
         if has_changed:
             self.model_original.update(original_update)
             self.model_self_changed_fields.add(name)
```

### Comparing `pydantic_changedetect-0.6.7/pydantic_changedetect/utils.py` & `pydantic_changedetect-0.7.0/pydantic_changedetect/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.7/pyproject.toml` & `pydantic_changedetect-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pydantic-changedetect"
-version = "0.6.7"
+version = "0.7.0"
 description = "Extend pydantic models to also detect and record changes made to the model attributes."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-changedetect"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = ">=1.9.0,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2,<9.0.0"
 pytest-cov = ">=3,<6"
 tox = ">=3.26,<5.0"
-ruff = ">=0.2.0,<0.4.0"
+ruff = ">=0.2.0,<0.5.0"
 pyright = ">=1.1.350,<1.2"
 
 [tool.ruff]
 line-length = 115
 target-version = "py38"
 output-format = "grouped"
```

### Comparing `pydantic_changedetect-0.6.7/PKG-INFO` & `pydantic_changedetect-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-changedetect
-Version: 0.6.7
+Version: 0.7.0
 Summary: Extend pydantic models to also detect and record changes made to the model attributes.
 Home-page: https://github.com/team23/pydantic-changedetect
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

