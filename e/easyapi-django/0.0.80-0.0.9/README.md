# Comparing `tmp/easyapi_django-0.0.80.tar.gz` & `tmp/easyapi_django-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyapi_django-0.0.80.tar", last modified: Tue Apr 23 02:55:09 2024, max compression
+gzip compressed data, was "easyapi_django-0.0.9.tar", last modified: Wed Feb 15 04:27:28 2023, max compression
```

## Comparing `easyapi_django-0.0.80.tar` & `easyapi_django-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,18 @@
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2024-04-23 02:55:09.177877 easyapi_django-0.0.80/
--rw-r--r--   0 ssjunior   (501) staff       (20)     1076 2023-02-11 03:15:42.000000 easyapi_django-0.0.80/LICENSE
--rw-r--r--   0 ssjunior   (501) staff       (20)     4896 2024-04-23 02:55:09.177674 easyapi_django-0.0.80/PKG-INFO
--rw-r--r--   0 ssjunior   (501) staff       (20)     4333 2023-02-16 14:48:17.000000 easyapi_django-0.0.80/README.md
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2024-04-23 02:55:09.176331 easyapi_django-0.0.80/easyapi/
--rw-r--r--   0 ssjunior   (501) staff       (20)      406 2024-02-19 03:10:12.000000 easyapi_django-0.0.80/easyapi/__init__.py
--rw-r--r--   0 ssjunior   (501) staff       (20)    32092 2024-04-07 01:50:06.000000 easyapi_django-0.0.80/easyapi/base.py
--rw-r--r--   0 ssjunior   (501) staff       (20)    12730 2023-09-04 06:00:09.000000 easyapi_django-0.0.80/easyapi/calc.py
--rw-r--r--   0 ssjunior   (501) staff       (20)      319 2023-10-03 03:46:40.000000 easyapi_django-0.0.80/easyapi/calc_resource.py
--rw-r--r--   0 ssjunior   (501) staff       (20)     1167 2023-02-16 17:08:06.000000 easyapi_django-0.0.80/easyapi/constants.py
--rw-r--r--   0 ssjunior   (501) staff       (20)     7119 2023-08-21 03:41:03.000000 easyapi_django-0.0.80/easyapi/dates.py
--rw-r--r--   0 ssjunior   (501) staff       (20)      246 2023-04-06 04:11:58.000000 easyapi_django-0.0.80/easyapi/exception.py
--rw-r--r--   0 ssjunior   (501) staff       (20)    25670 2023-02-16 17:12:16.000000 easyapi_django-0.0.80/easyapi/filters.py
--rw-r--r--   0 ssjunior   (501) staff       (20)     2104 2024-04-01 18:06:18.000000 easyapi_django-0.0.80/easyapi/middleware.py
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2024-04-23 02:55:09.176458 easyapi_django-0.0.80/easyapi/orm/
--rw-r--r--   0 ssjunior   (501) staff       (20)      207 2023-04-08 03:44:13.000000 easyapi_django-0.0.80/easyapi/orm/__init__.py
--rw-r--r--   0 ssjunior   (501) staff       (20)     1061 2023-09-13 04:12:44.000000 easyapi_django-0.0.80/easyapi/routes.py
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2024-04-23 02:55:09.176807 easyapi_django-0.0.80/easyapi/tenant/
--rw-r--r--   0 ssjunior   (501) staff       (20)        0 2023-05-13 23:18:12.000000 easyapi_django-0.0.80/easyapi/tenant/__init__.py
--rw-r--r--   0 ssjunior   (501) staff       (20)     1205 2023-10-17 03:42:39.000000 easyapi_django-0.0.80/easyapi/tenant/db_router.py
--rw-r--r--   0 ssjunior   (501) staff       (20)     5978 2024-02-19 03:18:52.000000 easyapi_django-0.0.80/easyapi/tenant/tenant.py
--rw-r--r--   0 ssjunior   (501) staff       (20)      388 2023-02-16 17:12:06.000000 easyapi_django-0.0.80/easyapi/util.py
-drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2024-04-23 02:55:09.177501 easyapi_django-0.0.80/easyapi_django.egg-info/
--rw-r--r--   0 ssjunior   (501) staff       (20)     4896 2024-04-23 02:55:09.000000 easyapi_django-0.0.80/easyapi_django.egg-info/PKG-INFO
--rw-r--r--   0 ssjunior   (501) staff       (20)      499 2024-04-23 02:55:09.000000 easyapi_django-0.0.80/easyapi_django.egg-info/SOURCES.txt
--rw-r--r--   0 ssjunior   (501) staff       (20)        1 2024-04-23 02:55:09.000000 easyapi_django-0.0.80/easyapi_django.egg-info/dependency_links.txt
--rw-r--r--   0 ssjunior   (501) staff       (20)        8 2024-04-23 02:55:09.000000 easyapi_django-0.0.80/easyapi_django.egg-info/top_level.txt
--rw-r--r--   0 ssjunior   (501) staff       (20)      713 2024-04-05 21:46:20.000000 easyapi_django-0.0.80/pyproject.toml
--rw-r--r--   0 ssjunior   (501) staff       (20)       38 2024-04-23 02:55:09.177919 easyapi_django-0.0.80/setup.cfg
+drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:27:28.015940 easyapi_django-0.0.9/
+-rw-r--r--   0 ssjunior   (501) staff       (20)     1076 2023-02-11 03:15:42.000000 easyapi_django-0.0.9/LICENSE
+-rw-r--r--   0 ssjunior   (501) staff       (20)     4535 2023-02-15 04:27:28.015588 easyapi_django-0.0.9/PKG-INFO
+-rw-r--r--   0 ssjunior   (501) staff       (20)     3984 2023-02-11 17:19:30.000000 easyapi_django-0.0.9/README.md
+drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:27:28.013449 easyapi_django-0.0.9/easyapi/
+-rw-r--r--   0 ssjunior   (501) staff       (20)      171 2023-02-11 04:59:19.000000 easyapi_django-0.0.9/easyapi/__init__.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)    23880 2023-02-15 04:26:58.000000 easyapi_django-0.0.9/easyapi/base.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)      231 2022-11-04 05:07:41.000000 easyapi_django-0.0.9/easyapi/exception.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)    25731 2023-02-15 04:17:48.000000 easyapi_django-0.0.9/easyapi/filters.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)      383 2023-02-11 03:26:51.000000 easyapi_django-0.0.9/easyapi/middleware.py
+-rw-r--r--   0 ssjunior   (501) staff       (20)      982 2023-02-11 04:38:30.000000 easyapi_django-0.0.9/easyapi/routes.py
+drwxr-xr-x   0 ssjunior   (501) staff       (20)        0 2023-02-15 04:27:28.014965 easyapi_django-0.0.9/easyapi_django.egg-info/
+-rw-r--r--   0 ssjunior   (501) staff       (20)     4535 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/PKG-INFO
+-rw-r--r--   0 ssjunior   (501) staff       (20)      300 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/SOURCES.txt
+-rw-r--r--   0 ssjunior   (501) staff       (20)        1 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/dependency_links.txt
+-rw-r--r--   0 ssjunior   (501) staff       (20)        8 2023-02-15 04:27:28.000000 easyapi_django-0.0.9/easyapi_django.egg-info/top_level.txt
+-rw-r--r--   0 ssjunior   (501) staff       (20)      675 2023-02-15 04:27:16.000000 easyapi_django-0.0.9/pyproject.toml
+-rw-r--r--   0 ssjunior   (501) staff       (20)       38 2023-02-15 04:27:28.016056 easyapi_django-0.0.9/setup.cfg
```

### Comparing `easyapi_django-0.0.80/LICENSE` & `easyapi_django-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easyapi_django-0.0.80/PKG-INFO` & `easyapi_django-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: easyapi_django
-Version: 0.0.80
+Version: 0.0.9
 Summary: A simple rest api generator for django based on models
