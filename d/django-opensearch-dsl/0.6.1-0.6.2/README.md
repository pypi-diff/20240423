# Comparing `tmp/django_opensearch_dsl-0.6.1.tar.gz` & `tmp/django_opensearch_dsl-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_opensearch_dsl-0.6.1.tar", last modified: Sat Apr 13 21:23:39 2024, max compression
+gzip compressed data, was "django_opensearch_dsl-0.6.2.tar", last modified: Tue Apr 23 21:42:34 2024, max compression
```

## Comparing `django_opensearch_dsl-0.6.1.tar` & `django_opensearch_dsl-0.6.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.895295 django_opensearch_dsl-0.6.1/django_opensearch_dsl/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/indices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14826 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1701 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/django_opensearch_dsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14826 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/commands/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-04-23 21:42:34.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 21:42:34.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:42:34.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 21:42:34.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 21:42:34.000000 django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-23 21:42:34.920950 django_opensearch_dsl-0.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1701 2024-04-23 21:42:29.000000 django_opensearch_dsl-0.6.2/setup.py
```

### Comparing `django_opensearch_dsl-0.6.1/CONTRIBUTING.md` & `django_opensearch_dsl-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/LICENSE` & `django_opensearch_dsl-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/PKG-INFO` & `django_opensearch_dsl-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-opensearch-dsl
-Version: 0.6.1
+Version: 0.6.2
 Summary: Wrapper around opensearch-py for django models
 Home-page: https://github.com/qcoumes/django-opensearch-dsl
 Author: Quentin Coumes (Codoc)
 Author-email: coumes.quentin@gmail.com
 License: Apache Software License 2.0
 Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py
 Classifier: Development Status :: 4 - Beta
@@ -151,14 +151,20 @@
         # Paginate the django queryset used to populate the index with the specified size
         # This per-Document setting overrides settings.OPENSEARCH_DSL_QUERYSET_PAGINATION.
         queryset_pagination = 5000
 ```
 
 # Changelog
 
+### 0.6.2 (2024-04-23)
+
+* Fix `CelerySignalProcessor` previously using `RealTimeSignalProcessor`'s method due to wrong indentation ([#66](https://github.com/Codoc-os/django-opensearch-dsl/pull/66)),
+  Contributed by [jlariza](https://github.com/jlariza).
+* `models.PositiveBigIntegerField` is now automatically mapped to `LongField` ([#67](https://github.com/Codoc-os/django-opensearch-dsl/pull/67)), Contributed by [jlariza](https://github.com/jlariza).
+
 ### 0.6.1 (2024-04-13)
 
 * Multiple fixes to `CelerySignalProcessor` ([#62](https://github.com/Codoc-os/django-opensearch-dsl/pull/63)),
   Contributed by [Jordan Hyatt](https://github.com/JordanHyatt) and [jlariza](https://github.com/jlariza).
   * Correctly use `.delay` when calling tasks.
   * Only initiate tasks when needed by checking beforehand if an instance is connected to a Document (directly or related)
   * The tasks will only be created on transaction commit.
```

### Comparing `django_opensearch_dsl-0.6.1/README.md` & `django_opensearch_dsl-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/apps.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/apps.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/documents.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/documents.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     models.EmailField: fields.TextField,
     models.FileField: fields.FileField,
     models.FilePathField: fields.KeywordField,
     models.FloatField: fields.DoubleField,
     models.ImageField: fields.FileField,
     models.IntegerField: fields.IntegerField,
     models.NullBooleanField: fields.BooleanField,
+    models.PositiveBigIntegerField: fields.LongField,
     models.PositiveIntegerField: fields.IntegerField,
     models.PositiveSmallIntegerField: fields.ShortField,
     models.SlugField: fields.KeywordField,
     models.SmallIntegerField: fields.ShortField,
     models.TextField: fields.TextField,
     models.TimeField: fields.LongField,
     models.URLField: fields.TextField,
