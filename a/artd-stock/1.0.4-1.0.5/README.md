# Comparing `tmp/artd-stock-1.0.4.tar.gz` & `tmp/artd-stock-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-stock-1.0.4.tar", last modified: Mon Apr 22 16:12:03 2024, max compression
+gzip compressed data, was "artd-stock-1.0.5.tar", last modified: Mon Apr 22 22:14:36 2024, max compression
```

## Comparing `artd-stock-1.0.4.tar` & `artd-stock-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:55:31.000000 artd-stock-1.0.4/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      134 2024-03-04 16:05:08.000000 artd-stock-1.0.4/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1864 2024-04-22 16:12:03.714770 artd-stock-1.0.4/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      769 2024-03-04 16:04:44.000000 artd-stock-1.0.4/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_packages/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_packages/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_packages/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3642 2024-03-10 05:34:59.000000 artd-stock-1.0.4/artd_packages/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-10 05:35:42.000000 artd-stock-1.0.4/artd_packages/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_packages/wsgi.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_stock/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3146 2024-03-10 05:50:17.000000 artd-stock-1.0.4/artd_stock/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      241 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/apps.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.704770 artd-stock-1.0.4/artd_stock/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.704770 artd-stock-1.0.4/artd_stock/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_stock/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      421 2024-03-10 05:42:39.000000 artd-stock-1.0.4/artd_stock/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2033 2024-03-10 05:42:32.000000 artd-stock-1.0.4/artd_stock/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.704770 artd-stock-1.0.4/artd_stock/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_stock/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1262 2024-03-10 05:54:38.000000 artd-stock-1.0.4/artd_stock/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2254 2024-03-10 05:54:34.000000 artd-stock-1.0.4/artd_stock/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_stock/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5381 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1346 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/migrations/0002_stock_external_id_stock_source_stocklog_external_id_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1949 2024-03-10 06:01:29.000000 artd-stock-1.0.4/artd_stock/migrations/0003_alter_stock_partner_alter_stock_product_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2479 2024-03-10 05:52:03.000000 artd-stock-1.0.4/artd_stock/models.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_stock/utils/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/utils/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1801 2024-03-01 15:55:31.000000 artd-stock-1.0.4/artd_stock/utils/generators.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 16:12:03.714770 artd-stock-1.0.4/artd_stock.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1864 2024-04-22 16:12:03.000000 artd-stock-1.0.4/artd_stock.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      893 2024-04-22 16:12:03.000000 artd-stock-1.0.4/artd_stock.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-22 16:12:03.000000 artd-stock-1.0.4/artd_stock.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      137 2024-04-22 16:12:03.000000 artd-stock-1.0.4/artd_stock.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       25 2024-04-22 16:12:03.000000 artd-stock-1.0.4/artd_stock.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1175 2024-04-22 16:12:03.714770 artd-stock-1.0.4/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:55:31.000000 artd-stock-1.0.4/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:55:31.000000 artd-stock-1.0.5/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      134 2024-03-04 16:05:08.000000 artd-stock-1.0.5/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1864 2024-04-22 22:14:36.011888 artd-stock-1.0.5/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      769 2024-03-04 16:04:44.000000 artd-stock-1.0.5/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.001888 artd-stock-1.0.5/artd_packages/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_packages/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_packages/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3659 2024-04-22 22:13:22.000000 artd-stock-1.0.5/artd_packages/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-10 05:35:42.000000 artd-stock-1.0.5/artd_packages/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_packages/wsgi.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/artd_stock/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3146 2024-03-10 05:50:17.000000 artd-stock-1.0.5/artd_stock/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      241 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/apps.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.001888 artd-stock-1.0.5/artd_stock/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.001888 artd-stock-1.0.5/artd_stock/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/artd_stock/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      421 2024-03-10 05:42:39.000000 artd-stock-1.0.5/artd_stock/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2033 2024-03-10 05:42:32.000000 artd-stock-1.0.5/artd_stock/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.001888 artd-stock-1.0.5/artd_stock/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/artd_stock/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1262 2024-03-10 05:54:38.000000 artd-stock-1.0.5/artd_stock/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2254 2024-03-10 05:54:34.000000 artd-stock-1.0.5/artd_stock/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/artd_stock/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5381 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1346 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/migrations/0002_stock_external_id_stock_source_stocklog_external_id_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1949 2024-03-10 06:01:29.000000 artd-stock-1.0.5/artd_stock/migrations/0003_alter_stock_partner_alter_stock_product_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2479 2024-03-10 05:52:03.000000 artd-stock-1.0.5/artd_stock/models.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/artd_stock/utils/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/utils/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1801 2024-03-01 15:55:31.000000 artd-stock-1.0.5/artd_stock/utils/generators.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-22 22:14:36.011888 artd-stock-1.0.5/artd_stock.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1864 2024-04-22 22:14:35.000000 artd-stock-1.0.5/artd_stock.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      893 2024-04-22 22:14:35.000000 artd-stock-1.0.5/artd_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-22 22:14:35.000000 artd-stock-1.0.5/artd_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      154 2024-04-22 22:14:35.000000 artd-stock-1.0.5/artd_stock.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       25 2024-04-22 22:14:35.000000 artd-stock-1.0.5/artd_stock.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1193 2024-04-22 22:14:36.011888 artd-stock-1.0.5/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:55:31.000000 artd-stock-1.0.5/setup.py
```

### Comparing `artd-stock-1.0.4/LICENSE` & `artd-stock-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/PKG-INFO` & `artd-stock-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-stock
-Version: 1.0.4
+Version: 1.0.5
 Summary: ArtD Stock.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-stock-1.0.4/README.rst` & `artd-stock-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_packages/settings.py` & `artd-stock-1.0.5/artd_packages/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "django_json_widget",
     "dal",
     "dal_select2",
     "artd_location",
     "artd_partner",
