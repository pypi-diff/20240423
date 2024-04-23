# Comparing `tmp/motor-decorator-0.0.3.6.tar.gz` & `tmp/motor-decorator-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motor-decorator-0.0.3.6.tar", last modified: Tue Apr 23 07:29:52 2024, max compression
+gzip compressed data, was "motor-decorator-0.0.3.7.tar", last modified: Tue Apr 23 08:07:07 2024, max compression
```

## Comparing `motor-decorator-0.0.3.6.tar` & `motor-decorator-0.0.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 07:29:52.333943 motor-decorator-0.0.3.6/
--rw-rw-r--   0 tim       (1000) tim       (1000)    11357 2024-03-10 17:21:00.000000 motor-decorator-0.0.3.6/LICENSE
--rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-04-23 07:29:52.329943 motor-decorator-0.0.3.6/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3809 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.6/README.md
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 07:29:52.329943 motor-decorator-0.0.3.6/motor_decorator/
--rw-rw-r--   0 tim       (1000) tim       (1000)      242 2024-03-11 05:05:24.000000 motor-decorator-0.0.3.6/motor_decorator/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      620 2024-03-10 17:14:40.000000 motor-decorator-0.0.3.6/motor_decorator/abstract_view.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1463 2024-03-11 06:56:03.000000 motor-decorator-0.0.3.6/motor_decorator/base_db.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    14429 2024-04-23 07:29:31.000000 motor-decorator-0.0.3.6/motor_decorator/controller.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      423 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.6/motor_decorator/exception.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4352 2024-04-23 07:29:31.000000 motor-decorator-0.0.3.6/motor_decorator/objects.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3082 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.6/motor_decorator/profiler.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2693 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.6/motor_decorator/registrator.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      680 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.6/motor_decorator/settings.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2882 2024-04-23 07:29:31.000000 motor-decorator-0.0.3.6/motor_decorator/tools.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 07:29:52.329943 motor-decorator-0.0.3.6/motor_decorator.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-04-23 07:29:52.000000 motor-decorator-0.0.3.6/motor_decorator.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      506 2024-04-23 07:29:52.000000 motor-decorator-0.0.3.6/motor_decorator.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-04-23 07:29:52.000000 motor-decorator-0.0.3.6/motor_decorator.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       29 2024-04-23 07:29:52.000000 motor-decorator-0.0.3.6/motor_decorator.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       16 2024-04-23 07:29:52.000000 motor-decorator-0.0.3.6/motor_decorator.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-04-23 07:29:52.333943 motor-decorator-0.0.3.6/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      507 2024-04-23 07:29:31.000000 motor-decorator-0.0.3.6/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 08:07:07.279211 motor-decorator-0.0.3.7/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11357 2024-03-10 17:21:00.000000 motor-decorator-0.0.3.7/LICENSE
+-rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-04-23 08:07:07.279211 motor-decorator-0.0.3.7/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3809 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.7/README.md
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 08:07:07.279211 motor-decorator-0.0.3.7/motor_decorator/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      242 2024-03-11 05:05:24.000000 motor-decorator-0.0.3.7/motor_decorator/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      620 2024-03-10 17:14:40.000000 motor-decorator-0.0.3.7/motor_decorator/abstract_view.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1463 2024-03-11 06:56:03.000000 motor-decorator-0.0.3.7/motor_decorator/base_db.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14429 2024-04-23 07:29:31.000000 motor-decorator-0.0.3.7/motor_decorator/controller.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      423 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.7/motor_decorator/exception.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4352 2024-04-23 07:29:31.000000 motor-decorator-0.0.3.7/motor_decorator/objects.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3082 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.7/motor_decorator/profiler.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2693 2024-03-11 08:16:43.000000 motor-decorator-0.0.3.7/motor_decorator/registrator.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      680 2024-03-20 03:58:06.000000 motor-decorator-0.0.3.7/motor_decorator/settings.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3754 2024-04-23 08:05:35.000000 motor-decorator-0.0.3.7/motor_decorator/tools.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-23 08:07:07.279211 motor-decorator-0.0.3.7/motor_decorator.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)     4159 2024-04-23 08:07:07.000000 motor-decorator-0.0.3.7/motor_decorator.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      506 2024-04-23 08:07:07.000000 motor-decorator-0.0.3.7/motor_decorator.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-04-23 08:07:07.000000 motor-decorator-0.0.3.7/motor_decorator.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       29 2024-04-23 08:07:07.000000 motor-decorator-0.0.3.7/motor_decorator.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       16 2024-04-23 08:07:07.000000 motor-decorator-0.0.3.7/motor_decorator.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-04-23 08:07:07.279211 motor-decorator-0.0.3.7/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      507 2024-04-23 08:05:42.000000 motor-decorator-0.0.3.7/setup.py
```

### Comparing `motor-decorator-0.0.3.6/LICENSE` & `motor-decorator-0.0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/PKG-INFO` & `motor-decorator-0.0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motor-decorator
-Version: 0.0.3.6
+Version: 0.0.3.7
 Summary: Decorator for motor library
 Home-page: https://github.com/FeltsAzn/motor-decorator
 Author: Timur Galiev
 Author-email: timkin12321@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `motor-decorator-0.0.3.6/README.md` & `motor-decorator-0.0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/abstract_view.py` & `motor-decorator-0.0.3.7/motor_decorator/abstract_view.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/base_db.py` & `motor-decorator-0.0.3.7/motor_decorator/base_db.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/controller.py` & `motor-decorator-0.0.3.7/motor_decorator/controller.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/objects.py` & `motor-decorator-0.0.3.7/motor_decorator/objects.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/profiler.py` & `motor-decorator-0.0.3.7/motor_decorator/profiler.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/registrator.py` & `motor-decorator-0.0.3.7/motor_decorator/registrator.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/settings.py` & `motor-decorator-0.0.3.7/motor_decorator/settings.py`

 * *Files identical despite different names*

