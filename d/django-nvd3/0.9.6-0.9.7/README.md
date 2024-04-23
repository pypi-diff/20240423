# Comparing `tmp/django-nvd3-0.9.6.tar.gz` & `tmp/django-nvd3-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-nvd3-0.9.6.tar", last modified: Thu Dec 10 11:25:01 2015, max compression
+gzip compressed data, was "dist/django-nvd3-0.9.7.tar", last modified: Thu Dec 10 13:41:54 2015, max compression
```

## Comparing `django-nvd3-0.9.6.tar` & `django-nvd3-0.9.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/
--rw-rw-r--   0 areski    (1000) areski    (1000)     2091 2015-10-27 22:50:23.000000 django-nvd3-0.9.6/setup.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     3088 2015-10-28 12:02:44.000000 django-nvd3-0.9.6/CHANGELOG.rst
--rw-rw-r--   0 areski    (1000) areski    (1000)       59 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/setup.cfg
--rw-rw-r--   0 areski    (1000) areski    (1000)     6217 2015-10-27 22:50:23.000000 django-nvd3-0.9.6/README.rst
--rw-rw-r--   0 areski    (1000) areski    (1000)       19 2015-12-10 11:24:50.000000 django-nvd3-0.9.6/requirements.txt
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/demoproject/
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/demoproject/demoproject/
--rw-rw-r--   0 areski    (1000) areski    (1000)    15827 2015-04-06 12:54:03.000000 django-nvd3-0.9.6/demoproject/demoproject/views.py
--rw-r--r--   0 areski    (1000) areski    (1000)     1434 2014-01-27 13:16:38.000000 django-nvd3-0.9.6/demoproject/demoproject/wsgi.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     6114 2015-04-06 12:54:03.000000 django-nvd3-0.9.6/demoproject/demoproject/settings.py
--rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:38.000000 django-nvd3-0.9.6/demoproject/demoproject/__init__.py
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/demoproject/demoproject/templatetags/
--rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:38.000000 django-nvd3-0.9.6/demoproject/demoproject/templatetags/__init__.py
--rw-r--r--   0 areski    (1000) areski    (1000)      143 2014-01-27 13:16:38.000000 django-nvd3-0.9.6/demoproject/demoproject/templatetags/demo_tags.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     1712 2015-04-06 12:54:03.000000 django-nvd3-0.9.6/demoproject/demoproject/urls.py
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/django_nvd3.egg-info/
--rw-r--r--   0 areski    (1000) areski    (1000)        1 2015-12-10 11:25:00.000000 django-nvd3-0.9.6/django_nvd3.egg-info/dependency_links.txt
--rw-r--r--   0 areski    (1000) areski    (1000)       35 2015-12-10 11:25:00.000000 django-nvd3-0.9.6/django_nvd3.egg-info/top_level.txt
--rw-r--r--   0 areski    (1000) areski    (1000)        1 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/django_nvd3.egg-info/not-zip-safe
--rw-r--r--   0 areski    (1000) areski    (1000)       19 2015-12-10 11:25:00.000000 django-nvd3-0.9.6/django_nvd3.egg-info/requires.txt
--rw-r--r--   0 areski    (1000) areski    (1000)    13032 2015-12-10 11:25:00.000000 django-nvd3-0.9.6/django_nvd3.egg-info/PKG-INFO
--rw-r--r--   0 areski    (1000) areski    (1000)     1033 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/django_nvd3.egg-info/SOURCES.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)      173 2015-10-28 12:02:44.000000 django-nvd3-0.9.6/MANIFEST.in
--rw-r--r--   0 areski    (1000) areski    (1000)     1141 2014-01-27 13:16:36.000000 django-nvd3-0.9.6/MIT-LICENSE.txt
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/nvd3_tests/
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/nvd3_tests/testproject/
--rw-r--r--   0 areski    (1000) areski    (1000)     6340 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/testproject/views.py
--rw-r--r--   0 areski    (1000) areski    (1000)     1434 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/testproject/wsgi.py
--rw-r--r--   0 areski    (1000) areski    (1000)     5691 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/testproject/settings.py
--rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/testproject/__init__.py
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/nvd3_tests/testproject/templatetags/
--rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/testproject/templatetags/__init__.py
--rw-r--r--   0 areski    (1000) areski    (1000)     1399 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/testproject/urls.py
--rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/__init__.py
--rw-r--r--   0 areski    (1000) areski    (1000)      254 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/nvd3_tests/manage.py
--rw-rw-r--   0 areski    (1000) areski    (1000)    13032 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/PKG-INFO
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/django_nvd3/
--rw-rw-r--   0 areski    (1000) areski    (1000)      628 2015-12-10 11:25:00.000000 django-nvd3-0.9.6/django_nvd3/__init__.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)      508 2015-12-10 11:24:58.000000 django-nvd3-0.9.6/django_nvd3/__init__.py
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 11:25:01.000000 django-nvd3-0.9.6/django_nvd3/templatetags/
--rw-r--r--   0 areski    (1000) areski    (1000)      162 2014-09-22 15:24:45.000000 django-nvd3-0.9.6/django_nvd3/templatetags/__init__.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     5809 2015-10-27 22:50:23.000000 django-nvd3-0.9.6/django_nvd3/templatetags/nvd3_tags.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     5232 2015-04-17 10:35:20.000000 django-nvd3-0.9.6/django_nvd3/templatetags/nvd3_tags.pyc
--rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.6/django_nvd3/templatetags/__init__.py
--rw-rw-r--   0 areski    (1000) areski    (1000)        7 2015-10-27 22:50:23.000000 django-nvd3-0.9.6/test_requirements.txt
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/
+-rw-rw-r--   0 areski    (1000) areski    (1000)     2091 2015-10-27 22:50:23.000000 django-nvd3-0.9.7/setup.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3281 2015-12-10 13:41:42.000000 django-nvd3-0.9.7/CHANGELOG.rst
+-rw-rw-r--   0 areski    (1000) areski    (1000)       59 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/setup.cfg
+-rw-rw-r--   0 areski    (1000) areski    (1000)     6217 2015-10-27 22:50:23.000000 django-nvd3-0.9.7/README.rst
+-rw-rw-r--   0 areski    (1000) areski    (1000)       19 2015-12-10 11:24:50.000000 django-nvd3-0.9.7/requirements.txt
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/demoproject/
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/demoproject/demoproject/
+-rw-rw-r--   0 areski    (1000) areski    (1000)    15827 2015-04-06 12:54:03.000000 django-nvd3-0.9.7/demoproject/demoproject/views.py
+-rw-r--r--   0 areski    (1000) areski    (1000)     1434 2014-01-27 13:16:38.000000 django-nvd3-0.9.7/demoproject/demoproject/wsgi.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     6114 2015-04-06 12:54:03.000000 django-nvd3-0.9.7/demoproject/demoproject/settings.py
+-rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:38.000000 django-nvd3-0.9.7/demoproject/demoproject/__init__.py
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/demoproject/demoproject/templatetags/
+-rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:38.000000 django-nvd3-0.9.7/demoproject/demoproject/templatetags/__init__.py
+-rw-r--r--   0 areski    (1000) areski    (1000)      143 2014-01-27 13:16:38.000000 django-nvd3-0.9.7/demoproject/demoproject/templatetags/demo_tags.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     1381 2015-12-10 13:41:42.000000 django-nvd3-0.9.7/demoproject/demoproject/urls.py
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/django_nvd3.egg-info/
+-rw-r--r--   0 areski    (1000) areski    (1000)        1 2015-12-10 13:41:53.000000 django-nvd3-0.9.7/django_nvd3.egg-info/dependency_links.txt
+-rw-r--r--   0 areski    (1000) areski    (1000)       35 2015-12-10 13:41:53.000000 django-nvd3-0.9.7/django_nvd3.egg-info/top_level.txt
+-rw-r--r--   0 areski    (1000) areski    (1000)        1 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/django_nvd3.egg-info/not-zip-safe
+-rw-r--r--   0 areski    (1000) areski    (1000)       19 2015-12-10 13:41:53.000000 django-nvd3-0.9.7/django_nvd3.egg-info/requires.txt
+-rw-r--r--   0 areski    (1000) areski    (1000)    13281 2015-12-10 13:41:53.000000 django-nvd3-0.9.7/django_nvd3.egg-info/PKG-INFO
+-rw-r--r--   0 areski    (1000) areski    (1000)     1033 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/django_nvd3.egg-info/SOURCES.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)      173 2015-10-28 12:02:44.000000 django-nvd3-0.9.7/MANIFEST.in
+-rw-r--r--   0 areski    (1000) areski    (1000)     1141 2014-01-27 13:16:36.000000 django-nvd3-0.9.7/MIT-LICENSE.txt
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/nvd3_tests/
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/nvd3_tests/testproject/
+-rw-r--r--   0 areski    (1000) areski    (1000)     6340 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/testproject/views.py
+-rw-r--r--   0 areski    (1000) areski    (1000)     1434 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/testproject/wsgi.py
+-rw-r--r--   0 areski    (1000) areski    (1000)     5691 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/testproject/settings.py
+-rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/testproject/__init__.py
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/nvd3_tests/testproject/templatetags/
+-rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/testproject/templatetags/__init__.py
+-rw-r--r--   0 areski    (1000) areski    (1000)     1399 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/testproject/urls.py
+-rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/__init__.py
+-rw-r--r--   0 areski    (1000) areski    (1000)      254 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/nvd3_tests/manage.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)    13281 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/PKG-INFO
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/django_nvd3/
+-rw-rw-r--   0 areski    (1000) areski    (1000)      628 2015-12-10 13:41:53.000000 django-nvd3-0.9.7/django_nvd3/__init__.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)      508 2015-12-10 13:41:51.000000 django-nvd3-0.9.7/django_nvd3/__init__.py
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2015-12-10 13:41:54.000000 django-nvd3-0.9.7/django_nvd3/templatetags/
+-rw-r--r--   0 areski    (1000) areski    (1000)      162 2014-09-22 15:24:45.000000 django-nvd3-0.9.7/django_nvd3/templatetags/__init__.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     5809 2015-10-27 22:50:23.000000 django-nvd3-0.9.7/django_nvd3/templatetags/nvd3_tags.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     6446 2015-12-10 11:28:30.000000 django-nvd3-0.9.7/django_nvd3/templatetags/nvd3_tags.pyc
+-rw-r--r--   0 areski    (1000) areski    (1000)        0 2014-01-27 13:16:39.000000 django-nvd3-0.9.7/django_nvd3/templatetags/__init__.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)        7 2015-10-27 22:50:23.000000 django-nvd3-0.9.7/test_requirements.txt
```

### Comparing `django-nvd3-0.9.6/setup.py` & `django-nvd3-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/CHANGELOG.rst` & `django-nvd3-0.9.7/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 .. :changelog:
 
 History
 -------
 
 
+0.9.7 (2015-12-10)
+------------------
+
+* fix test suit + remove python3.3 support (Django 1.9)
+* demoproject: update your urlpatterns to be a list of django.conf.urls.url() instances instead
+
+
 0.9.4 (2015-10-28)
 ------------------
 
 * add test_requirements.txt to MANIFEST.in
 
 
 0.9.2 (2015-10-27)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_173n05ao_/tmp77ugkn87_TarContainer/0/2.rst", line 195, column 0: CDATA terminal not found*

