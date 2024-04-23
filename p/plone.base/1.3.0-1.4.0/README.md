# Comparing `tmp/plone.base-1.3.0.tar.gz` & `tmp/plone_base-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.base-1.3.0.tar", last modified: Fri Mar 15 10:33:15 2024, max compression
+gzip compressed data, was "plone_base-1.4.0.tar", last modified: Tue Apr 23 15:33:56 2024, max compression
```

## Comparing `plone.base-1.3.0.tar` & `plone_base-1.4.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.737251 plone.base-1.3.0/
--rw-r--r--   0 maurits    (501) staff       (20)     5073 2024-03-15 10:33:14.000000 plone.base-1.3.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      105 2024-03-15 10:33:14.000000 plone.base-1.3.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     8341 2024-03-15 10:33:15.736957 plone.base-1.3.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2025 2024-03-15 10:33:14.000000 plone.base-1.3.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4234 2024-03-15 10:33:14.000000 plone.base-1.3.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1263 2024-03-15 10:33:15.737975 plone.base-1.3.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       39 2024-03-15 10:33:14.000000 plone.base-1.3.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.716578 plone.base-1.3.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.719685 plone.base-1.3.0/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.724786 plone.base-1.3.0/src/plone/base/
--rw-r--r--   0 maurits    (501) staff       (20)      238 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2894 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/batch.py
--rw-r--r--   0 maurits    (501) staff       (20)     5502 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)    12075 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/i18nl10n.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.733389 plone.base-1.3.0/src/plone/base/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)     2658 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      305 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/atd.py
--rw-r--r--   0 maurits    (501) staff       (20)      289 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/basetool.py
--rw-r--r--   0 maurits    (501) staff       (20)      151 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/breadcrumbs.py
--rw-r--r--   0 maurits    (501) staff       (20)     3060 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)      316 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/content.py
--rw-r--r--   0 maurits    (501) staff       (20)    64021 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      403 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)      652 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/events.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/images.py
--rw-r--r--   0 maurits    (501) staff       (20)      529 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/installable.py
--rw-r--r--   0 maurits    (501) staff       (20)      697 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)      229 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/language.py
--rw-r--r--   0 maurits    (501) staff       (20)     1993 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/login.py
--rw-r--r--   0 maurits    (501) staff       (20)      853 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/migration.py
--rw-r--r--   0 maurits    (501) staff       (20)     1471 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/password_reset.py
--rw-r--r--   0 maurits    (501) staff       (20)      243 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)      495 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/properties.py
--rw-r--r--   0 maurits    (501) staff       (20)     4824 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/resources.py
--rw-r--r--   0 maurits    (501) staff       (20)      585 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/siteroot.py
--rw-r--r--   0 maurits    (501) staff       (20)      453 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/structure.py
--rw-r--r--   0 maurits    (501) staff       (20)     6328 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/syndication.py
--rw-r--r--   0 maurits    (501) staff       (20)     1499 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/translationservice.py
--rw-r--r--   0 maurits    (501) staff       (20)      159 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/interfaces/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2196 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/navigationroot.py
--rw-r--r--   0 maurits    (501) staff       (20)     2268 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.735748 plone.base-1.3.0/src/plone/base/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3507 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/messages.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1387 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/test_batch.py
--rw-r--r--   0 maurits    (501) staff       (20)      226 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    17957 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/test_i18nl10n.py
--rw-r--r--   0 maurits    (501) staff       (20)     2286 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/test_root.py
--rw-r--r--   0 maurits    (501) staff       (20)     6869 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    20346 2024-03-15 10:33:14.000000 plone.base-1.3.0/src/plone/base/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:33:15.736249 plone.base-1.3.0/src/plone.base.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     8341 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1744 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      142 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-15 10:33:15.000000 plone.base-1.3.0/src/plone.base.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.469552 plone_base-1.4.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     5525 2024-04-23 15:33:55.000000 plone_base-1.4.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2024-04-23 15:33:55.000000 plone_base-1.4.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     8793 2024-04-23 15:33:56.469339 plone_base-1.4.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2025 2024-04-23 15:33:55.000000 plone_base-1.4.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4234 2024-04-23 15:33:55.000000 plone_base-1.4.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1263 2024-04-23 15:33:56.470108 plone_base-1.4.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       39 2024-04-23 15:33:55.000000 plone_base-1.4.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.452102 plone_base-1.4.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.454647 plone_base-1.4.0/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.459097 plone_base-1.4.0/src/plone/base/
+-rw-r--r--   0 maurits    (501) staff       (20)      238 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2894 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/batch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5502 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12075 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/i18nl10n.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.466311 plone_base-1.4.0/src/plone/base/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)     2658 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      305 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/atd.py
+-rw-r--r--   0 maurits    (501) staff       (20)      289 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/basetool.py
+-rw-r--r--   0 maurits    (501) staff       (20)      151 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/breadcrumbs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3060 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)      316 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)    64642 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      652 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/images.py
+-rw-r--r--   0 maurits    (501) staff       (20)      529 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/installable.py
+-rw-r--r--   0 maurits    (501) staff       (20)      697 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1993 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/login.py
+-rw-r--r--   0 maurits    (501) staff       (20)      853 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/migration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1471 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/password_reset.py
+-rw-r--r--   0 maurits    (501) staff       (20)      243 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)      495 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4824 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/resources.py
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/siteroot.py
+-rw-r--r--   0 maurits    (501) staff       (20)      453 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/structure.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6328 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/syndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1499 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/translationservice.py
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/interfaces/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2196 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/navigationroot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2268 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.468353 plone_base-1.4.0/src/plone/base/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3507 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/messages.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1387 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/test_batch.py
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17957 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/test_i18nl10n.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2286 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/test_root.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6869 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20346 2024-04-23 15:33:55.000000 plone_base-1.4.0/src/plone/base/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:33:56.468770 plone_base-1.4.0/src/plone.base.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     8793 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1744 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 15:33:56.000000 plone_base-1.4.0/src/plone.base.egg-info/top_level.txt
```

### Comparing `plone.base-1.3.0/CHANGES.rst` & `plone_base-1.4.0/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.4.0 (2024-04-23)
+------------------
+
+New features:
+
+
+- enable Plugin 'accordion' for TinyMCE @1letter (#62)
+- Add a field ``webstats_head_js`` to the Site controlpanel and render its
+  contents in the head section using ``IHtmlHeadLinks`` viewlet manager.
+  See `issue 3931 <https://github.com/plone/Products.CMFPlone/issues/3931>`_:
+  some javascript needs to be loaded at the bottom of the page, and some in the head section.
+  [jladage] (#3931)
+
+
 1.3.0 (2024-03-15)
 ------------------
 
 New features:
 
 
 - Make the TinyMCE help plugin available as an option [rber474] (#41)
```

### Comparing `plone.base-1.3.0/PKG-INFO` & `plone_base-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.3.0
+Version: 1.4.0
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -89,14 +89,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.4.0 (2024-04-23)
+------------------
+
+New features:
+
+
+- enable Plugin 'accordion' for TinyMCE @1letter (#62)
+- Add a field ``webstats_head_js`` to the Site controlpanel and render its
+  contents in the head section using ``IHtmlHeadLinks`` viewlet manager.
+  See `issue 3931 <https://github.com/plone/Products.CMFPlone/issues/3931>`_:
+  some javascript needs to be loaded at the bottom of the page, and some in the head section.
+  [jladage] (#3931)
+
+
 1.3.0 (2024-03-15)
 ------------------
 
 New features:
 
 
 - Make the TinyMCE help plugin available as an option [rber474] (#41)
```

### Comparing `plone.base-1.3.0/README.rst` & `plone_base-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/pyproject.toml` & `plone_base-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/setup.cfg` & `plone_base-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.3.0
+version = 1.4.0
 name = plone.base
 description = Plone Interface contracts, plus basic features and utilities
 long_description = file: README.rst, CHANGES.rst
 keywords = plone
 author = Jens W. Klein
 author_email = jk@kleinundpartner.at
 maintainer = Plone Release Team
```

### Comparing `plone.base-1.3.0/src/plone/base/batch.py` & `plone_base-1.4.0/src/plone/base/batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/defaultpage.py` & `plone_base-1.4.0/src/plone/base/defaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/i18nl10n.py` & `plone_base-1.4.0/src/plone/base/i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/__init__.py` & `plone_base-1.4.0/src/plone/base/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/constrains.py` & `plone_base-1.4.0/src/plone/base/interfaces/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/controlpanel.py` & `plone_base-1.4.0/src/plone/base/interfaces/controlpanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,15 @@
             "samp",
             "section",
             "small",
             "source",
             "span",
             "strong",
             "sub",
+            "summary",
             "sup",
             "table",
             "tbody",
             "td",
             "tfoot",
             "th",
             "thead",
@@ -329,14 +330,15 @@
             "style",
             "controls",
             "poster",
             "autoplay",
             "loading",
             "srcset",
             "sizes",
+            "open",
         ],
         value_type=schema.TextLine(),
         missing_value=[],
         required=False,
     )
 
 
@@ -527,14 +529,15 @@
         title=_("label_tinymce_plugins", default="Editor plugins"),
         description=_(
             "help_tinymce_plugins", default=("Select plugins to include with tinymce")
         ),
         value_type=schema.Choice(
             vocabulary=SimpleVocabulary(
                 [
+                    SimpleTerm("accordion", "accordion", "accordion"),
                     SimpleTerm("advlist", "advlist", "advlist"),
                     SimpleTerm("anchor", "anchor", "anchor"),
                     SimpleTerm("autolink", "autolink", "autolink"),
                     SimpleTerm("autosave", "autosave", "autosave"),
                     SimpleTerm("charmap", "charmap", "charmap"),
                     SimpleTerm("code", "code", "code"),
                     SimpleTerm("colorpicker", "colorpicker", "colorpicker"),
@@ -1191,18 +1194,31 @@
             "these search engines to more intelligently "
             "crawl your site."
         ),
         default=False,
         required=False,
     )
 
+    webstats_head_js = schema.SourceText(
+        title=_("JavaScript integrations included in head section"),
+        description=_(
+            "For enabling third-party JavaScript integrations "
+            "from external providers (e.g., Google "
+            "Analytics), paste the provided code snippet here. "
+            "It will be rendered as "
+            "entered at the end of the head section of the page."
+        ),
+        default="",
+        required=False,
+    )
+
     webstats_js = schema.SourceText(
-        title=_("JavaScript for web statistics support"),
+        title=_("JavaScript integrations included after the footer"),
         description=_(
-            "For enabling web statistics support "
+            "For enabling third-party JavaScript integrations "
             "from external providers (e.g. Google "
             "Analytics). Paste the provided code snippet here. "
             "It will be rendered as "
             "entered near the end of the page."
         ),
         default="",
         required=False,
```

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/events.py` & `plone_base-1.4.0/src/plone/base/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/images.py` & `plone_base-1.4.0/src/plone/base/interfaces/images.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/installable.py` & `plone_base-1.4.0/src/plone/base/interfaces/installable.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/interface.py` & `plone_base-1.4.0/src/plone/base/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/login.py` & `plone_base-1.4.0/src/plone/base/interfaces/login.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/migration.py` & `plone_base-1.4.0/src/plone/base/interfaces/migration.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/password_reset.py` & `plone_base-1.4.0/src/plone/base/interfaces/password_reset.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/resources.py` & `plone_base-1.4.0/src/plone/base/interfaces/resources.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/siteroot.py` & `plone_base-1.4.0/src/plone/base/interfaces/siteroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/syndication.py` & `plone_base-1.4.0/src/plone/base/interfaces/syndication.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/interfaces/translationservice.py` & `plone_base-1.4.0/src/plone/base/interfaces/translationservice.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/navigationroot.py` & `plone_base-1.4.0/src/plone/base/navigationroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/permissions.py` & `plone_base-1.4.0/src/plone/base/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/tests/messages.rst` & `plone_base-1.4.0/src/plone/base/tests/messages.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/tests/test_batch.py` & `plone_base-1.4.0/src/plone/base/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/tests/test_i18nl10n.py` & `plone_base-1.4.0/src/plone/base/tests/test_i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/tests/test_root.py` & `plone_base-1.4.0/src/plone/base/tests/test_root.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/tests/test_utils.py` & `plone_base-1.4.0/src/plone/base/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone/base/utils.py` & `plone_base-1.4.0/src/plone/base/utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.3.0/src/plone.base.egg-info/PKG-INFO` & `plone_base-1.4.0/src/plone.base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.3.0
+Version: 1.4.0
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -89,14 +89,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.4.0 (2024-04-23)
+------------------
+
+New features:
+
+
+- enable Plugin 'accordion' for TinyMCE @1letter (#62)
+- Add a field ``webstats_head_js`` to the Site controlpanel and render its
+  contents in the head section using ``IHtmlHeadLinks`` viewlet manager.
+  See `issue 3931 <https://github.com/plone/Products.CMFPlone/issues/3931>`_:
+  some javascript needs to be loaded at the bottom of the page, and some in the head section.
+  [jladage] (#3931)
+
+
 1.3.0 (2024-03-15)
 ------------------
 
 New features:
 
 
 - Make the TinyMCE help plugin available as an option [rber474] (#41)
```

### Comparing `plone.base-1.3.0/src/plone.base.egg-info/SOURCES.txt` & `plone_base-1.4.0/src/plone.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

