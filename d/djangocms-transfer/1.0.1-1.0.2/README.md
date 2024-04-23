# Comparing `tmp/djangocms-transfer-1.0.1.tar.gz` & `tmp/djangocms_transfer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-transfer-1.0.1.tar", last modified: Mon Mar 13 10:10:00 2023, max compression
+gzip compressed data, was "djangocms_transfer-1.0.2.tar", last modified: Tue Apr 23 06:05:14 2024, max compression
```

## Comparing `djangocms-transfer-1.0.1.tar` & `djangocms_transfer-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.436732 djangocms-transfer-1.0.1/djangocms_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/cms_toolbars.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.436732 djangocms-transfer-1.0.1/djangocms_transfer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.436732 djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/css/transfer.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/img/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/img/icons.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.436732 djangocms-transfer-1.0.1/djangocms_transfer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/djangocms_transfer/templates/djangocms_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/templates/djangocms_transfer/import_plugins.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/templates/djangocms_transfer/placeholder_close_frame.html
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/djangocms_transfer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-03-13 10:10:00.000000 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-13 10:10:00.000000 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 10:10:00.000000 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 10:10:00.000000 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-13 10:10:00.000000 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 10:10:00.000000 djangocms-transfer-1.0.1/djangocms_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:10:00.440732 djangocms-transfer-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-13 10:09:41.000000 djangocms-transfer-1.0.1/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.271211 djangocms_transfer-1.0.2/djangocms_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/cms_toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.271211 djangocms_transfer-1.0.2/djangocms_transfer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.271211 djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/css/transfer.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/img/icons.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.271211 djangocms_transfer-1.0.2/djangocms_transfer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/djangocms_transfer/templates/djangocms_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/templates/djangocms_transfer/import_plugins.html
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/templates/djangocms_transfer/placeholder_close_frame.html
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/djangocms_transfer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-23 06:05:14.000000 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-23 06:05:14.000000 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:05:14.000000 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:05:14.000000 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 06:05:14.000000 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 06:05:14.000000 djangocms_transfer-1.0.2/djangocms_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:14.275212 djangocms_transfer-1.0.2/tests/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/transfer/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/transfer/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/transfer/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-23 06:05:06.000000 djangocms_transfer-1.0.2/tests/transfer/test_import.py
```

### Comparing `djangocms-transfer-1.0.1/LICENSE` & `djangocms_transfer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-transfer-1.0.1/PKG-INFO` & `djangocms_transfer-1.0.2/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: djangocms-transfer
-Version: 1.0.1
-Summary: Adds import and export of plugin data.
-Home-page: https://github.com/django-cms/djangocms-transfer
-Author: Divio AG
-Author-email: info@divio.ch
-Maintainer: Django CMS Association and contributors
-Maintainer-email: info@django-cms.org
-License: BSD-3-Clause
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django CMS
-Classifier: Framework :: Django CMS :: 3.7
-Classifier: Framework :: Django CMS :: 3.8
-Classifier: Framework :: Django CMS :: 3.9
-Classifier: Framework :: Django CMS :: 3.10
-Classifier: Framework :: Django CMS :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE
-
 ===================
 django CMS Transfer
 ===================
 
 |pypi| |build| |coverage|
 
 **django CMS Transfer** is an **experimental** package that allows you to export
@@ -89,24 +53,75 @@
 For a manual install:
 
 * run ``pip install djangocms-transfer``
 * add ``djangocms_transfer`` to your ``INSTALLED_APPS``
 * run ``python manage.py migrate djangocms_transfer``
 
 
