# Comparing `tmp/artd-shopify-1.1.3.tar.gz` & `tmp/artd-shopify-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-shopify-1.1.3.tar", last modified: Mon Apr 22 22:22:45 2024, max compression
+gzip compressed data, was "artd-shopify-1.1.4.tar", last modified: Tue Apr 23 03:13:37 2024, max compression
```

## Comparing `artd-shopify-1.1.3.tar` & `artd-shopify-1.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      138 2024-03-06 17:20:48.000000 artd-shopify-1.1.3/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1187 2024-03-06 21:00:51.000000 artd-shopify-1.1.3/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_package/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_package/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_package/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3966 2024-04-22 22:21:50.000000 artd-shopify-1.1.3/artd_package/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1132 2024-03-10 19:25:44.000000 artd-shopify-1.1.3/artd_package/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_package/wsgi.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     8624 2024-03-27 02:17:47.000000 artd-shopify-1.1.3/artd_shopify/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      247 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/apps.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      952 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/forms.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      425 2024-03-06 17:19:26.000000 artd-shopify-1.1.3/artd_shopify/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5183 2024-03-06 17:12:25.000000 artd-shopify-1.1.3/artd_shopify/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3810 2024-03-06 17:19:26.000000 artd-shopify-1.1.3/artd_shopify/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6341 2024-03-06 17:19:18.000000 artd-shopify-1.1.3/artd_shopify/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/management/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/management/__init__.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/management/commands/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/management/commands/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      950 2024-03-27 02:30:26.000000 artd-shopify-1.1.3/artd_shopify/management/commands/convert_tags_to_categories.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1059 2024-04-03 17:45:52.000000 artd-shopify-1.1.3/artd_shopify/management/commands/import_shopify_product.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      920 2024-03-27 02:30:23.000000 artd-shopify-1.1.3/artd_shopify/management/commands/import_shopify_tags.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      929 2024-03-27 07:04:40.000000 artd-shopify-1.1.3/artd_shopify/management/commands/update_categories_for_all_products.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    21297 2024-03-06 13:52:49.000000 artd-shopify-1.1.3/artd_shopify/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3028 2024-03-26 22:56:24.000000 artd-shopify-1.1.3/artd_shopify/migrations/0002_shopifytag.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2523 2024-03-27 01:47:25.000000 artd-shopify-1.1.3/artd_shopify/migrations/0003_shopifyroottag.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      979 2024-03-27 01:54:45.000000 artd-shopify-1.1.3/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    19937 2024-03-27 02:15:09.000000 artd-shopify-1.1.3/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    10833 2024-03-27 02:15:01.000000 artd-shopify-1.1.3/artd_shopify/models.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/tests.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/utils/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/utils/__init__.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify/utils/graphql/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/utils/graphql/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      499 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/utils/graphql/queries.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    22857 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/utils/shopify.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    36360 2024-03-27 06:59:35.000000 artd-shopify-1.1.3/artd_shopify/utils/shopify_graphql.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      254 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/artd_shopify/views.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/artd_shopify.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-04-22 22:22:45.000000 artd-shopify-1.1.3/artd_shopify.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1506 2024-04-22 22:22:45.000000 artd-shopify-1.1.3/artd_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-22 22:22:45.000000 artd-shopify-1.1.3/artd_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      172 2024-04-22 22:22:45.000000 artd-shopify-1.1.3/artd_shopify.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       26 2024-04-22 22:22:45.000000 artd-shopify-1.1.3/artd_shopify.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1216 2024-04-22 22:22:45.531829 artd-shopify-1.1.3/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-06 13:48:57.000000 artd-shopify-1.1.3/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.856417 artd-shopify-1.1.4/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      138 2024-03-06 17:20:48.000000 artd-shopify-1.1.4/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-04-23 03:13:37.856417 artd-shopify-1.1.4/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1187 2024-03-06 21:00:51.000000 artd-shopify-1.1.4/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_package/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_package/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_package/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3966 2024-04-23 02:37:55.000000 artd-shopify-1.1.4/artd_package/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1132 2024-03-10 19:25:44.000000 artd-shopify-1.1.4/artd_package/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_package/wsgi.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     8624 2024-03-27 02:17:47.000000 artd-shopify-1.1.4/artd_shopify/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      247 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/apps.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      952 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/forms.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.836417 artd-shopify-1.1.4/artd_shopify/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.836417 artd-shopify-1.1.4/artd_shopify/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      425 2024-03-06 17:19:26.000000 artd-shopify-1.1.4/artd_shopify/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5183 2024-03-06 17:12:25.000000 artd-shopify-1.1.4/artd_shopify/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3810 2024-03-06 17:19:26.000000 artd-shopify-1.1.4/artd_shopify/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6341 2024-03-06 17:19:18.000000 artd-shopify-1.1.4/artd_shopify/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/management/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/management/__init__.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/management/commands/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/management/commands/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1000 2024-04-23 02:11:21.000000 artd-shopify-1.1.4/artd_shopify/management/commands/convert_tags_to_categories.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1109 2024-04-23 03:07:53.000000 artd-shopify-1.1.4/artd_shopify/management/commands/import_shopify_product.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      970 2024-04-23 03:08:04.000000 artd-shopify-1.1.4/artd_shopify/management/commands/import_shopify_tags.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      979 2024-04-23 03:08:08.000000 artd-shopify-1.1.4/artd_shopify/management/commands/update_categories_for_all_products.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    21297 2024-03-06 13:52:49.000000 artd-shopify-1.1.4/artd_shopify/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3028 2024-03-26 22:56:24.000000 artd-shopify-1.1.4/artd_shopify/migrations/0002_shopifytag.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2523 2024-03-27 01:47:25.000000 artd-shopify-1.1.4/artd_shopify/migrations/0003_shopifyroottag.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      979 2024-03-27 01:54:45.000000 artd-shopify-1.1.4/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    19937 2024-03-27 02:15:09.000000 artd-shopify-1.1.4/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    10833 2024-03-27 02:15:01.000000 artd-shopify-1.1.4/artd_shopify/models.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/tests.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.856417 artd-shopify-1.1.4/artd_shopify/utils/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/utils/__init__.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.856417 artd-shopify-1.1.4/artd_shopify/utils/graphql/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/utils/graphql/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      499 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/utils/graphql/queries.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    22857 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/utils/shopify.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    35660 2024-04-23 03:11:50.000000 artd-shopify-1.1.4/artd_shopify/utils/shopify_graphql.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      254 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/artd_shopify/views.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-23 03:13:37.846417 artd-shopify-1.1.4/artd_shopify.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-04-23 03:13:37.000000 artd-shopify-1.1.4/artd_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1506 2024-04-23 03:13:37.000000 artd-shopify-1.1.4/artd_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-23 03:13:37.000000 artd-shopify-1.1.4/artd_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      173 2024-04-23 03:13:37.000000 artd-shopify-1.1.4/artd_shopify.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       26 2024-04-23 03:13:37.000000 artd-shopify-1.1.4/artd_shopify.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1217 2024-04-23 03:13:37.856417 artd-shopify-1.1.4/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-06 13:48:57.000000 artd-shopify-1.1.4/setup.py
```

### Comparing `artd-shopify-1.1.3/LICENSE` & `artd-shopify-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/PKG-INFO` & `artd-shopify-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-shopify
-Version: 1.1.3
+Version: 1.1.4
 Summary: ArtD Shopify.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-shopify-1.1.3/README.rst` & `artd-shopify-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_package/settings.py` & `artd-shopify-1.1.4/artd_package/settings.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_package/urls.py` & `artd-shopify-1.1.4/artd_package/urls.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/admin.py` & `artd-shopify-1.1.4/artd_shopify/admin.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/forms.py` & `artd-shopify-1.1.4/artd_shopify/forms.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/locale/en/LC_MESSAGES/django.po` & `artd-shopify-1.1.4/artd_shopify/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/locale/es/LC_MESSAGES/django.mo` & `artd-shopify-1.1.4/artd_shopify/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/locale/es/LC_MESSAGES/django.po` & `artd-shopify-1.1.4/artd_shopify/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/management/commands/convert_tags_to_categories.py` & `artd-shopify-1.1.4/artd_shopify/management/commands/convert_tags_to_categories.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def add_arguments(self, parser):
         # Define aquí los parámetros del comando
         parser.add_argument("partner_slug", type=str, help="Partner slug")
 
     def handle(self, *args, **kwargs):
         partner_slug = kwargs["partner_slug"]
