# Comparing `tmp/ellar_django_module-1.0.5.tar.gz` & `tmp/ellar_django_module-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar_django_module-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar_django_module-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar_django_module-1.0.5.tar` & `ellar_django_module-1.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7330 2024-03-07 11:31:03.369984 ellar_django_module-1.0.5/README.md
--rw-r--r--   0        0        0      158 2024-03-07 11:31:03.369984 ellar_django_module-1.0.5/ellar_django/__init__.py
--rw-r--r--   0        0        0     4729 2024-03-07 11:31:03.369984 ellar_django_module-1.0.5/ellar_django/commands.py
--rw-r--r--   0        0        0     1424 2024-03-07 11:31:03.369984 ellar_django_module-1.0.5/ellar_django/middleware.py
--rw-r--r--   0        0        0     1391 2024-03-07 11:31:03.373983 ellar_django_module-1.0.5/ellar_django/module.py
--rw-r--r--   0        0        0     2329 2024-03-07 11:31:03.373983 ellar_django_module-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     9188 1970-01-01 00:00:00.000000 ellar_django_module-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     7330 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/README.md
+-rw-r--r--   0        0        0      158 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/__init__.py
+-rw-r--r--   0        0        0     2228 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/commands.py
+-rw-r--r--   0        0        0     1424 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/middleware.py
+-rw-r--r--   0        0        0     1391 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/ellar_django/module.py
+-rw-r--r--   0        0        0     2329 2024-04-23 18:48:39.706184 ellar_django_module-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9188 1970-01-01 00:00:00.000000 ellar_django_module-1.0.6/PKG-INFO
```

### Comparing `ellar_django_module-1.0.5/README.md` & `ellar_django_module-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ellar_django_module-1.0.5/ellar_django/middleware.py` & `ellar_django_module-1.0.6/ellar_django/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar_django_module-1.0.5/ellar_django/module.py` & `ellar_django_module-1.0.6/ellar_django/module.py`

 * *Files identical despite different names*

### Comparing `ellar_django_module-1.0.5/pyproject.toml` & `ellar_django_module-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ellar_django_module-1.0.5/PKG-INFO` & `ellar_django_module-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar-django-module
-Version: 1.0.5
+Version: 1.0.6
 Summary: Enables Django ORM and Admin feature in Ellar's application
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