+Customization
+-------------
+
+Following settings are available:
+
+* **DJANGOCMS_TRANSFER_PROCESS_EXPORT_PLUGIN_DATA**:
+
+  Enables processing of plugin instances prior to serialization, e.g.
+  ``myapp.module.function``.
+
+* **DJANGOCMS_TRANSFER_PROCESS_IMPORT_PLUGIN_DATA**:
+
+  Enables processing of plugin instances prior to saving, e.g.
+  ``myapp.module.function``.
+  For example: set default-values for ForeignKeys (images for django_filer, ..)
+
+As an example the combination of ``_PROCESS_EXPORT_PLUGIN_DATA`` and
+``_PROCESS_IMPORT_PLUGIN_DATA`` lets you export and import the data between
+different systems while setting the contents as you need it::
+
+    # settings.py
+    .._PROCESS_EXPORT_PLUGIN_DATA = "myapp.some.module.export_function"
+    .._PROCESS_IMPORT_PLUGIN_DATA = "myapp.some.module.import_function"
+
+    # custom functions
+    def export_function(plugin, plugin_data):
+        # remove child-plugins which can't be handled
+        if plugin.parent_id and plugin.parent.plugin_type == "SomeParentPlugin":
+            return None
+        # change data
+        if plugin.plugin_type == "SomePlugin":
+            plugin_data["data"].update({
+                "some_field": "TODO: change me",
+            })
+        return plugin_data
+
+    def import_function(deserialized_object):
+        some_related_object = MyModel.objects.first()
+        for field in deserialized_object.object._meta.fields:
+            # example of setting a default value for a related field
+            if isinstance(field, ForeignKey):
+                value = getattr(deserialized_object.object, field.attname)
+                if field.related_model == MyModel and value is not None:
+                    setattr(deserialized_object.object, field.name, some_related_object)
+
+
 Running Tests
 -------------
 
 You can run tests by executing::
 
     virtualenv env
     source env/bin/activate
-    pip install -r tests/requirements.txt
+    pip install -r tests/requirements/base.txt
     python setup.py test
 
+For code formatting, `black` is used. To automatically fix errors reported from
+`black`, you can install it via virtualenv and
+`pip install -r tests/requirements/base.txt`.
+After this you just need to run `tools/black`.
+
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-transfer.svg
     :target: http://badge.fury.io/py/djangocms-transfer
 .. |build| image:: https://travis-ci.org/divio/djangocms-transfer.svg?branch=master
     :target: https://travis-ci.org/divio/djangocms-transfer
 .. |coverage| image:: https://codecov.io/gh/divio/djangocms-transfer/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/djangocms-transfer
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/cms_plugins.py` & `djangocms_transfer-1.0.2/djangocms_transfer/cms_plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,24 @@
 
 class PluginImporter(CMSPluginBase):
     system = True
     render_plugin = False
 
     def get_plugin_urls(self):
         urlpatterns = [
-            re_path(r'^export-plugins/$', self.export_plugins_view, name='cms_export_plugins'),
-            re_path(r'^import-plugins/$', self.import_plugins_view, name='cms_import_plugins'),
+            re_path(
+                r"^export-plugins/$",
+                self.export_plugins_view,
+                name="cms_export_plugins",
+            ),
+            re_path(
+                r"^import-plugins/$",
+                self.import_plugins_view,
+                name="cms_import_plugins",
+            ),
         ]
         return urlpatterns
 
     def get_extra_placeholder_menu_items(self, request, placeholder):  # noqa
         # django-cms 3.4 compatibility
         return self.get_extra_placeholder_menu_items(request, placeholder)
 
@@ -36,109 +44,113 @@
         return self.get_extra_plugin_menu_items(request, plugin)
 
     @classmethod
     def get_extra_plugin_menu_items(cls, request, plugin):
         if plugin.plugin_type == cls.__name__:
             return
 
-        data = urlencode({
-            'language': get_language_from_request(request),
-            'plugin': plugin.pk,
-        })
+        data = urlencode(
+            {
+                "language": get_language_from_request(request),
+                "plugin": plugin.pk,
+            }
+        )
         return [
             PluginMenuItem(
-                _('Export plugins'),
-                admin_reverse('cms_export_plugins') + '?' + data,
+                _("Export plugins"),
+                admin_reverse("cms_export_plugins") + "?" + data,
                 data={},
-                action='none',
+                action="none",
                 attributes={
-                    'icon': 'export',
+                    "icon": "export",
                 },
             ),
             PluginMenuItem(
-                _('Import plugins'),
-                admin_reverse('cms_import_plugins') + '?' + data,
+                _("Import plugins"),
+                admin_reverse("cms_import_plugins") + "?" + data,
                 data={},
-                action='modal',
+                action="modal",
                 attributes={
-                    'icon': 'import',
+                    "icon": "import",
                 },
             ),
         ]
 
     @classmethod  # noqa
     def get_extra_placeholder_menu_items(cls, request, placeholder):  # noqa
