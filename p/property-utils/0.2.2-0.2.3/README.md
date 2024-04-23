# Comparing `tmp/property_utils-0.2.2.tar.gz` & `tmp/property_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property_utils-0.2.2.tar", last modified: Mon Apr 22 06:48:25 2024, max compression
+gzip compressed data, was "property_utils-0.2.3.tar", last modified: Tue Apr 23 06:52:42 2024, max compression
```

## Comparing `property_utils-0.2.2.tar` & `property_utils-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.523544 property_utils-0.2.2/
--rw-r--r--   0 max       (1000) max       (1000)     1076 2024-03-28 17:51:01.000000 property_utils-0.2.2/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-22 06:48:25.523544 property_utils-0.2.2/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     2907 2024-04-09 14:48:45.000000 property_utils-0.2.2/README.md
--rw-r--r--   0 max       (1000) max       (1000)     1594 2024-04-22 06:47:39.000000 property_utils-0.2.2/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-22 06:48:25.523544 property_utils-0.2.2/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.516877 property_utils-0.2.2/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.516877 property_utils-0.2.2/src/property_utils/
--rw-r--r--   0 max       (1000) max       (1000)        0 2024-03-28 17:51:01.000000 property_utils-0.2.2/src/property_utils/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.520211 property_utils-0.2.2/src/property_utils/constants/
--rw-r--r--   0 max       (1000) max       (1000)       49 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/constants/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      898 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/constants/constants.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.520211 property_utils-0.2.2/src/property_utils/exceptions/
--rw-r--r--   0 max       (1000) max       (1000)      142 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/exceptions/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      524 2024-03-28 17:51:01.000000 property_utils-0.2.2/src/property_utils/exceptions/base.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.520211 property_utils-0.2.2/src/property_utils/exceptions/properties/
--rw-r--r--   0 max       (1000) max       (1000)      185 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/exceptions/properties/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      641 2024-03-28 17:51:01.000000 property_utils-0.2.2/src/property_utils/exceptions/properties/property.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.520211 property_utils-0.2.2/src/property_utils/exceptions/units/
--rw-r--r--   0 max       (1000) max       (1000)      364 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/exceptions/units/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      866 2024-04-06 06:13:47.000000 property_utils-0.2.2/src/property_utils/exceptions/units/converter_types.py
--rw-r--r--   0 max       (1000) max       (1000)      479 2024-03-28 17:51:01.000000 property_utils-0.2.2/src/property_utils/exceptions/units/descriptors.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.520211 property_utils-0.2.2/src/property_utils/properties/
--rw-r--r--   0 max       (1000) max       (1000)      134 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/properties/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    28066 2024-04-09 14:48:45.000000 property_utils-0.2.2/src/property_utils/properties/property.py
--rw-r--r--   0 max       (1000) max       (1000)     2794 2024-04-08 14:48:05.000000 property_utils-0.2.2/src/property_utils/properties/validated_property.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2024-04-22 06:47:39.000000 property_utils-0.2.2/src/property_utils/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.523544 property_utils-0.2.2/src/property_utils/units/
--rw-r--r--   0 max       (1000) max       (1000)       43 2024-04-08 13:07:09.000000 property_utils-0.2.2/src/property_utils/units/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2939 2024-04-08 15:23:31.000000 property_utils-0.2.2/src/property_utils/units/aliases.py
--rw-r--r--   0 max       (1000) max       (1000)    33193 2024-04-08 14:48:05.000000 property_utils-0.2.2/src/property_utils/units/converter_types.py
--rw-r--r--   0 max       (1000) max       (1000)    12051 2024-04-08 14:48:05.000000 property_utils-0.2.2/src/property_utils/units/converters.py
--rw-r--r--   0 max       (1000) max       (1000)    67715 2024-04-08 14:48:05.000000 property_utils-0.2.2/src/property_utils/units/descriptors.py
--rw-r--r--   0 max       (1000) max       (1000)     4383 2024-04-08 15:28:32.000000 property_utils-0.2.2/src/property_utils/units/units.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-22 06:48:25.523544 property_utils-0.2.2/src/property_utils.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-22 06:48:25.000000 property_utils-0.2.2/src/property_utils.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1089 2024-04-22 06:48:25.000000 property_utils-0.2.2/src/property_utils.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-22 06:48:25.000000 property_utils-0.2.2/src/property_utils.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       51 2024-04-22 06:48:25.000000 property_utils-0.2.2/src/property_utils.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)       15 2024-04-22 06:48:25.000000 property_utils-0.2.2/src/property_utils.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.799153 property_utils-0.2.3/
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2024-03-28 17:51:01.000000 property_utils-0.2.3/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-23 06:52:42.799153 property_utils-0.2.3/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2907 2024-04-09 14:48:45.000000 property_utils-0.2.3/README.md
+-rw-r--r--   0 max       (1000) max       (1000)     1594 2024-04-23 06:52:17.000000 property_utils-0.2.3/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-23 06:52:42.799153 property_utils-0.2.3/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.789153 property_utils-0.2.3/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.792486 property_utils-0.2.3/src/property_utils/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.792486 property_utils-0.2.3/src/property_utils/constants/
+-rw-r--r--   0 max       (1000) max       (1000)       49 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/constants/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      898 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/constants/constants.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/exceptions/
+-rw-r--r--   0 max       (1000) max       (1000)      142 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/exceptions/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      524 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/exceptions/base.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/exceptions/properties/
+-rw-r--r--   0 max       (1000) max       (1000)      185 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/exceptions/properties/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      641 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/exceptions/properties/property.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/exceptions/units/
+-rw-r--r--   0 max       (1000) max       (1000)      364 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/exceptions/units/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      866 2024-04-06 06:13:47.000000 property_utils-0.2.3/src/property_utils/exceptions/units/converter_types.py
+-rw-r--r--   0 max       (1000) max       (1000)      479 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/exceptions/units/descriptors.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/properties/
+-rw-r--r--   0 max       (1000) max       (1000)      134 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/properties/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    28066 2024-04-09 14:48:45.000000 property_utils-0.2.3/src/property_utils/properties/property.py
+-rw-r--r--   0 max       (1000) max       (1000)     2683 2024-04-23 06:52:05.000000 property_utils-0.2.3/src/property_utils/properties/validated_property.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2024-04-22 06:47:39.000000 property_utils-0.2.3/src/property_utils/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.799153 property_utils-0.2.3/src/property_utils/units/
+-rw-r--r--   0 max       (1000) max       (1000)       43 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/units/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2939 2024-04-08 15:23:31.000000 property_utils-0.2.3/src/property_utils/units/aliases.py
+-rw-r--r--   0 max       (1000) max       (1000)    33193 2024-04-08 14:48:05.000000 property_utils-0.2.3/src/property_utils/units/converter_types.py
+-rw-r--r--   0 max       (1000) max       (1000)    12051 2024-04-08 14:48:05.000000 property_utils-0.2.3/src/property_utils/units/converters.py
+-rw-r--r--   0 max       (1000) max       (1000)    67715 2024-04-08 14:48:05.000000 property_utils-0.2.3/src/property_utils/units/descriptors.py
+-rw-r--r--   0 max       (1000) max       (1000)     4383 2024-04-08 15:28:32.000000 property_utils-0.2.3/src/property_utils/units/units.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.799153 property_utils-0.2.3/src/property_utils.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1089 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       51 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       15 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/top_level.txt
```

### Comparing `property_utils-0.2.2/LICENSE` & `property_utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/PKG-INFO` & `property_utils-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utilities for programming that involves physical properties
 Author-email: Maximos Nikiforakis <nikiforos@live.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/Maxcode123/property-utils
 Project-URL: Issues, https://github.com/Maxcode123/property-utils/issues
 Keywords: physical properties,properties
 Classifier: Programming Language :: Python