+        partner_slug = partner_slug.split("=")[1]
         print(partner_slug)
         try:
             partner = Partner.objects.filter(
                 partner_slug=partner_slug,
             ).first()
             print(partner)
             sgq = ShopifyGraphQl(partner)
```

### Comparing `artd-shopify-1.1.3/artd_shopify/management/commands/import_shopify_product.py` & `artd-shopify-1.1.4/artd_shopify/management/commands/import_shopify_product.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def add_arguments(self, parser):
         # Define aquí los parámetros del comando
         parser.add_argument("partner_slug", type=str, help="Partner slug")
 
     def handle(self, *args, **kwargs):
         partner_slug = kwargs["partner_slug"]
+        partner_slug = partner_slug.split("=")[1]
         print(partner_slug)
         try:
             partner = Partner.objects.filter(
                 partner_slug=partner_slug,
             ).first()
             print(partner)
             sgq = ShopifyGraphQl(partner)
```

### Comparing `artd-shopify-1.1.3/artd_shopify/management/commands/import_shopify_tags.py` & `artd-shopify-1.1.4/artd_shopify/management/commands/import_shopify_tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def add_arguments(self, parser):
         # Define aquí los parámetros del comando
         parser.add_argument("partner_slug", type=str, help="Partner slug")
 
     def handle(self, *args, **kwargs):
         partner_slug = kwargs["partner_slug"]