-        data = urlencode({
-            'language': get_language_from_request(request),
-            'placeholder': placeholder.pk,
-        })
+        data = urlencode(
+            {
+                "language": get_language_from_request(request),
+                "placeholder": placeholder.pk,
+            }
+        )
         return [
             PluginMenuItem(
-                _('Export plugins'),
-                admin_reverse('cms_export_plugins') + '?' + data,
+                _("Export plugins"),
+                admin_reverse("cms_export_plugins") + "?" + data,
                 data={},
-                action='none',
+                action="none",
                 attributes={
-                    'icon': 'export',
+                    "icon": "export",
                 },
             ),
             PluginMenuItem(
-                _('Import plugins'),
-                admin_reverse('cms_import_plugins') + '?' + data,
+                _("Import plugins"),
+                admin_reverse("cms_import_plugins") + "?" + data,
                 data={},
-                action='modal',
+                action="modal",
                 attributes={
-                    'icon': 'import',
+                    "icon": "import",
                 },
-            )
+            ),
         ]
 
     @classmethod
     def import_plugins_view(cls, request):
         if not request.user.is_staff:
             raise PermissionDenied
 
         new_form = ExportImportForm(request.GET or None)
 
         if new_form.is_valid():
             initial_data = new_form.cleaned_data
         else:
             initial_data = None
 
-        if request.method == 'GET' and not new_form.is_valid():
-            return HttpResponseBadRequest(_('Form received unexpected values.'))
+        if request.method == "GET" and not new_form.is_valid():
+            return HttpResponseBadRequest(_("Form received unexpected values."))
 
         import_form = PluginImportForm(
             data=request.POST or None,
             files=request.FILES or None,
             initial=initial_data,
         )
 
         if not import_form.is_valid():
             opts = cls.model._meta
             context = {
-                'form': import_form,
-                'has_change_permission': True,
-                'opts': opts,
-                'root_path': reverse('admin:index'),
-                'is_popup': True,
-                'app_label': opts.app_label,
-                'media': (cls().media + import_form.media),
+                "form": import_form,
+                "has_change_permission": True,
+                "opts": opts,
+                "root_path": reverse("admin:index"),
+                "is_popup": True,
+                "app_label": opts.app_label,
+                "media": (cls().media + import_form.media),
             }
-            return render(request, 'djangocms_transfer/import_plugins.html', context)
+            return render(request, "djangocms_transfer/import_plugins.html", context)
 
-        plugin = import_form.cleaned_data.get('plugin')
-        language = import_form.cleaned_data['language']
+        plugin = import_form.cleaned_data.get("plugin")
+        language = import_form.cleaned_data["language"]
 
         if plugin:
             root_id = plugin.pk
             placeholder = plugin.placeholder
         else:
             root_id = None
-            placeholder = import_form.cleaned_data.get('placeholder')
+            placeholder = import_form.cleaned_data.get("placeholder")
 
         if not placeholder:
             # Page placeholders/plugins import
             # TODO: Check permissions
             import_form.run_import()
             return HttpResponse('<div><div class="messagelist"><div class="success"></div></div></div>')
 
@@ -154,30 +166,30 @@
             return plugin.get_plugin_class_instance().render_close_frame(request, obj=new_plugins[0])
 
         from cms.toolbar.utils import get_plugin_tree_as_json
 
         # Placeholder plugins import
         new_plugins = placeholder.get_plugins(language).exclude(pk__in=tree_order)
         data = json.loads(get_plugin_tree_as_json(request, list(new_plugins)))
-        data['plugin_order'] = tree_order + ['__COPY__']
-        data['target_placeholder_id'] = placeholder.pk
-        context = {'structure_data': json.dumps(data)}
-        return render(request, 'djangocms_transfer/placeholder_close_frame.html', context)
+        data["plugin_order"] = tree_order + ["__COPY__"]
+        data["target_placeholder_id"] = placeholder.pk
+        context = {"structure_data": json.dumps(data)}
+        return render(request, "djangocms_transfer/placeholder_close_frame.html", context)
 
     @classmethod
     def export_plugins_view(cls, request):
         if not request.user.is_staff:
             raise PermissionDenied
 
         form = PluginExportForm(request.GET or None)
 
         if not form.is_valid():
-            return HttpResponseBadRequest(_('Form received unexpected values.'))
+            return HttpResponseBadRequest(_("Form received unexpected values."))
 
         # TODO: Check permissions
         filename = form.get_filename()
