# Comparing `tmp/django-rest-gen-0.0.9.tar.gz` & `tmp/django_rest_gen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rest-gen-0.0.9.tar", last modified: Mon Feb 19 09:03:52 2024, max compression
+gzip compressed data, was "django_rest_gen-0.1.0.tar", last modified: Tue Apr 23 18:08:42 2024, max compression
```

## Comparing `django-rest-gen-0.0.9.tar` & `django_rest_gen-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-02-19 09:03:52.083188 django-rest-gen-0.0.9/
--rw-r--r--   0 aalobaid   (501) staff       (20)    11357 2023-09-15 17:27:36.000000 django-rest-gen-0.0.9/LICENSE
--rw-r--r--   0 aalobaid   (501) staff       (20)     1725 2024-02-19 09:03:52.082968 django-rest-gen-0.0.9/PKG-INFO
--rw-r--r--   0 aalobaid   (501) staff       (20)     1204 2023-09-19 14:18:47.000000 django-rest-gen-0.0.9/README.md
--rw-r--r--   0 aalobaid   (501) staff       (20)      594 2024-02-19 09:01:58.000000 django-rest-gen-0.0.9/pyproject.toml
--rw-r--r--   0 aalobaid   (501) staff       (20)       38 2024-02-19 09:03:52.083227 django-rest-gen-0.0.9/setup.cfg
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-02-19 09:03:52.080227 django-rest-gen-0.0.9/src/
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-02-19 09:03:52.081862 django-rest-gen-0.0.9/src/django-rest-gen/
--rw-r--r--   0 aalobaid   (501) staff       (20)        0 2023-09-15 17:31:56.000000 django-rest-gen-0.0.9/src/django-rest-gen/__init__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)      961 2023-09-19 13:33:46.000000 django-rest-gen-0.0.9/src/django-rest-gen/__main__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)    10155 2023-09-25 14:50:59.000000 django-rest-gen-0.0.9/src/django-rest-gen/apigen.py
--rw-r--r--   0 aalobaid   (501) staff       (20)      319 2023-09-17 17:32:50.000000 django-rest-gen-0.0.9/src/django-rest-gen/utils.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-02-19 09:03:52.082778 django-rest-gen-0.0.9/src/django_rest_gen.egg-info/
--rw-r--r--   0 aalobaid   (501) staff       (20)     1725 2024-02-19 09:03:52.000000 django-rest-gen-0.0.9/src/django_rest_gen.egg-info/PKG-INFO
--rw-r--r--   0 aalobaid   (501) staff       (20)      327 2024-02-19 09:03:52.000000 django-rest-gen-0.0.9/src/django_rest_gen.egg-info/SOURCES.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)        1 2024-02-19 09:03:52.000000 django-rest-gen-0.0.9/src/django_rest_gen.egg-info/dependency_links.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)       16 2024-02-19 09:03:52.000000 django-rest-gen-0.0.9/src/django_rest_gen.egg-info/top_level.txt
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.837767 django_rest_gen-0.1.0/
+-rw-r--r--   0 aalobaid   (501) staff       (20)    11357 2023-09-15 17:27:36.000000 django_rest_gen-0.1.0/LICENSE
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1820 2024-04-23 18:08:42.837586 django_rest_gen-0.1.0/PKG-INFO
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1299 2024-04-23 15:59:50.000000 django_rest_gen-0.1.0/README.md
+-rw-r--r--   0 aalobaid   (501) staff       (20)      594 2024-04-23 18:08:24.000000 django_rest_gen-0.1.0/pyproject.toml
+-rw-r--r--   0 aalobaid   (501) staff       (20)       38 2024-04-23 18:08:42.837812 django_rest_gen-0.1.0/setup.cfg
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.834946 django_rest_gen-0.1.0/src/
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.836373 django_rest_gen-0.1.0/src/django_rest_gen/
+-rw-r--r--   0 aalobaid   (501) staff       (20)        0 2023-09-15 17:31:56.000000 django_rest_gen-0.1.0/src/django_rest_gen/__init__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)      961 2023-09-19 13:33:46.000000 django_rest_gen-0.1.0/src/django_rest_gen/__main__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)    10461 2024-04-22 17:00:14.000000 django_rest_gen-0.1.0/src/django_rest_gen/apigen.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)      319 2023-09-17 17:32:50.000000 django_rest_gen-0.1.0/src/django_rest_gen/utils.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.837381 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1820 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/PKG-INFO
+-rw-r--r--   0 aalobaid   (501) staff       (20)      352 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)        1 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)       16 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/top_level.txt
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.837078 django_rest_gen-0.1.0/tests/
+-rw-r--r--   0 aalobaid   (501) staff       (20)     3120 2024-04-23 15:49:34.000000 django_rest_gen-0.1.0/tests/test_serializer.py
```

### Comparing `django-rest-gen-0.0.9/LICENSE` & `django_rest_gen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-gen-0.0.9/PKG-INFO` & `django_rest_gen-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: django-rest-gen
-Version: 0.0.9
+Version: 0.1.0
 Summary: Rest API Code Generator
 Author-email: Ahmad Alobaid <ahmad88me@gmail.com>
 Project-URL: Homepage, https://github.com/ahmad88me/django-rest-gen
 Project-URL: Bug Tracker, https://github.com/ahmad88me/django-rest-gen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-rest-gen