-Author-email: Stamatios Stamou Jr <bushier.outsets.0c@icloud.com>
+Author-email: Stamatios Stamou Jr <ssjunior@gmail.com>
 Project-URL: Homepage, https://github.com/ssjunior/easyapi-django
 Project-URL: Bug Tracker, https://github.com/ssjunior/easyapi-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -100,17 +100,14 @@
         'field1', 'field2'
     ]
 
     # define fields returned in a specific object
     edit_fields = [
         'field1', 'field2', 'field3', 'field3'
     ]
-
-    # define operator for searches
-    search_operator = 'icontains'
 ```
 
 ### Count
 
 By default in list calls, the api does not return the total of objects due to slow count in innodb tables used in MySql,
 but, it is very easy to get count objects simple add
 
@@ -126,29 +123,19 @@
 }
 ```
 
 ### Search
 
 To search you can use any field defined above in search_fields.
 The search will be applied in all fields defined using OR.
-By default all searches are made using icontains. You can change it for any allowed Django search operator.
 
 ```
 ?search=value
 ```
 
-To change the search operator define it in you Resource Class
-
-```
-class ResourceName(BaseResource):
-    model = YOUR_DJANGO_MODEL
-
-    search_operator = 'icontains'
-```
-
 ### Filter
 
 To filter just use querystrings. The filter will only be applied in defined fields above in filter_fields.
 
 ```
 ?field_name=value
 ?field_name__lte=value
```

### Comparing `easyapi_django-0.0.80/README.md` & `easyapi_django-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,17 +86,14 @@
         'field1', 'field2'
     ]
 
     # define fields returned in a specific object
     edit_fields = [
         'field1', 'field2', 'field3', 'field3'
     ]
-
-    # define operator for searches
-    search_operator = 'icontains'
 ```
 
 ### Count
 
 By default in list calls, the api does not return the total of objects due to slow count in innodb tables used in MySql,
 but, it is very easy to get count objects simple add
 
@@ -112,29 +109,19 @@
 }
 ```
 
 ### Search
 
 To search you can use any field defined above in search_fields.
 The search will be applied in all fields defined using OR.
-By default all searches are made using icontains. You can change it for any allowed Django search operator.
 
 ```
 ?search=value
 ```
 
-To change the search operator define it in you Resource Class
-
-```
-class ResourceName(BaseResource):
-    model = YOUR_DJANGO_MODEL
-
-    search_operator = 'icontains'
-```
-
 ### Filter
 
 To filter just use querystrings. The filter will only be applied in defined fields above in filter_fields.
 
 ```
 ?field_name=value
 ?field_name__lte=value
```

### Comparing `easyapi_django-0.0.80/easyapi/base.py` & `easyapi_django-0.0.9/easyapi/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,311 +1,212 @@
+# from typing import Any
+
+import decimal
+import importlib
 import json