+        partner_slug = partner_slug.split("=")[1]
         print(partner_slug)
         try:
             partner = Partner.objects.filter(
                 partner_slug=partner_slug,
             ).first()
             print(partner)
             sgq = ShopifyGraphQl(partner)
```

### Comparing `artd-shopify-1.1.3/artd_shopify/management/commands/update_categories_for_all_products.py` & `artd-shopify-1.1.4/artd_shopify/management/commands/update_categories_for_all_products.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def add_arguments(self, parser):
         # Define aquí los parámetros del comando
         parser.add_argument("partner_slug", type=str, help="Partner slug")
 
     def handle(self, *args, **kwargs):
         partner_slug = kwargs["partner_slug"]
+        partner_slug = partner_slug.split("=")[1]
         print(partner_slug)
         try:
             partner = Partner.objects.filter(
                 partner_slug=partner_slug,
             ).first()
             sgq = ShopifyGraphQl(partner)
             sgq.update_categories_for_all_products()
```

### Comparing `artd-shopify-1.1.3/artd_shopify/migrations/0001_initial.py` & `artd-shopify-1.1.4/artd_shopify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/migrations/0002_shopifytag.py` & `artd-shopify-1.1.4/artd_shopify/migrations/0002_shopifytag.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/migrations/0003_shopifyroottag.py` & `artd-shopify-1.1.4/artd_shopify/migrations/0003_shopifyroottag.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py` & `artd-shopify-1.1.4/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py` & `artd-shopify-1.1.4/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/models.py` & `artd-shopify-1.1.4/artd_shopify/models.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/utils/shopify.py` & `artd-shopify-1.1.4/artd_shopify/utils/shopify.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/artd_shopify/utils/shopify_graphql.py` & `artd-shopify-1.1.4/artd_shopify/utils/shopify_graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,15 +332,14 @@
                 name=self.__vendor,
                 partner=self.__partner,
             )
 
         first_category = True
 
         products = ShopifyProduct.objects.all()
-        # products = ShopifyProduct.objects.filter(id=11434)
         for product in products:
             node = product.json_data.get("node", {})
             category = node.get("productCategory", None)
             print(category)
             tax = Tax.objects.first()
             if category is not None:
                 product_taxonomy_node = category.get("productTaxonomyNode", {})
@@ -432,15 +431,14 @@
                 ):
                     Brand.objects.create(
                         name=vendor,
                     )
 
     def store_products_from_shopify_to_artd(self):
         all_products = ShopifyProduct.objects.all()