-        response = HttpResponse(form.run_export(), content_type='application/json')
-        response['Content-Disposition'] = 'attachment; filename={}'.format(filename)
+        response = HttpResponse(form.run_export(), content_type="application/json")
+        response["Content-Disposition"] = "attachment; filename={}".format(filename)
         return response
 
 
 plugin_pool.register_plugin(PluginImporter)
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/cms_toolbars.py` & `djangocms_transfer-1.0.2/djangocms_transfer/cms_toolbars.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,48 +9,48 @@
 
 from .compat import GTE_CMS_3_6
 
 
 @toolbar_pool.register
 class PluginImporter(CMSToolbar):
     class Media:
-        css = {
-            'all': ('djangocms_transfer/css/transfer.css',)
-        }
+        css = {"all": ("djangocms_transfer/css/transfer.css",)}
 
     def populate(self):
         # always use draft if we have a page
         page = get_page_draft(self.request.current_page)
 
         if not page:
             return
 
         if not user_can_change_page(self.request.user, page):
             return
 
-        page_menu = self.toolbar.get_menu('page')
+        page_menu = self.toolbar.get_menu("page")
 
         if not page_menu or page_menu.disabled:
             return
 
-        data = urlencode({
-            'language': self.current_lang,
-            'cms_page': page.pk,
-        })
+        data = urlencode(
+            {
+                "language": self.current_lang,
+                "cms_page": page.pk,
+            }
+        )
 
         if GTE_CMS_3_6:
             not_edit_mode = not self.toolbar.toolbar_language
         else:
             not_edit_mode = not self.toolbar.language
 
-        page_menu.add_break('Page menu importer break')
+        page_menu.add_break("Page menu importer break")
         page_menu.add_link_item(
-            gettext('Export'),
-            url=admin_reverse('cms_export_plugins') + '?' + data,
+            gettext("Export"),
+            url=admin_reverse("cms_export_plugins") + "?" + data,
             disabled=not_edit_mode,
         )
         page_menu.add_modal_item(
-            gettext('Import'),
-            url=admin_reverse('cms_import_plugins') + '?' + data,
+            gettext("Import"),
+            url=admin_reverse("cms_import_plugins") + "?" + data,
             disabled=not_edit_mode,
-            on_close=getattr(self.toolbar, 'request_path', self.request.path),
+            on_close=getattr(self.toolbar, "request_path", self.request.path),
         )
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/datastructures.py` & `djangocms_transfer-1.0.2/djangocms_transfer/datastructures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import namedtuple
 
+from django.conf import settings
 from django.core.serializers import deserialize
 from django.db import transaction
 from django.utils.encoding import force_str
 from django.utils.functional import cached_property
 
 from cms.models import CMSPlugin
 
@@ -51,10 +52,17 @@
             plugin = CMSPlugin.add_root(**plugin_kwargs)
 
         if with_data and self.plugin_type != "CMSPlugin":
             _d_instance = self.deserialized_instance
             _d_instance.object._no_reorder = True
             _d_instance.object.cmsplugin_ptr = plugin
             plugin.set_base_attr(_d_instance.object)
+
+            # customize plugin-data on import with configured function
+            pps = getattr(settings, "DJANGOCMS_TRANSFER_PROCESS_IMPORT_PLUGIN_DATA", None)
+            if pps:
+                module, function = pps.rsplit(".", 1)
+                getattr(__import__(module, fromlist=[""]), function)(_d_instance)
+
             _d_instance.save()
             return _d_instance.object
         return plugin
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/exporter.py` & `djangocms_transfer-1.0.2/djangocms_transfer/exporter.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,35 +23,35 @@
 def export_page(cms_page, language):
     data = get_page_export_data(cms_page, language)
     return dump_json(data)
 
 
 def get_plugin_export_data(plugin):
     get_data = helpers.get_plugin_data
-    descendants = plugin.get_descendants().order_by('path')
+    descendants = plugin.get_descendants().order_by("path")
     plugin_data = [get_data(plugin=plugin)]
-    plugin_data[0]['parent_id'] = None
+    plugin_data[0]["parent_id"] = None
     plugin_data.extend(get_data(plugin) for plugin in helpers.get_bound_plugins(descendants))
     return plugin_data
 
 
 def get_placeholder_export_data(placeholder, language):
     get_data = helpers.get_plugin_data
     plugins = placeholder.get_plugins(language)
     # The following results in two queries;
     # First all the root plugins are fetched, then all child plugins.
     # This is needed to account for plugin path corruptions.
     plugins = itertools.chain(
-        plugins.filter(depth=1).order_by('position'),
-        plugins.filter(depth__gt=1).order_by('path'),
+        plugins.filter(depth=1).order_by("position"),
+        plugins.filter(depth__gt=1).order_by("path"),
     )
     return [get_data(plugin) for plugin in helpers.get_bound_plugins(list(plugins))]
 
 
 def get_page_export_data(cms_page, language):
     data = []
     placeholders = cms_page.rescan_placeholders().values()
 
     for placeholder in list(placeholders):
         plugins = get_placeholder_export_data(placeholder, language)
