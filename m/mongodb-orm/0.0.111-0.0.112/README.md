# Comparing `tmp/mongodb_orm-0.0.111.tar.gz` & `tmp/mongodb_orm-0.0.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.111.tar", last modified: Tue Apr 23 14:52:37 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.112.tar", last modified: Tue Apr 23 14:56:42 2024, max compression
```

## Comparing `mongodb_orm-0.0.111.tar` & `mongodb_orm-0.0.112.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.618908 mongodb_orm-0.0.111/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 14:52:37.618171 mongodb_orm-0.0.111/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.111/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.593052 mongodb_orm-0.0.111/app/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.111/app/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.111/app/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.594459 mongodb_orm-0.0.111/app/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.111/app/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-04-23 14:17:15.000000 mongodb_orm-0.0.111/app/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.596408 mongodb_orm-0.0.111/app/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.111/app/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.111/app/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.597374 mongodb_orm-0.0.111/app/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.111/app/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.111/app/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.599252 mongodb_orm-0.0.111/app/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.111/app/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2343 2024-04-23 14:21:21.000000 mongodb_orm-0.0.111/app/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7142 2024-04-23 14:21:21.000000 mongodb_orm-0.0.111/app/interfaces/mongodb_model.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.600056 mongodb_orm-0.0.111/app/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.111/app/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.600828 mongodb_orm-0.0.111/app/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.111/app/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4532 2024-04-23 14:21:21.000000 mongodb_orm-0.0.111/app/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.601863 mongodb_orm-0.0.111/app/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.111/app/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.602358 mongodb_orm-0.0.111/app/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.111/app/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.111/app/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.612767 mongodb_orm-0.0.111/app/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.111/app/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.111/app/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.111/app/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.111/app/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.111/app/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      358 2024-04-23 14:21:21.000000 mongodb_orm-0.0.111/app/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.111/app/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.613870 mongodb_orm-0.0.111/app/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.111/app/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.111/app/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:52:37.617406 mongodb_orm-0.0.111/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 14:52:37.000000 mongodb_orm-0.0.111/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      894 2024-04-23 14:52:37.000000 mongodb_orm-0.0.111/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-23 14:52:37.000000 mongodb_orm-0.0.111/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-23 14:52:37.000000 mongodb_orm-0.0.111/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        4 2024-04-23 14:52:37.000000 mongodb_orm-0.0.111/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-23 14:52:37.619124 mongodb_orm-0.0.111/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      605 2024-04-23 14:52:29.000000 mongodb_orm-0.0.111/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.794741 mongodb_orm-0.0.112/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 14:56:42.793748 mongodb_orm-0.0.112/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.112/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.774209 mongodb_orm-0.0.112/app/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.112/app/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.112/app/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.775580 mongodb_orm-0.0.112/app/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.112/app/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-04-23 14:17:15.000000 mongodb_orm-0.0.112/app/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.776760 mongodb_orm-0.0.112/app/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.112/app/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.112/app/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.777915 mongodb_orm-0.0.112/app/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.112/app/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.112/app/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.779897 mongodb_orm-0.0.112/app/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.112/app/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2343 2024-04-23 14:21:21.000000 mongodb_orm-0.0.112/app/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7142 2024-04-23 14:21:21.000000 mongodb_orm-0.0.112/app/interfaces/mongodb_model.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.780634 mongodb_orm-0.0.112/app/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.112/app/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.781501 mongodb_orm-0.0.112/app/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.112/app/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4532 2024-04-23 14:21:21.000000 mongodb_orm-0.0.112/app/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.782634 mongodb_orm-0.0.112/app/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.112/app/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.783459 mongodb_orm-0.0.112/app/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.112/app/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.112/app/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.787560 mongodb_orm-0.0.112/app/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.112/app/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.112/app/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.112/app/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.112/app/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.112/app/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      358 2024-04-23 14:21:21.000000 mongodb_orm-0.0.112/app/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.112/app/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.788759 mongodb_orm-0.0.112/app/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.112/app/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.112/app/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:56:42.792884 mongodb_orm-0.0.112/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 14:56:42.000000 mongodb_orm-0.0.112/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      894 2024-04-23 14:56:42.000000 mongodb_orm-0.0.112/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-23 14:56:42.000000 mongodb_orm-0.0.112/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-23 14:56:42.000000 mongodb_orm-0.0.112/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        4 2024-04-23 14:56:42.000000 mongodb_orm-0.0.112/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-23 14:56:42.794904 mongodb_orm-0.0.112/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-23 14:56:35.000000 mongodb_orm-0.0.112/setup.py
```

### Comparing `mongodb_orm-0.0.111/README.md` & `mongodb_orm-0.0.112/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/app/custom_urls/bread_urls.py` & `mongodb_orm-0.0.112/app/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/app/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.112/app/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/app/interfaces/mongodb_model.py` & `mongodb_orm-0.0.112/app/interfaces/mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/app/management/commands/update_schema.py` & `mongodb_orm-0.0.112/app/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/app/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.112/app/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.112/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.111/setup.py` & `mongodb_orm-0.0.112/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.111",
+    version="0.0.112",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
-    package_data={'mongodb_orm': ['*']},
+    include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
     install_requires=requirements,
     classifiers=[
         "License :: OSI Approved :: MIT License",
     ],
-)
+)
```