@@ -56,18 +57,26 @@
         self._related_instance_to_ignore = related_instance_to_ignore
         self._prepared_fields = self.init_prepare()
 
     @classmethod
     def search(cls, using=None, index=None):
         """Return a `Search` object parametrized with the index' information."""
         return Search(
-            using=cls._get_using(using), index=cls._default_index(index), doc_type=[cls], model=cls.django.model
+            using=cls._get_using(using),
+            index=cls._default_index(index),
+            doc_type=[cls],
+            model=cls.django.model,
         )
 
-    def get_queryset(self, filter_: Optional[Q] = None, exclude: Optional[Q] = None, count: int = None) -> QuerySet:
+    def get_queryset(
+        self,
+        filter_: Optional[Q] = None,
+        exclude: Optional[Q] = None,
+        count: int = None,
+    ) -> QuerySet:
         """Return the queryset that should be indexed by this doc type."""
         qs = self.django.model.objects.all()
 
         if filter_:
             qs = qs.filter(filter_)
         if exclude:
             qs = qs.exclude(exclude)
@@ -140,15 +149,18 @@
             if prep_func:
                 fn = partial(prep_func, related_to_ignore=self._related_instance_to_ignore)
             else:
                 prep_func = getattr(self, "prepare_%s" % name, None)
                 if prep_func:
                     fn = prep_func
                 else:
-                    fn = partial(field.get_value_from_instance, field_value_to_ignore=self._related_instance_to_ignore)
+                    fn = partial(
+                        field.get_value_from_instance,
+                        field_value_to_ignore=self._related_instance_to_ignore,
+                    )
 
             preparers.append((name, field, fn))
 
         return preparers
 
     def prepare(self, instance):
         """Generate the opensearch's document from `instance` based on defined fields."""
@@ -229,8 +241,14 @@
             refresh = getattr(self.Index, "auto_refresh", DODConfig.auto_refresh_enabled())
 
         if isinstance(thing, models.Model):
             object_list = [thing]
         else:
             object_list = thing
 
-        return self._bulk(self._get_actions(object_list, action), *args, refresh=refresh, using=using, **kwargs)
+        return self._bulk(
+            self._get_actions(object_list, action),
+            *args,
+            refresh=refresh,
+            using=using,
+            **kwargs,
+        )
```

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/fields.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/fields.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/indices.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/indices.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/opensearch.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/commands/opensearch.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/enums.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/enums.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/types.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/management/types.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/registries.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/registries.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/search.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/search.py`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl/signals.py` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,29 +112,29 @@
     class CelerySignalProcessor(RealTimeSignalProcessor):
         """Celery signal processor.
 
         Allows automatic updates on the index as delayed background tasks using
         Celery.
         """
 
-    def handle_save(self, sender, instance, **kwargs):
-        """Update the instance in model and associated model indices."""
-        if self.instance_requires_update(instance):
-            transaction.on_commit(
-                partial(
-                    handle_save_task.delay,
-                    app_label=instance._meta.app_label,
-                    model=instance.__class__.__name__,
-                    pk=instance.pk,
+        def handle_save(self, sender, instance, **kwargs):
+            """Update the instance in model and associated model indices."""
+            if self.instance_requires_update(instance):
+                transaction.on_commit(
+                    partial(
+                        handle_save_task.delay,
+                        app_label=instance._meta.app_label,
+                        model=instance.__class__.__name__,
+                        pk=instance.pk,
+                    )
                 )
-            )
 
-    def handle_pre_delete(self, sender, instance, **kwargs):
-        """Delete the instance from model and associated model indices."""
-        if self.instance_requires_update(instance):
-            handle_pre_delete_task.delay(
-                serialize(
-                    "json",
-                    [instance],
-                    cls=DODConfig.signal_processor_serializer_class(),
+        def handle_pre_delete(self, sender, instance, **kwargs):
+            """Delete the instance from model and associated model indices."""
+            if self.instance_requires_update(instance):
+                handle_pre_delete_task.delay(
+                    serialize(
+                        "json",
+                        [instance],
+                        cls=DODConfig.signal_processor_serializer_class(),
+                    )
                 )
-            )
```

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/PKG-INFO` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-opensearch-dsl
-Version: 0.6.1
+Version: 0.6.2
 Summary: Wrapper around opensearch-py for django models
 Home-page: https://github.com/qcoumes/django-opensearch-dsl
 Author: Quentin Coumes (Codoc)
 Author-email: coumes.quentin@gmail.com
 License: Apache Software License 2.0
 Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py
 Classifier: Development Status :: 4 - Beta
@@ -151,14 +151,20 @@
         # Paginate the django queryset used to populate the index with the specified size
         # This per-Document setting overrides settings.OPENSEARCH_DSL_QUERYSET_PAGINATION.
         queryset_pagination = 5000
 ```
 
 # Changelog
 