-        data.append({'placeholder': placeholder.slot, 'plugins': plugins})
+        data.append({"placeholder": placeholder.slot, "plugins": plugins})
     return data
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/forms.py` & `djangocms_transfer-1.0.2/djangocms_transfer/forms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import json
 
 from django import forms
 from django.conf import settings
 from django.core.exceptions import ValidationError
+from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 
 from cms.models import CMSPlugin, Page, Placeholder
 
 from .datastructures import ArchivedPlaceholder, ArchivedPlugin
 from .exporter import export_page, export_placeholder, export_plugin
 from .importer import import_plugins, import_plugins_to_page
 
 
 def _object_version_data_hook(data, for_page=False):
     if not data:
         return data
 
-    if 'plugins' in data:
+    if "plugins" in data:
         return ArchivedPlaceholder(
-            slot=data['placeholder'],
-            plugins=data['plugins'],
+            slot=data["placeholder"],
+            plugins=data["plugins"],
         )
 
-    if 'plugin_type' in data:
+    if "plugin_type" in data:
         return ArchivedPlugin(**data)
     return data
 
 
 def _get_parsed_data(file_obj, for_page=False):
-    raw = file_obj.read().decode('utf-8')
+    raw = file_obj.read().decode("utf-8")
     return json.loads(raw, object_hook=_object_version_data_hook)
 
 
 class ExportImportForm(forms.Form):
     plugin = forms.ModelChoiceField(
         CMSPlugin.objects.all(),
         required=False,
@@ -54,111 +55,126 @@
         widget=forms.HiddenInput(),
     )
 
     def clean(self):
         if self.errors:
             return self.cleaned_data
 
-        plugin = self.cleaned_data.get('plugin')
-        placeholder = self.cleaned_data.get('placeholder')
-        cms_page = self.cleaned_data.get('cms_page')
+        plugin = self.cleaned_data.get("plugin")
+        placeholder = self.cleaned_data.get("placeholder")
+        cms_page = self.cleaned_data.get("cms_page")
 
         if not any([plugin, placeholder, cms_page]):
-            message = _('A plugin, placeholder or page is required.')
+            message = _("A plugin, placeholder or page is required.")
             raise forms.ValidationError(message)
 
         if cms_page and (plugin or placeholder):
-            message = _('Plugins can be imported to pages, plugins or placeholders. Not all three.')
+            message = _("Plugins can be imported to pages, plugins or placeholders. Not all three.")
             raise forms.ValidationError(message)
 
         if placeholder and (cms_page or plugin):
-            message = _('Plugins can be imported to pages, plugins or placeholders. Not all three.')
+            message = _("Plugins can be imported to pages, plugins or placeholders. Not all three.")
             raise forms.ValidationError(message)
 
         if plugin and (cms_page or placeholder):
-            message = _('Plugins can be imported to pages, plugins or placeholders. Not all three.')
+            message = _("Plugins can be imported to pages, plugins or placeholders. Not all three.")
             raise forms.ValidationError(message)
 
         if plugin:
             plugin_model = plugin.get_plugin_class().model
             plugin_is_bound = plugin_model.objects.filter(cmsplugin_ptr=plugin).exists()
         else:
             plugin_is_bound = False
 
         if plugin and not plugin_is_bound:
-            raise ValidationError('Plugin is unbound.')
+            raise ValidationError("Plugin is unbound.")
         return self.cleaned_data
 
 
 class PluginExportForm(ExportImportForm):
-
     def get_filename(self):
-        if self.cleaned_data.get('cms_page'):
-            return 'cms_page_plugins.json'
-        return 'plugins.json'
+        data = self.cleaned_data
+        language = data["language"]
+        page = data["cms_page"]
+        plugin = data["plugin"]
+        placeholder = data["placeholder"]
+
+        if page:
+            return "{}.json".format(page.get_slug(language=language))
+        elif placeholder and placeholder.page is not None:
+            return "{}_{}.json".format(
+                placeholder.page.get_slug(language=language),
+                slugify(placeholder.slot),
+            )
+        elif plugin is not None and plugin.page is not None:
+            return "{}_{}.json".format(
+                plugin.page.get_slug(language=language),
+                slugify(plugin.get_short_description()),
+            )
+        else:
+            return "plugins.json"
 
     def run_export(self):
         data = self.cleaned_data