-        # all_products = ShopifyProduct.objects.filter(id=4911)
         for product in all_products:
             node = product.json_data.get("node", {})
             id = node.get("id", None)
             main_product_id = self.get_id_from_gid_string(id)
             title = node.get("title", None)
             description = node.get("description", None)
             description_html = node.get("descriptionHtml", None)
@@ -479,233 +477,235 @@
                         artd_partner=self.__partner,
                     ).first()
                     artd_category = Category.objects.filter(
                         name=category.name,
                         partner=self.__partner,
                     ).first()
                     tax = category.artd_tax
-                for option in options:
-                    id = self.get_id_from_gid_string(option.get("id", None))
-                    name = option.get("name", None)
-                    values = option.get("values", [])
-                    option_list.append(
-                        {
-                            "id": id,
-                            "name": name,
-                            "values": values,
-                        }
-                    )
-
-                shopify_images = self.save_artd_images(images)
-                variant_products = []
-                brand = Brand.objects.filter(name=vendor).first()
-                print(f"Brand: {brand}")
-                if brand is None:
-                    brand = Brand.objects.first()
-                for variant in variants:
-                    variant_node = variant.get("node", {})
-                    variant_id = variant_node.get("id", None)
-                    variant_id = self.get_id_from_gid_string(variant_id)
-                    variant_title = variant_node.get("title", None)
-                    variant_sku = variant_node.get("sku", None)
-                    variant_price = variant_node.get("price", None)
-                    variant_weight = variant_node.get("weight", None)
-                    variant_inventory_quantity = variant_node.get(
-                        "inventoryQuantity", None
-                    )
-
-                    if variant_title == "Default Title":
-                        variant_title = title
-
-                    source = {
-                        "name": "shopify",
-                        "id": variant_id,
-                        "partner": self.__partner.id,
+            else:
+                artd_category = None
+                tax = Tax.objects.first()
+            for option in options:
+                id = self.get_id_from_gid_string(option.get("id", None))
+                name = option.get("name", None)
+                values = option.get("values", [])
+                option_list.append(
+                    {
+                        "id": id,
+                        "name": name,
+                        "values": values,
                     }
-                    print(f"Source: {source}")
-                    if first_product:
-                        sku = variant_sku
-                        first_product = False
-                    if (
-                        Product.objects.filter(
-                            partner=self.__partner,
-                            external_id=variant_id,
-                        ).count()
-                        == 0
-                    ):
-                        try:
-                            product_obj = Product.objects.create(
-                                partner=self.__partner,
-                                source=source,
-                                json_data=variant,
-                                external_id=variant_id,
-                                url_key=handle,
-                                meta_title=meta_title,
-                                meta_description=meta_description,
-                                meta_keywords="",
-                                type="physical",
-                                name=variant_title,
-                                sku=variant_sku,
-                                description=description_html,
-                                short_description=description,
-                                tax=tax,
-                                weight=variant_weight,
-                                unit_of_measure="kg",
-                                measure=variant_weight,
-                                variations=option_list,
-                                brand=brand,
-                            )
-                            product_obj.categories.add(artd_category)
-                            Stock.objects.create(
-                                partner=self.__partner,
-                                product=product_obj,
-                                stock=variant_inventory_quantity,
-                            )
-                            PriceList.objects.create(
-                                partner=self.__partner,
-                                product=product_obj,
-                                regular_price=variant_price,
-                            )
-                            print("Line 567")
-                        except Exception as e:
-                            print(f"Error creating product: {e}")
-                            product_obj = None
-                    else:
-                        try:
-                            product_obj = Product.objects.filter(
-                                partner=self.__partner,
-                                external_id=variant_id,
-                            ).first()
-                            Product.objects.filter(
-                                partner=self.__partner,
-                                external_id=variant_id,
-                            ).update(
-                                json_data=variant,
-                                url_key=handle,
-                                meta_title=meta_title,
-                                meta_description=meta_description,
-                                meta_keywords="",
-                                type="physical",
-                                name=variant_title,
-                                sku=variant_sku,
-                                description=description_html,
-                                short_description=description,
-                                tax=tax,
-                                weight=variant_weight,
-                                unit_of_measure="kg",
-                                measure=variant_weight,
-                                variations=option_list,
-                                brand=brand,
-                            )
-                            product_obj.categories.clear()
-                            product_obj.categories.add(artd_category)
-                            Stock.objects.filter(
-                                partner=self.__partner,
-                                product=product_obj,
-                            ).update(stock=variant_inventory_quantity)
-                            PriceList.objects.filter(
-                                partner=self.__partner,
-                                product=product_obj,
-                            ).update(regular_price=variant_price)
-                            print("Line 608")
-                        except Exception as e:
-                            print(f"Error updating product: {e}")
-                            product_obj = None
-                    if product_obj is not None:
-                        variant_products.append(product_obj)
-                        print("Line 614")
-                        for shopify_image in shopify_images:
-                            if (
-                                ProductImage.objects.filter(
-                                    product=product_obj,
-                                    image=shopify_image,
-                                ).count()
-                                == 0
-                            ):
-                                source = {
-                                    "name": "shopify",
-                                    "id": variant_id,
-                                    "partner": self.__partner.id,
-                                }
-                                ProductImage.objects.create(
-                                    source=source,
-                                    external_id=variant_id,
-                                    product=product_obj,
-                                    image=shopify_image,
-                                )
-                        print("Line 634")
+                )
 
+            shopify_images = self.save_artd_images(images)
+            variant_products = []
+            brand = Brand.objects.filter(name=vendor).first()
+            print(f"Brand: {brand}")
+            if brand is None:
+                brand = Brand.objects.first()
+            for variant in variants:
+                variant_node = variant.get("node", {})
+                variant_id = variant_node.get("id", None)
+                variant_id = self.get_id_from_gid_string(variant_id)
+                variant_title = variant_node.get("title", None)
+                variant_sku = variant_node.get("sku", None)
+                variant_price = variant_node.get("price", None)
+                variant_weight = variant_node.get("weight", None)
+                variant_inventory_quantity = variant_node.get("inventoryQuantity", None)
+
+                if variant_title == "Default Title":
+                    variant_title = title
+
+                source = {
+                    "name": "shopify",
+                    "id": variant_id,
+                    "partner": self.__partner.id,
+                }
+                if first_product:
+                    sku = variant_sku
+                    first_product = False
                 if (
-                    GroupedProduct.objects.filter(
+                    Product.objects.filter(
                         partner=self.__partner,
-                        external_id=main_product_id,
+                        external_id=variant_id,
                     ).count()
                     == 0
                 ):
                     try:
-                        print("Line 644")
-                        grouped_product_source = {
-                            "name": "shopify",
-                            "id": main_product_id,
-                            "partner": self.__partner.id,
-                        }
-                        grouped_product = GroupedProduct.objects.create(
-                            source=grouped_product_source,
-                            json_data=node,
-                            external_id=main_product_id,
+                        product_obj = Product.objects.create(
                             partner=self.__partner,
+                            source=source,
+                            json_data=variant,
+                            external_id=variant_id,
                             url_key=handle,
-                            name=title,
-                            sku=sku,
+                            meta_title=meta_title,
+                            meta_description=meta_description,
+                            meta_keywords="",
+                            type="physical",
+                            name=variant_title,
+                            tax=tax,
+                            sku=variant_sku,
                             description=description_html,
                             short_description=description,
-                            variations=options,
+                            weight=variant_weight,
+                            unit_of_measure="kg",
+                            measure=variant_weight,
+                            variations=option_list,
+                            brand=brand,
+                        )
+                        if artd_category is not None:
+                            product_obj.categories.add(artd_category)
+                            product_obj.save()
+
+                        Stock.objects.create(
+                            partner=self.__partner,
+                            product=product_obj,
+                            stock=variant_inventory_quantity,
+                        )
+                        PriceList.objects.create(
+                            partner=self.__partner,
+                            product=product_obj,
+                            regular_price=variant_price,
                         )
-                        for variant_product in variant_products:
-                            grouped_product.products.add(variant_product)
-                        print("Line 659")
+
                     except Exception as e:
-                        print(f"Error creating grouped product: {e}")
+                        print(f"Error creating product: {e}")
+                        product_obj = None
                 else:
                     try:
-                        grouped_product_source = {
-                            "name": "shopify",
-                            "id": main_product_id,
-                            "partner": self.__partner.id,
-                        }
-                        grouped_product = GroupedProduct.objects.filter(
+                        product_obj = Product.objects.filter(
                             partner=self.__partner,
-                            external_id=main_product_id,
+                            external_id=variant_id,
                         ).first()
-                        GroupedProduct.objects.filter(
+                        Product.objects.filter(
                             partner=self.__partner,
-                            external_id=main_product_id,
+                            external_id=variant_id,
                         ).update(
-                            source=grouped_product_source,
-                            json_data=node,
+                            json_data=variant,
                             url_key=handle,
-                            name=title,
-                            sku=sku,
+                            meta_title=meta_title,
+                            meta_description=meta_description,
+                            meta_keywords="",
+                            type="physical",
+                            name=variant_title,
+                            sku=variant_sku,
                             description=description_html,
                             short_description=description,
-                            variations=options,
+                            weight=variant_weight,
+                            unit_of_measure="kg",
+                            measure=variant_weight,
+                            variations=option_list,
+                            brand=brand,
+                            tax=tax,
                         )
-                        grouped_product.products.clear()
-                        for variant_product in variant_products:
-                            grouped_product.products.add(variant_product)
-                        print("Line 684")
+                        if artd_category is not None:
+                            product_obj.categories.clear()
+                            product_obj.categories.add(artd_category)
+                            product_obj.save()
+
+                        Stock.objects.filter(
+                            partner=self.__partner,
+                            product=product_obj,
+                        ).update(stock=variant_inventory_quantity)
+                        PriceList.objects.filter(
+                            partner=self.__partner,
+                            product=product_obj,
+                        ).update(regular_price=variant_price)
+
                     except Exception as e:
-                        print(f"Error updating grouped product: {e}")
+                        print(f"Error updating product: {e}")
+                        product_obj = None
+                if product_obj is not None:
+                    variant_products.append(product_obj)
+
+                    for shopify_image in shopify_images:
+                        if (
+                            ProductImage.objects.filter(
+                                product=product_obj,
+                                image=shopify_image,
+                            ).count()
+                            == 0
+                        ):
+                            source = {
+                                "name": "shopify",
+                                "id": variant_id,
+                                "partner": self.__partner.id,
+                            }
+                            ProductImage.objects.create(
+                                source=source,
+                                external_id=variant_id,
+                                product=product_obj,
+                                image=shopify_image,
+                            )
+
+            if (
+                GroupedProduct.objects.filter(
+                    partner=self.__partner,
+                    external_id=main_product_id,
+                ).count()
+                == 0
+            ):
+                try:
+                    grouped_product_source = {
+                        "name": "shopify",
+                        "id": main_product_id,
+                        "partner": self.__partner.id,
+                    }
+                    grouped_product = GroupedProduct.objects.create(
+                        source=grouped_product_source,
+                        json_data=node,
+                        external_id=main_product_id,
+                        partner=self.__partner,
+                        url_key=handle,
+                        name=title,
+                        sku=sku,
+                        description=description_html,
+                        short_description=description,
+                        variations=options,
+                    )
+                    for variant_product in variant_products:
+                        grouped_product.products.add(variant_product)
+
+                except Exception as e:
+                    print(f"Error creating grouped product: {e}")
+            else:
+                try:
+                    grouped_product_source = {
+                        "name": "shopify",
+                        "id": main_product_id,
+                        "partner": self.__partner.id,
+                    }
+                    grouped_product = GroupedProduct.objects.filter(
+                        partner=self.__partner,
+                        external_id=main_product_id,
+                    ).first()
+                    GroupedProduct.objects.filter(
+                        partner=self.__partner,
+                        external_id=main_product_id,
+                    ).update(
+                        source=grouped_product_source,
+                        json_data=node,
+                        url_key=handle,
+                        name=title,
+                        sku=sku,
+                        description=description_html,
+                        short_description=description,
+                        variations=options,
+                    )
+                    grouped_product.products.clear()
+                    for variant_product in variant_products:
+                        grouped_product.products.add(variant_product)
+
+                except Exception as e:
+                    print(f"Error updating grouped product: {e}")
             product.processed = True
             product.save()
-            print(f"Line 689 {product.id}")
 
     def store_tags(self, partner: Partner):
         all_products = ShopifyProduct.objects.all()
-        # all_products = ShopifyProduct.objects.filter(id=11438)
         tags_list = []
         for product in all_products:
             node = product.json_data.get("node", {})
             tags = node.get("tags", None)
 
             for tag in tags:
                 print(tag)
@@ -728,15 +728,18 @@
 
     def transform_text(self, text):
         parts = text.split("_")
         transformed_text = " ".join(part.capitalize() for part in parts)
         return transformed_text
 
     def tags_to_categories(self, partner: Partner):
-        all_tags = ShopifyTag.objects.values("tag").annotate(tag_count=Count("tag"))
+        all_tags = ShopifyTag.objects.values(
+            "tag",
+            "id",
+        ).annotate(tag_count=Count("tag"))
         root_tags = ShopifyRootTag.objects.filter(artd_partner=partner)
 
         root_tags_dict = {}
         for root_tag in root_tags:
             root_tag_text_base = root_tag.root_tag
             root_tag_text = self.transform_text(root_tag_text_base[:-1])
             root_tags_dict[root_tag_text_base] = {
@@ -764,40 +767,49 @@
                     partner=partner,
                 ).last()
 
             root_tags_dict[root_tag_text_base]["category"] = category
 
         for tag in all_tags:
             tag_text = tag["tag"]
+            tag_id = tag["id"]
             splited_tag = tag_text.split("_")
             splited_root_tag = f"{splited_tag[0]}_"
             if splited_root_tag in root_tags_dict:
                 base_category = self.transform_text(
                     tag_text.replace(splited_root_tag, "")
                 )
                 if (
                     Category.objects.filter(
                         name=base_category,
                         parent=root_tags_dict[splited_root_tag]["category"],
                         partner=partner,
                     ).count()
                     == 0
                 ):
-                    Category.objects.create(
+                    category = Category.objects.create(
                         name=base_category,
                         parent=root_tags_dict[splited_root_tag]["category"],
                         partner=partner,
                     )
                     print(f"Category {base_category} created")
                 else:
+                    category = Category.objects.filter(
+                        name=base_category,
+                        parent=root_tags_dict[splited_root_tag]["category"],
+                        partner=partner,
+                    ).last()
                     print(f"Category {base_category} already exist")
 
+                tag_object = ShopifyTag.objects.get(id=tag_id)
+                tag_object.category = category
+                tag_object.save()
+
     def update_categories_for_all_products(self):
         all_grouped_products = GroupedProduct.objects.all()
-        # all_grouped_products = GroupedProduct.objects.filter(id=1675)
         for grouped_product in all_grouped_products:
             grouped_product_shopify_id = grouped_product.external_id
             shopify_product_queryset = ShopifyProduct.objects.filter(
                 product_id=grouped_product_shopify_id,
             )
             if shopify_product_queryset.count() > 0:
                 product = shopify_product_queryset.last()
```

### Comparing `artd-shopify-1.1.3/artd_shopify.egg-info/PKG-INFO` & `artd-shopify-1.1.4/artd_shopify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-shopify
-Version: 1.1.3
+Version: 1.1.4
 Summary: ArtD Shopify.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-shopify-1.1.3/artd_shopify.egg-info/SOURCES.txt` & `artd-shopify-1.1.4/artd_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.3/setup.cfg` & `artd-shopify-1.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd-shopify
-version = 1.1.3
+version = 1.1.4
 long_description_content_type = text/markdown
 description = ArtD Shopify.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
@@ -32,16 +32,16 @@
 packages = find:
 install_requires = 
 	Django>=4.2
 	django-json-widget==1.1.1
 	pillow==10.2.0
 	artd-location==1.0.2
 	artd-partner==1.0.1
-	artd-product==1.0.9
+	artd-price-list==1.0.7
+	artd-product==1.0.10
+	artd-stock==1.0.6
 	artd-urls==1.0.2
-	artd_price_list==1.0.6
-	artd-stock==1.0.5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

