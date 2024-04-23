# Comparing `tmp/mongodb_orm-0.0.113.tar.gz` & `tmp/mongodb_orm-0.0.114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.113.tar", last modified: Tue Apr 23 15:00:34 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.114.tar", last modified: Tue Apr 23 15:18:14 2024, max compression
```

## Comparing `mongodb_orm-0.0.113.tar` & `mongodb_orm-0.0.114.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.680109 mongodb_orm-0.0.113/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 15:00:34.679245 mongodb_orm-0.0.113/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.113/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.660205 mongodb_orm-0.0.113/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.113/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.113/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.664940 mongodb_orm-0.0.113/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.113/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-04-23 14:17:15.000000 mongodb_orm-0.0.113/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.666014 mongodb_orm-0.0.113/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.113/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.113/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.667125 mongodb_orm-0.0.113/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.113/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.113/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.668913 mongodb_orm-0.0.113/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.113/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2343 2024-04-23 14:21:21.000000 mongodb_orm-0.0.113/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7142 2024-04-23 14:21:21.000000 mongodb_orm-0.0.113/mongodb_orm/interfaces/mongodb_model.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.669540 mongodb_orm-0.0.113/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.113/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.670681 mongodb_orm-0.0.113/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.113/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4532 2024-04-23 14:21:21.000000 mongodb_orm-0.0.113/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.671520 mongodb_orm-0.0.113/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.113/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.672685 mongodb_orm-0.0.113/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.113/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.113/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.676252 mongodb_orm-0.0.113/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.113/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.113/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.113/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.113/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.113/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      358 2024-04-23 14:21:21.000000 mongodb_orm-0.0.113/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.113/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.677617 mongodb_orm-0.0.113/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.113/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.113/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:00:34.678384 mongodb_orm-0.0.113/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 15:00:34.000000 mongodb_orm-0.0.113/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1102 2024-04-23 15:00:34.000000 mongodb_orm-0.0.113/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-23 15:00:34.000000 mongodb_orm-0.0.113/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-23 15:00:34.000000 mongodb_orm-0.0.113/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-23 15:00:34.000000 mongodb_orm-0.0.113/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-23 15:00:34.680297 mongodb_orm-0.0.113/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-23 15:00:31.000000 mongodb_orm-0.0.113/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.754684 mongodb_orm-0.0.114/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 15:18:14.754054 mongodb_orm-0.0.114/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.114/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.741396 mongodb_orm-0.0.114/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.114/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.114/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.744021 mongodb_orm-0.0.114/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.114/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1526 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.744663 mongodb_orm-0.0.114/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.114/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.114/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.745653 mongodb_orm-0.0.114/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.114/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.114/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.746823 mongodb_orm-0.0.114/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.114/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2383 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7213 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/mongodb_orm/interfaces/mongodb_model.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.747279 mongodb_orm-0.0.114/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.114/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.747783 mongodb_orm-0.0.114/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.114/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.748122 mongodb_orm-0.0.114/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.114/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.748774 mongodb_orm-0.0.114/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.114/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.114/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.751773 mongodb_orm-0.0.114/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.114/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.114/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.114/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.114/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.114/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.114/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.752338 mongodb_orm-0.0.114/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.114/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1159 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.753030 mongodb_orm-0.0.114/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.114/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.114/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:18:14.753580 mongodb_orm-0.0.114/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 15:18:14.000000 mongodb_orm-0.0.114/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1161 2024-04-23 15:18:14.000000 mongodb_orm-0.0.114/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-23 15:18:14.000000 mongodb_orm-0.0.114/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-23 15:18:14.000000 mongodb_orm-0.0.114/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-23 15:18:14.000000 mongodb_orm-0.0.114/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-23 15:18:14.754808 mongodb_orm-0.0.114/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-23 15:18:03.000000 mongodb_orm-0.0.114/setup.py
```

### Comparing `mongodb_orm-0.0.113/README.md` & `mongodb_orm-0.0.114/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.113/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.114/mongodb_orm/custom_urls/bread_urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import sys
 import importlib.util
-
 from django.conf import settings
 from rest_framework import routers
 from django.urls import path, include