-        language = data['language']
-        plugin = data['plugin']
-        placeholder = data['placeholder']
+        language = data["language"]
+        plugin = data["plugin"]
+        placeholder = data["placeholder"]
 
         if plugin:
             return export_plugin(plugin.get_bound_plugin())
 
         if placeholder:
             return export_placeholder(placeholder, language)
-        return export_page(data['cms_page'], language)
+        return export_page(data["cms_page"], language)
 
 
 class PluginImportForm(ExportImportForm):
-
     import_file = forms.FileField(required=True)
 
     def clean(self):
         if self.errors:
             return self.cleaned_data
 
-        import_file = self.cleaned_data['import_file']
+        import_file = self.cleaned_data["import_file"]
 
         try:
             data = _get_parsed_data(import_file)
         except (ValueError, TypeError):
-            raise ValidationError('File is not valid')
+            raise ValidationError("File is not valid")
 
         first_item = data[0]
         is_placeholder = isinstance(first_item, ArchivedPlaceholder)
-        page_import = bool(self.cleaned_data['cms_page'])
+        page_import = bool(self.cleaned_data["cms_page"])
         plugins_import = not page_import
 
         if (is_placeholder and plugins_import) or (page_import and not is_placeholder):
-            raise ValidationError('Incorrect json format used.')
+            raise ValidationError("Incorrect json format used.")
 
-        self.cleaned_data['import_data'] = data
+        self.cleaned_data["import_data"] = data
         return self.cleaned_data
 
     def run_import(self):
         data = self.cleaned_data
-        language = data['language']
-        target_page = data['cms_page']
-        target_plugin = data['plugin']
-        target_placeholder = data['placeholder']
+        language = data["language"]
+        target_page = data["cms_page"]
+        target_plugin = data["plugin"]
+        target_placeholder = data["placeholder"]
 
         if target_plugin:
             target_plugin_id = target_plugin.pk
             target_placeholder = target_plugin.placeholder
         else:
             target_plugin_id = None
 
         if target_page:
             import_plugins_to_page(
-                placeholders=data['import_data'],
+                placeholders=data["import_data"],
                 page=target_page,
                 language=language,
             )
         else:
             import_plugins(
-                plugins=data['import_data'],
+                plugins=data["import_data"],
                 placeholder=target_placeholder,
                 language=language,
                 root_plugin_id=target_plugin_id,
             )
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/helpers.py` & `djangocms_transfer-1.0.2/djangocms_transfer/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 
+from django.conf import settings
 from django.core import serializers
 
 from . import get_serializer_name
 from .utils import get_plugin_fields, get_plugin_model
 
 
 def get_bound_plugins(plugins):
@@ -25,32 +26,38 @@
 
         # put them in a map so we can replace the base CMSPlugins with their
         # downcasted versions
         for instance in plugin_queryset.iterator():
             plugin_lookup[instance.pk] = instance
 
     for plugin in plugins:
-        parent_not_available = (not plugin.parent_id or plugin.parent_id not in plugin_ids)
+        parent_not_available = not plugin.parent_id or plugin.parent_id not in plugin_ids
         # The plugin either has no parent or needs to have a non-ghost parent
-        valid_parent = (parent_not_available or plugin.parent_id in plugin_lookup)
+        valid_parent = parent_not_available or plugin.parent_id in plugin_lookup
 
         if valid_parent and plugin.pk in plugin_lookup:
             yield plugin_lookup[plugin.pk]
 
 
 def get_plugin_data(plugin, only_meta=False):
     if only_meta:
         custom_data = None
     else:
         plugin_fields = get_plugin_fields(plugin.plugin_type)
         _plugin_data = serializers.serialize(get_serializer_name(), (plugin,), fields=plugin_fields)[0]
-        custom_data = _plugin_data['fields']
+        custom_data = _plugin_data["fields"]
 
     plugin_data = {
-        'pk': plugin.pk,
-        'creation_date': plugin.creation_date,
-        'position': plugin.position,
-        'plugin_type': plugin.plugin_type,
-        'parent_id': plugin.parent_id,
-        'data': custom_data,
+        "pk": plugin.pk,
+        "creation_date": plugin.creation_date,
+        "position": plugin.position,
+        "plugin_type": plugin.plugin_type,
+        "parent_id": plugin.parent_id,
+        "data": custom_data,
     }
