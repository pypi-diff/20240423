# Comparing `tmp/django-custom-modal-admin-0.2.2.tar.gz` & `tmp/django_custom_modal_admin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-custom-modal-admin-0.2.2.tar", last modified: Tue Apr 18 14:06:00 2023, max compression
+gzip compressed data, was "django_custom_modal_admin-1.0.0.tar", last modified: Tue Apr 23 11:03:32 2024, max compression
```

## Comparing `django-custom-modal-admin-0.2.2.tar` & `django_custom_modal_admin-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.228304 django-custom-modal-admin-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-18 14:06:00.228304 django-custom-modal-admin-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.220304 django-custom-modal-admin-0.2.2/custom_modal_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.216304 django-custom-modal-admin-0.2.2/custom_modal_admin/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.220304 django-custom-modal-admin-0.2.2/custom_modal_admin/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/static/css/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.224305 django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/custom_modal_admin.js
--rw-r--r--   0 runner    (1001) docker     (123)   253747 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:06:00.224305 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:05:59.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 14:06:00.000000 django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 14:06:00.228304 django-custom-modal-admin-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-04-18 14:05:49.000000 django-custom-modal-admin-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:03:32.975913 django_custom_modal_admin-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-23 11:03:32.975913 django_custom_modal_admin-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:03:32.975913 django_custom_modal_admin-1.0.0/custom_modal_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/custom_modal_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/custom_modal_admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/custom_modal_admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:03:32.971912 django_custom_modal_admin-1.0.0/custom_modal_admin/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:03:32.975913 django_custom_modal_admin-1.0.0/custom_modal_admin/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    35973 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/custom_modal_admin/static/css/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:03:32.975913 django_custom_modal_admin-1.0.0/custom_modal_admin/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/custom_modal_admin/static/js/custom_modal_admin.js
+-rw-r--r--   0 runner    (1001) docker     (127)   253747 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/custom_modal_admin/static/js/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:03:32.975913 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-23 11:03:32.000000 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 11:03:32.000000 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:03:32.000000 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:03:32.000000 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 11:03:32.000000 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 11:03:32.000000 django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-23 11:03:32.979913 django_custom_modal_admin-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2296 2024-04-23 11:03:29.000000 django_custom_modal_admin-1.0.0/setup.py
```

### Comparing `django-custom-modal-admin-0.2.2/CONTRIBUTING.rst` & `django_custom_modal_admin-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/LICENSE.md` & `django_custom_modal_admin-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/PKG-INFO` & `django_custom_modal_admin-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: django-custom-modal-admin
-Version: 0.2.2
+Version: 1.0.0
 Summary: Your project description goes here
 Home-page: https://github.com/frankhood/django-custom-modal-admin
 Author: FrankHood Business Solutions srl
 Author-email: info@frankhood.it
 License: MIT
 Keywords: django-custom-modal-admin
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.md
+Requires-Dist: Django>=3.2
 
 =============================
 Django custom modal admin
 =============================
 
 .. image:: https://badge.fury.io/py/django-custom-modal-admin.svg/?style=flat-square
     :target: https://badge.fury.io/py/django-custom-modal-admin
```

### Comparing `django-custom-modal-admin-0.2.2/README.rst` & `django_custom_modal_admin-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/custom_modal_admin/static/css/jquery-ui.css` & `django_custom_modal_admin-1.0.0/custom_modal_admin/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/custom_modal_admin.js` & `django_custom_modal_admin-1.0.0/custom_modal_admin/static/js/custom_modal_admin.js`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/custom_modal_admin/static/js/jquery-ui.min.js` & `django_custom_modal_admin-1.0.0/custom_modal_admin/static/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/PKG-INFO` & `django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: django-custom-modal-admin
-Version: 0.2.2
+Version: 1.0.0
 Summary: Your project description goes here
 Home-page: https://github.com/frankhood/django-custom-modal-admin
 Author: FrankHood Business Solutions srl
 Author-email: info@frankhood.it
 License: MIT
 Keywords: django-custom-modal-admin
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.md
+Requires-Dist: Django>=3.2
 
 =============================
 Django custom modal admin
 =============================
 
 .. image:: https://badge.fury.io/py/django-custom-modal-admin.svg/?style=flat-square
     :target: https://badge.fury.io/py/django-custom-modal-admin
```

### Comparing `django-custom-modal-admin-0.2.2/django_custom_modal_admin.egg-info/SOURCES.txt` & `django_custom_modal_admin-1.0.0/django_custom_modal_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/setup.cfg` & `django_custom_modal_admin-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.2/setup.py` & `django_custom_modal_admin-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import os
 import re
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
@@ -33,15 +32,15 @@
         sys.exit()
     os.system("python setup.py sdist upload")
     os.system("python setup.py bdist_wheel upload")
     sys.exit()
 
 if sys.argv[-1] == "tag":
     print("Tagging the version on git:")
-    os.system("git tag -a %s -m 'version %s'" % (version, version))
+    os.system(f"git tag -a {version} -m 'version {version}'")
     os.system("git push --tags")
     sys.exit()
 
 readme = open("README.rst").read()
 history = open("HISTORY.rst").read().replace(".. :changelog:", "")
 requirements = open("requirements.txt").readlines()
 
@@ -59,17 +58,18 @@
     include_package_data=True,
     install_requires=requirements,
     license="MIT",
     zip_safe=False,
     keywords="django-custom-modal-admin",
     classifiers=[
         "Development Status :: 3 - Alpha",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