-import os
 import re
 from functools import reduce
 from urllib import parse
 
 from asgiref.sync import sync_to_async
 from django.db import connections
 from django.db.models import Q
 from django.forms.models import model_to_dict
-from django.http import JsonResponse
 from django.views import View
+
+# import orjson
 import operator
-from redis import asyncio as aioredis
 
-from .filters import Filter as OrmFilter
+from django.http import JsonResponse
+
+from settings.context import session
+
 from .exception import HTTPException
-from .tenant.tenant import aset_tenant
-from settings.env import REDIS_PREFIX
-from settings.settings import COOKIE_ID
 
-re_id = re.compile(r'(.*)\/(?:(?P<uuid>\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b)|(?P<int_id>\d+))(?:\/)?$')
+re_id = re.compile(r'(.*)\/(\d+)(\/.)?$')
 search_regex = re.compile(r'__isnull|__gte|__lte|__lt|__gt|__startswith')
 
-REDIS_SERVER = os.environ['REDIS_SERVER']
-REDIS_DB = 1
+
+def fake_tenant(*args, **kwargs):
+    return 'default'
+
+
+tenant = importlib.find_loader('tenant')
+if tenant:
+    set_tenant = tenant.set_tenant
+    OrmFilter = tenant.Filter
+else:
+    set_tenant = fake_tenant
+    OrmFilter = None
 
 
 async def method_not_allowed(self, **kwargs):
     raise HTTPException(405, 'Method not allowed')
 
 
-def get_edit_related(args, field):
-    result = args['result']
-    model = args['model']
-    obj = args['obj']
-
-    model = model.split('__')
-
-    if len(model) > 1:
-        obj = getattr(obj, model[0])
-        model = '__'. join(model[1:])
-        reduce(get_edit_related, [field], {'model': model, 'obj': obj, 'result': result})
-    else:
-        model = model[0]
-        keys = field.split('__')
-        if len(keys) == 1:
-            obj = getattr(obj, model)
-            result[field] = getattr(obj, field, None)
-            if 'id' not in result:
-                result['id'] = getattr(obj, 'id')
-        else:
-            result[keys[0]] = {}
-            reduce(get_edit_related, keys[1:], {'model': keys[0], 'obj': getattr(obj, model), 'result': result[keys[0]]})
-    return args
-
-
-def get_related_objects(args, model):
-    obj = args[0]
-    result = args[1]
-    count = args[2]
-    parent = args[3]
-    related_models = args[4]
-    related_fields = args[5]
-    model_obj = getattr(obj, model, None)
-
-    if count == 0:
-        # Adicionado para não ser excluído no return_result
-        if model not in related_models:
-            related_models[model] = []
-
-        if model_obj:
-            result[model] = {}
-            for field in related_fields[parent]:
-                result[model][field] = getattr(model_obj, field, None)
-                related_models[model].append(field)
-        else:
-            result[model] = None
+def decoder(obj):
+    # option=orjson.OPT_NON_STR_KEYS | orjson.OPT_NAIVE_UTC
+    # orjson.dumps(list(objects), option=orjson.OPT_NAIVE_UTC)
+    if isinstance(obj, decimal.Decimal):
+        return float(obj)
+
 
-    else:
-        return model_obj, result, count - 1, parent, related_models, related_fields
+# class JsonResponse(JsonResponse):
+#     def render(self, content: Any) -> bytes:
+#         return orjson.dumps(content, option=orjson.OPT_NON_STR_KEYS, default=decoder)
 
 
 class BaseResource(View):
-    authenticated = True
     allowed_methods = ['delete', 'get', 'patch', 'post']
     routes = []
 
-    account_db = 'default'
-    cache = False
-    cache_ttl = 60
-    session_cache = False
-
     limit = 25
     page = 1
     order_by = 'id'
     count_results = False
 
-    id = None
     model = None
     queryset = None
 
     app_label = None
     model_name = None
     contextId = None
 
     fields = []
     all_fields = []
     fk_fields = []
     m2m_fields = []
 
-    related_models = {}
-    list_related_fields = {}
+    related_models = None
+    list_related_fields = None
+    # related_fields = []
     many_to_many_models = {}
 
     filter_fields = []
-    queryset_filter = []
     search_fields = []
     order_fields = []
     list_fields = []
     edit_fields = []
     edit_related_fields = {}
-    edit_set = {}
     edit_exclude_fields = ['_state']
     update_fields = []
-    create_fields = []
 
     default_filter = None
     search_operator = 'icontains'
 
     obj = None
     obj_id = None
     data = None
 
     normalize_list = False
-    normalize_obj = False
-    normalized = False
-
-    diff = {}
-
-    user = None
-    account = None
-    body = None
 
     def __init__(self):
-
-        self.diff = {}
+        user_session = session.get()
+        self.account_id = user_session['account'].id if user_session else None
+        self.account = user_session['account'] if user_session else None
+        self.user = user_session['user'] if user_session else None
 
         if self.model:
             fields = []
             for field in self.model._meta.get_fields():
                 if not field.is_relation:
                     fields.append(field.name)
                     continue
 
                 if field.concrete and field.many_to_many:
                     self.m2m_fields.append(field.name)
                     continue
 
                 if field.concrete and field.many_to_one:
                     self.fk_fields.append(field.name)
-                    fields.append(f'{field.name}_id')
                     continue
 