-    return plugin_data
+
+    gpd = getattr(settings, "DJANGOCMS_TRANSFER_PROCESS_EXPORT_PLUGIN_DATA", None)
+    if gpd:
+        module, function = gpd.rsplit(".", 1)
+        return getattr(__import__(module, fromlist=[""]), function)(plugin, plugin_data)
+    else:
+        return plugin_data
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/importer.py` & `djangocms_transfer-1.0.2/djangocms_transfer/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,19 @@
         source_map[root_plugin_id] = root_plugin
     else:
         root_plugin = None
 
     tree_order = placeholder.get_plugin_tree_order(language, parent_id=root_plugin_id)
 
     for archived_plugin in plugins:
+        # custom handling via "get_plugin_data" can lead to "null"-values
+        # instead of plugin-dictionaries. We skip those here.
+        if archived_plugin is None:
+            continue
+
         if archived_plugin.parent_id:
             parent = source_map[archived_plugin.parent_id]
         else:
             parent = root_plugin
 
         if parent and parent.__class__ != CMSPlugin:
             parent = parent.cmsplugin_ptr
@@ -38,15 +43,15 @@
         if parent == root_plugin:
             tree_order.append(plugin.pk)
         new_plugins.append(plugin)
 
     for new_plugin in new_plugins:
         plugin_class = get_plugin_class(new_plugin.plugin_type)
 