```diff
@@ -1,32 +1,34 @@
-.. :changelog: History ------- 0.9.4 (2015-10-28) ------------------ * add
-test_requirements.txt to MANIFEST.in 0.9.2 (2015-10-27) ------------------ *
-Fix test suits by @lgp171188 (L. Guruprasad) * Add Travis-CI test for Python
-version 3.4 & 3.5 0.9.1 (2015-10-12) ------------------ * Add changelog to
-MANIFEST.in 0.9.0 (2015-10-12) ------------------ * add charset to js script
-tag 0.8.2 (2015-04-06) ------------------ * bump python-nvd3==0.13.7 0.8.1
-(2015-04-06) ------------------ * fix error linePlusBarWithFocusChart 0.8.0
-(2015-04-06) ------------------ * add support for nvd3 version 1.7.1 * bump
-requirement python-nvd3==0.13.6 * remove lineplusbarwithfocuschart 0.7.8 (2015-
-03-09) ------------------ * python3 * replace 'unicode' with 'str' 0.6.1 (2013-
-12-05) ------------------ * fix y-series not sorted alphabetically thanks
-@miquelcamprodon 0.6.0 (2013-10-31) ------------------ * fixes on demo project
-to include js tag in html * update on simple_tag to work with Django 1.3 0.5.0
-(2013-10-09) ------------------ * change settings behavior, now it works with a
-global extra settings passed as kwargs * refactoring 0.4.1 (2013-10-04) -------
------------ * discreteBarChart support date on xAxis 0.4.0 (2013-10-03) -------
------------ * Support new chart linePlusBarWithFocusChart 0.3.1 (2013-09-30) --
----------------- * Documentation / Readme update 0.3.0 (2013-09-30) -----------
-------- * Use Bower to install D3 and NVD3 0.2.0 (2013-09-20) -----------------
-- * Enable resize by default 0.1.12 (2013-07-09) ------------------- *
-Generalise the axis_formatting 0.1.11 (2013-05-30) ------------------- *
-Python3 Fix for setup.py TypeError (by DanMeakin) 0.1.10 (2013-05-30) ---------
----------- * Add example for multichart with Date + test 0.1.9 (2013-04-06) ---
---------------- * Make sure we got something in chartype parameter / help the
-test 0.1.8 (2013-04-25) ------------------ * Option to use cdn or use local
-file for the JS and CSS 0.1.7 (2013-04-24) ------------------ * Add custom
-dateformat for tooltip : ``x_axis_date_format`` * display x-axis date in
-various format ie "%d %b %Y" 0.1.6 (2013-04-23) ------------------ * Add
-color_category : Define color category (eg. category10, category20,
-category20c) 0.1.5 (2013-04-23) ------------------ * Fix set height and width
-useset_graph_height and set_graph_width 0.1.4 (2013-04-23) ------------------ *
-Add tag_script_js : disable javascript
+.. :changelog: History ------- 0.9.7 (2015-12-10) ------------------ * fix test
+suit + remove python3.3 support (Django 1.9) * demoproject: update your
+urlpatterns to be a list of django.conf.urls.url() instances instead 0.9.4
+(2015-10-28) ------------------ * add test_requirements.txt to MANIFEST.in
+0.9.2 (2015-10-27) ------------------ * Fix test suits by @lgp171188 (L.
+Guruprasad) * Add Travis-CI test for Python version 3.4 & 3.5 0.9.1 (2015-10-
+12) ------------------ * Add changelog to MANIFEST.in 0.9.0 (2015-10-12) ------
+------------ * add charset to js script tag 0.8.2 (2015-04-06) ----------------
+-- * bump python-nvd3==0.13.7 0.8.1 (2015-04-06) ------------------ * fix error
+linePlusBarWithFocusChart 0.8.0 (2015-04-06) ------------------ * add support
+for nvd3 version 1.7.1 * bump requirement python-nvd3==0.13.6 * remove
+lineplusbarwithfocuschart 0.7.8 (2015-03-09) ------------------ * python3 *
+replace 'unicode' with 'str' 0.6.1 (2013-12-05) ------------------ * fix y-
+series not sorted alphabetically thanks @miquelcamprodon 0.6.0 (2013-10-31) ---
+--------------- * fixes on demo project to include js tag in html * update on
+simple_tag to work with Django 1.3 0.5.0 (2013-10-09) ------------------ *
+change settings behavior, now it works with a global extra settings passed as
+kwargs * refactoring 0.4.1 (2013-10-04) ------------------ * discreteBarChart
+support date on xAxis 0.4.0 (2013-10-03) ------------------ * Support new chart
+linePlusBarWithFocusChart 0.3.1 (2013-09-30) ------------------ * Documentation
+/ Readme update 0.3.0 (2013-09-30) ------------------ * Use Bower to install D3
+and NVD3 0.2.0 (2013-09-20) ------------------ * Enable resize by default
+0.1.12 (2013-07-09) ------------------- * Generalise the axis_formatting 0.1.11
+(2013-05-30) ------------------- * Python3 Fix for setup.py TypeError (by
+DanMeakin) 0.1.10 (2013-05-30) ------------------- * Add example for multichart
+with Date + test 0.1.9 (2013-04-06) ------------------ * Make sure we got
+something in chartype parameter / help the test 0.1.8 (2013-04-25) ------------
+------ * Option to use cdn or use local file for the JS and CSS 0.1.7 (2013-04-
+24) ------------------ * Add custom dateformat for tooltip :
+``x_axis_date_format`` * display x-axis date in various format ie "%d %b %Y"
+0.1.6 (2013-04-23) ------------------ * Add color_category : Define color
+category (eg. category10, category20, category20c) 0.1.5 (2013-04-23) ---------
+--------- * Fix set height and width useset_graph_height and set_graph_width
+0.1.4 (2013-04-23) ------------------ * Add tag_script_js : disable javascript
```