-                # if not field.concrete and field.one_to_many:
-                #     self.related_fields.append(field.name)
-                #     continue
+                if not field.concrete and field.one_to_many:
+                    #     self.related_fields.append(field.name)
+                    continue
 
             all_fields = [
-                field.name for field in self.model._meta.local_fields
-            ]
+                field.name for field in self.model._meta.local_fields]
             self.all_fields = all_fields + self.m2m_fields
 
             self.fields = fields
             self.list_fields = self.list_fields or fields
 
             if not self.edit_fields:
-                self.edit_fields = [field.column for field in self.model._meta.local_fields]  # + m2m_fields
+                self.edit_fields = fields  # + m2m_fields
 
             self.queryset = self.model.objects
 
     def get_method(self, request, args, kwargs):
         self.request = request
         for route in self.routes:
             match = re.search(route['path'], request.path)
             if match:
                 allowed_methods = route.get('allowed_methods')
-                return getattr(self, route['func']), match.groupdict(), allowed_methods
+                return getattr(self, route['func']), match, allowed_methods
 
         return None, None, None
 
     async def dispatch(self, request, *args, **kwargs) -> None:
-        session = None
-        if request.headers.get('X-Api-Key') and hasattr(request, 'api_session'):
-            # session = request.api_session
-            pass
-        else:
-            session_key = request.COOKIES.get(COOKIE_ID)
-            if session_key:
-                redis = await aioredis.Redis(
-                    host=REDIS_SERVER, db=REDIS_DB, decode_responses=True
-                ).client()
-                prefix = f'{REDIS_PREFIX}:' if REDIS_PREFIX else ''
-                session_key = f'{prefix}sessions:{session_key}'
-                session = await redis.get(session_key)
-                await redis.close()
-                await redis.connection_pool.disconnect()
-                if session:
-                    session = json.loads(session)
-                    self.user = session['user']
-                    self.account = session.get('account')
-
-        if self.authenticated and not session:
-            raise HTTPException(401, 'Not authorized')
-
-        if session and session.get('account'):
-            self.account_db = await aset_tenant(session['account']['id'])
-            self.account_id = session['account']['id']
-
-        self.method = 'get' if request.method == 'HEAD' else request.method.lower()
+        method = "get" if request.method == "HEAD" else request.method.lower()
 
         # func é o método que será executado, caso exista rota personalizada
         func, match, allowed_methods = self.get_method(request, args, kwargs)
 
         if func:
             self.allowed_methods = allowed_methods or self.allowed_methods
 
-        if self.method not in self.allowed_methods:
-            raise HTTPException(405, f'{self.method.upper()} not allowed')
+        if method not in self.allowed_methods:
+            return HTTPException(
+                status=405, detail=f'{method} not allowed'
+            )
 
         if not func:
-            handler = getattr(self, self.method, method_not_allowed)
+            handler = getattr(self, method, method_not_allowed)
 
-        self.cache = self.cache and self.method == 'get'
-        if self.cache:
-            self.cache_key = f'{REDIS_PREFIX}:cache' if REDIS_PREFIX else 'easyapi:cache'
-            if self.session_cache:
-                self.cache_key += f':{session_key}'
-            self.cache_key += f':{request.path}'
-
-            redis = await aioredis.Redis(
-                host=REDIS_SERVER, db=REDIS_DB, decode_responses=True
-            ).client()
-            response = await redis.get(self.cache_key)
-            await redis.close()
-            await redis.connection_pool.disconnect()
-
-            if response:
-                return JsonResponse(json.loads(response), safe=False)
-
-        await self.pre_process(request)
-
-        if self.method in ['get', 'patch']:
-            id_match = re_id.match(request.path_info)
-            if id_match:
-                uuid = id_match.group('uuid')
-                id = id_match.group('int_id')
-                self.id = id or uuid
-
-        if self.method in ['post', 'patch']:
-            if request.content_type != 'multipart/form-data':
-                try:
-                    self.body = json.loads(request.body.decode('utf-8'))
-                except Exception:
-                    raise HTTPException(
-                        400, 'Invalid body'
-                    )
-                await self.hydrate(self.body)
-        else:
-            self.body = None
+        self.build_filters(request)
+        self.paginate(request)
+        self.ordenate(request)
 
-        if self.method == 'get' and not self.id:
-            self.build_filters(request)
-            self.paginate(request)
-            self.ordenate(request)
+        if method in ['post', 'patch']:
+            try:
+                body = json.loads(request.body.decode('utf-8'))
+            except Exception:
+                # Patch/post sem body
+                body = {}
 
-        if self.queryset_filter:
-            self.queryset = self.queryset.filter(**self.queryset_filter)
+            body = self.hydrate(body)
+            request.json = body
+        else:
+            body = None
 
         if func:
-            if self.method in ['post', 'patch']:
-                response = await func(request, match=match, body=self.body)
+            if method in ['post', 'patch']:
+                response = await func(request, match=match.groups(), body=body)
             else:
-                response = await func(request, match=match)
+                response = await func(request, match=match.groups())
         else:
             response = await handler(request)
 
-        if type(response) is dict:
-            response = await self.serialize(response)
+        if type(response) == dict:
+            response = self.serialize(response)
 
         return response
 
     def build_filters(self, request):
         if not self.queryset:
             return
 
         if hasattr(self, 'model_filter'):
             self.queryset = self.queryset.filter(**self.model_filter)
 
