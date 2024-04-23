# Comparing `tmp/motor-decorator-0.0.3.4.tar.gz` & `tmp/motor-decorator-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motor-decorator-0.0.3.4.tar", last modified: Tue Mar 26 13:27:03 2024, max compression
+gzip compressed data, was "motor-decorator-0.0.3.5.tar", last modified: Tue Apr 23 06:56:48 2024, max compression
```

## Comparing `motor-decorator-0.0.3.4.tar` & `motor-decorator-0.0.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-26 13:27:03.618772 motor-decorator-0.0.3.4/
--rw-rw-r--   0 tim       (1000) tim       (1000)    11357 2024-03-10 17:21:00.000000 motor-decorator-0.0.3.4/LICENSE
--rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-03-26 13:27:03.618772 motor-decorator-0.0.3.4/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3809 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.4/README.md
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-26 13:27:03.618772 motor-decorator-0.0.3.4/motor_decorator/
--rw-rw-r--   0 tim       (1000) tim       (1000)      242 2024-03-11 05:05:24.000000 motor-decorator-0.0.3.4/motor_decorator/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      620 2024-03-10 17:14:40.000000 motor-decorator-0.0.3.4/motor_decorator/abstract_view.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1463 2024-03-11 06:56:03.000000 motor-decorator-0.0.3.4/motor_decorator/base_db.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    13356 2024-03-26 13:23:53.000000 motor-decorator-0.0.3.4/motor_decorator/controller.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      423 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.4/motor_decorator/exception.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4157 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.4/motor_decorator/objects.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3082 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.4/motor_decorator/profiler.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2693 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.4/motor_decorator/registrator.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      680 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.4/motor_decorator/settings.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2120 2024-03-21 12:04:46.000000 motor-decorator-0.0.3.4/motor_decorator/tools.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-03-26 13:27:03.618772 motor-decorator-0.0.3.4/motor_decorator.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-03-26 13:27:03.000000 motor-decorator-0.0.3.4/motor_decorator.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      506 2024-03-26 13:27:03.000000 motor-decorator-0.0.3.4/motor_decorator.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-03-26 13:27:03.000000 motor-decorator-0.0.3.4/motor_decorator.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       29 2024-03-26 13:27:03.000000 motor-decorator-0.0.3.4/motor_decorator.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       16 2024-03-26 13:27:03.000000 motor-decorator-0.0.3.4/motor_decorator.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-03-26 13:27:03.618772 motor-decorator-0.0.3.4/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      507 2024-03-26 13:24:08.000000 motor-decorator-0.0.3.4/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 06:56:47.999810 motor-decorator-0.0.3.5/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11357 2024-03-10 17:21:00.000000 motor-decorator-0.0.3.5/LICENSE
+-rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-04-23 06:56:47.999810 motor-decorator-0.0.3.5/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3809 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.5/README.md
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 06:56:47.999810 motor-decorator-0.0.3.5/motor_decorator/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      242 2024-03-11 05:05:24.000000 motor-decorator-0.0.3.5/motor_decorator/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      620 2024-03-10 17:14:40.000000 motor-decorator-0.0.3.5/motor_decorator/abstract_view.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1463 2024-03-11 06:56:03.000000 motor-decorator-0.0.3.5/motor_decorator/base_db.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13866 2024-04-23 06:54:52.000000 motor-decorator-0.0.3.5/motor_decorator/controller.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      423 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.5/motor_decorator/exception.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4157 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.5/motor_decorator/objects.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3082 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.5/motor_decorator/profiler.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2693 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.5/motor_decorator/registrator.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      680 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.5/motor_decorator/settings.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2734 2024-04-23 06:54:52.000000 motor-decorator-0.0.3.5/motor_decorator/tools.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 06:56:47.999810 motor-decorator-0.0.3.5/motor_decorator.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-04-23 06:56:47.000000 motor-decorator-0.0.3.5/motor_decorator.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      506 2024-04-23 06:56:47.000000 motor-decorator-0.0.3.5/motor_decorator.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-04-23 06:56:47.000000 motor-decorator-0.0.3.5/motor_decorator.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       29 2024-04-23 06:56:47.000000 motor-decorator-0.0.3.5/motor_decorator.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       16 2024-04-23 06:56:47.000000 motor-decorator-0.0.3.5/motor_decorator.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-04-23 06:56:47.999810 motor-decorator-0.0.3.5/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      507 2024-04-23 06:55:04.000000 motor-decorator-0.0.3.5/setup.py
```

### Comparing `motor-decorator-0.0.3.4/LICENSE` & `motor-decorator-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/PKG-INFO` & `motor-decorator-0.0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motor-decorator
-Version: 0.0.3.4
+Version: 0.0.3.5
 Summary: Decorator for motor library
 Home-page: https://github.com/FeltsAzn/motor-decorator
 Author: Timur Galiev
 Author-email: timkin12321@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `motor-decorator-0.0.3.4/README.md` & `motor-decorator-0.0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/abstract_view.py` & `motor-decorator-0.0.3.5/motor_decorator/abstract_view.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/base_db.py` & `motor-decorator-0.0.3.5/motor_decorator/base_db.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/controller.py` & `motor-decorator-0.0.3.5/motor_decorator/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -174,39 +174,43 @@
         )
 
     async def do_insert_one(
             self,
             document: dict,
             return_id: bool = False,
             raw_response: bool = False,
+            duplicate_skip: bool = False,
             **kwargs
     ) -> bool | ObjectId | InsertOneResult:
         response: InsertOneResult = await self._execute(
             function=self._collection.insert_one,
             document=document,
+            duplicate_skip=duplicate_skip,
             **kwargs
         )
         if return_id:
             return response.inserted_id
         elif raw_response:
             return response
         return response.acknowledged
 
     async def do_insert_many(
             self,
             records: list[dict],
             ordered: bool = True,
             return_id: bool = False,
             raw_response: bool = False,
+            duplicate_skip: bool = False,
             **kwargs
     ) -> bool | list[ObjectId] | InsertManyResult:
         response = await self._execute(
             function=self._collection.insert_many,
             documents=records,
             ordered=ordered,
+            duplicate_skip=duplicate_skip,
             **kwargs
         )
         if return_id:
             return response.inserted_ids
         elif raw_response:
             return response
         return response.acknowledged
@@ -214,41 +218,45 @@
     async def do_update_one(
             self,
             condition: dict,
             updating_fields: dict,
             return_id: bool = False,
             upsert: bool = False,
             raw_response: bool = False,
+            duplicate_skip: bool = False,
             **kwargs
     ) -> int | ObjectId | UpdateResult:
         response = await self._execute(
             function=self._collection.update_one,
             filter=condition,
             update=updating_fields,
             upsert=upsert,
+            duplicate_skip=duplicate_skip,
             **kwargs
         )
         if return_id:
             return response.upserted_id
         elif raw_response:
             return response
         return response.modified_count
 
     async def do_update_many(
             self,
             condition: dict,
             updating_fields: dict,
             return_id: bool = False,
             raw_response: bool = False,
+            duplicate_skip: bool = False,
             **kwargs
     ) -> int | list[ObjectId] | UpdateResult:
         response = await self._execute(
             function=self._collection.update_many,
             filter=condition,
             update=updating_fields,
+            duplicate_skip=duplicate_skip,
             **kwargs)
         if return_id:
             return response.upserted_id
         elif raw_response:
             return response
         return response.modified_count
 
@@ -283,14 +291,15 @@
             self,
             condition: dict,
             updating_fields: dict,
             upsert: bool = False,
             projection: dict | None = None,
             view_class: Type[MotorDecoratorAbstractView] | None = None,
             return_before: bool = True,
+            duplicate_skip: bool = False,
             **kwargs,
     ) -> dict | MotorDecoratorAbstractView | None:
         if return_before is True:
             return_document = ReturnDocument.BEFORE
         else:
             return_document = ReturnDocument.AFTER
 
@@ -300,14 +309,15 @@
         response = await self._execute(
             function=self._collection.find_one_and_update,
             filter=condition,
             update=updating_fields,
             projection=projection,
             upsert=upsert,
             return_document=return_document,
+            duplicate_skip=duplicate_skip,
             **kwargs
         )
         if view_class and response:
             return self._wrap_entity(view_class, response)
         return response
 
     async def do_delete_one(self, condition: dict, raw_response: bool = False, **kwargs) -> int | DeleteResult:
@@ -342,20 +352,22 @@
 
     async def do_bulk_write(
             self,
             operations: list[UpdateOne | DeleteOne | InsertOne],
             ordered: bool = True,
             return_id: bool = False,
             raw_response: bool = False,
+            duplicate_skip: bool = False,
             **kwargs
     ) -> bool | list[ObjectId] | BulkWriteResult:
         response = await self._execute(
             function=self._collection.bulk_write,
             requests=operations,
             ordered=ordered,
+            duplicate_skip=duplicate_skip,
             **kwargs
         )
         if return_id:
             return response.upserted_ids  # type: ignore
         elif raw_response:
             return response
```