### Comparing `django-nvd3-0.9.6/README.rst` & `django-nvd3-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/demoproject/demoproject/views.py` & `django-nvd3-0.9.7/demoproject/demoproject/views.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/demoproject/demoproject/wsgi.py` & `django-nvd3-0.9.7/demoproject/demoproject/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/demoproject/demoproject/settings.py` & `django-nvd3-0.9.7/demoproject/demoproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/demoproject/demoproject/urls.py` & `django-nvd3-0.9.7/nvd3_tests/testproject/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,25 +5,22 @@
 # admin.autodiscover()
 
 urlpatterns = patterns('demoproject.views',
     # Examples:
     url(r'^$', 'home', name='home'),
     url(r'^piechart/', 'demo_piechart', name='demo_piechart'),
     url(r'^linechart/', 'demo_linechart', name='demo_linechart'),
-    url(r'^linechart_without_date/', 'demo_linechart_without_date', name='demo_linechart_without_date'),
     url(r'^linewithfocuschart/', 'demo_linewithfocuschart', name='demo_linewithfocuschart'),
     url(r'^multibarchart/', 'demo_multibarchart', name='demo_multibarchart'),
     url(r'^stackedareachart/', 'demo_stackedareachart', name='demo_stackedareachart'),
     url(r'^multibarhorizontalchart/', 'demo_multibarhorizontalchart', name='demo_multibarhorizontalchart'),
     url(r'^lineplusbarchart/', 'demo_lineplusbarchart', name='demo_lineplusbarchart'),
     url(r'^cumulativelinechart/', 'demo_cumulativelinechart', name='demo_cumulativelinechart'),
     url(r'^discretebarchart/', 'demo_discretebarchart', name='demo_discretebarchart'),
-    url(r'^discretebarchart_with_date/', 'demo_discretebarchart_with_date', name='demo_discretebarchart_date'),
     url(r'^scatterchart/', 'demo_scatterchart', name='demo_scatterchart'),
-    url(r'^linechart_with_ampm/', 'demo_linechart_with_ampm', name='demo_linechart_with_ampm'),
     # url(r'^demoproject/', include('demoproject.foo.urls')),
 
     # Uncomment the admin/doc line below to enable admin documentation:
     # url(r'^admin/doc/', include('django.contrib.admindocs.urls')),
 
     # Uncomment the next line to enable the admin:
     # url(r'^admin/', include(admin.site.urls)),
```

### Comparing `django-nvd3-0.9.6/django_nvd3.egg-info/PKG-INFO` & `django-nvd3-0.9.7/django_nvd3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-nvd3
-Version: 0.9.6
+Version: 0.9.7
 Summary: Django NVD3 - Chart Library for d3.js
 Home-page: http://github.com/areski/django-nvd3
 Author: Belaid Arezqui
 Author-email: areski@gmail.com
 License: MIT License
 Description: Django Wrapper for NVD3 - It's time for beautiful charts
         ========================================================
@@ -196,14 +196,21 @@
         
         
         
         History
         -------
         
         
+        0.9.7 (2015-12-10)
+        ------------------
+        
+        * fix test suit + remove python3.3 support (Django 1.9)
+        * demoproject: update your urlpatterns to be a list of django.conf.urls.url() instances instead
+        
+        
         0.9.4 (2015-10-28)
         ------------------
         
         * add test_requirements.txt to MANIFEST.in
         
         
         0.9.2 (2015-10-27)
```

### Comparing `django-nvd3-0.9.6/django_nvd3.egg-info/SOURCES.txt` & `django-nvd3-0.9.7/django_nvd3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/MIT-LICENSE.txt` & `django-nvd3-0.9.7/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/nvd3_tests/testproject/views.py` & `django-nvd3-0.9.7/nvd3_tests/testproject/views.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/nvd3_tests/testproject/wsgi.py` & `django-nvd3-0.9.7/nvd3_tests/testproject/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/nvd3_tests/testproject/settings.py` & `django-nvd3-0.9.7/nvd3_tests/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/PKG-INFO` & `django-nvd3-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-nvd3
-Version: 0.9.6
+Version: 0.9.7
 Summary: Django NVD3 - Chart Library for d3.js
 Home-page: http://github.com/areski/django-nvd3
 Author: Belaid Arezqui
 Author-email: areski@gmail.com
 License: MIT License
 Description: Django Wrapper for NVD3 - It's time for beautiful charts
         ========================================================
@@ -196,14 +196,21 @@
         
         
         
         History
         -------
         
         
+        0.9.7 (2015-12-10)
+        ------------------
+        
+        * fix test suit + remove python3.3 support (Django 1.9)
+        * demoproject: update your urlpatterns to be a list of django.conf.urls.url() instances instead
+        
+        
         0.9.4 (2015-10-28)
         ------------------
         
         * add test_requirements.txt to MANIFEST.in
         
         
         0.9.2 (2015-10-27)
```

### Comparing `django-nvd3-0.9.6/django_nvd3/__init__.pyc` & `django-nvd3-0.9.7/django_nvd3/__init__.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 0a61 6956 6300 0000 0000 0000  .....aiVc.......
+00000000: 03f3 0d0a 1f81 6956 6300 0000 0000 0000  ......iVc.......
 00000010: 0001 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000020: 005a 0000 6401 005a 0100 6402 005a 0200  .Z..d..Z..d..Z..
 00000030: 6403 005a 0300 6404 005a 0400 6405 005a  d..Z..d..Z..d..Z
 00000040: 0500 6406 0053 2807 0000 0073 eb00 0000  ..d..S(....s....
 00000050: 0a44 6a61 6e67 6f2d 6e76 6433 2069 7320  .Django-nvd3 is 
 00000060: 6120 7772 6170 7065 7220 666f 7220 4e56  a wrapper for NV
 00000070: 4433 2067 7261 7068 206c 6962 7261 7279  D3 graph library
@@ -14,15 +14,15 @@
 000000d0: 686f 7574 2074 616b 696e 6720 6177 6179  hout taking away
 000000e0: 2074 6865 2070 6f77 6572 2074 6861 7420   the power that 
 000000f0: 6433 2e6a 7320 6769 7665 7320 796f 752e  d3.js gives you.
 00000100: 0a0a 5072 6f6a 6563 7420 6c6f 6361 7469  ..Project locati
 00000110: 6f6e 203a 2068 7474 7073 3a2f 2f67 6974  on : https://git
 00000120: 6875 622e 636f 6d2f 6172 6573 6b69 2f64  hub.com/areski/d
 00000130: 6a61 6e67 6f2d 6e76 6433 0a73 0500 0000  jango-nvd3.s....
-00000140: 302e 392e 3673 0d00 0000 4172 6573 6b69  0.9.6s....Areski
+00000140: 302e 392e 3773 0d00 0000 4172 6573 6b69  0.9.7s....Areski
 00000150: 2042 656c 6169 6473 1000 0000 6172 6573   Belaids....ares
 00000160: 6b69 4067 6d61 696c 2e63 6f6d 7318 0000  ki@gmail.coms...
 00000170: 0068 7474 703a 2f2f 6172 6573 6b69 6265  .http://areskibe
 00000180: 6c61 6964 2e63 6f6d 2f74 1000 0000 7265  laid.com/t....re
 00000190: 7374 7275 6374 7572 6564 7465 7874 4e28  structuredtextN(
 000001a0: 0600 0000 7407 0000 005f 5f64 6f63 5f5f  ....t....__doc__
 000001b0: 740b 0000 005f 5f76 6572 7369 6f6e 5f5f  t....__version__
```

### Comparing `django-nvd3-0.9.6/django_nvd3/templatetags/nvd3_tags.py` & `django-nvd3-0.9.7/django_nvd3/templatetags/nvd3_tags.py`

 * *Files identical despite different names*

### Comparing `django-nvd3-0.9.6/django_nvd3/templatetags/nvd3_tags.pyc` & `django-nvd3-0.9.7/django_nvd3/templatetags/nvd3_tags.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,327 +1,403 @@
-00000000: 03f3 0d0a 9b9c 2255 6300 0000 0000 0000  ......"Uc.......
-00000010: 0004 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
-00000020: 0064 0100 6c00 006d 0100 5a01 0001 6400  .d..l..m..Z...d.
-00000030: 0064 0200 6c02 006d 0300 5a03 0001 6400  .d..l..m..Z...d.
-00000040: 0064 0300 6c04 006d 0500 5a05 0001 6400  .d..l..m..Z...d.
-00000050: 0064 0400 6c06 006d 0700 5a07 0001 6400  .d..l..m..Z...d.
-00000060: 0064 0500 6c08 006d 0900 5a09 006d 0a00  .d..l..m..Z..m..
-00000070: 5a0a 006d 0b00 5a0b 006d 0c00 5a0c 006d  Z..m..Z..m..Z..m
-00000080: 0d00 5a0d 006d 0e00 5a0e 006d 0f00 5a0f  ..Z..m..Z..m..Z.
-00000090: 006d 1000 5a10 006d 1100 5a11 006d 1200  .m..Z..m..Z..m..
-000000a0: 5a12 0001 6501 006a 1300 6900 0064 0600  Z...e..j..i..d..
-000000b0: 8401 0083 0100 5a14 0065 0100 6a13 0064  ......Z..e..j..d
-000000c0: 0700 6408 0064 0900 8402 0083 0100 5a15  ..d..d........Z.
-000000d0: 0065 0100 6a13 0064 0a00 640b 0084 0100  .e..j..d..d.....
-000000e0: 8301 005a 1600 640c 0053 280d 0000 0069  ...Z..d..S(....i
-000000f0: ffff ffff 2801 0000 0074 0800 0000 7265  ....(....t....re
-00000100: 6769 7374 6572 2801 0000 0074 0900 0000  gister(....t....
-00000110: 6d61 726b 5f73 6166 6528 0100 0000 7408  mark_safe(....t.
-00000120: 0000 0073 6574 7469 6e67 7328 0100 0000  ...settings(....
-00000130: 7409 0000 004e 5644 3343 6861 7274 280a  t....NVD3Chart(.
-00000140: 0000 0074 1200 0000 6c69 6e65 5769 7468  ...t....lineWith
-00000150: 466f 6375 7343 6861 7274 7409 0000 006c  FocusChartt....l
-00000160: 696e 6543 6861 7274 740d 0000 006d 756c  ineChartt....mul
-00000170: 7469 4261 7243 6861 7274 7408 0000 0070  tiBarChartt....p
-00000180: 6965 4368 6172 7474 1000 0000 7374 6163  ieChartt....stac
-00000190: 6b65 6441 7265 6143 6861 7274 7417 0000  kedAreaChartt...
-000001a0: 006d 756c 7469 4261 7248 6f72 697a 6f6e  .multiBarHorizon
-000001b0: 7461 6c43 6861 7274 7410 0000 006c 696e  talChartt....lin
-000001c0: 6550 6c75 7342 6172 4368 6172 7474 1300  ePlusBarChartt..
-000001d0: 0000 6375 6d75 6c61 7469 7665 4c69 6e65  ..cumulativeLine
-000001e0: 4368 6172 7474 1000 0000 6469 7363 7265  Chartt....discre
-000001f0: 7465 4261 7243 6861 7274 740c 0000 0073  teBarChartt....s
-00000200: 6361 7474 6572 4368 6172 7463 0400 0000  catterChartc....
-00000210: 1000 0000 0b00 0000 4f00 0000 73fd 0100  ........O...s...
-00000220: 007c 0000 730a 0074 0000 5364 0100 7c03  .|..s..t..Sd..|.
-00000230: 006b 0700 7223 0074 0000 7c03 0064 0100  .k..r#.t..|..d..
-00000240: 3c6e 0000 6402 007c 0300 6b07 0072 3c00  <n..d..|..k..r<.
-00000250: 6403 007c 0300 6402 003c 6e00 0064 0400  d..|..d..<n..d..
-00000260: 7c03 006b 0700 7255 0064 0500 7c03 0064  |..k..rU.d..|..d
-00000270: 0400 3c6e 0000 6406 007c 0300 6b07 0072  ..<n..d..|..k..r
-00000280: 6e00 7401 007c 0300 6406 003c 6e00 0064  n.t..|..d..<n..d
-00000290: 0700 7c03 006b 0700 7287 0069 0000 7c03  ..|..k..r..i..|.
-000002a0: 0064 0700 3c6e 0000 7402 007c 0200 8301  .d..<n..t..|....
-000002b0: 007c 0300 6408 003c 7403 007c 0000 8301  .|..d..<t..|....
-000002c0: 007c 0300 8d00 007d 0600 7c01 0064 0900  .|.....}..|..d..
-000002d0: 197d 0700 6700 007c 0100 6a04 0083 0000  .}..g..|..j.....
-000002e0: 445d 1b00 7d08 007c 0800 6a05 0064 0a00  D]..}..|..j..d..
-000002f0: 8301 0072 c000 7c08 005e 0200 71c0 007d  ...r..|..^..q..}
-00000300: 0900 7406 007c 0900 8301 0064 0b00 6b04  ..t..|.....d..k.
-00000310: 0072 0b01 7407 007c 0900 640c 0064 0d00  .r..t..|..d..d..
-00000320: 8400 0083 0101 7d09 006e 0000 78c5 007c  ......}..n..x..|
-00000330: 0900 445d bd00 7d0a 007c 0100 7c0a 0019  ..D]..}..|..|...
-00000340: 7d0b 007c 0a00 6a08 0064 0a00 8301 0064  }..|..j..d.....d
-00000350: 0b00 197d 0c00 7c01 006a 0900 6408 007c  ...}..|..j..d..|
-00000360: 0c00 1783 0100 7256 017c 0100 6408 007c  ......rV.|..d..|
-00000370: 0c00 1719 6e03 0064 1100 7d0d 007c 0100  ....n..d..}..|..
-00000380: 6a09 0064 0e00 7c0c 0017 8301 0072 7d01  j..d..|......r}.
-00000390: 7c01 0064 0e00 7c0c 0017 196e 0300 6900  |..d..|....n..i.
-000003a0: 007d 0e00 7c01 006a 0900 640f 007c 0c00  .}..|..j..d..|..
-000003b0: 1783 0100 72a4 017c 0100 640f 007c 0c00  ....r..|..d..|..
-000003c0: 1719 6e03 0069 0000 7d05 007c 0600 6a0b  ..n..i..}..|..j.
-000003d0: 0064 0800 7c0d 0064 0a00 7c0b 0064 0900  .d..|..d..|..d..
-000003e0: 7c07 0064 0e00 7c0e 007c 0500 8d00 0401  |..d..|..|......
-000003f0: 7112 0157 7400 007c 0600 5f0c 007c 0600  q..Wt..|.._..|..
-00000400: 6a0d 0083 0000 017c 0600 6a0e 0064 1000  j......|..j..d..
-00000410: 177d 0f00 740f 007c 0f00 8301 0053 2812  .}..t..|.....S(.
-00000420: 0000 0073 c103 0000 4c6f 6164 7320 7468  ...s....Loads th
-00000430: 6520 4368 6172 7420 6f62 6a65 6374 7320  e Chart objects 
-00000440: 696e 2074 6865 2063 6f6e 7461 696e 6572  in the container
-00000450: 2e0a 0a20 2020 202a 2a75 7361 6765 2a2a  ...    **usage**
-00000460: 3a0a 0a20 2020 2020 2020 207b 2520 6c6f  :..        {% lo
-00000470: 6164 5f63 6861 7274 2022 6c69 6e65 5769  ad_chart "lineWi
-00000480: 7468 466f 6375 7343 6861 7274 2220 6461  thFocusChart" da
-00000490: 7461 5f73 6574 2022 6469 765f 6c69 6e65  ta_set "div_line
-000004a0: 5769 7468 466f 6375 7343 6861 7274 2220  WithFocusChart" 
-000004b0: 257d 0a0a 2020 2020 2a2a 4172 6775 6d65  %}..    **Argume
-000004c0: 6e74 732a 2a3a 0a0a 2020 2020 2020 2020  nts**:..        
-000004d0: 2a20 6060 6368 6172 745f 7479 7065 6060  * ``chart_type``
-000004e0: 202d 2047 6976 6520 6368 6172 7420 7479   - Give chart ty
-000004f0: 7065 206e 616d 6520 6567 2e20 6c69 6e65  pe name eg. line
-00000500: 5769 7468 466f 6375 7343 6861 7274 2f70  WithFocusChart/p
-00000510: 6965 4368 6172 740a 2020 2020 2020 2020  ieChart.        
-00000520: 2a20 6060 7365 7269 6573 6060 202d 2044  * ``series`` - D
-00000530: 6174 6120 7365 7420 7768 6963 6820 6172  ata set which ar
-00000540: 6520 676f 696e 6720 746f 2062 6520 706c  e going to be pl
-00000550: 6f74 7465 6420 696e 2063 6861 7274 2e0a  otted in chart..
-00000560: 2020 2020 2020 2020 2a20 6060 636f 6e74          * ``cont
-00000570: 6169 6e65 7260 6020 2d20 4368 6172 7420  ainer`` - Chart 
-00000580: 686f 6c64 6572 2069 6e20 6874 6d6c 2070  holder in html p
-00000590: 6167 652e 0a0a 2020 2020 2a2a 6b77 5f65  age...    **kw_e
-000005a0: 7874 7261 2073 6574 7469 6e67 732a 2a3a  xtra settings**:
-000005b0: 3a0a 2020 2020 2020 2020 2a20 6060 785f  :.        * ``x_
-000005c0: 6973 5f64 6174 6560 6020 2d20 6966 2065  is_date`` - if e
-000005d0: 6e61 626c 6564 2074 6865 2078 2d61 7869  nabled the x-axi
-000005e0: 7320 7769 6c6c 2062 6520 6469 7370 6c61  s will be displa
-000005f0: 7920 6173 2064 6174 6520 666f 726d 6174  y as date format
-00000600: 0a20 2020 2020 2020 202a 2060 6078 5f61  .        * ``x_a
-00000610: 7869 735f 666f 726d 6174 6060 202d 2073  xis_format`` - s
-00000620: 6574 2074 6865 2078 2d61 7869 7320 6461  et the x-axis da
-00000630: 7465 2066 6f72 6d61 742c 2069 652e 2022  te format, ie. "
-00000640: 2564 2025 6220 2559 220a 2020 2020 2020  %d %b %Y".      
-00000650: 2020 2a20 6060 7461 675f 7363 7269 7074    * ``tag_script
-00000660: 5f6a 7360 6020 2d20 6966 2065 6e61 626c  _js`` - if enabl
-00000670: 6564 2069 7420 7769 6c6c 2061 6464 2074  ed it will add t
-00000680: 6865 206a 6176 6173 6372 6970 7420 7461  he javascript ta
-00000690: 6720 273c 7363 7269 7074 3e27 0a20 2020  g '<script>'.   
-000006a0: 2020 2020 202a 2060 606a 7175 6572 795f       * ``jquery_
-000006b0: 6f6e 5f72 6561 6479 6060 202d 2069 6620  on_ready`` - if 
-000006c0: 656e 6162 6c65 6420 6974 2077 696c 6c20  enabled it will 
-000006d0: 6c6f 6164 2074 6865 206a 6176 6173 6372  load the javascr
-000006e0: 6970 7420 6f6e 6c79 2077 6865 6e20 7061  ipt only when pa
-000006f0: 6765 2069 7320 6c6f 6164 6564 0a20 2020  ge is loaded.   
-00000700: 2020 2020 2020 2020 2074 6869 7320 7769           this wi
-00000710: 6c6c 2075 7365 206a 7175 6572 7920 6c69  ll use jquery li
-00000720: 6272 6172 792c 2073 6f20 6d61 6b65 2073  brary, so make s
-00000730: 7572 6520 746f 2061 6464 206a 7175 6572  ure to add jquer
-00000740: 7920 746f 2074 6865 2074 656d 706c 6174  y to the templat
-00000750: 652e 0a20 2020 2020 2020 202a 2060 6063  e..        * ``c
-00000760: 6f6c 6f72 5f63 6174 6567 6f72 7960 6020  olor_category`` 
-00000770: 2d20 4465 6669 6e65 2063 6f6c 6f72 2063  - Define color c
-00000780: 6174 6567 6f72 7920 2865 672e 2063 6174  ategory (eg. cat
-00000790: 6567 6f72 7931 302c 2063 6174 6567 6f72  egory10, categor
-000007a0: 7932 302c 2063 6174 6567 6f72 7932 3063  y20, category20c
-000007b0: 290a 2020 2020 2020 2020 2a20 6060 6368  ).        * ``ch
-000007c0: 6172 745f 6174 7472 6060 202d 2043 7573  art_attr`` - Cus
-000007d0: 746f 6d20 6368 6172 7420 6174 7472 6962  tom chart attrib
-000007e0: 7574 6573 0a20 2020 2074 0900 0000 785f  utes.    t....x_
-000007f0: 6973 5f64 6174 6574 0d00 0000 785f 6178  is_datet....x_ax
-00000800: 6973 5f66 6f72 6d61 7473 0800 0000 2564  is_formats....%d
-00000810: 2025 6220 2559 740e 0000 0063 6f6c 6f72   %b %Yt....color
-00000820: 5f63 6174 6567 6f72 7974 0a00 0000 6361  _categoryt....ca
-00000830: 7465 676f 7279 3230 740d 0000 0074 6167  tegory20t....tag
-00000840: 5f73 6372 6970 745f 6a73 740a 0000 0063  _script_jst....c
-00000850: 6861 7274 5f61 7474 7274 0400 0000 6e61  hart_attrt....na
-00000860: 6d65 7401 0000 0078 7401 0000 0079 6901  met....xt....yi.
-00000870: 0000 0074 0300 0000 6b65 7963 0100 0000  ...t....keyc....
-00000880: 0100 0000 0300 0000 5300 0000 730e 0000  ........S...s...
-00000890: 0074 0000 7c00 0064 0100 1f83 0100 5328  .t..|..d......S(
-000008a0: 0200 0000 4e69 0100 0000 2801 0000 0074  ....Ni....(....t
-000008b0: 0300 0000 696e 7428 0100 0000 5215 0000  ....int(....R...
-000008c0: 0028 0000 0000 2800 0000 0073 4c00 0000  .(....(....sL...
-000008d0: 2f68 6f6d 652f 6172 6573 6b69 2f70 726f  /home/areski/pro
-000008e0: 6a65 6374 732f 6e76 6433 2f64 6a61 6e67  jects/nvd3/djang
-000008f0: 6f2d 6e76 6433 2f64 6a61 6e67 6f5f 6e76  o-nvd3/django_nv
-00000900: 6433 2f74 656d 706c 6174 6574 6167 732f  d3/templatetags/
-00000910: 6e76 6433 5f74 6167 732e 7079 7408 0000  nvd3_tags.pyt...
-00000920: 003c 6c61 6d62 6461 3e39 0000 0073 0000  .<lambda>9...s..
-00000930: 0000 7405 0000 0065 7874 7261 7406 0000  ..t....extrat...
-00000940: 006b 7761 7267 7373 0100 0000 0a4e 2810  .kwargss.....N(.
-00000950: 0000 0074 0500 0000 4661 6c73 6574 0400  ...t....Falset..
-00000960: 0000 5472 7565 7403 0000 0073 7472 7404  ..Truet....strt.
-00000970: 0000 0065 7661 6c74 0400 0000 6b65 7973  ...evalt....keys
-00000980: 740a 0000 0073 7461 7274 7377 6974 6874  t....startswitht
-00000990: 0300 0000 6c65 6e74 0600 0000 736f 7274  ....lent....sort
-000009a0: 6564 7405 0000 0073 706c 6974 7403 0000  edt....splitt...
-000009b0: 0067 6574 7404 0000 004e 6f6e 6574 0900  .gett....Nonet..
-000009c0: 0000 6164 645f 7365 7269 6574 1100 0000  ..add_seriet....
-000009d0: 6469 7370 6c61 795f 636f 6e74 6169 6e65  display_containe
-000009e0: 7274 0c00 0000 6275 696c 6463 6f6e 7465  rt....buildconte
-000009f0: 6e74 740b 0000 0068 746d 6c63 6f6e 7465  ntt....htmlconte
-00000a00: 6e74 5201 0000 0028 1000 0000 740a 0000  ntR....(....t...
-00000a10: 0063 6861 7274 5f74 7970 6574 0600 0000  .chart_typet....
-00000a20: 7365 7269 6573 7409 0000 0063 6f6e 7461  seriest....conta
-00000a30: 696e 6572 7408 0000 006b 775f 6578 7472  inert....kw_extr
-00000a40: 6174 0400 0000 6172 6773 521b 0000 0074  at....argsR....t
-00000a50: 0500 0000 6368 6172 7474 0500 0000 7864  ....chartt....xd
-00000a60: 6174 6174 0100 0000 6b74 0b00 0000 795f  atat....kt....y_
-00000a70: 6178 6973 5f6c 6973 7452 1700 0000 7405  axis_listR....t.
-00000a80: 0000 0079 6461 7461 7407 0000 0061 7869  ...ydatat....axi
-00000a90: 735f 6e6f 5214 0000 0052 1a00 0000 740b  s_noR....R....t.
-00000aa0: 0000 0068 746d 6c5f 7374 7269 6e67 2800  ...html_string(.
-00000ab0: 0000 0028 0000 0000 734c 0000 002f 686f  ...(....sL.../ho
-00000ac0: 6d65 2f61 7265 736b 692f 7072 6f6a 6563  me/areski/projec
-00000ad0: 7473 2f6e 7664 332f 646a 616e 676f 2d6e  ts/nvd3/django-n
-00000ae0: 7664 332f 646a 616e 676f 5f6e 7664 332f  vd3/django_nvd3/
-00000af0: 7465 6d70 6c61 7465 7461 6773 2f6e 7664  templatetags/nvd
-00000b00: 335f 7461 6773 2e70 7974 0a00 0000 6c6f  3_tags.pyt....lo
-00000b10: 6164 5f63 6861 7274 0b00 0000 733a 0000  ad_chart....s:..
-00000b20: 0000 1706 0104 020c 010d 010c 010d 010c  ................
-00000b30: 010d 010c 010d 010c 010d 0210 0312 020a  ................
-00000b40: 012e 0112 0218 020d 010a 0113 0227 0127  .............'.'
-00000b50: 0127 0229 0209 010a 020d 0169 9001 0000  .'.).......i....
-00000b60: 6958 0200 0063 0300 0000 0400 0000 0300  iX...c..........
-00000b70: 0000 4300 0000 734d 0000 0074 0000 8300  ..C...sM...t....
-00000b80: 007d 0300 7401 007c 0000 8301 007c 0300  .}..t..|.....|..
-00000b90: 5f02 007c 0300 6a03 007c 0100 8301 0001  _..|..j..|......
-00000ba0: 7c03 006a 0400 7c02 0083 0100 017c 0300  |..j..|......|..
-00000bb0: 6a05 0083 0000 0174 0600 7c03 006a 0700  j......t..|..j..
-00000bc0: 6401 0017 8301 0053 2802 0000 0073 9e01  d......S(....s..
-00000bd0: 0000 0a20 2020 2049 6e63 6c75 6465 2074  ...    Include t
-00000be0: 6865 2068 746d 6c20 666f 7220 7468 6520  he html for the 
-00000bf0: 6368 6172 7420 636f 6e74 6169 6e65 7220  chart container 
-00000c00: 616e 6420 6373 7320 666f 7220 6e76 6433  and css for nvd3
-00000c10: 0a20 2020 2054 6869 7320 7769 6c6c 2069  .    This will i
-00000c20: 6e63 6c75 6465 2073 6f6d 6574 6869 6e67  nclude something
-00000c30: 2073 696d 696c 6172 2061 7320 3a0a 2020   similar as :.  
-00000c40: 2020 2020 2020 3c64 6976 2069 643d 2263        <div id="c
-00000c50: 6f6e 7461 696e 6572 6e61 6d65 223e 3c73  ontainername"><s
-00000c60: 7667 2073 7479 6c65 3d22 6865 6967 6874  vg style="height
-00000c70: 3a34 3030 7078 3b77 6964 7468 3a36 3030  :400px;width:600
-00000c80: 7078 3b22 3e3c 2f73 7667 3e3c 2f64 6976  px;"></svg></div
-00000c90: 3e0a 0a20 2020 202a 2a75 7361 6765 2a2a  >..    **usage**
-00000ca0: 3a0a 0a20 2020 2020 2020 207b 2520 696e  :..        {% in
-00000cb0: 636c 7564 655f 636f 6e74 6169 6e65 7220  clude_container 
-00000cc0: 226c 696e 6557 6974 6846 6f63 7573 4368  "lineWithFocusCh
-00000cd0: 6172 7422 2034 3030 2034 3030 2025 7d0a  art" 400 400 %}.
-00000ce0: 0a20 2020 202a 2a41 7267 756d 656e 7473  .    **Arguments
-00000cf0: 2a2a 3a0a 0a20 2020 2020 2020 202a 2060  **:..        * `
-00000d00: 6069 6e63 6c75 6465 5f63 6f6e 7461 696e  `include_contain
-00000d10: 6572 6060 202d 2063 6f6e 7461 696e 6572  er`` - container
-00000d20: 5f6e 616d 650a 2020 2020 2020 2020 2a20  _name.        * 
-00000d30: 6060 6865 6967 6874 6060 202d 2043 6861  ``height`` - Cha
-00000d40: 7274 2068 6569 6768 740a 2020 2020 2020  rt height.      
-00000d50: 2020 2a20 6060 7769 6474 6860 6020 2d20    * ``width`` - 
-00000d60: 4368 6172 7420 7769 6474 680a 2020 2020  Chart width.    
-00000d70: 7301 0000 000a 2808 0000 0052 0300 0000  s.....(....R....
-00000d80: 521e 0000 0052 1400 0000 7410 0000 0073  R....R....t....s
-00000d90: 6574 5f67 7261 7068 5f68 6569 6768 7474  et_graph_heightt
-00000da0: 0f00 0000 7365 745f 6772 6170 685f 7769  ....set_graph_wi
-00000db0: 6474 6874 0e00 0000 6275 696c 6463 6f6e  dtht....buildcon
-00000dc0: 7461 696e 6572 5201 0000 0052 2d00 0000  tainerR....R-...
-00000dd0: 2804 0000 0074 1100 0000 696e 636c 7564  (....t....includ
-00000de0: 655f 636f 6e74 6169 6e65 7274 0600 0000  e_containert....
-00000df0: 6865 6967 6874 7405 0000 0077 6964 7468  heightt....width
-00000e00: 5230 0000 0028 0000 0000 2800 0000 0073  R0...(....(....s
-00000e10: 4c00 0000 2f68 6f6d 652f 6172 6573 6b69  L.../home/areski
-00000e20: 2f70 726f 6a65 6374 732f 6e76 6433 2f64  /projects/nvd3/d
-00000e30: 6a61 6e67 6f2d 6e76 6433 2f64 6a61 6e67  jango-nvd3/djang
-00000e40: 6f5f 6e76 6433 2f74 656d 706c 6174 6574  o_nvd3/templatet
-00000e50: 6167 732f 6e76 6433 5f74 6167 732e 7079  ags/nvd3_tags.py
-00000e60: 523b 0000 004c 0000 0073 0c00 0000 0011  R;...L...s......
-00000e70: 0901 0f01 0d01 0d01 0a02 7400 0000 0063  ..........t....c
-00000e80: 0100 0000 0300 0000 0500 0000 4300 0000  ............C...
-00000e90: 73a7 0000 007c 0000 7213 007c 0000 6401  s....|..r..|..d.
-00000ea0: 0037 7d00 006e 0000 7400 0083 0000 7d01  .7}..n..t.....}.
-00000eb0: 0067 0000 6402 0074 0100 6a02 007c 0000  .g..d..t..j..|..
-00000ec0: 6602 0016 6601 0044 5d10 007d 0200 6403  f...f..D]..}..d.
-00000ed0: 007c 0200 165e 0200 7133 007c 0100 5f03  .|...^..q3.|.._.
-00000ee0: 0067 0000 6404 0074 0100 6a02 007c 0000  .g..d..t..j..|..
-00000ef0: 6602 0016 6405 0074 0100 6a02 007c 0000  f...d..t..j..|..
-00000f00: 6602 0016 6602 0044 5d10 007d 0200 6406  f...f..D]..}..d.
-00000f10: 007c 0200 165e 0200 7173 007c 0100 5f04  .|...^..qs.|.._.
-00000f20: 007c 0100 6a05 0083 0000 0174 0600 7c01  .|..j......t..|.
-00000f30: 006a 0700 6407 0017 8301 0053 2808 0000  .j..d......S(...
-00000f40: 0073 db01 0000 0a20 2020 2049 6e63 6c75  .s.....    Inclu
-00000f50: 6465 2074 6865 2068 746d 6c20 666f 7220  de the html for 
-00000f60: 7468 6520 6368 6172 7420 636f 6e74 6169  the chart contai
-00000f70: 6e65 7220 616e 6420 6373 7320 666f 7220  ner and css for 
-00000f80: 6e76 6433 0a20 2020 2054 6869 7320 7769  nvd3.    This wi
-00000f90: 6c6c 2069 6e63 6c75 6465 2073 6f6d 6574  ll include somet
-00000fa0: 6869 6e67 2073 696d 696c 6172 2061 7320  hing similar as 
-00000fb0: 3a0a 0a20 2020 2020 2020 203c 6c69 6e6b  :..        <link
-00000fc0: 206d 6564 6961 3d22 616c 6c22 2068 7265   media="all" hre
-00000fd0: 663d 222f 7374 6174 6963 2f6e 7664 332f  f="/static/nvd3/
-00000fe0: 7372 632f 6e76 2e64 332e 6373 7322 2074  src/nv.d3.css" t
-00000ff0: 7970 653d 2274 6578 742f 6373 7322 2072  ype="text/css" r
-00001000: 656c 3d22 7374 796c 6573 6865 6574 2220  el="stylesheet" 
-00001010: 2f3e 0a20 2020 2020 2020 203c 7363 7269  />.        <scri
-00001020: 7074 2073 7263 3d22 2f73 7461 7469 632f  pt src="/static/
-00001030: 6433 2f64 332e 6d69 6e2e 6a73 2220 7479  d3/d3.min.js" ty
-00001040: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
-00001050: 6970 7422 3e3c 2f73 6372 6970 743e 0a20  ipt"></script>. 
-00001060: 2020 2020 2020 203c 7363 7269 7074 2073         <script s
-00001070: 7263 3d22 2f73 7461 7469 632f 6e76 6433  rc="/static/nvd3
-00001080: 2f6e 762e 6433 2e6d 696e 2e6a 7322 2074  /nv.d3.min.js" t
-00001090: 7970 653d 2274 6578 742f 6a61 7661 7363  ype="text/javasc
-000010a0: 7269 7074 223e 3c2f 7363 7269 7074 3e0a  ript"></script>.
-000010b0: 0a20 2020 202a 2a75 7361 6765 2a2a 3a0a  .    **usage**:.
-000010c0: 0a20 2020 2020 2020 207b 2520 696e 636c  .        {% incl
-000010d0: 7564 655f 6368 6172 745f 6a73 6373 7320  ude_chart_jscss 
-000010e0: 276e 6577 6669 6573 2720 257d 0a0a 2020  'newfies' %}..  
-000010f0: 2020 2a2a 4172 6775 6d65 6e74 732a 2a3a    **Arguments**:
-00001100: 0a0a 2020 2020 2020 2020 2a20 6060 7374  ..        * ``st
-00001110: 6174 6963 5f64 6972 6060 202d 0a20 2020  atic_dir`` -.   
-00001120: 2074 0100 0000 2f73 1c00 0000 2573 2573   t..../s....%s%s
-00001130: 6e76 6433 2f62 7569 6c64 2f6e 762e 6433  nvd3/build/nv.d3
-00001140: 2e6d 696e 2e63 7373 7340 0000 003c 6c69  .min.csss@...<li
-00001150: 6e6b 206d 6564 6961 3d22 616c 6c22 2068  nk media="all" h
-00001160: 7265 663d 2225 7322 2074 7970 653d 2274  ref="%s" type="t
-00001170: 6578 742f 6373 7322 2072 656c 3d22 7374  ext/css" rel="st
-00001180: 796c 6573 6865 6574 2220 2f3e 0a73 1000  ylesheet" />.s..
-00001190: 0000 2573 2573 6433 2f64 332e 6d69 6e2e  ..%s%sd3/d3.min.
-000011a0: 6a73 731b 0000 0025 7325 736e 7664 332f  jss....%s%snvd3/
-000011b0: 6275 696c 642f 6e76 2e64 332e 6d69 6e2e  build/nv.d3.min.
-000011c0: 6a73 7332 0000 003c 7363 7269 7074 2073  jss2...<script s
-000011d0: 7263 3d22 2573 2220 7479 7065 3d22 7465  rc="%s" type="te
-000011e0: 7874 2f6a 6176 6173 6372 6970 7422 3e3c  xt/javascript"><
-000011f0: 2f73 6372 6970 743e 0a73 0100 0000 0a28  /script>.s.....(
-00001200: 0800 0000 5203 0000 0052 0200 0000 740a  ....R....R....t.
-00001210: 0000 0053 5441 5449 435f 5552 4c74 0a00  ...STATIC_URLt..
-00001220: 0000 6865 6164 6572 5f63 7373 7409 0000  ..header_csst...
-00001230: 0068 6561 6465 725f 6a73 740f 0000 0062  .header_jst....b
-00001240: 7569 6c64 6874 6d6c 6865 6164 6572 5201  uildhtmlheaderR.
-00001250: 0000 0074 0a00 0000 6874 6d6c 6865 6164  ...t....htmlhead
-00001260: 6572 2803 0000 0074 0a00 0000 7374 6174  er(....t....stat
-00001270: 6963 5f64 6972 5230 0000 0074 0100 0000  ic_dirR0...t....
-00001280: 6828 0000 0000 2800 0000 0073 4c00 0000  h(....(....sL...
-00001290: 2f68 6f6d 652f 6172 6573 6b69 2f70 726f  /home/areski/pro
-000012a0: 6a65 6374 732f 6e76 6433 2f64 6a61 6e67  jects/nvd3/djang
-000012b0: 6f2d 6e76 6433 2f64 6a61 6e67 6f5f 6e76  o-nvd3/django_nv
-000012c0: 6433 2f74 656d 706c 6174 6574 6167 732f  d3/templatetags/
-000012d0: 6e76 6433 5f74 6167 732e 7079 7413 0000  nvd3_tags.pyt...
-000012e0: 0069 6e63 6c75 6465 5f63 6861 7274 5f6a  .include_chart_j
-000012f0: 7363 7373 6600 0000 7314 0000 0000 1206  scssf...s.......
-00001300: 010d 0209 0203 022d 0503 0210 012d 030a  .......-.....-..
-00001310: 014e 2817 0000 0074 1e00 0000 646a 616e  .N(....t....djan
-00001320: 676f 2e74 656d 706c 6174 652e 6465 6661  go.template.defa
-00001330: 756c 7466 696c 7465 7273 5200 0000 0074  ultfiltersR....t
-00001340: 1700 0000 646a 616e 676f 2e75 7469 6c73  ....django.utils
-00001350: 2e73 6166 6573 7472 696e 6752 0100 0000  .safestringR....
-00001360: 740b 0000 0064 6a61 6e67 6f2e 636f 6e66  t....django.conf
-00001370: 5202 0000 0074 0e00 0000 6e76 6433 2e4e  R....t....nvd3.N
-00001380: 5644 3343 6861 7274 5203 0000 0074 0400  VD3ChartR....t..
-00001390: 0000 6e76 6433 5204 0000 0052 0500 0000  ..nvd3R....R....
-000013a0: 5206 0000 0052 0700 0000 5208 0000 0052  R....R....R....R
-000013b0: 0900 0000 520a 0000 0052 0b00 0000 520c  ....R....R....R.
-000013c0: 0000 0052 0d00 0000 740a 0000 0073 696d  ...R....t....sim
-000013d0: 706c 655f 7461 6752 3700 0000 523b 0000  ple_tagR7...R;..
-000013e0: 0052 4700 0000 2800 0000 0028 0000 0000  .RG...(....(....
-000013f0: 2800 0000 0073 4c00 0000 2f68 6f6d 652f  (....sL.../home/
-00001400: 6172 6573 6b69 2f70 726f 6a65 6374 732f  areski/projects/
-00001410: 6e76 6433 2f64 6a61 6e67 6f2d 6e76 6433  nvd3/django-nvd3
-00001420: 2f64 6a61 6e67 6f5f 6e76 6433 2f74 656d  /django_nvd3/tem
-00001430: 706c 6174 6574 6167 732f 6e76 6433 5f74  platetags/nvd3_t
-00001440: 6167 732e 7079 7408 0000 003c 6d6f 6475  ags.pyt....<modu
-00001450: 6c65 3e01 0000 0073 1400 0000 1001 1001  le>....s........
-00001460: 1001 1001 4606 0601 0f40 0601 1219 0601  ....F....@......
+00000000: 03f3 0d0a afff 2f56 6300 0000 0000 0000  ....../Vc.......
+00000010: 0005 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
+00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
+00000030: 6c01 006d 0200 5a02 0001 6400 0064 0300  l..m..Z...d..d..
+00000040: 6c03 006d 0400 5a04 0001 6400 0064 0400  l..m..Z...d..d..
+00000050: 6c05 006d 0600 5a06 0001 6400 0064 0500  l..m..Z...d..d..
+00000060: 6c07 006d 0800 5a08 0001 6400 0064 0600  l..m..Z...d..d..
+00000070: 6c09 006d 0a00 5a0a 006d 0b00 5a0b 006d  l..m..Z..m..Z..m
+00000080: 0c00 5a0c 006d 0d00 5a0d 006d 0e00 5a0e  ..Z..m..Z..m..Z.
+00000090: 006d 0f00 5a0f 006d 1000 5a10 006d 1100  .m..Z..m..Z..m..
+000000a0: 5a11 006d 1200 5a12 006d 1300 5a13 0001  Z..m..Z..m..Z...
+000000b0: 6502 006a 1400 6900 0064 0700 8401 0083  e..j..i..d......
+000000c0: 0100 5a15 0065 0200 6a14 0064 0800 6409  ..Z..e..j..d..d.
+000000d0: 0064 0a00 8402 0083 0100 5a16 0065 0200  .d........Z..e..
+000000e0: 6a14 0064 0b00 640b 0064 0b00 640c 0084  j..d..d..d..d...
+000000f0: 0300 8301 005a 1700 6401 0053 280d 0000  .....Z..d..S(...
+00000100: 0069 ffff ffff 4e28 0100 0000 7408 0000  .i....N(....t...
+00000110: 0072 6567 6973 7465 7228 0100 0000 7409  .register(....t.
+00000120: 0000 006d 6172 6b5f 7361 6665 2801 0000  ...mark_safe(...
+00000130: 0074 0800 0000 7365 7474 696e 6773 2801  .t....settings(.
+00000140: 0000 0074 0900 0000 4e56 4433 4368 6172  ...t....NVD3Char
+00000150: 7428 0a00 0000 7412 0000 006c 696e 6557  t(....t....lineW
+00000160: 6974 6846 6f63 7573 4368 6172 7474 0900  ithFocusChartt..
+00000170: 0000 6c69 6e65 4368 6172 7474 0d00 0000  ..lineChartt....
+00000180: 6d75 6c74 6942 6172 4368 6172 7474 0800  multiBarChartt..
+00000190: 0000 7069 6543 6861 7274 7410 0000 0073  ..pieChartt....s
+000001a0: 7461 636b 6564 4172 6561 4368 6172 7474  tackedAreaChartt
+000001b0: 1700 0000 6d75 6c74 6942 6172 486f 7269  ....multiBarHori
+000001c0: 7a6f 6e74 616c 4368 6172 7474 1000 0000  zontalChartt....
+000001d0: 6c69 6e65 506c 7573 4261 7243 6861 7274  linePlusBarChart
+000001e0: 7413 0000 0063 756d 756c 6174 6976 654c  t....cumulativeL
+000001f0: 696e 6543 6861 7274 7410 0000 0064 6973  ineChartt....dis
+00000200: 6372 6574 6542 6172 4368 6172 7474 0c00  creteBarChartt..
+00000210: 0000 7363 6174 7465 7243 6861 7274 6304  ..scatterChartc.
+00000220: 0000 0010 0000 000b 0000 004f 0000 0073  ...........O...s
+00000230: fd01 0000 7c00 0073 0a00 7400 0053 6401  ....|..s..t..Sd.
+00000240: 007c 0300 6b07 0072 2300 7400 007c 0300  .|..k..r#.t..|..
+00000250: 6401 003c 6e00 0064 0200 7c03 006b 0700  d..<n..d..|..k..
+00000260: 723c 0064 0300 7c03 0064 0200 3c6e 0000  r<.d..|..d..<n..
+00000270: 6404 007c 0300 6b07 0072 5500 6405 007c  d..|..k..rU.d..|
+00000280: 0300 6404 003c 6e00 0064 0600 7c03 006b  ..d..<n..d..|..k
+00000290: 0700 726e 0074 0100 7c03 0064 0600 3c6e  ..rn.t..|..d..<n
+000002a0: 0000 6407 007c 0300 6b07 0072 8700 6900  ..d..|..k..r..i.
+000002b0: 007c 0300 6407 003c 6e00 0074 0200 7c02  .|..d..<n..t..|.
+000002c0: 0083 0100 7c03 0064 0800 3c74 0300 7c00  ....|..d..<t..|.
+000002d0: 0083 0100 7c03 008d 0000 7d06 007c 0100  ....|.....}..|..
+000002e0: 6409 0019 7d07 0067 0000 7c01 006a 0400  d...}..g..|..j..
+000002f0: 8300 0044 5d1b 007d 0800 7c08 006a 0500  ...D]..}..|..j..
+00000300: 640a 0083 0100 72c0 007c 0800 5e02 0071  d.....r..|..^..q
+00000310: c000 7d09 0074 0600 7c09 0083 0100 640b  ..}..t..|.....d.
+00000320: 006b 0400 720b 0174 0700 7c09 0064 0c00  .k..r..t..|..d..
+00000330: 640d 0084 0000 8301 017d 0900 6e00 0078  d........}..n..x
+00000340: c500 7c09 0044 5dbd 007d 0a00 7c01 007c  ..|..D]..}..|..|
+00000350: 0a00 197d 0b00 7c0a 006a 0800 640a 0083  ...}..|..j..d...
+00000360: 0100 640b 0019 7d0c 007c 0100 6a09 0064  ..d...}..|..j..d
+00000370: 0800 7c0c 0017 8301 0072 5601 7c01 0064  ..|......rV.|..d
+00000380: 0800 7c0c 0017 196e 0300 6411 007d 0d00  ..|....n..d..}..
+00000390: 7c01 006a 0900 640e 007c 0c00 1783 0100  |..j..d..|......
+000003a0: 727d 017c 0100 640e 007c 0c00 1719 6e03  r}.|..d..|....n.
+000003b0: 0069 0000 7d0e 007c 0100 6a09 0064 0f00  .i..}..|..j..d..
+000003c0: 7c0c 0017 8301 0072 a401 7c01 0064 0f00  |......r..|..d..
+000003d0: 7c0c 0017 196e 0300 6900 007d 0500 7c06  |....n..i..}..|.
+000003e0: 006a 0b00 6408 007c 0d00 640a 007c 0b00  .j..d..|..d..|..
+000003f0: 6409 007c 0700 640e 007c 0e00 7c05 008d  d..|..d..|..|...
+00000400: 0004 0171 1201 5774 0000 7c06 005f 0c00  ...q..Wt..|.._..
+00000410: 7c06 006a 0d00 8300 0001 7c06 006a 0e00  |..j......|..j..
+00000420: 6410 0017 7d0f 0074 0f00 7c0f 0083 0100  d...}..t..|.....
+00000430: 5328 1200 0000 73c1 0300 004c 6f61 6473  S(....s....Loads
+00000440: 2074 6865 2043 6861 7274 206f 626a 6563   the Chart objec
+00000450: 7473 2069 6e20 7468 6520 636f 6e74 6169  ts in the contai
+00000460: 6e65 722e 0a0a 2020 2020 2a2a 7573 6167  ner...    **usag
+00000470: 652a 2a3a 0a0a 2020 2020 2020 2020 7b25  e**:..        {%
+00000480: 206c 6f61 645f 6368 6172 7420 226c 696e   load_chart "lin
+00000490: 6557 6974 6846 6f63 7573 4368 6172 7422  eWithFocusChart"
+000004a0: 2064 6174 615f 7365 7420 2264 6976 5f6c   data_set "div_l
+000004b0: 696e 6557 6974 6846 6f63 7573 4368 6172  ineWithFocusChar
+000004c0: 7422 2025 7d0a 0a20 2020 202a 2a41 7267  t" %}..    **Arg
+000004d0: 756d 656e 7473 2a2a 3a0a 0a20 2020 2020  uments**:..     
+000004e0: 2020 202a 2060 6063 6861 7274 5f74 7970     * ``chart_typ
+000004f0: 6560 6020 2d20 4769 7665 2063 6861 7274  e`` - Give chart
+00000500: 2074 7970 6520 6e61 6d65 2065 672e 206c   type name eg. l
+00000510: 696e 6557 6974 6846 6f63 7573 4368 6172  ineWithFocusChar
+00000520: 742f 7069 6543 6861 7274 0a20 2020 2020  t/pieChart.     
+00000530: 2020 202a 2060 6073 6572 6965 7360 6020     * ``series`` 
+00000540: 2d20 4461 7461 2073 6574 2077 6869 6368  - Data set which
+00000550: 2061 7265 2067 6f69 6e67 2074 6f20 6265   are going to be
+00000560: 2070 6c6f 7474 6564 2069 6e20 6368 6172   plotted in char
+00000570: 742e 0a20 2020 2020 2020 202a 2060 6063  t..        * ``c
+00000580: 6f6e 7461 696e 6572 6060 202d 2043 6861  ontainer`` - Cha
+00000590: 7274 2068 6f6c 6465 7220 696e 2068 746d  rt holder in htm
+000005a0: 6c20 7061 6765 2e0a 0a20 2020 202a 2a6b  l page...    **k
+000005b0: 775f 6578 7472 6120 7365 7474 696e 6773  w_extra settings
+000005c0: 2a2a 3a3a 0a20 2020 2020 2020 202a 2060  **::.        * `
+000005d0: 6078 5f69 735f 6461 7465 6060 202d 2069  `x_is_date`` - i
+000005e0: 6620 656e 6162 6c65 6420 7468 6520 782d  f enabled the x-
+000005f0: 6178 6973 2077 696c 6c20 6265 2064 6973  axis will be dis
+00000600: 706c 6179 2061 7320 6461 7465 2066 6f72  play as date for
+00000610: 6d61 740a 2020 2020 2020 2020 2a20 6060  mat.        * ``
+00000620: 785f 6178 6973 5f66 6f72 6d61 7460 6020  x_axis_format`` 
+00000630: 2d20 7365 7420 7468 6520 782d 6178 6973  - set the x-axis
+00000640: 2064 6174 6520 666f 726d 6174 2c20 6965   date format, ie
+00000650: 2e20 2225 6420 2562 2025 5922 0a20 2020  . "%d %b %Y".   
+00000660: 2020 2020 202a 2060 6074 6167 5f73 6372       * ``tag_scr
+00000670: 6970 745f 6a73 6060 202d 2069 6620 656e  ipt_js`` - if en
+00000680: 6162 6c65 6420 6974 2077 696c 6c20 6164  abled it will ad
+00000690: 6420 7468 6520 6a61 7661 7363 7269 7074  d the javascript
+000006a0: 2074 6167 2027 3c73 6372 6970 743e 270a   tag '<script>'.
+000006b0: 2020 2020 2020 2020 2a20 6060 6a71 7565          * ``jque
+000006c0: 7279 5f6f 6e5f 7265 6164 7960 6020 2d20  ry_on_ready`` - 
+000006d0: 6966 2065 6e61 626c 6564 2069 7420 7769  if enabled it wi
+000006e0: 6c6c 206c 6f61 6420 7468 6520 6a61 7661  ll load the java
+000006f0: 7363 7269 7074 206f 6e6c 7920 7768 656e  script only when
+00000700: 2070 6167 6520 6973 206c 6f61 6465 640a   page is loaded.
+00000710: 2020 2020 2020 2020 2020 2020 7468 6973              this
+00000720: 2077 696c 6c20 7573 6520 6a71 7565 7279   will use jquery
+00000730: 206c 6962 7261 7279 2c20 736f 206d 616b   library, so mak
+00000740: 6520 7375 7265 2074 6f20 6164 6420 6a71  e sure to add jq
+00000750: 7565 7279 2074 6f20 7468 6520 7465 6d70  uery to the temp
+00000760: 6c61 7465 2e0a 2020 2020 2020 2020 2a20  late..        * 
+00000770: 6060 636f 6c6f 725f 6361 7465 676f 7279  ``color_category
+00000780: 6060 202d 2044 6566 696e 6520 636f 6c6f  `` - Define colo
+00000790: 7220 6361 7465 676f 7279 2028 6567 2e20  r category (eg. 
+000007a0: 6361 7465 676f 7279 3130 2c20 6361 7465  category10, cate
+000007b0: 676f 7279 3230 2c20 6361 7465 676f 7279  gory20, category
+000007c0: 3230 6329 0a20 2020 2020 2020 202a 2060  20c).        * `
+000007d0: 6063 6861 7274 5f61 7474 7260 6020 2d20  `chart_attr`` - 
+000007e0: 4375 7374 6f6d 2063 6861 7274 2061 7474  Custom chart att
+000007f0: 7269 6275 7465 730a 2020 2020 7409 0000  ributes.    t...
+00000800: 0078 5f69 735f 6461 7465 740d 0000 0078  .x_is_datet....x
+00000810: 5f61 7869 735f 666f 726d 6174 7308 0000  _axis_formats...
+00000820: 0025 6420 2562 2025 5974 0e00 0000 636f  .%d %b %Yt....co
+00000830: 6c6f 725f 6361 7465 676f 7279 740a 0000  lor_categoryt...
+00000840: 0063 6174 6567 6f72 7932 3074 0d00 0000  .category20t....
+00000850: 7461 675f 7363 7269 7074 5f6a 7374 0a00  tag_script_jst..
+00000860: 0000 6368 6172 745f 6174 7472 7404 0000  ..chart_attrt...
+00000870: 006e 616d 6574 0100 0000 7874 0100 0000  .namet....xt....
+00000880: 7969 0100 0000 7403 0000 006b 6579 6301  yi....t....keyc.
+00000890: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
+000008a0: 0e00 0000 7400 007c 0000 6401 001f 8301  ....t..|..d.....
+000008b0: 0053 2802 0000 004e 6901 0000 0028 0100  .S(....Ni....(..
+000008c0: 0000 7403 0000 0069 6e74 2801 0000 0052  ..t....int(....R
+000008d0: 1500 0000 2800 0000 0028 0000 0000 734c  ....(....(....sL
+000008e0: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
+000008f0: 7072 6f6a 6563 7473 2f6e 7664 332f 646a  projects/nvd3/dj
+00000900: 616e 676f 2d6e 7664 332f 646a 616e 676f  ango-nvd3/django
+00000910: 5f6e 7664 332f 7465 6d70 6c61 7465 7461  _nvd3/templateta
+00000920: 6773 2f6e 7664 335f 7461 6773 2e70 7974  gs/nvd3_tags.pyt
+00000930: 0800 0000 3c6c 616d 6264 613e 3b00 0000  ....<lambda>;...
+00000940: 7300 0000 0074 0500 0000 6578 7472 6174  s....t....extrat
+00000950: 0600 0000 6b77 6172 6773 7301 0000 000a  ....kwargss.....
+00000960: 4e28 1000 0000 7405 0000 0046 616c 7365  N(....t....False
+00000970: 7404 0000 0054 7275 6574 0300 0000 7374  t....Truet....st
+00000980: 7274 0400 0000 6576 616c 7404 0000 006b  rt....evalt....k
+00000990: 6579 7374 0a00 0000 7374 6172 7473 7769  eyst....startswi
+000009a0: 7468 7403 0000 006c 656e 7406 0000 0073  tht....lent....s
+000009b0: 6f72 7465 6474 0500 0000 7370 6c69 7474  ortedt....splitt
+000009c0: 0300 0000 6765 7474 0400 0000 4e6f 6e65  ....gett....None
+000009d0: 7409 0000 0061 6464 5f73 6572 6965 7411  t....add_seriet.
+000009e0: 0000 0064 6973 706c 6179 5f63 6f6e 7461  ...display_conta
+000009f0: 696e 6572 740c 0000 0062 7569 6c64 636f  inert....buildco
+00000a00: 6e74 656e 7474 0b00 0000 6874 6d6c 636f  ntentt....htmlco
+00000a10: 6e74 656e 7452 0100 0000 2810 0000 0074  ntentR....(....t
+00000a20: 0a00 0000 6368 6172 745f 7479 7065 7406  ....chart_typet.
+00000a30: 0000 0073 6572 6965 7374 0900 0000 636f  ...seriest....co
+00000a40: 6e74 6169 6e65 7274 0800 0000 6b77 5f65  ntainert....kw_e
+00000a50: 7874 7261 7404 0000 0061 7267 7352 1b00  xtrat....argsR..
+00000a60: 0000 7405 0000 0063 6861 7274 7405 0000  ..t....chartt...
+00000a70: 0078 6461 7461 7401 0000 006b 740b 0000  .xdatat....kt...
+00000a80: 0079 5f61 7869 735f 6c69 7374 5217 0000  .y_axis_listR...
+00000a90: 0074 0500 0000 7964 6174 6174 0700 0000  .t....ydatat....
+00000aa0: 6178 6973 5f6e 6f52 1400 0000 521a 0000  axis_noR....R...
+00000ab0: 0074 0b00 0000 6874 6d6c 5f73 7472 696e  .t....html_strin
+00000ac0: 6728 0000 0000 2800 0000 0073 4c00 0000  g(....(....sL...
+00000ad0: 2f68 6f6d 652f 6172 6573 6b69 2f70 726f  /home/areski/pro
+00000ae0: 6a65 6374 732f 6e76 6433 2f64 6a61 6e67  jects/nvd3/djang
+00000af0: 6f2d 6e76 6433 2f64 6a61 6e67 6f5f 6e76  o-nvd3/django_nv
+00000b00: 6433 2f74 656d 706c 6174 6574 6167 732f  d3/templatetags/
+00000b10: 6e76 6433 5f74 6167 732e 7079 740a 0000  nvd3_tags.pyt...
+00000b20: 006c 6f61 645f 6368 6172 740d 0000 0073  .load_chart....s
+00000b30: 3a00 0000 0017 0601 0402 0c01 0d01 0c01  :...............
+00000b40: 0d01 0c01 0d01 0c01 0d01 0c01 0d02 1003  ................
+00000b50: 1202 0a01 2e01 1202 1802 0d01 0a01 1302  ................
+00000b60: 2701 2701 2702 2902 0901 0a02 0d01 6990  '.'.'.).......i.
+00000b70: 0100 0069 5802 0000 6303 0000 0004 0000  ...iX...c.......
+00000b80: 0003 0000 0043 0000 0073 4d00 0000 7400  .....C...sM...t.
+00000b90: 0083 0000 7d03 0074 0100 7c00 0083 0100  ....}..t..|.....
+00000ba0: 7c03 005f 0200 7c03 006a 0300 7c01 0083  |.._..|..j..|...
+00000bb0: 0100 017c 0300 6a04 007c 0200 8301 0001  ...|..j..|......
+00000bc0: 7c03 006a 0500 8300 0001 7406 007c 0300  |..j......t..|..
+00000bd0: 6a07 0064 0100 1783 0100 5328 0200 0000  j..d......S(....
+00000be0: 739e 0100 000a 2020 2020 496e 636c 7564  s.....    Includ
+00000bf0: 6520 7468 6520 6874 6d6c 2066 6f72 2074  e the html for t
+00000c00: 6865 2063 6861 7274 2063 6f6e 7461 696e  he chart contain
+00000c10: 6572 2061 6e64 2063 7373 2066 6f72 206e  er and css for n
+00000c20: 7664 330a 2020 2020 5468 6973 2077 696c  vd3.    This wil
+00000c30: 6c20 696e 636c 7564 6520 736f 6d65 7468  l include someth
+00000c40: 696e 6720 7369 6d69 6c61 7220 6173 203a  ing similar as :
+00000c50: 0a20 2020 2020 2020 203c 6469 7620 6964  .        <div id
+00000c60: 3d22 636f 6e74 6169 6e65 726e 616d 6522  ="containername"
+00000c70: 3e3c 7376 6720 7374 796c 653d 2268 6569  ><svg style="hei
+00000c80: 6768 743a 3430 3070 783b 7769 6474 683a  ght:400px;width:
+00000c90: 3630 3070 783b 223e 3c2f 7376 673e 3c2f  600px;"></svg></
+00000ca0: 6469 763e 0a0a 2020 2020 2a2a 7573 6167  div>..    **usag
+00000cb0: 652a 2a3a 0a0a 2020 2020 2020 2020 7b25  e**:..        {%
+00000cc0: 2069 6e63 6c75 6465 5f63 6f6e 7461 696e   include_contain
+00000cd0: 6572 2022 6c69 6e65 5769 7468 466f 6375  er "lineWithFocu
+00000ce0: 7343 6861 7274 2220 3430 3020 3430 3020  sChart" 400 400 
+00000cf0: 257d 0a0a 2020 2020 2a2a 4172 6775 6d65  %}..    **Argume
+00000d00: 6e74 732a 2a3a 0a0a 2020 2020 2020 2020  nts**:..        
+00000d10: 2a20 6060 696e 636c 7564 655f 636f 6e74  * ``include_cont
+00000d20: 6169 6e65 7260 6020 2d20 636f 6e74 6169  ainer`` - contai
+00000d30: 6e65 725f 6e61 6d65 0a20 2020 2020 2020  ner_name.       
+00000d40: 202a 2060 6068 6569 6768 7460 6020 2d20   * ``height`` - 
+00000d50: 4368 6172 7420 6865 6967 6874 0a20 2020  Chart height.   
+00000d60: 2020 2020 202a 2060 6077 6964 7468 6060       * ``width``
+00000d70: 202d 2043 6861 7274 2077 6964 7468 0a20   - Chart width. 
+00000d80: 2020 2073 0100 0000 0a28 0800 0000 5203     s.....(....R.
+00000d90: 0000 0052 1e00 0000 5214 0000 0074 1000  ...R....R....t..
+00000da0: 0000 7365 745f 6772 6170 685f 6865 6967  ..set_graph_heig
+00000db0: 6874 740f 0000 0073 6574 5f67 7261 7068  htt....set_graph
+00000dc0: 5f77 6964 7468 740e 0000 0062 7569 6c64  _widtht....build
+00000dd0: 636f 6e74 6169 6e65 7252 0100 0000 522d  containerR....R-
+00000de0: 0000 0028 0400 0000 7411 0000 0069 6e63  ...(....t....inc
+00000df0: 6c75 6465 5f63 6f6e 7461 696e 6572 7406  lude_containert.
+00000e00: 0000 0068 6569 6768 7474 0500 0000 7769  ...heightt....wi
+00000e10: 6474 6852 3000 0000 2800 0000 0028 0000  dthR0...(....(..
+00000e20: 0000 734c 0000 002f 686f 6d65 2f61 7265  ..sL.../home/are
+00000e30: 736b 692f 7072 6f6a 6563 7473 2f6e 7664  ski/projects/nvd
+00000e40: 332f 646a 616e 676f 2d6e 7664 332f 646a  3/django-nvd3/dj
+00000e50: 616e 676f 5f6e 7664 332f 7465 6d70 6c61  ango_nvd3/templa
+00000e60: 7465 7461 6773 2f6e 7664 335f 7461 6773  tetags/nvd3_tags
+00000e70: 2e70 7952 3b00 0000 4e00 0000 730c 0000  .pyR;...N...s...
+00000e80: 0000 1109 010f 010d 010d 010a 0274 0000  .............t..
+00000e90: 0000 6303 0000 0009 0000 0005 0000 0043  ..c............C
+00000ea0: 0000 0073 9401 0000 7c00 0072 1300 7c00  ...s....|..r..|.
+00000eb0: 0064 0100 377d 0000 6e00 0074 0000 6a01  .d..7}..n..t..j.
+00000ec0: 0083 0000 7d03 0074 0000 6a01 0083 0000  ....}..t..j.....
+00000ed0: 7d04 0064 0200 7402 006a 0300 7c00 0066  }..d..t..j..|..f
+00000ee0: 0200 167c 0300 6403 003c 6404 0074 0200  ...|..d..<d..t..
+00000ef0: 6a03 007c 0000 6602 0016 7c04 0064 0500  j..|..f...|..d..
+00000f00: 3c64 0200 7402 006a 0300 7c00 0066 0200  <d..t..j..|..f..
+00000f10: 167c 0400 6406 003c 7c01 0072 c000 7c01  .|..d..<|..r..|.
+00000f20: 006a 0400 6401 0083 0100 7392 007c 0100  .j..d.....s..|..
+00000f30: 6401 0037 7d01 006e 0000 782b 007c 0300  d..7}..n..x+.|..
+00000f40: 445d 2000 7d05 0064 0700 7402 006a 0300  D] .}..d..t..j..
+00000f50: 7c00 007c 0100 6603 0016 7c03 007c 0500  |..|..f...|..|..
+00000f60: 3c71 9900 576e 0000 7c02 0072 1001 7c02  <q..Wn..|..r..|.
+00000f70: 006a 0400 6401 0083 0100 73e2 007c 0200  .j..d.....s..|..
+00000f80: 6401 0037 7d02 006e 0000 782b 007c 0400  d..7}..n..x+.|..
+00000f90: 445d 2000 7d06 0064 0700 7402 006a 0300  D] .}..d..t..j..
+00000fa0: 7c00 007c 0200 6603 0016 7c04 007c 0600  |..|..f...|..|..
+00000fb0: 3c71 e900 576e 0000 7405 0083 0000 7d07  <q..Wn..t.....}.
+00000fc0: 0067 0000 6408 0084 0000 7c03 006a 0600  .g..d.....|..j..
+00000fd0: 8300 0044 8301 0044 5d10 007d 0800 6409  ...D...D]..}..d.
+00000fe0: 007c 0800 165e 0200 7130 017c 0700 5f07  .|...^..q0.|.._.
+00000ff0: 0067 0000 640a 0084 0000 7c04 006a 0600  .g..d.....|..j..
+00001000: 8300 0044 8301 0044 5d10 007d 0800 640b  ...D...D]..}..d.
+00001010: 007c 0800 165e 0200 7160 017c 0700 5f08  .|...^..q`.|.._.
+00001020: 007c 0700 6a09 0083 0000 0174 0a00 7c07  .|..j......t..|.
+00001030: 006a 0b00 640c 0017 8301 0053 280d 0000  .j..d......S(...
+00001040: 0073 2103 0000 0a20 2020 2049 6e63 6c75  .s!....    Inclu
+00001050: 6465 2074 6865 2068 746d 6c20 666f 7220  de the html for 
+00001060: 7468 6520 6368 6172 7420 636f 6e74 6169  the chart contai
+00001070: 6e65 7220 616e 6420 6373 7320 666f 7220  ner and css for 
+00001080: 6e76 6433 0a20 2020 2054 6869 7320 7769  nvd3.    This wi
+00001090: 6c6c 2069 6e63 6c75 6465 2073 6f6d 6574  ll include somet
+000010a0: 6869 6e67 2073 696d 696c 6172 2061 7320  hing similar as 
+000010b0: 3a0a 0a20 2020 2020 2020 203c 6c69 6e6b  :..        <link
+000010c0: 206d 6564 6961 3d22 616c 6c22 2068 7265   media="all" hre
+000010d0: 663d 222f 7374 6174 6963 2f6e 7664 332f  f="/static/nvd3/
+000010e0: 7372 632f 6e76 2e64 332e 6373 7322 2074  src/nv.d3.css" t
+000010f0: 7970 653d 2274 6578 742f 6373 7322 2072  ype="text/css" r
+00001100: 656c 3d22 7374 796c 6573 6865 6574 2220  el="stylesheet" 
+00001110: 2f3e 0a20 2020 2020 2020 203c 7363 7269  />.        <scri
+00001120: 7074 2073 7263 3d22 2f73 7461 7469 632f  pt src="/static/
+00001130: 6433 2f64 332e 6d69 6e2e 6a73 2220 7479  d3/d3.min.js" ty
+00001140: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00001150: 6970 7422 3e3c 2f73 6372 6970 743e 0a20  ipt"></script>. 
+00001160: 2020 2020 2020 203c 7363 7269 7074 2073         <script s
+00001170: 7263 3d22 2f73 7461 7469 632f 6e76 6433  rc="/static/nvd3
+00001180: 2f6e 762e 6433 2e6d 696e 2e6a 7322 2074  /nv.d3.min.js" t
+00001190: 7970 653d 2274 6578 742f 6a61 7661 7363  ype="text/javasc
+000011a0: 7269 7074 223e 3c2f 7363 7269 7074 3e0a  ript"></script>.
+000011b0: 0a20 2020 202a 2a75 7361 6765 2a2a 3a0a  .    **usage**:.
+000011c0: 0a20 2020 2020 2020 207b 2520 696e 636c  .        {% incl
+000011d0: 7564 655f 6368 6172 745f 6a73 6373 7320  ude_chart_jscss 
+000011e0: 257d 0a0a 2020 2020 4f72 2069 6620 796f  %}..    Or if yo
+000011f0: 7520 7761 6e74 2074 6f20 7370 6563 6966  u want to specif
+00001200: 7920 6120 7375 6264 6972 6563 746f 7279  y a subdirectory
+00001210: 2062 656c 6f77 2053 5441 5449 435f 5552   below STATIC_UR
+00001220: 4c20 666f 7220 616c 6c20 7374 6174 6963  L for all static
+00001230: 2066 696c 6573 2c0a 0a20 2020 2020 2020   files,..       
+00001240: 207b 2520 696e 636c 7564 655f 6368 6172   {% include_char
+00001250: 745f 6a73 6373 7320 276e 6577 6669 6573  t_jscss 'newfies
+00001260: 2720 257d 0a0a 2020 2020 4f72 2069 6620  ' %}..    Or if 
+00001270: 796f 7520 6861 7665 2061 6c6c 2079 6f75  you have all you
+00001280: 7220 4353 5320 616e 6420 4a53 2066 696c  r CSS and JS fil
+00001290: 6573 2069 6e20 7061 7274 6963 756c 6172  es in particular
+000012a0: 2064 6972 6563 746f 7269 6573 2061 6e64   directories and
+000012b0: 2077 616e 7420 746f 2073 7065 6369 6679   want to specify
+000012c0: 2074 6865 6d2c 0a0a 2020 2020 2020 2020   them,..        
+000012d0: 7b25 2069 6e63 6c75 6465 5f63 6861 7274  {% include_chart
+000012e0: 5f6a 7363 7373 2063 7373 5f64 6972 3d27  _jscss css_dir='
+000012f0: 6373 7327 206a 735f 6469 723d 276a 7327  css' js_dir='js'
+00001300: 2025 7d0a 0a20 2020 202a 2a41 7267 756d   %}..    **Argum
+00001310: 656e 7473 2a2a 3a0a 0a20 2020 2020 2020  ents**:..       
+00001320: 202a 2060 6073 7461 7469 635f 6469 7260   * ``static_dir`
+00001330: 6020 2d0a 2020 2020 2020 2020 2a20 6060  ` -.        * ``
+00001340: 6373 735f 6469 7260 6020 2d0a 2020 2020  css_dir`` -.    
+00001350: 2020 2020 2a20 6060 6a73 5f64 6972 6060      * ``js_dir``
+00001360: 202d 0a20 2020 2074 0100 0000 2f73 0f00   -.    t..../s..
+00001370: 0000 2573 2573 6e76 6433 2f62 7569 6c64  ..%s%snvd3/build
+00001380: 2f73 0d00 0000 6e76 2e64 332e 6d69 6e2e  /s....nv.d3.min.
+00001390: 6373 7373 0700 0000 2573 2573 6433 2f73  csss....%s%sd3/s
+000013a0: 0900 0000 6433 2e6d 696e 2e6a 7373 0c00  ....d3.min.jss..
+000013b0: 0000 6e76 2e64 332e 6d69 6e2e 6a73 7306  ..nv.d3.min.jss.
+000013c0: 0000 0025 7325 7325 7363 0100 0000 0300  ...%s%s%sc......
+000013d0: 0000 0400 0000 7300 0000 7325 0000 007c  ......s...s%...|
+000013e0: 0000 5d1b 005c 0200 7d01 007d 0200 6400  ..]..\..}..}..d.
+000013f0: 007c 0200 7c01 0066 0200 1656 0171 0300  .|..|..f...V.q..
+00001400: 6401 0053 2802 0000 0073 0400 0000 2573  d..S(....s....%s
+00001410: 2573 4e28 0000 0000 2803 0000 0074 0200  %sN(....(....t..
+00001420: 0000 2e30 7408 0000 0063 7373 5f66 696c  ...0t....css_fil
+00001430: 6574 0400 0000 7061 7468 2800 0000 0028  et....path(....(
+00001440: 0000 0000 734c 0000 002f 686f 6d65 2f61  ....sL.../home/a
+00001450: 7265 736b 692f 7072 6f6a 6563 7473 2f6e  reski/projects/n
+00001460: 7664 332f 646a 616e 676f 2d6e 7664 332f  vd3/django-nvd3/
+00001470: 646a 616e 676f 5f6e 7664 332f 7465 6d70  django_nvd3/temp
+00001480: 6c61 7465 7461 6773 2f6e 7664 335f 7461  latetags/nvd3_ta
+00001490: 6773 2e70 7973 0900 0000 3c67 656e 6578  gs.pys....<genex
+000014a0: 7072 3e9f 0000 0073 0200 0000 0600 7340  pr>....s......s@
+000014b0: 0000 003c 6c69 6e6b 206d 6564 6961 3d22  ...<link media="
+000014c0: 616c 6c22 2068 7265 663d 2225 7322 2074  all" href="%s" t
+000014d0: 7970 653d 2274 6578 742f 6373 7322 2072  ype="text/css" r
+000014e0: 656c 3d22 7374 796c 6573 6865 6574 2220  el="stylesheet" 
+000014f0: 2f3e 0a63 0100 0000 0300 0000 0400 0000  />.c............
+00001500: 7300 0000 7325 0000 007c 0000 5d1b 005c  s...s%...|..]..\
+00001510: 0200 7d01 007d 0200 6400 007c 0200 7c01  ..}..}..d..|..|.
+00001520: 0066 0200 1656 0171 0300 6401 0053 2802  .f...V.q..d..S(.
+00001530: 0000 0073 0400 0000 2573 2573 4e28 0000  ...s....%s%sN(..
+00001540: 0000 2803 0000 0052 4000 0000 7407 0000  ..(....R@...t...
+00001550: 006a 735f 6669 6c65 5242 0000 0028 0000  .js_fileRB...(..
+00001560: 0000 2800 0000 0073 4c00 0000 2f68 6f6d  ..(....sL.../hom
+00001570: 652f 6172 6573 6b69 2f70 726f 6a65 6374  e/areski/project
+00001580: 732f 6e76 6433 2f64 6a61 6e67 6f2d 6e76  s/nvd3/django-nv
+00001590: 6433 2f64 6a61 6e67 6f5f 6e76 6433 2f74  d3/django_nvd3/t
+000015a0: 656d 706c 6174 6574 6167 732f 6e76 6433  emplatetags/nvd3
+000015b0: 5f74 6167 732e 7079 7309 0000 003c 6765  _tags.pys....<ge
+000015c0: 6e65 7870 723e a600 0000 7302 0000 0006  nexpr>....s.....
+000015d0: 0073 4200 0000 3c73 6372 6970 7420 7372  .sB...<script sr
+000015e0: 633d 2225 7322 2074 7970 653d 2274 6578  c="%s" type="tex
+000015f0: 742f 6a61 7661 7363 7269 7074 2220 6368  t/javascript" ch
+00001600: 6172 7365 743d 2275 7466 2d38 223e 3c2f  arset="utf-8"></
+00001610: 7363 7269 7074 3e0a 7301 0000 000a 280c  script>.s.....(.
+00001620: 0000 0074 0b00 0000 636f 6c6c 6563 7469  ...t....collecti
+00001630: 6f6e 7374 0b00 0000 4f72 6465 7265 6444  onst....OrderedD
+00001640: 6963 7452 0200 0000 740a 0000 0053 5441  ictR....t....STA
+00001650: 5449 435f 5552 4c74 0800 0000 656e 6473  TIC_URLt....ends
+00001660: 7769 7468 5203 0000 0074 0500 0000 6974  withR....t....it
+00001670: 656d 7374 0a00 0000 6865 6164 6572 5f63  emst....header_c
+00001680: 7373 7409 0000 0068 6561 6465 725f 6a73  sst....header_js
+00001690: 740f 0000 0062 7569 6c64 6874 6d6c 6865  t....buildhtmlhe
+000016a0: 6164 6572 5201 0000 0074 0a00 0000 6874  aderR....t....ht
+000016b0: 6d6c 6865 6164 6572 2809 0000 0074 0a00  mlheader(....t..
+000016c0: 0000 7374 6174 6963 5f64 6972 7407 0000  ..static_dirt...
+000016d0: 0063 7373 5f64 6972 7406 0000 006a 735f  .css_dirt....js_
+000016e0: 6469 7274 0e00 0000 6373 735f 6669 6c65  dirt....css_file
+000016f0: 735f 6469 7273 740d 0000 006a 735f 6669  s_dirst....js_fi
+00001700: 6c65 735f 6469 7273 5241 0000 0052 4300  les_dirsRA...RC.
+00001710: 0000 5230 0000 0074 0100 0000 6828 0000  ..R0...t....h(..
+00001720: 0000 2800 0000 0073 4c00 0000 2f68 6f6d  ..(....sL.../hom
+00001730: 652f 6172 6573 6b69 2f70 726f 6a65 6374  e/areski/project
+00001740: 732f 6e76 6433 2f64 6a61 6e67 6f2d 6e76  s/nvd3/django-nv
+00001750: 6433 2f64 6a61 6e67 6f5f 6e76 6433 2f74  d3/django_nvd3/t
+00001760: 656d 706c 6174 6574 6167 732f 6e76 6433  emplatetags/nvd3
+00001770: 5f74 6167 732e 7079 7413 0000 0069 6e63  _tags.pyt....inc
+00001780: 6c75 6465 5f63 6861 7274 5f6a 7363 7373  lude_chart_jscss
+00001790: 6800 0000 7330 0000 0000 1c06 010d 020c  h...s0..........
+000017a0: 010c 0217 0217 0117 0206 010f 010d 010d  ................
+000017b0: 0121 0206 010f 010d 010d 0121 0209 0203  .!.........!....
+000017c0: 022d 0503 022d 030a 0128 1800 0000 5244  .-...-...(....RD
+000017d0: 0000 0074 1e00 0000 646a 616e 676f 2e74  ...t....django.t
+000017e0: 656d 706c 6174 652e 6465 6661 756c 7466  emplate.defaultf
+000017f0: 696c 7465 7273 5200 0000 0074 1700 0000  iltersR....t....
+00001800: 646a 616e 676f 2e75 7469 6c73 2e73 6166  django.utils.saf
+00001810: 6573 7472 696e 6752 0100 0000 740b 0000  estringR....t...
+00001820: 0064 6a61 6e67 6f2e 636f 6e66 5202 0000  .django.confR...
+00001830: 0074 0e00 0000 6e76 6433 2e4e 5644 3343  .t....nvd3.NVD3C
+00001840: 6861 7274 5203 0000 0074 0400 0000 6e76  hartR....t....nv
+00001850: 6433 5204 0000 0052 0500 0000 5206 0000  d3R....R....R...
+00001860: 0052 0700 0000 5208 0000 0052 0900 0000  .R....R....R....
+00001870: 520a 0000 0052 0b00 0000 520c 0000 0052  R....R....R....R
+00001880: 0d00 0000 740a 0000 0073 696d 706c 655f  ....t....simple_
+00001890: 7461 6752 3700 0000 523b 0000 0052 5300  tagR7...R;...RS.
+000018a0: 0000 2800 0000 0028 0000 0000 2800 0000  ..(....(....(...
+000018b0: 0073 4c00 0000 2f68 6f6d 652f 6172 6573  .sL.../home/ares
+000018c0: 6b69 2f70 726f 6a65 6374 732f 6e76 6433  ki/projects/nvd3
+000018d0: 2f64 6a61 6e67 6f2d 6e76 6433 2f64 6a61  /django-nvd3/dja
+000018e0: 6e67 6f5f 6e76 6433 2f74 656d 706c 6174  ngo_nvd3/templat
+000018f0: 6574 6167 732f 6e76 6433 5f74 6167 732e  etags/nvd3_tags.
+00001900: 7079 7408 0000 003c 6d6f 6475 6c65 3e01  pyt....<module>.
+00001910: 0000 0073 1600 0000 0c02 1001 1001 1001  ...s............
+00001920: 1001 4606 0601 0f40 0601 1219 0601       ..F....@......
```