-        if request.GET.get('search'):
-            self.search_fields += ['id']
+        if request.GET.get('search') and self.search_fields:
             filters = reduce(
                 operator.or_, [
-                    Q((f'{field}__{self.search_operator}',
+                    Q((f"{field}__{self.search_operator}",
                       request.GET.get('search')))
                     for field in self.search_fields
                 ]
             )
             self.queryset = self.queryset.filter(filters)
 
         params = dict(request.GET)
@@ -380,70 +281,46 @@
                 self.limit = int(limit)
             except Exception:
                 pass
 
     #########################################################
     # Funçoes dentro do Resource
     #########################################################
-    async def serialize(self, result, **kwargs):
-
-        if type(result) is JsonResponse:
+    def serialize(self, result, **kwargs):
+        response = kwargs.get('response')
+        if type(result) == JsonResponse:
             return result
 
-        response = kwargs.get('response')
         if response:
             return response
 
-        if not self.count_results:
-            if isinstance(result, list):
-                for row in result:
-                    await self.dehydrate(row)
-
-            elif type(result) is dict and 'objects' in result:
-                for row in result['objects']:
-                    await self.dehydrate(row)
-            else:
-                await self.dehydrate(result)
-
-        result = await self.post_process(result)
-        await self.save_cache(result)
-
-        return JsonResponse(result, safe=False)
+        if isinstance(result, list):
+            for row in result:
+                self.dehydrate(row)
+        else:
+            result = self.dehydrate(result)
 
-    async def save_cache(self, content):
-        if not self.cache:
-            return
+        return JsonResponse(result)
 
-        redis = await aioredis.Redis(
-            host=REDIS_SERVER, db=REDIS_DB, decode_responses=True
-        ).client()
-        await redis.set(self.cache_key, json.dumps(content))
-        await redis.expire(self.cache_key, self.cache_ttl)
-        await redis.close()
-        await redis.connection_pool.disconnect()
+    def filter_objs(self):
+        pass
 
     async def add_m2m(self, result):
         return await result
 
     async def alter_detail(self, result):
         return result
 
     async def alter_list(self, results):
         return results
 
-    async def hydrate(self, body):
+    def hydrate(self, body):
         return body
 
-    async def pre_process(self, request):
-        return request
-
-    async def dehydrate(self, response):
-        return response
-
-    async def post_process(self, response):
+    def dehydrate(self, response):
         return response
 
     #########################################################
     # GET
     #########################################################
 
     # count só se aplica a listagens
@@ -457,16 +334,16 @@
         query, params = self.queryset.query.sql_with_params()
         table = self.model._meta.db_table
         query = re.sub(
             r'^SELECT .*? FROM',
             f'SELECT count(DISTINCT {table}.id) FROM',
             query,
         )
-
-        connection = connections[self.account_db]
+        account_db = set_tenant(self.account_id)
+        connection = connections[account_db]
         cursor = connection.cursor()
         cursor.execute(query, params)
         count = cursor.fetchone()[0]
 
         self.count_results = {'count': count}
 
     # filtro por segmento/filter só se aplica a listagens
@@ -492,17 +369,14 @@
 
     async def return_results(self, results):
         if self.count_results:
             return self.count_results
 
         results = await self.alter_list(results)
 
-        if self.normalized:
-            return results
-
         if self.normalize_list:
             normalized = {}
             for result in results:
                 normalized[result['id']] = result
             return normalized
 
         result = {}
@@ -524,62 +398,15 @@
                 result['meta']['previous'] = previous_page
 
         result['objects'] = results
         return result
 
     async def get_objs(self, request):
         self.get_filters(request)
-
-        if request.GET.get('count'):
-            return await self.count()
-
-        if self.page > 0:
-            start = (self.page - 1) * self.limit
-        else:
-            start = 0
-
-        if self.list_related_fields:
-            self.queryset = self.queryset.select_related(*self.list_related_fields.keys())
-
-        self.queryset = self.queryset.order_by(
-            self.order_by
-        )
-
-        if self.limit:
-            self.queryset = self.queryset[start:start + self.limit]
-
-        results = []
-
-        fields = request.GET.get('fields')
-        if fields:
-            list_fields = fields.split(',')
-            related = False
-        else:
-            list_fields = self.list_fields
-            related = True
-
-        async for row in self.queryset:
-            result = {}
-            if related:
-                for key, fields in self.list_related_fields.items():
-                    model = key.split('__')
-                    count = len(model) - 1
-                    reduce(
-                        get_related_objects, model, (row, result, count, key, self.related_models, self.list_related_fields)
-                    )
-
-            for field in list_fields:
-                result[field] = getattr(row, field, None)
-
-            results.append(result)
-
-        return results
-
-    async def get_objs_old(self, request):
-        self.get_filters(request)
+        self.filter_objs()
 
         if request.GET.get('count'):
             return await self.count()
 
         if self.page > 0:
             start = (self.page - 1) * self.limit
         else:
@@ -596,152 +423,112 @@
             self.order_by
         )
 
         if self.limit:
             self.queryset = self.queryset[start:start + self.limit]
 
         results = []
-
-        fields = request.GET.get('fields')
-        if fields:
-            values = fields.split(',')
-        else:
-            values = self.list_fields
-
-        async for result in self.queryset.values(*values):
+        async for result in self.queryset.values(*self.list_fields):
             if self.list_related_fields:
                 for key, value in self.list_related_fields.items():
                     result[key] = {}
                     result[key]['id'] = result[f'{key}__id']
                     del result[f'{key}__id']
                     for field in value:
+                        # if result.get(f'{key}__{field}'):
                         try:
                             result[key][field] = result[f'{key}__{field}']
                             del result[f'{key}__{field}']
                         except Exception as err:
                             print('ERRO', err)
 
             results.append(result)
 
         return results
 
     async def return_result(self, result):
+        # if type(result) != dict:
+        #     result = await self.add_m2m(result)
+
         for key in list(result):
-            if (
-                self.edit_fields and
-                key not in self.edit_fields and
-                key not in self.edit_related_fields and
-                key != '_result' and
-                key not in self.related_models
-            ):
+            if self.edit_fields and key not in self.edit_fields and key != '_result':
                 if result.get(key):
                     del result[key]
 
             if self.edit_exclude_fields and key in self.edit_exclude_fields:
                 if result.get(key):
                     del result[key]
 
-            if (
-                key not in self.edit_fields and
-                key not in self.edit_related_fields and
-                key in self.fk_fields and
-                key not in self.related_models and
-                key in result
-            ):
+            if key not in self.edit_fields and key in self.fk_fields and key in result:
                 result[key + '_id'] = {'id': result.pop(key)}
 
         result = await self.alter_detail(result)
-        if self.normalize_obj:
-            normalized = {}
-            normalized[result['id']] = result
-            return await self.serialize(normalized)
 
         return result
 
     async def get_obj(self, id):
-        related_fields = None
-
-        if self.edit_related_fields:
-            related_fields = list(self.edit_related_fields.keys())
-            for key in self.edit_related_fields.keys():
-                for rf in self.edit_related_fields[key]:
-                    rf = rf.split('__')
-                    if len(rf) > 1:
-                        new_rf = key + '__' + '__'.join(rf[:-1])
-                        related_fields.append(new_rf)
-
-            self.queryset = self.queryset.select_related(*related_fields)
+        related_models = list(self.edit_related_fields.keys())
+        if related_models:
+            self.queryset = self.queryset.select_related(*related_models)
 
+        # para uso dentro dos resources
         self.obj = await self.queryset.filter(pk=id).afirst()
+
         if not self.obj:
             raise HTTPException(404, 'Object does not exist')
 
-        result = {}
-
-        for model, fields in self.edit_related_fields.items():
-            final = {}
-            obj = self.obj
+        results = {}
+        for field in self.edit_fields:
+            results[field] = getattr(self.obj, field, None)
 
-            if hasattr(obj, model) and not getattr(obj, model):
-                result[model] = {}
+        for model in related_models:
+            obj = getattr(self.obj, model, None)
+            if not obj:
+                results[model] = None
                 continue
 
-            reduce(get_edit_related, fields, {'model': model, 'obj': obj, 'result': final})
-            result[model] = final
-
-        for field in self.edit_fields:
-            result[field] = getattr(self.obj, field, None)
-
-        for key, value in self.edit_set.items():
-            query = getattr(self.obj, key)
-            result[key] = []
-            async for item in query.values(*value):
-                result[key].append(item)
+            results[model] = {}
+            for field in self.edit_related_fields[model]:
+                results[model][field] = getattr(obj, field, None)
 
-        return result
+        return results
 
     async def _get_objs(self, request):
         data = await self.get_objs(request)
         return await self.return_results(data)
 
     async def get(self, request):
-        if self.id:
-            data = await self.get_obj(self.id)
-            data = await self.alter_detail(data)
-            if self.normalize_obj:
-                normalized = {}
-                normalized[data['id']] = data
-                return await self.serialize(normalized)
-
-            return await self.serialize(data)
+        match = re_id.match(request.path)
+        if match:
+            id = match[2]
+            data = await self.get_obj(id)
+            return self.serialize(data)
         else:
             data = await self._get_objs(request)
-            return await self.serialize(data)
+            return self.serialize(data)
 
     #########################################################
     # DELETE
     #########################################################
     async def delete_obj(self, id):
         try:
             await self.queryset.filter(pk=id).adelete()
         except Exception as err:
             raise HTTPException(400, err.__class__.__name__ + ': ' + err.__str__())
 
         return {'success': True, 'id': id, 'message': 'Deleted'}
 
     async def delete(self, request):
-        id_match = re_id.match(request.path_info)
-        if id_match:
-            uuid = id_match.group('uuid')
-            id = id_match.group('int_id')
-            self.id = id or uuid
-            results = await self.delete_obj(self.id)
-            return await self.serialize(results)
+        match = re_id.match(request.path_info)
+        if match:
+            id = match[2]
+            results = await self.delete_obj(id)
+            return self.serialize(results)
         else:
-            raise HTTPException(404, 'Item not found')
+            raise HTTPException(404, "Item not found")
 
     #########################################################
     # PATCH
     #########################################################
 
     def save_related_tags(self, tags):
         core_tag_model = self.model.tags.field.related_model
@@ -764,43 +551,40 @@
             tag_model.objects.filter(
                 **{tag_field: self.obj.id}
             ).values_list('tag_id', flat=True)
         ]
 
         # Removendo tags
         tag_model.objects.filter(
-            **{tag_field: self.obj.id, 'tag_id__in': set(existing_tags) - set(tags_ids)}
+            **{tag_field: self.obj.id, "tag_id__in": set(existing_tags) - set(tags_ids)}
         ).delete()
 
         # Inserindo tags
         insert_tags = set(tags_ids) - set(existing_tags)
         if insert_tags:
             tag_list = [
                 tag_model(
-                    **{'tag_id': tag_id, tag_field: self.obj.id}
+                    **{"tag_id": tag_id, tag_field: self.obj.id}
                 ) for tag_id in insert_tags
             ]
             tag_model.objects.bulk_create(tag_list)
 
     async def update_obj(self, id, body):
         keys = list(body.keys())
         allowed = False
