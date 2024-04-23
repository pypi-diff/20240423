# Comparing `tmp/drfexts-3.8.3.tar.gz` & `tmp/drfexts-3.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfexts-3.8.3.tar", max compression
+gzip compressed data, was "drfexts-3.8.4.tar", max compression
```

## Comparing `drfexts-3.8.3.tar` & `drfexts-3.8.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.8.3/LICENSE
--rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.8.3/README.md
--rw-r--r--   0        0        0       22 2024-04-16 10:31:27.000400 drfexts-3.8.3/drfexts/__init__.py
--rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.8.3/drfexts/authentication.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.8.3/drfexts/choices.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.8.3/drfexts/constants.py
--rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.8.3/drfexts/exceptions.py
--rw-r--r--   0        0        0    14579 2024-02-19 06:44:03.902452 drfexts-3.8.3/drfexts/fields.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.8.3/drfexts/filtersets/__init__.py
--rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.8.3/drfexts/filtersets/backends.py
--rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.8.3/drfexts/filtersets/fields.py
--rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.8.3/drfexts/filtersets/filters.py
--rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.8.3/drfexts/filtersets/widgets.py
--rw-r--r--   0        0        0      534 2024-04-09 09:51:19.663972 drfexts-3.8.3/drfexts/middlewares.py
--rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.8.3/drfexts/models.py
--rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.8.3/drfexts/pagination.py
--rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.8.3/drfexts/paginators.py
--rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.8.3/drfexts/parsers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.8.3/drfexts/permissions.py
--rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.8.3/drfexts/renderers.py
--rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.8.3/drfexts/routers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.8.3/drfexts/serializers/__init__.py
--rw-r--r--   0        0        0    11825 2024-04-16 10:30:55.229868 drfexts-3.8.3/drfexts/serializers/fields.py
--rw-r--r--   0        0        0     4748 2024-04-09 09:51:46.898835 drfexts-3.8.3/drfexts/serializers/mixins.py
--rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.8.3/drfexts/serializers/serializers.py
--rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.8.3/drfexts/settings.py
--rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.8.3/drfexts/storages.py
--rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.8.3/drfexts/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.8.3/drfexts/utils/encoders.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.8.3/drfexts/utils/log.py
--rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.8.3/drfexts/utils/string.py
--rw-r--r--   0        0        0     3976 2024-04-15 02:12:05.521855 drfexts-3.8.3/drfexts/utils/utils.py
--rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.8.3/drfexts/viewsets.py
--rw-r--r--   0        0        0     1649 2024-04-16 10:31:27.006487 drfexts-3.8.3/pyproject.toml
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 drfexts-3.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.8.4/LICENSE
+-rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.8.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-22 08:42:05.860518 drfexts-3.8.4/drfexts/__init__.py
+-rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.8.4/drfexts/authentication.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.8.4/drfexts/choices.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.8.4/drfexts/constants.py
+-rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.8.4/drfexts/exceptions.py
+-rw-r--r--   0        0        0    14673 2024-04-22 08:41:55.352402 drfexts-3.8.4/drfexts/fields.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.8.4/drfexts/filtersets/__init__.py
+-rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.8.4/drfexts/filtersets/backends.py
+-rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.8.4/drfexts/filtersets/fields.py
+-rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.8.4/drfexts/filtersets/filters.py
+-rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.8.4/drfexts/filtersets/widgets.py
+-rw-r--r--   0        0        0      534 2024-04-09 09:51:19.663972 drfexts-3.8.4/drfexts/middlewares.py
+-rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.8.4/drfexts/models.py
+-rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.8.4/drfexts/pagination.py
+-rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.8.4/drfexts/paginators.py
+-rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.8.4/drfexts/parsers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.8.4/drfexts/permissions.py
+-rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.8.4/drfexts/renderers.py
+-rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.8.4/drfexts/routers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.8.4/drfexts/serializers/__init__.py
+-rw-r--r--   0        0        0    11857 2024-04-22 07:53:44.283450 drfexts-3.8.4/drfexts/serializers/fields.py
+-rw-r--r--   0        0        0     4748 2024-04-09 09:51:46.898835 drfexts-3.8.4/drfexts/serializers/mixins.py
+-rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.8.4/drfexts/serializers/serializers.py
+-rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.8.4/drfexts/settings.py
+-rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.8.4/drfexts/storages.py
+-rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.8.4/drfexts/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.8.4/drfexts/utils/encoders.py
+-rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.8.4/drfexts/utils/log.py
+-rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.8.4/drfexts/utils/string.py
+-rw-r--r--   0        0        0     3976 2024-04-15 02:12:05.521855 drfexts-3.8.4/drfexts/utils/utils.py
+-rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.8.4/drfexts/viewsets.py
+-rw-r--r--   0        0        0     1650 2024-04-22 08:42:05.866574 drfexts-3.8.4/pyproject.toml
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 drfexts-3.8.4/PKG-INFO
```

### Comparing `drfexts-3.8.3/LICENSE` & `drfexts-3.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/README.md` & `drfexts-3.8.4/README.md`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/choices.py` & `drfexts-3.8.4/drfexts/choices.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/constants.py` & `drfexts-3.8.4/drfexts/constants.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/exceptions.py` & `drfexts-3.8.4/drfexts/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/fields.py` & `drfexts-3.8.4/drfexts/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import uuid
 from functools import partial
 
+import django
 from django import forms
 from django.conf import settings
 from django.contrib.contenttypes import fields as ct_fields
 from django.contrib.postgres.fields import ArrayField as PGArrayField
 from django.core import checks
 from django.db import models
 from django.db.models import CASCADE
@@ -236,30 +237,32 @@
     """
     update_datetime = ModifyDateTimeField()
     """
 
     def __init__(self, verbose_name="修改时间", **kwargs):
         kwargs["editable"] = False
         kwargs["auto_now"] = True
-        kwargs["db_default"] = Now()
+        if django.VERSION > (5, 0):
+            kwargs["db_default"] = Now()
         kwargs.setdefault("db_comment", verbose_name)
         kwargs.setdefault("help_text", "该记录的最后修改时间")
         kwargs.setdefault("blank", True)
         super().__init__(verbose_name, **kwargs)
 
 
 class CreatedAtField(models.DateTimeField):
     """
     create_datetime = CreateDateTimeField()
     """
 
     def __init__(self, verbose_name="创建时间", **kwargs):
         kwargs["editable"] = False
         kwargs["auto_now_add"] = True
-        kwargs["db_default"] = Now()
+        if django.VERSION > (5, 0):
+            kwargs["db_default"] = Now()
         kwargs.setdefault("db_comment", verbose_name)
         kwargs.setdefault("help_text", "该记录的创建时间")
         kwargs.setdefault("blank", True)
         super().__init__(verbose_name, **kwargs)
 
 
 class CreatedByField(CurrentUserField):
```