+![tests](https://github.com/ahmad88me/django-rest-gen/actions/workflows/pytest.yml/badge.svg)
+
 This generates a fully functioning apis using generated serializers and class-views. 
 
 
 # How to use it
 1. Install it in your django project `pip install django-rest-gen`.
-2. Run it and specify your app `python -m django-rest-gen`. You should also
-specify the appropriate arguments (e.g., `python -m django-rest-gen  --settings iires/settings.py --apppath iirapp`)
+2. Run it and specify your app `python -m django_rest_gen`. You should also
+specify the appropriate arguments (e.g., `python -m django_rest_gen  --settings iires/settings.py --apppath iirapp`)
 *Note: if the file already exists and is not empty, the content will be printed instead in the stdout*
 
 ## Arguments
 ```
-usage: django-rest-gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
+usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
 
 Generate Django REST API code
 
 optional arguments:
   -h, --help            show this help message and exit
   --pythonpath PYTHONPATH
                         Python Path directory.
```

### Comparing `django-rest-gen-0.0.9/README.md` & `django_rest_gen-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # django-rest-gen
+![tests](https://github.com/ahmad88me/django-rest-gen/actions/workflows/pytest.yml/badge.svg)
+
 This generates a fully functioning apis using generated serializers and class-views. 
 
 
 # How to use it
 1. Install it in your django project `pip install django-rest-gen`.
-2. Run it and specify your app `python -m django-rest-gen`. You should also
-specify the appropriate arguments (e.g., `python -m django-rest-gen  --settings iires/settings.py --apppath iirapp`)
+2. Run it and specify your app `python -m django_rest_gen`. You should also
+specify the appropriate arguments (e.g., `python -m django_rest_gen  --settings iires/settings.py --apppath iirapp`)
 *Note: if the file already exists and is not empty, the content will be printed instead in the stdout*
 
 ## Arguments
 ```
-usage: django-rest-gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
+usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
 
 Generate Django REST API code
 
 optional arguments:
   -h, --help            show this help message and exit
   --pythonpath PYTHONPATH
                         Python Path directory.
```

### Comparing `django-rest-gen-0.0.9/pyproject.toml` & `django_rest_gen-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-rest-gen"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Ahmad Alobaid", email="ahmad88me@gmail.com" },
 ]
 description = "Rest API Code Generator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django-rest-gen-0.0.9/src/django-rest-gen/__main__.py` & `django_rest_gen-0.1.0/src/django_rest_gen/__main__.py`

 * *Files identical despite different names*

### Comparing `django-rest-gen-0.0.9/src/django-rest-gen/apigen.py` & `django_rest_gen-0.1.0/src/django_rest_gen/apigen.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 import django
 from django.db import models
 
 
 def get_classes(models_obj):
     """
     Get class names from models.py file
-
     :param fpath: the path of the models.py file
     :return: list of classes
     """
     # Get classes
     clsmembers = inspect.getmembers(models_obj, inspect.isclass)
 
     # Filter Models
     # classes = [(c[0], c[1]._meta.verbose_name_plural.title()) for c in clsmembers if issubclass(c[1], models.Model)]
     classes = [(c[0], c[1]._meta.verbose_name_plural.title(), c[1]._meta.verbose_name.title()) for c in clsmembers if issubclass(c[1], models.Model)]
 
-
     print(f"classes: {classes}")
     return classes
 
 
 def load_models(python_path, models_fpath, settings_fpath):
     """
     Load models from the django project and returns the module object
@@ -40,15 +38,15 @@
     # Setup Django
     settings_stops = settings_fpath.split(os.sep)
     proj_settings = ".".join(settings_stops[-2:])
     if proj_settings[-3:] == ".py":
         proj_settings = proj_settings[:-3]
 
     print(f"Project settings {proj_settings}")
-    os.environ["DJANGO_SETTINGS_MODULE"] = proj_settings #"iires.settings"
+    os.environ["DJANGO_SETTINGS_MODULE"] = proj_settings
     django.setup()
 
     stops = models_fpath.split(os.sep)
     app_name = stops[-2]
     parts = stops[-1].split(".")
     mod_name = ".".join(parts[:-1])
     mod_pkg_name = f"{app_name}.{mod_name}"
@@ -126,14 +124,15 @@
 from rest_framework.response import Response
 from rest_framework.reverse import reverse
 from rest_framework import generics\n\n"""
     if write:
         with open(views_path, "a") as f:
             f.write(content)
     else:
+        print("\n\n\n\n=========================== views.py ===========================\n\n")
         print(content)
 
 
 def add_serializers_imports(app_path, serializers_path, write=False):
     """
     Add the imports for serializers.py
     :param app_path:
@@ -143,14 +142,15 @@
     """
     content = f"""from {app_path}.models import *
 from rest_framework import serializers\n\n"""
     if write:
         with open(serializers_path, "a") as f:
             f.write(content)
     else:
+        print("\n\n\n\n=========================== serializers.py ===========================\n\n")
         print(content)
 
 
 def write_root_view(views_path, classes, write):
     """
     Write the root api view
     :param views_path:
@@ -180,15 +180,14 @@
 
 def write_views(classes, views_path, app_path):
     """
     Write API views
     :param classes:
     :param views_path:
     :param app_path:
-
     :return: None
     """
     empty = utils.empty_fpath(fpath=views_path)
     add_views_imports(views_path=views_path, app_path=app_path, write=empty)
     write_root_view(views_path=views_path, classes=classes, write=empty)
     for c in classes:
         write_class_view(class_name=c[0], fpath=views_path, write=empty)
@@ -205,27 +204,27 @@
     content = f"""from {app_path}.models import *
 from {app_path} import views
 from django.urls import path, re_path, include\n\n"""
     if write:
         with open(urls_path, "a") as f:
             f.write(content)
     else:
+        print("\n\n\n\n=========================== urls.py ===========================\n\n")
         print(content)
 
 
 def get_class_url_name(verbose_name, joiner="_"):
     """
     Transform the class verbose name to a url friendly name
     :param verbose_name:
     :param joiner:
     :return:
     """
     url_name = verbose_name.replace(" ", joiner)
     url_name = url_name.lower()
-    # print(f" {verbose_name} -> {url_name}")
     return url_name
 
 
 def get_class_url(class_pair):
     """
     Appends the class url path to urls.py
     :param class_pair:
@@ -298,19 +297,20 @@
     :param admin_path:
     :return:
     """
     content = ""
     for c in classes:
         content += get_class_admin(c)
     empty = utils.empty_fpath(admin_path)
+    content = get_admin_imports(app_path) + content
     if empty:
         with open(admin_path, "a") as f:
-            content = get_admin_imports(app_path) + content
             f.write(content)
     else:
+        print("\n\n\n\n=========================== admin.py ===========================\n\n")
         print(content)
 
 
 def write_dummy(classes, app_path, dummy_path, overwrite):
     """
 
     :param classes:
```

### Comparing `django-rest-gen-0.0.9/src/django_rest_gen.egg-info/PKG-INFO` & `django_rest_gen-0.1.0/src/django_rest_gen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: django-rest-gen
-Version: 0.0.9
+Version: 0.1.0
 Summary: Rest API Code Generator
 Author-email: Ahmad Alobaid <ahmad88me@gmail.com>
 Project-URL: Homepage, https://github.com/ahmad88me/django-rest-gen
 Project-URL: Bug Tracker, https://github.com/ahmad88me/django-rest-gen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-rest-gen
+![tests](https://github.com/ahmad88me/django-rest-gen/actions/workflows/pytest.yml/badge.svg)
+
 This generates a fully functioning apis using generated serializers and class-views. 
 
 
 # How to use it
 1. Install it in your django project `pip install django-rest-gen`.
-2. Run it and specify your app `python -m django-rest-gen`. You should also
-specify the appropriate arguments (e.g., `python -m django-rest-gen  --settings iires/settings.py --apppath iirapp`)
+2. Run it and specify your app `python -m django_rest_gen`. You should also
+specify the appropriate arguments (e.g., `python -m django_rest_gen  --settings iires/settings.py --apppath iirapp`)
 *Note: if the file already exists and is not empty, the content will be printed instead in the stdout*
 
 ## Arguments
 ```
-usage: django-rest-gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
+usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
 
 Generate Django REST API code
 
 optional arguments:
   -h, --help            show this help message and exit
   --pythonpath PYTHONPATH
                         Python Path directory.
```