-        diff = None
         if self.update_fields:
-            diff = list(set(keys) - set(self.update_fields))
-            allowed = not diff
-            diff = (', ').join(list(diff))
+            allowed = all(elem in self.update_fields for elem in keys)
 
         if not allowed:
-            raise HTTPException(403, f'Changes on field(s): {diff} is not allowed')
+            raise HTTPException(403, "Changes on this field is not allowed")
 
         try:
             self.obj = await self.queryset.aget(pk=id)
         except Exception:
-            raise HTTPException(404, 'Item not found')
+            raise HTTPException(404, "Item not found")
 
         to_update = {}
         for key, value in body.items():
             if key == 'tags':
                 self.save_related_tags(value)
 
             elif key == 'custom_attributes':
@@ -809,110 +593,91 @@
 
             else:
                 field = getattr(self.model, key)
                 if field.field.primary_key:
                     key += '_id'
                     value = int(value)
                 to_update[key] = value
-
-                old_value = getattr(self.obj, key)
-                self.diff[key] = {'old': old_value, 'new': value}
-
                 setattr(self.obj, key, value)
 
         await self.model.objects.filter(pk=id).aupdate(**to_update)
 
         return await self.get_obj(id)
 
+    async def _update_obj(self, id, body):
+        self.obj_id = id
+        result = await self.update_obj(id, body)
+        return await self.return_result(result)
+
     async def patch(self, request):