### Comparing `drfexts-3.8.3/drfexts/filtersets/backends.py` & `drfexts-3.8.4/drfexts/filtersets/backends.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/filtersets/fields.py` & `drfexts-3.8.4/drfexts/filtersets/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/filtersets/filters.py` & `drfexts-3.8.4/drfexts/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/filtersets/widgets.py` & `drfexts-3.8.4/drfexts/filtersets/widgets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/middlewares.py` & `drfexts-3.8.4/drfexts/middlewares.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/models.py` & `drfexts-3.8.4/drfexts/models.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/pagination.py` & `drfexts-3.8.4/drfexts/pagination.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/paginators.py` & `drfexts-3.8.4/drfexts/paginators.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/parsers.py` & `drfexts-3.8.4/drfexts/parsers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/renderers.py` & `drfexts-3.8.4/drfexts/renderers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/serializers/fields.py` & `drfexts-3.8.4/drfexts/serializers/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,16 @@
         self.values_to_choice_strings = dict(self.choices)
 
     choices = property(ChoiceField._get_choices, _set_choices)
 
 
 class ChoiceSerializer(Serializer):
     id = CharField(label="值")
-    label = CharField(required=False, label="键")
-    color = CharField(required=False, label="颜色", allow_null=True)
+    label = CharField(required=False, read_only=True, label="键")
+    color = CharField(required=False, read_only=True, label="颜色", allow_null=True)
 
 
 @extend_schema_field(ChoiceSerializer())
 class ChoiceObjectField(ChoiceField):
     def to_internal_value(self, data):
         if isinstance(data, dict):
             data = data.get("id")
```

### Comparing `drfexts-3.8.3/drfexts/serializers/mixins.py` & `drfexts-3.8.4/drfexts/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/serializers/serializers.py` & `drfexts-3.8.4/drfexts/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/settings.py` & `drfexts-3.8.4/drfexts/settings.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/storages.py` & `drfexts-3.8.4/drfexts/storages.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/utils/utils.py` & `drfexts-3.8.4/drfexts/utils/utils.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/drfexts/viewsets.py` & `drfexts-3.8.4/drfexts/viewsets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.3/pyproject.toml` & `drfexts-3.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.commitizen]
-version = "3.8.3"
+version = "3.8.4"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = ["pyproject.toml:version", "drfexts/__init__.py"]
 
 [tool.poetry]
 name = "drfexts"
-version = "3.8.3"
+version = "3.8.4"
 package-mode = true
 readme = "README.md"
 description = "Django Restframework Utils"
 authors = ["aiden <allaher@icloud.com>"]
 keywords = ["django", "restframework"]
 homepage = "https://github.com/aiden520/drfexts"
 repository = "https://github.com/aiden520/drfexts"
 license = "Apache-2.0"
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0.0"
-django = "^5.0"
+django = ">=4.2"
 django-storages = ">=1.12.3"
 django-filter = ">=21.1"
 djangorestframework = "^3.15.1"
 pip = ">=21.3.1"
 djangorestframework-csv = ">=2.1.1"
 openpyxl = ">=3.0.9"
 orjson = "^3.9.15"
```

### Comparing `drfexts-3.8.3/PKG-INFO` & `drfexts-3.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: drfexts
-Version: 3.8.3
+Version: 3.8.4
 Summary: Django Restframework Utils
 Home-page: https://github.com/aiden520/drfexts
 License: Apache-2.0
 Keywords: django,restframework
 Author: aiden
 Author-email: allaher@icloud.com
 Requires-Python: >=3.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: django (>=5.0,<6.0)
+Requires-Dist: django (>=4.2)
 Requires-Dist: django-currentuser (>=0.5.3)
 Requires-Dist: django-filter (>=21.1)
 Requires-Dist: django-storages (>=1.12.3)
 Requires-Dist: djangorestframework (>=3.15.1,<4.0.0)
 Requires-Dist: djangorestframework-csv (>=2.1.1)
 Requires-Dist: drf-flex-fields (>=0.9.8)
 Requires-Dist: openpyxl (>=3.0.9)
```

