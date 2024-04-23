# Comparing `tmp/pinax-announcements-4.0.0.tar.gz` & `tmp/pinax-announcements-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinax-announcements-4.0.0.tar", last modified: Fri Jul 17 23:11:14 2020, max compression
+gzip compressed data, was "pinax-announcements-4.0.1.tar", last modified: Tue Apr 23 13:30:26 2024, max compression
```

## Comparing `pinax-announcements-4.0.0.tar` & `pinax-announcements-4.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.268395 pinax-announcements-4.0.0/
--rw-r--r--   0 katherinemichel   (501) staff       (20)      691 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/AUTHORS
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1104 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/LICENSE
--rw-r--r--   0 katherinemichel   (501) staff       (20)       50 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/MANIFEST.in
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3588 2020-07-17 23:11:14.268112 pinax-announcements-4.0.0/PKG-INFO
--rw-r--r--   0 katherinemichel   (501) staff       (20)    13206 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/README.md
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.255910 pinax-announcements-4.0.0/pinax/
--rw-r--r--   0 katherinemichel   (501) staff       (20)       87 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/__init__.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.261395 pinax-announcements-4.0.0/pinax/announcements/
--rw-r--r--   0 katherinemichel   (501) staff       (20)       98 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1196 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/admin.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      360 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/auth_backends.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      358 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/forms.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.262370 pinax-announcements-4.0.0/pinax/announcements/migrations/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2447 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/migrations/0001_initial.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/migrations/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2096 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/models.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      294 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/signals.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.262930 pinax-announcements-4.0.0/pinax/announcements/templatetags/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/templatetags/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1422 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/templatetags/pinax_announcements_tags.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.265791 pinax-announcements-4.0.0/pinax/announcements/tests/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/tests/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)       93 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/tests/test.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)    17593 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/tests/tests.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      322 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/tests/urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      817 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3871 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/pinax/announcements/views.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:11:14.267678 pinax-announcements-4.0.0/pinax_announcements.egg-info/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3588 2020-07-17 23:11:14.000000 pinax-announcements-4.0.0/pinax_announcements.egg-info/PKG-INFO
--rw-r--r--   0 katherinemichel   (501) staff       (20)      902 2020-07-17 23:11:14.000000 pinax-announcements-4.0.0/pinax_announcements.egg-info/SOURCES.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        1 2020-07-17 23:11:14.000000 pinax-announcements-4.0.0/pinax_announcements.egg-info/dependency_links.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        1 2020-07-17 23:11:14.000000 pinax-announcements-4.0.0/pinax_announcements.egg-info/not-zip-safe
--rw-r--r--   0 katherinemichel   (501) staff       (20)       12 2020-07-17 23:11:14.000000 pinax-announcements-4.0.0/pinax_announcements.egg-info/requires.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        6 2020-07-17 23:11:14.000000 pinax-announcements-4.0.0/pinax_announcements.egg-info/top_level.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)       38 2020-07-17 23:11:14.268485 pinax-announcements-4.0.0/setup.cfg
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3593 2020-07-17 23:10:07.000000 pinax-announcements-4.0.0/setup.py
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.735697 pinax-announcements-4.0.1/
+-rw-r--r--   0 agus       (502) staff       (20)      726 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/AUTHORS
+-rw-r--r--   0 agus       (502) staff       (20)     1104 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/LICENSE
+-rw-r--r--   0 agus       (502) staff       (20)       50 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/MANIFEST.in
+-rw-r--r--   0 agus       (502) staff       (20)     3525 2024-04-23 13:30:26.735457 pinax-announcements-4.0.1/PKG-INFO
+-rw-r--r--   0 agus       (502) staff       (20)    13347 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/README.md
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.731674 pinax-announcements-4.0.1/pinax/
+-rw-r--r--   0 agus       (502) staff       (20)       87 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/__init__.py
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.732675 pinax-announcements-4.0.1/pinax/announcements/
+-rw-r--r--   0 agus       (502) staff       (20)       98 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/__init__.py
+-rw-r--r--   0 agus       (502) staff       (20)     1196 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/admin.py
+-rw-r--r--   0 agus       (502) staff       (20)      360 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/auth_backends.py
+-rw-r--r--   0 agus       (502) staff       (20)      358 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/forms.py
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.732940 pinax-announcements-4.0.1/pinax/announcements/migrations/
+-rw-r--r--   0 agus       (502) staff       (20)     2447 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/migrations/0001_initial.py
+-rw-r--r--   0 agus       (502) staff       (20)        0 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/migrations/__init__.py
+-rw-r--r--   0 agus       (502) staff       (20)     2096 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/models.py
+-rw-r--r--   0 agus       (502) staff       (20)      168 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/signals.py
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.733178 pinax-announcements-4.0.1/pinax/announcements/templatetags/
+-rw-r--r--   0 agus       (502) staff       (20)        0 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/templatetags/__init__.py
+-rw-r--r--   0 agus       (502) staff       (20)     1350 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/templatetags/pinax_announcements_tags.py
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.734048 pinax-announcements-4.0.1/pinax/announcements/tests/
+-rw-r--r--   0 agus       (502) staff       (20)        0 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/tests/__init__.py
+-rw-r--r--   0 agus       (502) staff       (20)       93 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/tests/test.py
+-rw-r--r--   0 agus       (502) staff       (20)    17593 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/tests/tests.py
+-rw-r--r--   0 agus       (502) staff       (20)      322 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/tests/urls.py
+-rw-r--r--   0 agus       (502) staff       (20)      840 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/urls.py
+-rw-r--r--   0 agus       (502) staff       (20)     3939 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/pinax/announcements/views.py
+drwxr-xr-x   0 agus       (502) staff       (20)        0 2024-04-23 13:30:26.735180 pinax-announcements-4.0.1/pinax_announcements.egg-info/
+-rw-r--r--   0 agus       (502) staff       (20)     3525 2024-04-23 13:30:26.000000 pinax-announcements-4.0.1/pinax_announcements.egg-info/PKG-INFO
+-rw-r--r--   0 agus       (502) staff       (20)      902 2024-04-23 13:30:26.000000 pinax-announcements-4.0.1/pinax_announcements.egg-info/SOURCES.txt
+-rw-r--r--   0 agus       (502) staff       (20)        1 2024-04-23 13:30:26.000000 pinax-announcements-4.0.1/pinax_announcements.egg-info/dependency_links.txt
+-rw-r--r--   0 agus       (502) staff       (20)        1 2024-04-23 13:30:26.000000 pinax-announcements-4.0.1/pinax_announcements.egg-info/not-zip-safe
+-rw-r--r--   0 agus       (502) staff       (20)       12 2024-04-23 13:30:26.000000 pinax-announcements-4.0.1/pinax_announcements.egg-info/requires.txt
+-rw-r--r--   0 agus       (502) staff       (20)        6 2024-04-23 13:30:26.000000 pinax-announcements-4.0.1/pinax_announcements.egg-info/top_level.txt
+-rw-r--r--   0 agus       (502) staff       (20)       38 2024-04-23 13:30:26.735752 pinax-announcements-4.0.1/setup.cfg
+-rw-r--r--   0 agus       (502) staff       (20)     3935 2024-04-23 13:30:14.000000 pinax-announcements-4.0.1/setup.py
```

### Comparing `pinax-announcements-4.0.0/AUTHORS` & `pinax-announcements-4.0.1/AUTHORS`

 * *Files 17% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 Primoz Kerin <primoz.kerin@xlab.si>
 Anna Ossowski <ossanna16@gmx.de>
 Patrick Cloke <clokep@patrick.cloke.us>
 arthur <arthur@wallstreetweb.net>
 Graham Ullrich <graham@flyingcracker.com>
 Mfon Eti-mfon <mfonetimfon@gmail.com>
 Katherine Michel <kthrnmichel@gmail.com>
-
+Agus Makmun <summon.agus@gmail.com>
```