### Comparing `motor-decorator-0.0.3.6/motor_decorator/tools.py` & `motor-decorator-0.0.3.7/motor_decorator/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 import asyncio
 import functools
 import logging
 from typing import Callable, Any
 
-from pymongo.errors import DuplicateKeyError
+from pymongo.errors import DuplicateKeyError, BulkWriteError
 
 from .objects import MotorDecoratorRetryParameters
 
 
 class MotorDecoratorTools:
     info_format: str = "[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s [%(filename)s/%(funcName)s:%(lineno)d]"
     LOGGING_LEVEL: str = "INFO"
+    base_retry_param: MotorDecoratorRetryParameters = MotorDecoratorRetryParameters()
 
     @staticmethod
     def retry(logger: logging.Logger, init_retries: int = 3, timeout: int = 1) -> Callable:
         def send_request(func: Callable) -> Callable:
             @functools.wraps(func)
             async def wrap(*args, **kwargs) -> Any | None:
 
                 retries = init_retries
                 delay = timeout
 
-                retry_param = kwargs.pop("retry_param", MotorDecoratorRetryParameters())
+                retry_param = kwargs.pop("retry_param", MotorDecoratorTools.base_retry_param)
 
                 while retries:
                     try:
                         return await func(*args, **kwargs)
                     except DuplicateKeyError as ex:
                         error_message = (
-                            f"Database connection error (retry={retries % 4}). "
+                            f"DuplicateKeyError (retry={retries % 4}). "
                             f"execution function: <{func.__name__}>, "
-                            f"exception class: <{ex.__class__.__name__}>, "
                             f"exception description: {ex}"
                         )
 
                         if retry_param.skip_duplicate_key_error_info is False:
                             logger.error(error_message)
                         return
+                    except BulkWriteError as ex:
+                        error_message = (
+                            f"BulkWriteError (retry={retries % 4}). "
+                            f"execution function: <{func.__name__}>, "
+                            f"exception description: {ex}"
+                        )
+                        if error_description := ex.details.get('writeErrors', []):
+                            if "E11000" in error_description[0].get("errmsg", ""):
+                                if retry_param.skip_duplicate_key_error_info is False:
+                                    logger.error(error_message)
+                                return
+
+                        logger.error(error_message)
+                        retries -= 1
+                        await asyncio.sleep(delay)
+                        delay *= 2
                     except Exception as ex:
                         error_message = (
                             f"Database connection error (retry={retries % 4}). "
                             f"execution function: <{func.__name__}>, "
                             f"exception class: <{ex.__class__.__name__}>, "
                             f"exception description: {ex}"
                         )
```

### Comparing `motor-decorator-0.0.3.6/motor_decorator.egg-info/PKG-INFO` & `motor-decorator-0.0.3.7/motor_decorator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motor-decorator
-Version: 0.0.3.6
+Version: 0.0.3.7
 Summary: Decorator for motor library
 Home-page: https://github.com/FeltsAzn/motor-decorator
 Author: Timur Galiev
 Author-email: timkin12321@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