-        result = await self.update_obj(self.id, self.body)
-        result = await self.return_result(result)
-        return await self.serialize(result)
+        try:
+            body = request.json
+        except Exception:
+            return HTTPException(
+                status=400, detail='Invalid body'
+            )
+        match = re_id.match(request.path_info)
+        if match:
+            results = await self._update_obj(match[2], body)
+            return self.serialize(results)
+        else:
+            return HTTPException(status=404, detail="Item not found")
 
     #########################################################
     # POST
     #########################################################
     async def create_obj(self, request, body):
-        keys = list(body.keys())
-        allowed = False
-        diff = None
-        if self.create_fields:
-            diff = list(set(keys) - set(self.create_fields))
-            allowed = not diff
-            diff = (', ').join(diff)
-
-        if not allowed:
-            if self.create_fields:
-                raise HTTPException(403, f'Creation on field(s): {diff} is not allowed')
-            raise HTTPException(500, 'Create fields not defined')
-
         to_save = {}
         user = self.user
 
         if user:
             if 'created_by' in self.all_fields:
-                body['created_by_id'] = user['id']
-            if 'updated_by' in self.all_fields:
-                body['updated_by_id'] = user['id']
+                to_save['created_by_id'] = user.id
             if 'owner' in self.all_fields:
-                body['owner_id'] = user['id']
-
-        blank_errors = []
-        null_errors = []
+                to_save['owner_id'] = user.id
 
         for field in self.model._meta.local_fields:
             if field.primary_key:
                 continue
 
-            allow_blank = field.blank
-            allow_null = field.null
-            default = field.has_default() or hasattr(field, 'auto_now') or hasattr(field, 'auto_now_add')
-
-            field_key = f'{field.name}_id' if field.is_relation else field.name
-
-            field_value = body.get(field_key)
+            field_key = field.name
+            if field.many_to_one:
+                field_key = field.name + '_id'
 
-            if not default and not allow_blank and field_value == '':
-                blank_errors.append(field.verbose_name)
-
-            if not default and not allow_null and not field_value:
-                null_errors.append(field.verbose_name)
-
-            if body.get(field_key) is not None:
+            if body.get(field_key):
                 to_save[field_key] = body[field_key]
 
-        if blank_errors or null_errors:
-            errors = ''
-            if blank_errors:
-                errors += 'Field(s): ' + ', '.join(blank_errors) + ' can\'t be blank. '
-
-            if null_errors:
-                errors += 'Field(s): ' + ', '.join(null_errors) + ' can\'t be null.'
-
-            raise HTTPException(403, errors)
-
+        # try:
         obj = await self.model.objects.acreate(**to_save)
+        # except Exception as err:
+        #     error = err.__str__()
+        #     return HTTPException(
+        #         status=400, detail=error
+        #     )
 
         self.obj = obj
         self.obj_id = obj.id
         result = await self.get_obj(obj.id)
         return await self.return_result(result)
 
     async def post(self, request):
         match = re_id.match(request.path_info)
         if match:
-            raise HTTPException(403, 'Path not allowed')
+            return HTTPException(status=403, detail="Not allowed")
 
-        try:
-            result = await self.create_obj(request, self.body)
-        except Exception as err:
-            error = err.__str__()
-            raise HTTPException(400, error)
+        body = request.json
+        # try:
+        result = await self.create_obj(request, body)
+        # except Exception as err:
+        #     error = err.__str__()
+        #     return HTTPException(
+        #         status=400, detail=error
+        #     )
 
-        return await self.serialize(result)
+        return self.serialize(result)
 
 
 class BaseTagsResource(BaseResource):
 
     async def add_m2m(self, result):
         super().add_m2m(result)