-from ..interfaces.mongodb_model import MongoDBModel
-from ..views.mongodb_api_model_view import MongoDBAPIModelView
+from mongodb_orm.interfaces.mongodb_model import MongoDBModel
+from mongodb_orm.views.mongodb_api_model_view import MongoDBAPIModelView
 
 current_directory = os.path.dirname(os.path.abspath(__file__))
 if hasattr(settings, 'MONGODB_ORM_MODELS_FOLDER'):
     MONGODB_MODELS_PATH = settings.MONGODB_ORM_MODELS_FOLDER
     BASE_DIR = settings.BASE_DIR
 else:
     BASE_DIR = "../.."
```

### Comparing `mongodb_orm-0.0.113/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.114/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 from pymongo.database import Database
 from pymongo.collection import Collection
-from ..types.index import Index
-from ..types.options import Options
-from ..types.Relation import Relation
-from ..singletons.mongodb_singleton_client import MongoDBClient
+from mongodb_orm.types.index import Index
+from mongodb_orm.types.options import Options
+from mongodb_orm.types.Relation import Relation
+from mongodb_orm.singletons.mongodb_singleton_client import MongoDBClient
 
 
 class BaseMongoDBModel:
     """
             Preventing direct Instantiation of this class
     """
```

### Comparing `mongodb_orm-0.0.113/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.114/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import math
-
 import pymongo
 from bson import ObjectId
 from datetime import datetime
 from typing import List, Union, Sequence
-from utils.helpers import Helper
 from pymongo.cursor import Cursor
 from pymongo.collection import Collection
 from pymongo.results import InsertOneResult
-from ..types.index import Index
-from ..types.options import Options
-from ..types.Relation import Relation
-from ..decorators.chained import chained
-from ..exceptions.syntax_exceptions import ChainingError
-from ..interfaces.base_mongodb_model import BaseMongoDBModel
+from mongodb_orm.types.index import Index
+from mongodb_orm.utils.helpers import Helper
+from mongodb_orm.types.options import Options
+from mongodb_orm.types.Relation import Relation
+from mongodb_orm.decorators.chained import chained
+from mongodb_orm.exceptions.syntax_exceptions import ChainingError
+from mongodb_orm.interfaces.base_mongodb_model import BaseMongoDBModel
 
 
 class MongoDBModel(BaseMongoDBModel):
     """
         Public class variables to be overridden by the model
     """
     collection_name: str = ''
```

### Comparing `mongodb_orm-0.0.113/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.0.114/mongodb_orm/management/commands/update_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import pkgutil
 import importlib
 from typing import Union, List, Callable
 from django.core.management import BaseCommand
-from ...types.options import ValidationLevel
-from ...interfaces.mongodb_model import MongoDBModel
-from ...singletons.mongodb_singleton_client import MongoDBClient
+from mongodb_orm.types.options import ValidationLevel
+from mongodb_orm.interfaces.mongodb_model import MongoDBModel
+from mongodb_orm.singletons.mongodb_singleton_client import MongoDBClient
 
 
 class Command(BaseCommand):
     help = """
         Update a specific schema, or update the schema for all collections if a schema is not explicitly provided.
         If a collection model is specified, the command will update the schema for that collection;
         otherwise, the command will iterate over all collections in the database, updating their schemas.
```

### Comparing `mongodb_orm-0.0.113/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.114/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.113/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.114/mongodb_orm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,11 @@
 mongodb_orm/singletons/mongodb_singleton_client.py
 mongodb_orm/types/Relation.py
 mongodb_orm/types/__init__.py
 mongodb_orm/types/index.py
 mongodb_orm/types/logger_object.py
 mongodb_orm/types/model_schema.py
 mongodb_orm/types/options.py
+mongodb_orm/utils/__init__.py
+mongodb_orm/utils/helpers.py
 mongodb_orm/views/__init__.py
 mongodb_orm/views/mongodb_api_model_view.py
```

### Comparing `mongodb_orm-0.0.113/setup.py` & `mongodb_orm-0.0.114/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.113",
+    version="0.0.114",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