-        if getattr(plugin_class, '_has_do_post_copy', False):
+        if getattr(plugin_class, "_has_do_post_copy", False):
             # getattr is used for django CMS 3.4 compatibility
             # apps on 3.4 wishing to leverage this callback will need
             # to manually set the _has_do_post_copy attribute.
             plugin_class.do_post_copy(new_plugin, source_map)
 
     reorder_plugins(
         placeholder,
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/css/transfer.css` & `djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/css/transfer.css`

 * *Files identical despite different names*

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/static/djangocms_transfer/img/icons.png` & `djangocms_transfer-1.0.2/djangocms_transfer/static/djangocms_transfer/img/icons.png`

 * *Files identical despite different names*

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/templates/djangocms_transfer/import_plugins.html` & `djangocms_transfer-1.0.2/djangocms_transfer/templates/djangocms_transfer/import_plugins.html`

 * *Files identical despite different names*

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer/utils.py` & `djangocms_transfer-1.0.2/djangocms_transfer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from cms.plugin_pool import plugin_pool
 
 
 @lru_cache()
 def get_local_fields(model):
     opts = model._meta.concrete_model._meta
     fields = opts.local_fields
-    return [field.name for field in fields
-            if not field.is_relation and not field.primary_key]
+    return [field.name for field in fields if not field.is_relation and not field.primary_key]
 
 
 @lru_cache()
 def get_related_fields(model):
     opts = model._meta.concrete_model._meta
     fields = opts.local_fields + list(opts.many_to_many)
     return [field.name for field in fields if field.is_relation]
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer.egg-info/PKG-INFO` & `djangocms_transfer-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-transfer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Adds import and export of plugin data.
 Home-page: https://github.com/django-cms/djangocms-transfer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -29,14 +29,15 @@
 Classifier: Framework :: Django CMS :: 3.10
 Classifier: Framework :: Django CMS :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
+Requires-Dist: django-cms>=3.7
 
 ===================
 django CMS Transfer
 ===================
 
 |pypi| |build| |coverage|
 
@@ -89,24 +90,75 @@
 For a manual install:
 
 * run ``pip install djangocms-transfer``
 * add ``djangocms_transfer`` to your ``INSTALLED_APPS``
 * run ``python manage.py migrate djangocms_transfer``
 
 
+Customization
+-------------
+
+Following settings are available:
+
+* **DJANGOCMS_TRANSFER_PROCESS_EXPORT_PLUGIN_DATA**:
+
+  Enables processing of plugin instances prior to serialization, e.g.
+  ``myapp.module.function``.
+
+* **DJANGOCMS_TRANSFER_PROCESS_IMPORT_PLUGIN_DATA**:
+
+  Enables processing of plugin instances prior to saving, e.g.
+  ``myapp.module.function``.
+  For example: set default-values for ForeignKeys (images for django_filer, ..)
+
+As an example the combination of ``_PROCESS_EXPORT_PLUGIN_DATA`` and
+``_PROCESS_IMPORT_PLUGIN_DATA`` lets you export and import the data between
+different systems while setting the contents as you need it::
+
+    # settings.py
+    .._PROCESS_EXPORT_PLUGIN_DATA = "myapp.some.module.export_function"
+    .._PROCESS_IMPORT_PLUGIN_DATA = "myapp.some.module.import_function"
+
+    # custom functions
+    def export_function(plugin, plugin_data):
+        # remove child-plugins which can't be handled
+        if plugin.parent_id and plugin.parent.plugin_type == "SomeParentPlugin":
+            return None
+        # change data
+        if plugin.plugin_type == "SomePlugin":
+            plugin_data["data"].update({
+                "some_field": "TODO: change me",
+            })
+        return plugin_data
+
+    def import_function(deserialized_object):
+        some_related_object = MyModel.objects.first()
+        for field in deserialized_object.object._meta.fields:
+            # example of setting a default value for a related field
+            if isinstance(field, ForeignKey):
+                value = getattr(deserialized_object.object, field.attname)
+                if field.related_model == MyModel and value is not None:
+                    setattr(deserialized_object.object, field.name, some_related_object)
+
+
 Running Tests
 -------------
 
 You can run tests by executing::
 
     virtualenv env
     source env/bin/activate
-    pip install -r tests/requirements.txt
+    pip install -r tests/requirements/base.txt
     python setup.py test
 
+For code formatting, `black` is used. To automatically fix errors reported from
+`black`, you can install it via virtualenv and
+`pip install -r tests/requirements/base.txt`.
+After this you just need to run `tools/black`.
+
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-transfer.svg
     :target: http://badge.fury.io/py/djangocms-transfer
 .. |build| image:: https://travis-ci.org/divio/djangocms-transfer.svg?branch=master
     :target: https://travis-ci.org/divio/djangocms-transfer
 .. |coverage| image:: https://codecov.io/gh/divio/djangocms-transfer/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/divio/djangocms-transfer
```

### Comparing `djangocms-transfer-1.0.1/djangocms_transfer.egg-info/SOURCES.txt` & `djangocms_transfer-1.0.2/djangocms_transfer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -22,8 +22,13 @@
 djangocms_transfer.egg-info/top_level.txt
 djangocms_transfer/static/djangocms_transfer/css/transfer.css
 djangocms_transfer/static/djangocms_transfer/img/icons.png
 djangocms_transfer/templates/djangocms_transfer/import_plugins.html
 djangocms_transfer/templates/djangocms_transfer/placeholder_close_frame.html
 tests/__init__.py
 tests/settings.py
-tests/test_migrations.py
+tests/test_migrations.py
+tests/transfer/__init__.py
+tests/transfer/abstract.py
+tests/transfer/test_export.py
+tests/transfer/test_forms.py
+tests/transfer/test_import.py
```

### Comparing `djangocms-transfer-1.0.1/setup.cfg` & `djangocms_transfer-1.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 	tmp
 
 [isort]
 line_length = 79
 skip = manage.py, *migrations*, .tox, .eggs, data
 include_trailing_comma = true
 multi_line_output = 5
-not_skip = __init__.py
 lines_after_imports = 2
 default_section = THIRDPARTY
-sections = FUTURE, STDLIB, DJANGO, CMS, THIRDPARTY, FIRSTPARTY, LIB, LOCALFOLDER
+sections = FUTURE, STDLIB, DJANGO, CMS, THIRDPARTY, FIRSTPARTY, LOCALFOLDER
 known_first_party = djangocms_transfer
 known_cms = cms, menus
 known_django = django
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `djangocms-transfer-1.0.1/setup.py` & `djangocms_transfer-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-transfer-1.0.1/tests/test_migrations.py` & `djangocms_transfer-1.0.2/tests/test_migrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from io import StringIO
 
 from django.core.management import call_command
 from django.test import TestCase, override_settings
 
 
 class MigrationTestCase(TestCase):
-    @override_settings(
-        MIGRATION_MODULES={}, DEFAULT_AUTO_FIELD="django.db.models.AutoField"
-    )
+    @override_settings(MIGRATION_MODULES={}, DEFAULT_AUTO_FIELD="django.db.models.AutoField")
     def test_for_missing_migrations(self):
         output = StringIO()
         options = {
             "interactive": False,
             "dry_run": True,
             "stdout": output,
             "check_changes": True,
```