```

### Comparing `easyapi_django-0.0.80/easyapi/filters.py` & `easyapi_django-0.0.9/easyapi/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from django.db.models import Func, Q, IntegerField, CharField, FloatField
 from django.db.models.functions import Concat
 from django.utils import timezone
 from operator import __or__ as OR
 from operator import __and__ as AND
 from pytz import timezone as pytz_timezone
 
-from .constants import CustomAttributePresentations
-from .dates import Dates
-from .util import make_list, normalize_field
+from constants.custom_attributes import CustomAttributePresentations
+from util.date import Dates
+from ._util import normalize_field
+from util import make_list
 
 
 CHAR = [
     'CharField', 'BinaryField', 'FileField', 'FilePathField', 'IPAddressField',
     'GenericIPAddressField', 'SlugField', 'TextField', 'UUIDField'
 ]
 
@@ -398,17 +399,17 @@
                         custom_attributes__name=custom,
                         custom_attributes__presentation_id=CustomAttributePresentations.CHECKBOX
                     )
 
                     if is_checkbox and value == 'false':
 
                         false_list = [pk for pk in self.working_model.filter(**{
-                            'custom_attributes__name': custom,
-                            '{}__{}'.format(custom_field, operator): value
-                        }).values_list('pk', flat=True)]
+                                'custom_attributes__name': custom,
+                                '{}__{}'.format(custom_field, operator): value
+                            }).values_list('pk', flat=True)]
 
                         _filter.update({
                             'pk__in': [pk for pk in self.working_model.exclude(
                                 custom_attributes__name=custom
                             ).values_list('pk', flat=True)] + false_list or [0]
                         })
 
@@ -438,17 +439,17 @@
                                 end_date = f'{end_date}'[:19]
                                 value = (start_date, end_date)
 
                         elif operator in ['lte', 'gte']:
                             value = CastFloat(value)
 
                         working_model = self.working_model.filter(**{
-                            'custom_attributes__name': custom,
-                            '{}__{}'.format(custom_field, operator): value
-                        })
+                                'custom_attributes__name': custom,
+                                '{}__{}'.format(custom_field, operator): value
+                            })
 
                         ids = set(working_model.values_list(
                             'pk', flat=True
                         ))
                         null_list = set(null_list)
                         pks = list(ids.difference(null_list))
```

### Comparing `easyapi_django-0.0.80/easyapi/routes.py` & `easyapi_django-0.0.9/easyapi/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from django.urls import path, re_path
 from django.http import HttpResponse
 
-from .calc_resource import Metrics
-
 
 def get_route(route, view):
     if hasattr(view, 'as_view'):
         view = view.as_view()
         return re_path(rf'{route}', view)
 
     return path(route, view)
@@ -32,9 +30,8 @@
 
         return HttpResponse('Docs')
 
     return [
         get_route(key, value) for key, value in endpoints.items()
     ] + [
         path('docs', docs),
-        path('metrics', Metrics.as_view())
     ]
```

### Comparing `easyapi_django-0.0.80/easyapi_django.egg-info/PKG-INFO` & `easyapi_django-0.0.9/easyapi_django.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: easyapi_django
-Version: 0.0.80
+Name: easyapi-django
+Version: 0.0.9
 Summary: A simple rest api generator for django based on models
-Author-email: Stamatios Stamou Jr <bushier.outsets.0c@icloud.com>
+Author-email: Stamatios Stamou Jr <ssjunior@gmail.com>
 Project-URL: Homepage, https://github.com/ssjunior/easyapi-django
 Project-URL: Bug Tracker, https://github.com/ssjunior/easyapi-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -100,17 +100,14 @@
         'field1', 'field2'
     ]
 
     # define fields returned in a specific object
     edit_fields = [
         'field1', 'field2', 'field3', 'field3'
     ]
-
-    # define operator for searches
-    search_operator = 'icontains'
 ```
 
 ### Count
 
 By default in list calls, the api does not return the total of objects due to slow count in innodb tables used in MySql,
 but, it is very easy to get count objects simple add
 
@@ -126,29 +123,19 @@
 }
 ```
 
 ### Search
 
 To search you can use any field defined above in search_fields.
 The search will be applied in all fields defined using OR.
-By default all searches are made using icontains. You can change it for any allowed Django search operator.
 
 ```
 ?search=value
 ```
 
-To change the search operator define it in you Resource Class
-
-```
-class ResourceName(BaseResource):
-    model = YOUR_DJANGO_MODEL
-
-    search_operator = 'icontains'
-```
-
 ### Filter
 
 To filter just use querystrings. The filter will only be applied in defined fields above in filter_fields.
 
 ```
 ?field_name=value
 ?field_name__lte=value
```

### Comparing `easyapi_django-0.0.80/pyproject.toml` & `easyapi_django-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [build-system]
 requires = [
-    "Django>=4.2",
-    "pandas",
-    "pytz",
-    "redis",
     "setuptools>=42",
     "wheel",
+    "Django>=4.1.3",
+    "pytz"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "easyapi_django"
-version = "0.0.80"
+version = "0.0.9"
 authors = [
-  { name="Stamatios Stamou Jr", email="bushier.outsets.0c@icloud.com" },
+  { name="Stamatios Stamou Jr", email="ssjunior@gmail.com" },
 ]
 description = "A simple rest api generator for django based on models"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

