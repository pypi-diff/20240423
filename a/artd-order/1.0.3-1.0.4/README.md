# Comparing `tmp/artd-order-1.0.3.tar.gz` & `tmp/artd-order-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-order-1.0.3.tar", last modified: Mon Apr 22 16:14:36 2024, max compression
+gzip compressed data, was "artd-order-1.0.4.tar", last modified: Mon Apr 22 22:29:20 2024, max compression
```

## Comparing `artd-order-1.0.3.tar` & `artd-order-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:55:41.000000 artd-order-1.0.3/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      134 2024-03-04 16:30:21.000000 artd-order-1.0.3/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1974 2024-04-22 16:14:36.534749 artd-order-1.0.3/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      879 2024-03-04 04:47:59.000000 artd-order-1.0.3/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    12441 2024-03-10 18:59:01.000000 artd-order-1.0.3/artd_order/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      241 2024-03-04 04:14:34.000000 artd-order-1.0.3/artd_order/apps.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/data/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/data/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      398 2024-03-04 04:37:56.000000 artd-order-1.0.3/artd_order/data/order_delivery_methods.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      681 2024-03-04 04:51:01.000000 artd-order-1.0.3/artd_order/data/order_status.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.524749 artd-order-1.0.3/artd_order/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.524749 artd-order-1.0.3/artd_order/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     8142 2024-03-10 18:48:51.000000 artd-order-1.0.3/artd_order/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.524749 artd-order-1.0.3/artd_order/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     9698 2024-03-10 18:56:30.000000 artd-order-1.0.3/artd_order/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/management/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/management/__init__.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/management/commands/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/management/commands/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1732 2024-03-06 17:56:34.000000 artd-order-1.0.3/artd_order/management/commands/create_base_order_delivery_method.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1016 2024-03-04 04:51:47.000000 artd-order-1.0.3/artd_order/management/commands/create_order_statuses.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    26140 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5027 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/migrations/0002_order_external_id_order_source_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      704 2024-03-10 06:10:21.000000 artd-order-1.0.3/artd_order/migrations/0003_alter_orderadress_city.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      752 2024-03-10 15:06:13.000000 artd-order-1.0.3/artd_order/migrations/0004_alter_order_coupon_code.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      986 2024-03-10 15:28:36.000000 artd-order-1.0.3/artd_order/migrations/0005_orderadress_json_data_orderstatus_json_data_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2989 2024-03-10 18:47:52.000000 artd-order-1.0.3/artd_order/migrations/0006_alter_order_json_data_alter_order_order_status_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    12430 2024-03-10 18:47:44.000000 artd-order-1.0.3/artd_order/models.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      756 2024-03-10 15:14:21.000000 artd-order-1.0.3/artd_order/signals.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/tests.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       63 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_order/views.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_order.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1974 2024-04-22 16:14:36.000000 artd-order-1.0.3/artd_order.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1288 2024-04-22 16:14:36.000000 artd-order-1.0.3/artd_order.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-22 16:14:36.000000 artd-order-1.0.3/artd_order.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      206 2024-04-22 16:14:36.000000 artd-order-1.0.3/artd_order.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       25 2024-04-22 16:14:36.000000 artd-order-1.0.3/artd_order.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:14:36.534749 artd-order-1.0.3/artd_packages/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_packages/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_packages/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3713 2024-03-10 14:55:34.000000 artd-order-1.0.3/artd_packages/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-10 14:55:56.000000 artd-order-1.0.3/artd_packages/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:41.000000 artd-order-1.0.3/artd_packages/wsgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1247 2024-04-22 16:14:36.534749 artd-order-1.0.3/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:55:41.000000 artd-order-1.0.3/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.351771 artd-order-1.0.4/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:55:41.000000 artd-order-1.0.4/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      134 2024-03-04 16:30:21.000000 artd-order-1.0.4/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1974 2024-04-22 22:29:20.351771 artd-order-1.0.4/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      879 2024-03-04 04:47:59.000000 artd-order-1.0.4/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    12441 2024-03-10 18:59:01.000000 artd-order-1.0.4/artd_order/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      241 2024-03-04 04:14:34.000000 artd-order-1.0.4/artd_order/apps.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/data/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/data/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      398 2024-03-04 04:37:56.000000 artd-order-1.0.4/artd_order/data/order_delivery_methods.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      681 2024-03-04 04:51:01.000000 artd-order-1.0.4/artd_order/data/order_status.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     8142 2024-03-10 18:48:51.000000 artd-order-1.0.4/artd_order/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     9698 2024-03-10 18:56:30.000000 artd-order-1.0.4/artd_order/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.351771 artd-order-1.0.4/artd_order/management/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/management/__init__.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.351771 artd-order-1.0.4/artd_order/management/commands/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/management/commands/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1732 2024-03-06 17:56:34.000000 artd-order-1.0.4/artd_order/management/commands/create_base_order_delivery_method.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1016 2024-03-04 04:51:47.000000 artd-order-1.0.4/artd_order/management/commands/create_order_statuses.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.351771 artd-order-1.0.4/artd_order/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    26140 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5027 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/migrations/0002_order_external_id_order_source_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      704 2024-03-10 06:10:21.000000 artd-order-1.0.4/artd_order/migrations/0003_alter_orderadress_city.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      752 2024-03-10 15:06:13.000000 artd-order-1.0.4/artd_order/migrations/0004_alter_order_coupon_code.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      986 2024-03-10 15:28:36.000000 artd-order-1.0.4/artd_order/migrations/0005_orderadress_json_data_orderstatus_json_data_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2989 2024-03-10 18:47:52.000000 artd-order-1.0.4/artd_order/migrations/0006_alter_order_json_data_alter_order_order_status_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    12430 2024-03-10 18:47:44.000000 artd-order-1.0.4/artd_order/models.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      756 2024-03-10 15:14:21.000000 artd-order-1.0.4/artd_order/signals.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/tests.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       63 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_order/views.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.341771 artd-order-1.0.4/artd_order.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1974 2024-04-22 22:29:20.000000 artd-order-1.0.4/artd_order.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1288 2024-04-22 22:29:20.000000 artd-order-1.0.4/artd_order.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-22 22:29:20.000000 artd-order-1.0.4/artd_order.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      223 2024-04-22 22:29:20.000000 artd-order-1.0.4/artd_order.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       25 2024-04-22 22:29:20.000000 artd-order-1.0.4/artd_order.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:29:20.351771 artd-order-1.0.4/artd_packages/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_packages/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_packages/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3730 2024-04-22 22:28:21.000000 artd-order-1.0.4/artd_packages/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-10 14:55:56.000000 artd-order-1.0.4/artd_packages/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:41.000000 artd-order-1.0.4/artd_packages/wsgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1265 2024-04-22 22:29:20.351771 artd-order-1.0.4/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:55:41.000000 artd-order-1.0.4/setup.py
```

### Comparing `artd-order-1.0.3/LICENSE` & `artd-order-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/PKG-INFO` & `artd-order-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-order
-Version: 1.0.3
+Version: 1.0.4
 Summary: ArtD Order.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-order-1.0.3/README.rst` & `artd-order-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/admin.py` & `artd-order-1.0.4/artd_order/admin.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/data/order_status.py` & `artd-order-1.0.4/artd_order/data/order_status.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/locale/en/LC_MESSAGES/django.po` & `artd-order-1.0.4/artd_order/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/locale/es/LC_MESSAGES/django.po` & `artd-order-1.0.4/artd_order/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/management/commands/create_base_order_delivery_method.py` & `artd-order-1.0.4/artd_order/management/commands/create_base_order_delivery_method.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/management/commands/create_order_statuses.py` & `artd-order-1.0.4/artd_order/management/commands/create_order_statuses.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/migrations/0001_initial.py` & `artd-order-1.0.4/artd_order/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/migrations/0002_order_external_id_order_source_and_more.py` & `artd-order-1.0.4/artd_order/migrations/0002_order_external_id_order_source_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/migrations/0003_alter_orderadress_city.py` & `artd-order-1.0.4/artd_order/migrations/0003_alter_orderadress_city.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/migrations/0004_alter_order_coupon_code.py` & `artd-order-1.0.4/artd_order/migrations/0004_alter_order_coupon_code.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/migrations/0005_orderadress_json_data_orderstatus_json_data_and_more.py` & `artd-order-1.0.4/artd_order/migrations/0005_orderadress_json_data_orderstatus_json_data_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/migrations/0006_alter_order_json_data_alter_order_order_status_and_more.py` & `artd-order-1.0.4/artd_order/migrations/0006_alter_order_json_data_alter_order_order_status_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/models.py` & `artd-order-1.0.4/artd_order/models.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order/signals.py` & `artd-order-1.0.4/artd_order/signals.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_order.egg-info/PKG-INFO` & `artd-order-1.0.4/artd_order.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-order
