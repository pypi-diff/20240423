# Comparing `tmp/pygrocy-2.0.0.tar.gz` & `tmp/pygrocy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrocy-2.0.0.tar", last modified: Thu Aug 17 12:43:35 2023, max compression
+gzip compressed data, was "pygrocy-2.1.0.tar", last modified: Tue Apr 23 12:42:46 2024, max compression
```

## Comparing `pygrocy-2.0.0.tar` & `pygrocy-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-17 12:43:35.244207 pygrocy-2.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-08-17 12:41:52.000000 pygrocy-2.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2023-08-17 12:43:35.244207 pygrocy-2.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-08-17 12:41:52.000000 pygrocy-2.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-17 12:43:35.236206 pygrocy-2.0.0/pygrocy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      202 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      424 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-17 12:43:35.240206 pygrocy-2.0.0/pygrocy/data_models/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2900 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/battery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4724 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/chore.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      814 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/generic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3755 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/meal_items.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6846 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/product.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3237 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2426 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/task.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      747 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/data_models/user.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-17 12:43:35.240206 pygrocy-2.0.0/pygrocy/errors/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/errors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      670 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/errors/grocy_error.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14137 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/grocy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26080 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/grocy_api_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1015 2023-08-17 12:41:52.000000 pygrocy-2.0.0/pygrocy/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-17 12:43:35.240206 pygrocy-2.0.0/pygrocy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2023-08-17 12:43:35.000000 pygrocy-2.0.0/pygrocy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1017 2023-08-17 12:43:35.000000 pygrocy-2.0.0/pygrocy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-08-17 12:43:35.000000 pygrocy-2.0.0/pygrocy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2023-08-17 12:43:35.000000 pygrocy-2.0.0/pygrocy.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2023-08-17 12:43:35.000000 pygrocy-2.0.0/pygrocy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-08-17 12:43:35.244207 pygrocy-2.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2023-08-17 12:41:52.000000 pygrocy-2.0.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-17 12:43:35.244207 pygrocy-2.0.0/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2066 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_battery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3017 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_chores.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2546 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_generic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13057 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_grocy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_grocy_api_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2668 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_meal_plan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1335 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_meal_plan_sections.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_product.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1338 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_product_groups.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2842 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_shoppinglist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_stock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1746 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1952 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      529 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_users.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2722 2023-08-17 12:41:52.000000 pygrocy-2.0.0/test/test_utils.py
+drwxr-xr-x   0 sebastian  (1000) users      (100)        0 2024-04-23 12:42:46.520793 pygrocy-2.1.0/
+-rw-r--r--   0 sebastian  (1000) users      (100)     1075 2024-04-23 12:01:08.000000 pygrocy-2.1.0/LICENSE
+-rw-r--r--   0 sebastian  (1000) users      (100)     2350 2024-04-23 12:42:46.520793 pygrocy-2.1.0/PKG-INFO
+-rw-r--r--   0 sebastian  (1000) users      (100)     1806 2024-04-23 12:15:11.000000 pygrocy-2.1.0/README.md
+drwxr-xr-x   0 sebastian  (1000) users      (100)        0 2024-04-23 12:42:46.517792 pygrocy-2.1.0/pygrocy/
+-rw-r--r--   0 sebastian  (1000) users      (100)      202 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/__init__.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      424 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/base.py
+drwxr-xr-x   0 sebastian  (1000) users      (100)        0 2024-04-23 12:42:46.518792 pygrocy-2.1.0/pygrocy/data_models/
+-rw-r--r--   0 sebastian  (1000) users      (100)        0 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/__init__.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2900 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/battery.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     4724 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/chore.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      814 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/generic.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     3755 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/meal_items.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     7007 2024-04-23 12:15:11.000000 pygrocy-2.1.0/pygrocy/data_models/product.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     3237 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/system.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2426 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/task.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      747 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/data_models/user.py
+drwxr-xr-x   0 sebastian  (1000) users      (100)        0 2024-04-23 12:42:46.519793 pygrocy-2.1.0/pygrocy/errors/
+-rw-r--r--   0 sebastian  (1000) users      (100)       50 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/errors/__init__.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      670 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/errors/grocy_error.py
+-rw-r--r--   0 sebastian  (1000) users      (100)    14143 2024-04-23 12:15:11.000000 pygrocy-2.1.0/pygrocy/grocy.py
+-rw-r--r--   0 sebastian  (1000) users      (100)    26132 2024-04-23 12:15:11.000000 pygrocy-2.1.0/pygrocy/grocy_api_client.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     1015 2024-04-23 12:01:08.000000 pygrocy-2.1.0/pygrocy/utils.py
+drwxr-xr-x   0 sebastian  (1000) users      (100)        0 2024-04-23 12:42:46.520793 pygrocy-2.1.0/pygrocy.egg-info/
+-rw-r--r--   0 sebastian  (1000) users      (100)     2350 2024-04-23 12:42:46.000000 pygrocy-2.1.0/pygrocy.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian  (1000) users      (100)     1017 2024-04-23 12:42:46.000000 pygrocy-2.1.0/pygrocy.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian  (1000) users      (100)        1 2024-04-23 12:42:46.000000 pygrocy-2.1.0/pygrocy.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian  (1000) users      (100)       98 2024-04-23 12:42:46.000000 pygrocy-2.1.0/pygrocy.egg-info/requires.txt
+-rw-r--r--   0 sebastian  (1000) users      (100)       13 2024-04-23 12:42:46.000000 pygrocy-2.1.0/pygrocy.egg-info/top_level.txt
+-rw-r--r--   0 sebastian  (1000) users      (100)       38 2024-04-23 12:42:46.520793 pygrocy-2.1.0/setup.cfg
+-rw-r--r--   0 sebastian  (1000) users      (100)      844 2024-04-23 12:15:20.000000 pygrocy-2.1.0/setup.py
+drwxr-xr-x   0 sebastian  (1000) users      (100)        0 2024-04-23 12:42:46.520793 pygrocy-2.1.0/test/
+-rw-r--r--   0 sebastian  (1000) users      (100)        0 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/__init__.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      542 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/conftest.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2066 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_battery.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     3017 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_chores.py
+-rw-r--r--   0 sebastian  (1000) users      (100)       72 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_const.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2546 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_generic.py
+-rw-r--r--   0 sebastian  (1000) users      (100)    13057 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_grocy.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      902 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_grocy_api_client.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2668 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_meal_plan.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     1335 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_meal_plan_sections.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      449 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_misc.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2961 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_product.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     1338 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_product_groups.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2842 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_shoppinglist.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2197 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_stock.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     1746 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_system.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     1952 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_tasks.py
+-rw-r--r--   0 sebastian  (1000) users      (100)      529 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_users.py
+-rw-r--r--   0 sebastian  (1000) users      (100)     2722 2024-04-23 12:01:08.000000 pygrocy-2.1.0/test/test_utils.py
```

### Comparing `pygrocy-2.0.0/LICENSE` & `pygrocy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/PKG-INFO` & `pygrocy-2.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: pygrocy
-Version: 2.0.0
-Home-page: https://github.com/sebrut/pygrocy
-Author: Sebastian Rutofski
-Author-email: kontakt@sebastian-rutofski.de
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
+**This project is de-facto unmaintained as haven't been using grocy for a while. Feel free to fork and create pygrocy2!**
 
 # pygrocy
 [![Development Build Status](https://api.travis-ci.com/SebRut/pygrocy.svg?branch=develop)](https://travis-ci.com/SebRut/pygrocy)
 [![PyPI](https://img.shields.io/pypi/v/pygrocy.svg)](https://pypi.org/project/pygrocy/)
 ![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
 ![Grocy Version](https://img.shields.io/badge/grocy-3.1.0-yellow)
 [![Coverage Status](https://coveralls.io/repos/github/SebRut/pygrocy/badge.svg?branch=master)](https://coveralls.io/github/SebRut/pygrocy?branch=master)
```

### Comparing `pygrocy-2.0.0/pygrocy/data_models/battery.py` & `pygrocy-2.1.0/pygrocy/data_models/battery.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/data_models/chore.py` & `pygrocy-2.1.0/pygrocy/data_models/chore.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/data_models/generic.py` & `pygrocy-2.1.0/pygrocy/data_models/generic.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/data_models/meal_items.py` & `pygrocy-2.1.0/pygrocy/data_models/meal_items.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/data_models/product.py` & `pygrocy-2.1.0/pygrocy/data_models/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List
+from typing import List, Optional
 
 from pygrocy.base import DataModel
 from pygrocy.grocy_api_client import (
     CurrentStockResponse,
     GrocyApiClient,
     LocationData,
     MissingProductResponse,
@@ -15,19 +15,24 @@
     StockLogResponse,
 )
 
 
 class ProductBarcode(DataModel):
     def __init__(self, data: ProductBarcodeData):
         self._barcode = data.barcode
+        self._amount = float(data.amount) if data.amount else None
 
     @property
     def barcode(self) -> str:
         return self._barcode
 
+    @property
+    def amount(self) -> Optional[float]:
+        return self._amount
+
 
 class QuantityUnit(DataModel):
     def __init__(self, data: QuantityUnitData):
         self._id = data.id
         self._name = data.name
         self._name_plural = data.name_plural
         self._description = data.description
```

### Comparing `pygrocy-2.0.0/pygrocy/data_models/system.py` & `pygrocy-2.1.0/pygrocy/data_models/system.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/data_models/task.py` & `pygrocy-2.1.0/pygrocy/data_models/task.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/data_models/user.py` & `pygrocy-2.1.0/pygrocy/data_models/user.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/errors/grocy_error.py` & `pygrocy-2.1.0/pygrocy/errors/grocy_error.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy/grocy.py` & `pygrocy-2.1.0/pygrocy/grocy.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
     def update_generic(self, entity_type: EntityType, object_id: int, updated_data):
         return self._api_client.update_generic(
             entity_type.value, object_id, updated_data
         )
 
     def delete_generic(self, entity_type: EntityType, object_id: int):
-        return self._api_client.delete_generic(entity_type, object_id)
+        return self._api_client.delete_generic(entity_type.value, object_id)
 
     def get_generic_objects_for_type(
         self, entity_type: EntityType, query_filters: List[str] = None
     ):
         return self._api_client.get_generic_objects_for_type(
             entity_type.value, query_filters
         )
```

### Comparing `pygrocy-2.0.0/pygrocy/grocy_api_client.py` & `pygrocy-2.1.0/pygrocy/grocy_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     row_created_timestamp: datetime
     userfields: Optional[Dict] = None
 
 
 class QuantityUnitData(BaseModel):
     id: int
     name: str
-    name_plural: str
+    name_plural: Optional[str] = None
     description: Optional[str] = None
     row_created_timestamp: datetime
 
 
 class LocationData(BaseModel):
     id: int
     name: str
@@ -157,14 +157,15 @@
     overdue_products: Optional[List[CurrentStockResponse]] = None
     expired_products: Optional[List[CurrentStockResponse]] = None
     missing_products: Optional[List[MissingProductResponse]] = None
 
 
 class ProductBarcodeData(BaseModel):
     barcode: str
+    amount: Optional[float] = None
 
 
 class ProductDetailsResponse(BaseModel):
     last_purchased: Optional[date] = None
     last_used: Optional[date] = None
     stock_amount: float
     stock_amount_opened: float
```

### Comparing `pygrocy-2.0.0/pygrocy/utils.py` & `pygrocy-2.1.0/pygrocy/utils.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/pygrocy.egg-info/SOURCES.txt` & `pygrocy-2.1.0/pygrocy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/setup.py` & `pygrocy-2.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pygrocy",
-    version="2.0.0",
+    version="2.1.0",
     author="Sebastian Rutofski",
     author_email="kontakt@sebastian-rutofski.de",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sebrut/pygrocy",
     license="MIT",
```

### Comparing `pygrocy-2.0.0/test/conftest.py` & `pygrocy-2.1.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_battery.py` & `pygrocy-2.1.0/test/test_battery.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_chores.py` & `pygrocy-2.1.0/test/test_chores.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_generic.py` & `pygrocy-2.1.0/test/test_generic.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_grocy.py` & `pygrocy-2.1.0/test/test_grocy.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_grocy_api_client.py` & `pygrocy-2.1.0/test/test_grocy_api_client.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_meal_plan.py` & `pygrocy-2.1.0/test/test_meal_plan.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_meal_plan_sections.py` & `pygrocy-2.1.0/test/test_meal_plan_sections.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_product.py` & `pygrocy-2.1.0/test/test_product.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_product_groups.py` & `pygrocy-2.1.0/test/test_product_groups.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_shoppinglist.py` & `pygrocy-2.1.0/test/test_shoppinglist.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_stock.py` & `pygrocy-2.1.0/test/test_stock.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_system.py` & `pygrocy-2.1.0/test/test_system.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_tasks.py` & `pygrocy-2.1.0/test/test_tasks.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_users.py` & `pygrocy-2.1.0/test/test_users.py`

 * *Files identical despite different names*

### Comparing `pygrocy-2.0.0/test/test_utils.py` & `pygrocy-2.1.0/test/test_utils.py`

 * *Files identical despite different names*