### Comparing `motor-decorator-0.0.3.4/motor_decorator/objects.py` & `motor-decorator-0.0.3.5/motor_decorator/objects.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/profiler.py` & `motor-decorator-0.0.3.5/motor_decorator/profiler.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/registrator.py` & `motor-decorator-0.0.3.5/motor_decorator/registrator.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/settings.py` & `motor-decorator-0.0.3.5/motor_decorator/settings.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.4/motor_decorator/tools.py` & `motor-decorator-0.0.3.5/motor_decorator/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import functools
 import logging
 from typing import Callable, Any
 
+from pymongo.errors import DuplicateKeyError
+
 
 class MotorDecoratorTools:
     info_format: str = "[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s [%(filename)s/%(funcName)s:%(lineno)d]"
     LOGGING_LEVEL: str = "INFO"
 
     @staticmethod
     def retry(logger: logging.Logger, init_retries: int = 3, timeout: int = 1) -> Callable:
@@ -16,14 +18,25 @@
 
                 retries = init_retries
                 delay = timeout
 
                 while retries:
                     try:
                         return await func(*args, **kwargs)
+                    except DuplicateKeyError as ex:
+                        error_message = (
+                            f"Database connection error (retry={retries % 4}). "
+                            f"execution function: <{func.__name__}>, "
+                            f"exception class: <{ex.__class__.__name__}>, "
+                            f"exception description: {ex}"
+                        )
+
+                        if kwargs.get("duplicate_skip", False) is False:
+                            logger.error(error_message)
+                        return
                     except Exception as ex:
                         error_message = (
                             f"Database connection error (retry={retries % 4}). "
                             f"execution function: <{func.__name__}>, "
                             f"exception class: <{ex.__class__.__name__}>, "
                             f"exception description: {ex}"
                         )
```

### Comparing `motor-decorator-0.0.3.4/motor_decorator.egg-info/PKG-INFO` & `motor-decorator-0.0.3.5/motor_decorator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motor-decorator
-Version: 0.0.3.4
+Version: 0.0.3.5
 Summary: Decorator for motor library
 Home-page: https://github.com/FeltsAzn/motor-decorator
 Author: Timur Galiev
 Author-email: timkin12321@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```