+    "artd_urls",
     "artd_product",
     "artd_stock",
 ]
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
```

### Comparing `artd-stock-1.0.4/artd_packages/urls.py` & `artd-stock-1.0.5/artd_packages/urls.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/admin.py` & `artd-stock-1.0.5/artd_stock/admin.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/locale/en/LC_MESSAGES/django.po` & `artd-stock-1.0.5/artd_stock/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/locale/es/LC_MESSAGES/django.mo` & `artd-stock-1.0.5/artd_stock/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/locale/es/LC_MESSAGES/django.po` & `artd-stock-1.0.5/artd_stock/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/migrations/0001_initial.py` & `artd-stock-1.0.5/artd_stock/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/migrations/0002_stock_external_id_stock_source_stocklog_external_id_and_more.py` & `artd-stock-1.0.5/artd_stock/migrations/0002_stock_external_id_stock_source_stocklog_external_id_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/migrations/0003_alter_stock_partner_alter_stock_product_and_more.py` & `artd-stock-1.0.5/artd_stock/migrations/0003_alter_stock_partner_alter_stock_product_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/models.py` & `artd-stock-1.0.5/artd_stock/models.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock/utils/generators.py` & `artd-stock-1.0.5/artd_stock/utils/generators.py`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/artd_stock.egg-info/PKG-INFO` & `artd-stock-1.0.5/artd_stock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-stock
-Version: 1.0.4
+Version: 1.0.5
 Summary: ArtD Stock.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-stock-1.0.4/artd_stock.egg-info/SOURCES.txt` & `artd-stock-1.0.5/artd_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-stock-1.0.4/setup.cfg` & `artd-stock-1.0.5/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd-stock
-version = 1.0.4
+version = 1.0.5
 long_description_content_type = text/markdown
 description = ArtD Stock.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
@@ -33,13 +33,14 @@
 install_requires = 
 	Django>=4.2.10
 	django-admin==2.0.2
 	django-json-widget==1.1.1
 	pillow==10.2.0
 	artd-location==1.0.2
 	artd-partner==1.0.1
-	artd-product==1.0.7
+	artd-product==1.0.9
+	artd-urls==1.0.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

