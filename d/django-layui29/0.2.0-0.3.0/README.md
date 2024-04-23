# Comparing `tmp/django_layui29-0.2.0.tar.gz` & `tmp/django_layui29-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_layui29-0.2.0.tar", max compression
+gzip compressed data, was "django_layui29-0.3.0.tar", max compression
```

## Comparing `django_layui29-0.2.0.tar` & `django_layui29-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0     1270 2024-04-06 05:01:05.929798 django_layui29-0.2.0/LICENSE
--rw-r--r--   0        0        0      950 2024-04-06 05:32:23.274001 django_layui29-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 04:54:09.874487 django_layui29-0.2.0/src/django_layui29/__init__.py
--rw-r--r--   0        0        0       66 2024-04-06 04:54:09.875486 django_layui29-0.2.0/src/django_layui29/admin.py
--rw-r--r--   0        0        0      163 2024-04-06 05:13:09.757522 django_layui29-0.2.0/src/django_layui29/apps.py
--rw-r--r--   0        0        0        0 2024-04-06 04:54:09.875486 django_layui29-0.2.0/src/django_layui29/migrations/__init__.py
--rw-r--r--   0        0        0      191 2024-04-06 05:27:31.853623 django_layui29-0.2.0/src/django_layui29/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       60 2024-04-06 04:54:09.875486 django_layui29-0.2.0/src/django_layui29/models.py
--rw-r--r--   0        0        0      618 2023-12-26 02:35:21.643462 django_layui29-0.2.0/src/django_layui29/static/layui29/css/center.css
--rw-r--r--   0        0        0      662 2024-04-06 05:23:27.634917 django_layui29-0.2.0/src/django_layui29/static/layui29/css/global.css
--rw-r--r--   0        0        0      556 2024-04-06 04:57:22.665192 django_layui29-0.2.0/src/django_layui29/templates/layui29/base.html
--rw-r--r--   0        0        0      482 2024-04-06 05:31:10.540298 django_layui29-0.2.0/src/django_layui29/templates/layui29/layout/center.html
--rw-r--r--   0        0        0       63 2024-04-06 04:54:09.876486 django_layui29-0.2.0/src/django_layui29/tests.py
--rw-r--r--   0        0        0       66 2024-04-06 04:54:09.876486 django_layui29-0.2.0/src/django_layui29/views.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 django_layui29-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1262 2024-04-14 05:19:29.566270 django_layui29-0.3.0/LICENSE
+-rw-r--r--   0        0        0      942 2024-04-23 11:59:56.699567 django_layui29-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 05:19:29.568366 django_layui29-0.3.0/src/django_layui29/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-14 05:19:29.568505 django_layui29-0.3.0/src/django_layui29/admin.py
+-rw-r--r--   0        0        0      157 2024-04-14 05:19:29.568618 django_layui29-0.3.0/src/django_layui29/apps.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:19:29.568732 django_layui29-0.3.0/src/django_layui29/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-14 05:19:29.568860 django_layui29-0.3.0/src/django_layui29/models.py
+-rw-r--r--   0        0        0      618 2024-04-14 05:19:29.569205 django_layui29-0.3.0/src/django_layui29/static/layui29/css/center.css
+-rw-r--r--   0        0        0      662 2024-04-14 05:19:29.569326 django_layui29-0.3.0/src/django_layui29/static/layui29/css/global.css
+-rw-r--r--   0        0        0     1051 2024-04-16 09:27:19.862964 django_layui29-0.3.0/src/django_layui29/static/layui29/js/base.js
+-rw-r--r--   0        0        0     1681 2024-04-16 09:25:36.599514 django_layui29-0.3.0/src/django_layui29/static/layui29/js/js.cookie.min.js
+-rw-r--r--   0        0        0      688 2024-04-23 11:55:11.219106 django_layui29-0.3.0/src/django_layui29/templates/layui29/base.html
+-rw-r--r--   0        0        0     2587 2024-04-23 11:57:40.311596 django_layui29-0.3.0/src/django_layui29/templates/layui29/component/base/header.html
+-rw-r--r--   0        0        0     1772 2024-04-16 09:33:15.587946 django_layui29-0.3.0/src/django_layui29/templates/layui29/component/base/left_nav.html
+-rw-r--r--   0        0        0     8696 2024-04-16 09:32:40.052522 django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/admin.html
+-rw-r--r--   0        0        0      464 2024-04-14 05:19:29.569815 django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/center.html
+-rw-r--r--   0        0        0      338 2024-04-23 11:54:35.415857 django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/normal.html
+-rw-r--r--   0        0        0       60 2024-04-14 05:19:29.569937 django_layui29-0.3.0/src/django_layui29/tests.py
+-rw-r--r--   0        0        0       77 2024-04-16 09:22:21.866608 django_layui29-0.3.0/src/django_layui29/utils.py
+-rw-r--r--   0        0        0       63 2024-04-14 05:19:29.570083 django_layui29-0.3.0/src/django_layui29/views.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 django_layui29-0.3.0/PKG-INFO
```

### Comparing `django_layui29-0.2.0/LICENSE` & `django_layui29-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright 2024 svtter
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
+Copyright 2024 svtter
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `django_layui29-0.2.0/src/django_layui29/static/layui29/css/center.css` & `django_layui29-0.3.0/src/django_layui29/static/layui29/css/center.css`

 * *Files identical despite different names*

### Comparing `django_layui29-0.2.0/src/django_layui29/static/layui29/css/global.css` & `django_layui29-0.3.0/src/django_layui29/static/layui29/css/global.css`

 * *Files identical despite different names*

### Comparing `django_layui29-0.2.0/PKG-INFO` & `django_layui29-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django_layui29
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: svtter
 Author-email: svtter@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (<6.0)
 Project-URL: bugs, https://github.com/Svtter/django-layui/issues
 Project-URL: changelog, https://github.com/Svtter/django-layui/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/Svtter/django-layui
 Project-URL: repository, https://github.com/Svtter/django-layui.git
```