### Comparing `pinax-announcements-4.0.0/LICENSE` & `pinax-announcements-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinax-announcements-4.0.0/PKG-INFO` & `pinax-announcements-4.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,113 @@
-Metadata-Version: 1.1
-Name: pinax-announcements
-Version: 4.0.0
-Summary: a Django announcements app
-Home-page: http://github.com/pinax/pinax-announcements/
-Author: Pinax Team
-Author-email: team@pinaxproject.com
-License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-announcements.svg
-            :target: https://pypi.python.org/pypi/pinax-announcements/
-        
-        ===================
-        Pinax Announcements
-        ===================
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-announcements.svg
-            :target: https://pypi.python.org/pypi/pinax-announcements/
-        
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-announcements.svg
-            :target: https://circleci.com/gh/pinax/pinax-announcements
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-announcements.svg
-            :target: https://codecov.io/gh/pinax/pinax-announcements
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-announcements.svg
-            :target: https://github.com/pinax/pinax-announcements/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-announcements.svg
-            :target: https://github.com/pinax/pinax-announcements/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-announcements.svg
-            :target: https://github.com/pinax/pinax-announcements/pulls?q=is%3Apr+is%3Aclosed
-        
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://opensource.org/licenses/MIT/
-        
-        
-        ``pinax-announcements`` is a well tested, documented, and proven solution
-        for any site wanting announcements for it's users.
-        
-        Announcements have title and content, with options for filtering their display:
-        
-        * ``site_wide`` - True or False
-        * ``members_only`` - True or False
-        * ``publish_start`` - date/time or none
-        * ``publish_end`` - date/time or none
-        
-        ``pinax-announcements`` has three options for dismissing an announcement:
-        
-        * ``DISMISSAL_NO`` - always visible
-        * ``DISMISSAL_SESSION`` - dismiss for the session
-        * ``DISMISSAL_PERMANENT`` - dismiss forever
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+
-        | Django / Python | 3.6 | 3.7 | 3.8 |
-        +=================+=====+=====+=====+
-        |  2.2            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        |  3.0            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+from setuptools import find_packages, setup
+
+VERSION = "4.0.1"
+LONG_DESCRIPTION = """
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-announcements.svg
+    :target: https://pypi.python.org/pypi/pinax-announcements/
+
+===================
+Pinax Announcements
+===================
+
+.. image:: https://img.shields.io/pypi/v/pinax-announcements.svg
+    :target: https://pypi.python.org/pypi/pinax-announcements/
+
+\
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-announcements.svg
+    :target: https://circleci.com/gh/pinax/pinax-announcements
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-announcements.svg
+    :target: https://codecov.io/gh/pinax/pinax-announcements
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-announcements.svg
+    :target: https://github.com/pinax/pinax-announcements/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-announcements.svg
+    :target: https://github.com/pinax/pinax-announcements/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-announcements.svg
+    :target: https://github.com/pinax/pinax-announcements/pulls?q=is%3Apr+is%3Aclosed
+
+\
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://opensource.org/licenses/MIT/
+
+\
+
+``pinax-announcements`` is a well tested, documented, and proven solution
+for any site wanting announcements for it's users.
+
+Announcements have title and content, with options for filtering their display:
+
+* ``site_wide`` - True or False
+* ``members_only`` - True or False
+* ``publish_start`` - date/time or none
+* ``publish_end`` - date/time or none
+
+``pinax-announcements`` has three options for dismissing an announcement:
+
+* ``DISMISSAL_NO`` - always visible
+* ``DISMISSAL_SESSION`` - dismiss for the session
+* ``DISMISSAL_PERMANENT`` - dismiss forever
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+
+| Django / Python | 3.6 | 3.7 | 3.8 |
++=================+=====+=====+=====+
+|  2.2            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+|  3.0            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+|  3.1            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+|  3.2            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+|  4.0            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+"""
+
+setup(
+    author="Pinax Team",
+    author_email="team@pinaxproject.com",
+    description="a Django announcements app",
+    name="pinax-announcements",
+    long_description=LONG_DESCRIPTION,
+    version=VERSION,
+    url="http://github.com/pinax/pinax-announcements/",
+    license="MIT",
+    packages=find_packages(),
+    package_data={
+        "announcements": []
+    },
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Django",
+        "Framework :: Django :: 2.2",
+        "Framework :: Django :: 3.0",
+        "Framework :: Django :: 3.1",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
+    install_requires=[
+        "django>=2.2",
+    ],
+    tests_require=[
+        "django-test-plus>=1.0.22",
+        "pinax-templates>=1.0.4",
+        "mock>=2.0.0",
+    ],
+    test_suite="runtests.runtests",
+    zip_safe=False
+)
```

### Comparing `pinax-announcements-4.0.0/README.md` & `pinax-announcements-4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,17 @@
 * `DISMISSAL_SESSION` - dismiss for the session
 * `DISMISSAL_PERMANENT` - dismiss forever
 
 #### Supported Django and Python Versions
 
 Django / Python | 3.6 | 3.7 | 3.8
 --------------- | --- | --- | ---  
