# Comparing `tmp/qstd_core-0.2.0.tar.gz` & `tmp/qstd_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_core-0.2.0.tar", last modified: Sun Apr 21 19:24:00 2024, max compression
+gzip compressed data, was "qstd_core-0.2.1.tar", last modified: Tue Apr 23 09:27:53 2024, max compression
```

## Comparing `qstd_core-0.2.0.tar` & `qstd_core-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.2.0/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-21 19:24:00.114144 qstd_core-0.2.0/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.2.0/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.110144 qstd_core-0.2.0/qstd_core/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.2.0/qstd_core/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.110144 qstd_core-0.2.0/qstd_core/exceptions/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.2.0/qstd_core/exceptions/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.2.0/qstd_core/exceptions/base.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.2.0/qstd_core/exceptions/localization.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.110144 qstd_core-0.2.0/qstd_core/localization/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.2.0/qstd_core/localization/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.110144 qstd_core-0.2.0/qstd_core/logger/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.2.0/qstd_core/logger/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/qstd_core/marshmallow/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-04-16 12:32:13.000000 qstd_core-0.2.0/qstd_core/marshmallow/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5299 2024-03-13 13:59:27.000000 qstd_core-0.2.0/qstd_core/marshmallow/fields.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      465 2024-03-31 12:23:58.000000 qstd_core-0.2.0/qstd_core/marshmallow/schema.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2798 2024-03-31 12:24:08.000000 qstd_core-0.2.0/qstd_core/marshmallow/validate.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/qstd_core/openapi/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.2.0/qstd_core/openapi/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5600 2024-04-16 15:28:39.000000 qstd_core-0.2.0/qstd_core/openapi/decorators.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.2.0/qstd_core/openapi/enum.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5368 2024-04-06 10:15:52.000000 qstd_core-0.2.0/qstd_core/openapi/mapper_marsmallow.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      238 2024-04-06 10:07:24.000000 qstd_core-0.2.0/qstd_core/openapi/mapper_pydantic.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.2.0/qstd_core/openapi/router.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8925 2024-04-06 10:20:57.000000 qstd_core-0.2.0/qstd_core/openapi/spec.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     7459 2024-04-16 16:52:41.000000 qstd_core-0.2.0/qstd_core/openapi/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/qstd_core/sanic/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.2.0/qstd_core/sanic/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/qstd_core/sanic/request/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.2.0/qstd_core/sanic/request/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/qstd_core/sanic/server/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.2.0/qstd_core/sanic/server/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.2.0/qstd_core/sanic/server/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.114144 qstd_core-0.2.0/qstd_core/validator/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1993 2024-04-21 19:14:09.000000 qstd_core-0.2.0/qstd_core/validator/ValidatorABS.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2169 2024-04-16 16:34:52.000000 qstd_core-0.2.0/qstd_core/validator/ValidatorMarshmallow.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1024 2024-04-16 16:40:32.000000 qstd_core-0.2.0/qstd_core/validator/ValidatorPydantic.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-21 19:18:09.000000 qstd_core-0.2.0/qstd_core/validator/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.2.0/qstd_core/validator/enums.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-04-21 19:14:09.000000 qstd_core-0.2.0/qstd_core/validator/exceptions.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.2.0/qstd_core/validator/types.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-21 19:24:00.110144 qstd_core-0.2.0/qstd_core.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-21 19:24:00.000000 qstd_core-0.2.0/qstd_core.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1138 2024-04-21 19:24:00.000000 qstd_core-0.2.0/qstd_core.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-21 19:24:00.000000 qstd_core-0.2.0/qstd_core.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       82 2024-04-21 19:24:00.000000 qstd_core-0.2.0/qstd_core.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-04-21 19:24:00.000000 qstd_core-0.2.0/qstd_core.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-21 19:24:00.114144 qstd_core-0.2.0/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      734 2024-04-21 19:22:32.000000 qstd_core-0.2.0/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.2.1/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-23 09:27:53.385282 qstd_core-0.2.1/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.2.1/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.2.1/qstd_core/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/exceptions/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.2.1/qstd_core/exceptions/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.2.1/qstd_core/exceptions/base.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.2.1/qstd_core/exceptions/localization.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/localization/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.2.1/qstd_core/localization/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/logger/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.2.1/qstd_core/logger/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/marshmallow/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-04-16 12:32:13.000000 qstd_core-0.2.1/qstd_core/marshmallow/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5299 2024-03-13 13:59:27.000000 qstd_core-0.2.1/qstd_core/marshmallow/fields.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      465 2024-03-31 12:23:58.000000 qstd_core-0.2.1/qstd_core/marshmallow/schema.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2798 2024-03-31 12:24:08.000000 qstd_core-0.2.1/qstd_core/marshmallow/validate.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/openapi/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.2.1/qstd_core/openapi/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5600 2024-04-16 15:28:39.000000 qstd_core-0.2.1/qstd_core/openapi/decorators.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.2.1/qstd_core/openapi/enum.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5368 2024-04-06 10:15:52.000000 qstd_core-0.2.1/qstd_core/openapi/mapper_marsmallow.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      238 2024-04-06 10:07:24.000000 qstd_core-0.2.1/qstd_core/openapi/mapper_pydantic.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.2.1/qstd_core/openapi/router.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8925 2024-04-06 10:20:57.000000 qstd_core-0.2.1/qstd_core/openapi/spec.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     7459 2024-04-16 16:52:41.000000 qstd_core-0.2.1/qstd_core/openapi/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/sanic/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.2.1/qstd_core/sanic/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/sanic/request/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.2.1/qstd_core/sanic/request/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/sanic/server/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.2.1/qstd_core/sanic/server/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.2.1/qstd_core/sanic/server/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core/validator/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1993 2024-04-21 19:14:09.000000 qstd_core-0.2.1/qstd_core/validator/ValidatorABS.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2169 2024-04-16 16:34:52.000000 qstd_core-0.2.1/qstd_core/validator/ValidatorMarshmallow.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1024 2024-04-16 16:40:32.000000 qstd_core-0.2.1/qstd_core/validator/ValidatorPydantic.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-23 09:26:58.000000 qstd_core-0.2.1/qstd_core/validator/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.2.1/qstd_core/validator/enums.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-04-21 19:14:09.000000 qstd_core-0.2.1/qstd_core/validator/exceptions.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.2.1/qstd_core/validator/types.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-23 09:27:53.385282 qstd_core-0.2.1/qstd_core.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-04-23 09:27:53.000000 qstd_core-0.2.1/qstd_core.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1138 2024-04-23 09:27:53.000000 qstd_core-0.2.1/qstd_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-23 09:27:53.000000 qstd_core-0.2.1/qstd_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       82 2024-04-23 09:27:53.000000 qstd_core-0.2.1/qstd_core.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-04-23 09:27:53.000000 qstd_core-0.2.1/qstd_core.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-23 09:27:53.385282 qstd_core-0.2.1/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      734 2024-04-23 09:27:20.000000 qstd_core-0.2.1/setup.py
```

### Comparing `qstd_core-0.2.0/LICENSE` & `qstd_core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/exceptions/base.py` & `qstd_core-0.2.1/qstd_core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/exceptions/localization.py` & `qstd_core-0.2.1/qstd_core/exceptions/localization.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/localization/__init__.py` & `qstd_core-0.2.1/qstd_core/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/marshmallow/fields.py` & `qstd_core-0.2.1/qstd_core/marshmallow/fields.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/marshmallow/validate.py` & `qstd_core-0.2.1/qstd_core/marshmallow/validate.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/openapi/decorators.py` & `qstd_core-0.2.1/qstd_core/openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/openapi/mapper_marsmallow.py` & `qstd_core-0.2.1/qstd_core/openapi/mapper_marsmallow.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/openapi/spec.py` & `qstd_core-0.2.1/qstd_core/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/openapi/utils.py` & `qstd_core-0.2.1/qstd_core/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/sanic/request/__init__.py` & `qstd_core-0.2.1/qstd_core/sanic/request/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/validator/ValidatorABS.py` & `qstd_core-0.2.1/qstd_core/validator/ValidatorABS.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/validator/ValidatorMarshmallow.py` & `qstd_core-0.2.1/qstd_core/validator/ValidatorMarshmallow.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/validator/ValidatorPydantic.py` & `qstd_core-0.2.1/qstd_core/validator/ValidatorPydantic.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core/validator/__init__.py` & `qstd_core-0.2.1/qstd_core/validator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,55 +10,55 @@
 from ..marshmallow import Schema
 
 
 def validator_factory(
     *,
     schema: SchemaType,
     target: TargetNameType,
-    pass_data: typing.Optional[bool] = None,
-    docs: typing.Optional[bool] = None
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
 ) -> ValidatorABS:
     if isinstance(schema, Schema):
         return ValidatorMarshmallow(schema, target, pass_data=pass_data, docs=docs)
     elif issubclass(schema, BaseModel):
         return ValidatorPydantic(schema, target, pass_data=pass_data, docs=docs)
     else:
         raise NotImplementedError()
 
 
 def body(
     schema: typing.Type[SchemaType],
     *,
-    pass_data: typing.Optional[bool] = None,
-    docs: typing.Optional[bool] = None
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
 ):
     return validator_factory(schema=schema, target=TargetNameType.BODY, pass_data=pass_data, docs=docs)
 
 
 def query(
     schema: typing.Type[SchemaType],
     *,
-    pass_data: typing.Optional[bool] = None,
-    docs: typing.Optional[bool] = None
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
 ):
     return validator_factory(schema=schema, target=TargetNameType.QUERY, pass_data=pass_data, docs=docs)
 
 
 def params(
     schema: typing.Type[SchemaType],
     *,
-    pass_data: typing.Optional[bool] = None,
-    docs: typing.Optional[bool] = None
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
 ):
     return validator_factory(schema=schema, target=TargetNameType.PARAMS, pass_data=pass_data, docs=docs)
 
 
 def validate(
     schema: typing.Type[SchemaType],
     *,
     target: TargetNameType = TargetNameType.UNION,
     payload: dict,
-    pass_data: typing.Optional[bool] = None,
-    docs: typing.Optional[bool] = None
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
 ):
     return validator_factory(schema=schema, target=target, pass_data=pass_data, docs=docs).validate(payload)
```

### Comparing `qstd_core-0.2.0/qstd_core/validator/exceptions.py` & `qstd_core-0.2.1/qstd_core/validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/qstd_core.egg-info/SOURCES.txt` & `qstd_core-0.2.1/qstd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qstd_core-0.2.0/setup.py` & `qstd_core-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_core',
-    version='0.2.0',
+    version='0.2.1',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Application core based on sanic',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-core',
     packages=find_packages(exclude=['tmp', 'example']),
```

