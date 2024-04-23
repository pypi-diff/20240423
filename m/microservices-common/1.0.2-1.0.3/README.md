# Comparing `tmp/microservices_common-1.0.2.tar.gz` & `tmp/microservices_common-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservices_common-1.0.2.tar", last modified: Sat Apr  6 10:09:29 2024, max compression
+gzip compressed data, was "microservices_common-1.0.3.tar", last modified: Tue Apr 23 07:43:08 2024, max compression
```

## Comparing `microservices_common-1.0.2.tar` & `microservices_common-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.200464 microservices_common-1.0.2/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      560 2024-04-06 10:09:29.200204 microservices_common-1.0.2/PKG-INFO
--rw-r--r--   0 AliZaidi   (502) staff       (20)       38 2024-04-06 10:09:29.200631 microservices_common-1.0.2/setup.cfg
--rw-r--r--   0 AliZaidi   (502) staff       (20)      752 2024-04-06 10:09:25.000000 microservices_common-1.0.2/setup.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.190241 microservices_common-1.0.2/src/
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.190846 microservices_common-1.0.2/src/microservices_common/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      134 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/__init__.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.194822 microservices_common-1.0.2/src/microservices_common/exceptions/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      498 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/__init__.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/authentication_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      361 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/custom_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      387 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      469 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/invalid_input_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      379 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/not_found_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/owner_not_found_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      352 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/exceptions/userid_not_found_exception.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.198305 microservices_common-1.0.2/src/microservices_common/middlewares/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      176 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/middlewares/__init__.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      349 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/middlewares/admin.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     3402 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/middlewares/authorized.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     1116 2024-04-05 12:38:51.000000 microservices_common-1.0.2/src/microservices_common/middlewares/exception_handler.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.199631 microservices_common-1.0.2/src/microservices_common/utils/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      149 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/utils/__init__.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     2779 2023-08-18 11:57:19.000000 microservices_common-1.0.2/src/microservices_common/utils/datetime_util.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     1293 2024-03-05 07:23:11.000000 microservices_common-1.0.2/src/microservices_common/utils/logger.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)    15465 2024-04-06 10:09:14.000000 microservices_common-1.0.2/src/microservices_common/utils/util.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-06 10:09:29.192130 microservices_common-1.0.2/src/microservices_common.egg-info/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      560 2024-04-06 10:09:29.000000 microservices_common-1.0.2/src/microservices_common.egg-info/PKG-INFO
--rw-r--r--   0 AliZaidi   (502) staff       (20)     1156 2024-04-06 10:09:29.000000 microservices_common-1.0.2/src/microservices_common.egg-info/SOURCES.txt
--rw-r--r--   0 AliZaidi   (502) staff       (20)        1 2024-04-06 10:09:29.000000 microservices_common-1.0.2/src/microservices_common.egg-info/dependency_links.txt
--rw-r--r--   0 AliZaidi   (502) staff       (20)      140 2024-04-06 10:09:29.000000 microservices_common-1.0.2/src/microservices_common.egg-info/requires.txt
--rw-r--r--   0 AliZaidi   (502) staff       (20)       21 2024-04-06 10:09:29.000000 microservices_common-1.0.2/src/microservices_common.egg-info/top_level.txt
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.876639 microservices_common-1.0.3/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      330 2024-04-23 07:43:08.876498 microservices_common-1.0.3/PKG-INFO
+-rw-r--r--   0 AliZaidi   (502) staff       (20)       38 2024-04-23 07:43:08.876685 microservices_common-1.0.3/setup.cfg
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      752 2024-04-23 07:42:22.000000 microservices_common-1.0.3/setup.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.871022 microservices_common-1.0.3/src/
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.871650 microservices_common-1.0.3/src/microservices_common/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      134 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/__init__.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.874576 microservices_common-1.0.3/src/microservices_common/exceptions/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      580 2024-04-23 07:37:34.000000 microservices_common-1.0.3/src/microservices_common/exceptions/__init__.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/authentication_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      361 2024-04-23 07:37:34.000000 microservices_common-1.0.3/src/microservices_common/exceptions/company_profile_not_found_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      361 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/custom_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      387 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      469 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/invalid_input_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      379 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/not_found_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/owner_not_found_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      352 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/exceptions/userid_not_found_exception.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.875259 microservices_common-1.0.3/src/microservices_common/middlewares/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      176 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/middlewares/__init__.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      349 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/middlewares/admin.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     3402 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/middlewares/authorized.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     1116 2024-04-05 12:38:51.000000 microservices_common-1.0.3/src/microservices_common/middlewares/exception_handler.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.876141 microservices_common-1.0.3/src/microservices_common/utils/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      149 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/utils/__init__.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     2779 2023-08-18 11:57:19.000000 microservices_common-1.0.3/src/microservices_common/utils/datetime_util.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     1293 2024-03-05 07:23:11.000000 microservices_common-1.0.3/src/microservices_common/utils/logger.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)    15785 2024-04-23 07:37:34.000000 microservices_common-1.0.3/src/microservices_common/utils/util.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-23 07:43:08.872575 microservices_common-1.0.3/src/microservices_common.egg-info/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      330 2024-04-23 07:43:08.000000 microservices_common-1.0.3/src/microservices_common.egg-info/PKG-INFO
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     1231 2024-04-23 07:43:08.000000 microservices_common-1.0.3/src/microservices_common.egg-info/SOURCES.txt
+-rw-r--r--   0 AliZaidi   (502) staff       (20)        1 2024-04-23 07:43:08.000000 microservices_common-1.0.3/src/microservices_common.egg-info/dependency_links.txt
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      140 2024-04-23 07:43:08.000000 microservices_common-1.0.3/src/microservices_common.egg-info/requires.txt
+-rw-r--r--   0 AliZaidi   (502) staff       (20)       21 2024-04-23 07:43:08.000000 microservices_common-1.0.3/src/microservices_common.egg-info/top_level.txt
```

### Comparing `microservices_common-1.0.2/setup.py` & `microservices_common-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="microservices_common",
-    version="1.0.2",
+    version="1.0.3",
     author="Ali Zaidi",
     author_email="support@arrivy.com",
     description="",
     long_description="",
     url="https://github.com/arrivy-dev/microservices-python-common",
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `microservices_common-1.0.2/src/microservices_common/middlewares/authorized.py` & `microservices_common-1.0.3/src/microservices_common/middlewares/authorized.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.2/src/microservices_common/middlewares/exception_handler.py` & `microservices_common-1.0.3/src/microservices_common/middlewares/exception_handler.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.2/src/microservices_common/utils/datetime_util.py` & `microservices_common-1.0.3/src/microservices_common/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.2/src/microservices_common/utils/logger.py` & `microservices_common-1.0.3/src/microservices_common/utils/logger.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.2/src/microservices_common/utils/util.py` & `microservices_common-1.0.3/src/microservices_common/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,23 @@
 
         userid = auth_info.get('user', dict()).get('userId', None)
         if not userid:
             raise UserIdNotFound()
         return userid
 
     @classmethod
+    def get_company_profile_from_auth(cls, auth_info):
+        from microservices_common.exceptions import CompanyProfileNotFound
+
+        company_profile = auth_info.get('company_profile', None)
+        if not company_profile:
+            raise CompanyProfileNotFound()
+        return company_profile
+
+    @classmethod
     def is_valid_uuid(cls, uuid_to_test, version=4):
         from uuid import UUID
         try:
             uuid_obj = UUID(uuid_to_test, version=version)
         except ValueError:
             return False
         return str(uuid_obj) == uuid_to_test
```

### Comparing `microservices_common-1.0.2/src/microservices_common.egg-info/SOURCES.txt` & `microservices_common-1.0.3/src/microservices_common.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/microservices_common.egg-info/PKG-INFO
 src/microservices_common.egg-info/SOURCES.txt
 src/microservices_common.egg-info/dependency_links.txt
 src/microservices_common.egg-info/requires.txt
 src/microservices_common.egg-info/top_level.txt
 src/microservices_common/exceptions/__init__.py
 src/microservices_common/exceptions/authentication_exception.py
+src/microservices_common/exceptions/company_profile_not_found_exception.py
 src/microservices_common/exceptions/custom_exception.py
 src/microservices_common/exceptions/incorrect_parameter_format_exception.py
 src/microservices_common/exceptions/invalid_input_exception.py
 src/microservices_common/exceptions/not_found_exception.py
 src/microservices_common/exceptions/owner_not_found_exception.py
 src/microservices_common/exceptions/userid_not_found_exception.py
 src/microservices_common/middlewares/__init__.py
```