```

### Comparing `property_utils-0.2.2/README.md` & `property_utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/pyproject.toml` & `property_utils-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-utils"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name="Maximos Nikiforakis", email="nikiforos@live.co.uk" },
 ]
 description = "Utilities for programming that involves physical properties"
 keywords = ["physical properties", "properties"]
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `property_utils-0.2.2/src/property_utils/constants/constants.py` & `property_utils-0.2.3/src/property_utils/constants/constants.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/exceptions/base.py` & `property_utils-0.2.3/src/property_utils/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/exceptions/properties/property.py` & `property_utils-0.2.3/src/property_utils/exceptions/properties/property.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/exceptions/units/converter_types.py` & `property_utils-0.2.3/src/property_utils/exceptions/units/converter_types.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/properties/property.py` & `property_utils-0.2.3/src/property_utils/properties/property.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/properties/validated_property.py` & `property_utils-0.2.3/src/property_utils/properties/validated_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, ClassVar, Optional
+from typing import ClassVar, Optional
 from abc import abstractmethod
 
 from property_utils.units.descriptors import UnitDescriptor, GenericUnitDescriptor
 from property_utils.properties.property import Property
 from property_utils.exceptions.properties.property import PropertyValidationError
 
 
@@ -46,25 +46,24 @@
 
         super().__init__(value, unit)
         if not unit.isinstance(self.generic_unit_descriptor):
             raise PropertyValidationError(
                 f"cannot create {self.__class__.__name__} with {unit} units; "
                 f"expected {self.generic_unit_descriptor} units. "
             )
-        self.validate_value(value)
+
+        self.__post_init__()
+
+    def __post_init__(self) -> None:
+        self.validate_value(self.value)
 
     @abstractmethod
     def validate_value(self, value: float) -> None:
         """
         Validate the `value` for this property. This validation takes place after
         initialization; hence all initialized attributes are available.
 
         The only exception this method should raise is `PropertyValidationError`.
         """
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.value} {self.unit}>"
-
-    def __setattr__(self, __name: str, __value: Any) -> None:
-        if __name == "value":
-            self.validate_value(__value)
-        super().__setattr__(__name, __value)
```

### Comparing `property_utils-0.2.2/src/property_utils/units/aliases.py` & `property_utils-0.2.3/src/property_utils/units/aliases.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/units/converter_types.py` & `property_utils-0.2.3/src/property_utils/units/converter_types.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/units/converters.py` & `property_utils-0.2.3/src/property_utils/units/converters.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/units/descriptors.py` & `property_utils-0.2.3/src/property_utils/units/descriptors.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils/units/units.py` & `property_utils-0.2.3/src/property_utils/units/units.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.2/src/property_utils.egg-info/PKG-INFO` & `property_utils-0.2.3/src/property_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utilities for programming that involves physical properties
 Author-email: Maximos Nikiforakis <nikiforos@live.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/Maxcode123/property-utils
 Project-URL: Issues, https://github.com/Maxcode123/property-utils/issues
 Keywords: physical properties,properties
 Classifier: Programming Language :: Python
```

### Comparing `property_utils-0.2.2/src/property_utils.egg-info/SOURCES.txt` & `property_utils-0.2.3/src/property_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