-2.2  |  *  |  *  |  *   
-3.0  |  *  |  *  |  *  
+2.2             |  *  |  *  |  *   
+3.0             |  *  |  *  |  *  
+4.0             |  *  |  *  |  *  
 
 
 ## Documentation
 
 ### Installation
 
 To install pinax-announcements:
@@ -268,14 +269,19 @@
 #### `announcement_list.html`
 
 #### `base.html`
 
 
 ## Change Log
 
+### 4.0.1
+
+* Support Django 4.0
+* Avoid extra queries when fetching dismissals #63
+
 ### 4.0.0
 
 * Drop Django 1.11, 2.0, and 2.1, and Python 2,7, 3.4, and 3.5 support
 * Add Django 2.2 and 3.0, and Python 3.6, 3.7, and 3.8 support
 * Update packaging configs
 * Direct users to community resources
```

### Comparing `pinax-announcements-4.0.0/pinax/announcements/admin.py` & `pinax-announcements-4.0.1/pinax/announcements/admin.py`

 * *Files identical despite different names*

### Comparing `pinax-announcements-4.0.0/pinax/announcements/migrations/0001_initial.py` & `pinax-announcements-4.0.1/pinax/announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pinax-announcements-4.0.0/pinax/announcements/models.py` & `pinax-announcements-4.0.1/pinax/announcements/models.py`

 * *Files identical despite different names*

### Comparing `pinax-announcements-4.0.0/pinax/announcements/templatetags/pinax_announcements_tags.py` & `pinax-announcements-4.0.1/pinax/announcements/templatetags/pinax_announcements_tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         ).filter(
             site_wide=True
         )
 
         exclusions = request.session.get("excluded_announcements", [])
         exclusions = set(exclusions)
         if request.user.is_authenticated:
-            for dismissal in request.user.announcement_dismissals.all():
-                exclusions.add(dismissal.announcement.pk)
+            qs = qs.exclude(dismissals__user=request.user)
         else:
             qs = qs.exclude(members_only=True)
         context[self.as_var] = qs.exclude(pk__in=exclusions)
         return ""
 
 
 @register.tag
```

### Comparing `pinax-announcements-4.0.0/pinax/announcements/tests/tests.py` & `pinax-announcements-4.0.1/pinax/announcements/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pinax-announcements-4.0.0/pinax/announcements/urls.py` & `pinax-announcements-4.0.1/pinax/announcements/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from django.conf.urls import url
+from django.urls import re_path
 
 from .views import (
     AnnouncementCreateView,
     AnnouncementDeleteView,
     AnnouncementDetailView,
     AnnouncementDismissView,
     AnnouncementListView,
     AnnouncementUpdateView,
 )
 
 app_name = "pinax_announcements"
 
 urlpatterns = [
-    url(r"^$", AnnouncementListView.as_view(), name="announcement_list"),
-    url(r"^create/$", AnnouncementCreateView.as_view(), name="announcement_create"),
-    url(r"^(?P<pk>\d+)/$", AnnouncementDetailView.as_view(), name="announcement_detail"),
-    url(r"^(?P<pk>\d+)/hide/$", AnnouncementDismissView.as_view(), name="announcement_dismiss"),
-    url(r"^(?P<pk>\d+)/update/$", AnnouncementUpdateView.as_view(), name="announcement_update"),
-    url(r"^(?P<pk>\d+)/delete/$", AnnouncementDeleteView.as_view(), name="announcement_delete"),
+    re_path(r"^$", AnnouncementListView.as_view(), name="announcement_list"),
+    re_path(r"^create/$", AnnouncementCreateView.as_view(), name="announcement_create"),
+    re_path(r"^(?P<pk>\d+)/$", AnnouncementDetailView.as_view(), name="announcement_detail"),
+    re_path(r"^(?P<pk>\d+)/hide/$", AnnouncementDismissView.as_view(), name="announcement_dismiss"),
+    re_path(r"^(?P<pk>\d+)/update/$", AnnouncementUpdateView.as_view(), name="announcement_update"),
+    re_path(r"^(?P<pk>\d+)/delete/$", AnnouncementDeleteView.as_view(), name="announcement_delete"),
 ]