+### 0.6.2 (2024-04-23)
+
+* Fix `CelerySignalProcessor` previously using `RealTimeSignalProcessor`'s method due to wrong indentation ([#66](https://github.com/Codoc-os/django-opensearch-dsl/pull/66)),
+  Contributed by [jlariza](https://github.com/jlariza).
+* `models.PositiveBigIntegerField` is now automatically mapped to `LongField` ([#67](https://github.com/Codoc-os/django-opensearch-dsl/pull/67)), Contributed by [jlariza](https://github.com/jlariza).
+
 ### 0.6.1 (2024-04-13)
 
 * Multiple fixes to `CelerySignalProcessor` ([#62](https://github.com/Codoc-os/django-opensearch-dsl/pull/63)),
   Contributed by [Jordan Hyatt](https://github.com/JordanHyatt) and [jlariza](https://github.com/jlariza).
   * Correctly use `.delay` when calling tasks.
   * Only initiate tasks when needed by checking beforehand if an instance is connected to a Document (directly or related)
   * The tasks will only be created on transaction commit.
```

### Comparing `django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/SOURCES.txt` & `django_opensearch_dsl-0.6.2/django_opensearch_dsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/docs/CHANGELOG.md` & `django_opensearch_dsl-0.6.2/docs/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+### 0.6.2 (2024-04-23)
+
+* Fix `CelerySignalProcessor` previously using `RealTimeSignalProcessor`'s method due to wrong indentation ([#66](https://github.com/Codoc-os/django-opensearch-dsl/pull/66)),
+  Contributed by [jlariza](https://github.com/jlariza).
+* `models.PositiveBigIntegerField` is now automatically mapped to `LongField` ([#67](https://github.com/Codoc-os/django-opensearch-dsl/pull/67)), Contributed by [jlariza](https://github.com/jlariza).
+
 ### 0.6.1 (2024-04-13)
 
 * Multiple fixes to `CelerySignalProcessor` ([#62](https://github.com/Codoc-os/django-opensearch-dsl/pull/63)),
   Contributed by [Jordan Hyatt](https://github.com/JordanHyatt) and [jlariza](https://github.com/jlariza).
   * Correctly use `.delay` when calling tasks.
   * Only initiate tasks when needed by checking beforehand if an instance is connected to a Document (directly or related)
   * The tasks will only be created on transaction commit.
```

### Comparing `django_opensearch_dsl-0.6.1/setup.cfg` & `django_opensearch_dsl-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_opensearch_dsl-0.6.1/setup.py` & `django_opensearch_dsl-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 EXTRA_REQUIREMENTS = {
     'celery': ["celery>=4.1.0"],
 }
 
 setup(
     name='django-opensearch-dsl',
-    version='0.6.1',
+    version='0.6.2',
     description="""Wrapper around opensearch-py for django models""",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Quentin Coumes (Codoc)',
     author_email='coumes.quentin@gmail.com',
     url='https://github.com/qcoumes/django-opensearch-dsl',
     packages=['django_opensearch_dsl'],
```