-Version: 1.0.3
+Version: 1.0.4
 Summary: ArtD Order.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-order-1.0.3/artd_order.egg-info/SOURCES.txt` & `artd-order-1.0.4/artd_order.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/artd_packages/settings.py` & `artd-order-1.0.4/artd_packages/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "django.contrib.staticfiles",
     "django_json_widget",
     "dal",
     "dal_select2",
     "artd_location",
     "artd_partner",
     "artd_customer",
+    "artd_urls",
     "artd_product",
     "artd_price_list",
     "artd_stock",
     "artd_promotion",
     "artd_order",
 ]
```

### Comparing `artd-order-1.0.3/artd_packages/urls.py` & `artd-order-1.0.4/artd_packages/urls.py`

 * *Files identical despite different names*

### Comparing `artd-order-1.0.3/setup.cfg` & `artd-order-1.0.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd-order
-version = 1.0.3
+version = 1.0.4
 long_description_content_type = text/markdown
 description = ArtD Order.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
@@ -30,19 +30,20 @@
 [options]
 include_package_data = true
 packages = find:
 install_requires = 
 	Django>=4.2.10
 	django-admin==2.0.2
 	django-json-widget==1.1.1
+	artd-customer==1.0.1
 	artd-location==1.0.2
 	artd-partner==1.0.1
-	artd-customer==1.0.1
-	artd-product==1.0.7
-	artd_price_list==1.0.4
-	artd_promotion==1.0.3
-	artd-stock==1.0.4
+	artd-price-list==1.0.6
+	artd-product==1.0.9
+	artd-promotion==1.0.4
+	artd-stock==1.0.5
+	artd-urls==1.0.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