```

### Comparing `pinax-announcements-4.0.0/pinax/announcements/views.py` & `pinax-announcements-4.0.1/pinax/announcements/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         elif self.object.dismissal_type == Announcement.DISMISSAL_PERMANENT and \
                 request.user.is_authenticated:
             self.object.dismissals.create(user=request.user)
             status = 200
         else:
             status = 409
 
-        if request.is_ajax():
+        is_ajax = request.headers.get('x-requested-with') == 'XMLHttpRequest'
+        if is_ajax:
             return JsonResponse({}, status=status)
         else:
             return HttpResponse(content=b"", status=status)
 
 
 class ProtectedView(View):
     @method_decorator(permission_required("announcements.can_manage"))
```

### Comparing `pinax-announcements-4.0.0/pinax_announcements.egg-info/SOURCES.txt` & `pinax-announcements-4.0.1/pinax_announcements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinax-announcements-4.0.0/setup.py` & `pinax-announcements-4.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,65 @@
-from setuptools import find_packages, setup
+Metadata-Version: 2.1
+Name: pinax-announcements
+Version: 4.0.1
+Summary: a Django announcements app
+Home-page: http://github.com/pinax/pinax-announcements/
+Author: Pinax Team
+Author-email: team@pinaxproject.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: django>=2.2
+
 
-VERSION = "4.0.0"
-LONG_DESCRIPTION = """
 .. image:: http://pinaxproject.com/pinax-design/patches/pinax-announcements.svg
     :target: https://pypi.python.org/pypi/pinax-announcements/
 
 ===================
 Pinax Announcements
 ===================
 
 .. image:: https://img.shields.io/pypi/v/pinax-announcements.svg
     :target: https://pypi.python.org/pypi/pinax-announcements/
 
-\
 
 .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-announcements.svg
     :target: https://circleci.com/gh/pinax/pinax-announcements
 .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-announcements.svg
     :target: https://codecov.io/gh/pinax/pinax-announcements
 .. image:: https://img.shields.io/github/contributors/pinax/pinax-announcements.svg
     :target: https://github.com/pinax/pinax-announcements/graphs/contributors
 .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-announcements.svg
     :target: https://github.com/pinax/pinax-announcements/pulls
 .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-announcements.svg
     :target: https://github.com/pinax/pinax-announcements/pulls?q=is%3Apr+is%3Aclosed
 
-\
 
 .. image:: http://slack.pinaxproject.com/badge.svg
     :target: http://slack.pinaxproject.com/
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
     :target: https://opensource.org/licenses/MIT/
 
-\
 
 ``pinax-announcements`` is a well tested, documented, and proven solution
 for any site wanting announcements for it's users.
 
 Announcements have title and content, with options for filtering their display:
 
 * ``site_wide`` - True or False
@@ -56,49 +79,13 @@
 +-----------------+-----+-----+-----+
 | Django / Python | 3.6 | 3.7 | 3.8 |
 +=================+=====+=====+=====+
 |  2.2            |  *  |  *  |  *  |
 +-----------------+-----+-----+-----+
 |  3.0            |  *  |  *  |  *  |
 +-----------------+-----+-----+-----+
-"""
-
-setup(
-    author="Pinax Team",
-    author_email="team@pinaxproject.com",
-    description="a Django announcements app",
-    name="pinax-announcements",
-    long_description=LONG_DESCRIPTION,
-    version=VERSION,
-    url="http://github.com/pinax/pinax-announcements/",
-    license="MIT",
-    packages=find_packages(),
-    package_data={
-        "announcements": []
-    },
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Web Environment",
-        "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-    install_requires=[
-        "django>=2.2",
-    ],
-    tests_require=[
-        "django-test-plus>=1.0.22",
-        "pinax-templates>=1.0.4",
-        "mock>=2.0.0",
-    ],
-    test_suite="runtests.runtests",
-    zip_safe=False
-)
+|  3.1            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+|  3.2            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
+|  4.0            |  *  |  *  |  *  |
++-----------------+-----+-----+-----+
```

