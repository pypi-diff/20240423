# Comparing `tmp/plone.recipe.zope2instance-6.8.3.tar.gz` & `tmp/plone.recipe.zope2instance-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.recipe.zope2instance-6.8.3.tar", last modified: Wed Feb 17 09:12:09 2021, max compression
+gzip compressed data, was "dist/plone.recipe.zope2instance-6.9.0.tar", last modified: Mon Mar 22 12:58:25 2021, max compression
```

## Comparing `plone.recipe.zope2instance-6.8.3.tar` & `plone.recipe.zope2instance-6.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/
--rw-r--r--   0 maurits    (501) staff       (20)    83552 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      106 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     2281 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      182 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)    27981 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)    36875 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/CHANGES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    83552 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       19 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1778 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)      292 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)      136 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/dependency_links.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/
--rw-r--r--   0 maurits    (501) staff       (20)    37729 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/ctl.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     3851 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_beforestorage.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1866 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_blobstorage.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8818 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_zlibstorage.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13210 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/wsgi.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5158 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_tempstorage_off.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1918 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)     4385 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/test_wsgischema.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     8491 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_demostorage.rst
--rw-r--r--   0 maurits    (501) staff       (20)    11970 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_zeostorage.rst
--rw-r--r--   0 maurits    (501) staff       (20)    57964 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_zserver.rst
--rw-r--r--   0 maurits    (501) staff       (20)    20766 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_base.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3438 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_relstorage.rst
--rw-r--r--   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2914 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/make.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/bin/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/bin/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/etc/
--rw-r--r--   0 maurits    (501) staff       (20)      728 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/etc/site.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:09.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/var/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/var/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)    51773 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/recipe.py
--rw-r--r--   0 maurits    (501) staff       (20)      563 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/sentry.py
--rw-r--r--   0 maurits    (501) staff       (20)    21365 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/wsgischema.xml
--rw-r--r--   0 maurits    (501) staff       (20)       80 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/recipe/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2021-02-17 09:12:08.000000 plone.recipe.zope2instance-6.8.3/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    84231 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      305 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     2498 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      182 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)    27995 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    37217 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    84231 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       19 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1778 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      292 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      161 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/dependency_links.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/
+-rw-r--r--   0 maurits    (501) staff       (20)    38193 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/ctl.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     3851 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_beforestorage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1866 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_blobstorage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8818 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_zlibstorage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13256 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/wsgi.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5158 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_tempstorage_off.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1918 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4385 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/test_wsgischema.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8491 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_demostorage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    11970 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_zeostorage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    57964 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_zserver.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    20766 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_base.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3438 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_relstorage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2914 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/make.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/bin/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/bin/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/etc/
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/etc/site.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/var/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/var/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    51773 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/recipe.py
+-rw-r--r--   0 maurits    (501) staff       (20)      563 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/sentry.py
+-rw-r--r--   0 maurits    (501) staff       (20)    21365 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/wsgischema.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/recipe/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2021-03-22 12:58:25.000000 plone.recipe.zope2instance-6.9.0/src/plone/__init__.py
```

### Comparing `plone.recipe.zope2instance-6.8.3/PKG-INFO` & `plone.recipe.zope2instance-6.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.recipe.zope2instance
-Version: 6.8.3
+Version: 6.9.0
 Summary: Buildout recipe for creating a Zope instance
 Home-page: https://github.com/plone/plone.recipe.zope2instance
 Author: Hanno Schlichting
 Author-email: hanno@hannosch.eu
 License: ZPL 2.1
 Description: Introduction
         ============
@@ -31,16 +31,17 @@
           recipe = plone.recipe.zope2instance
           user = admin:admin
           http-address = 8080
           eggs = my.distribution
           zcml = my.distribution
         
         .. ATTENTION::
-           This release is targeted at Plone 5.2, ZODB 5, Zope 4, and Python 2.7, 3.6 or 3.7.
-           If you are using this recipe with earlier versions, you should use one of the releases from the 4.x series.
+           This release is targeted at Plone 5.2, ZODB 5, Zope 4 and Zope 5, and
+           Python 2.7 and 3.5-3.9. If you are using this recipe with earlier versions,
+           you should use one of the releases from the 4.x series.
         
         
         .. contents:: **Contents**
         
         
         Options
         =======
@@ -794,14 +795,33 @@
         .. You should *NOT* be adding new change log entries to this file.
            You should create a file in the news directory instead.
            For helpful instructions, please see:
            https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
         
         .. towncrier release notes start
         
+        6.9.0 (2021-03-22)
+        ------------------
+        
+        New features:
+        
+        
+        - Make any ctl script python-env aware
+          [sneridagh] (#162)
+        - Added support for Python 3.9 and restored support for Python 3.5 (needed for Zope 4)
+          [dataflake] (#164)
+        
+        
+        Bug fixes:
+        
+        
+        - Fixed ``$PYTHONSTARTUP`` file support for the ``debug`` command under Python 3
+          [dataflake] (#167)
+        
+        
         6.8.3 (2021-02-17)
         ------------------
         
         Bug fixes:
         
         
         - Fix windows `wsgi.ini` to have a configurable listen address. 
@@ -2214,13 +2234,16 @@
 Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Provides-Extra: test
 Provides-Extra: sentry
```

### Comparing `plone.recipe.zope2instance-6.8.3/setup.py` & `plone.recipe.zope2instance-6.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
 name = "plone.recipe.zope2instance"
-version = '6.8.3'
+version = '6.9.0'
 
 setup(
     name=name,
     version=version,
     author="Hanno Schlichting",
     author_email="hanno@hannosch.eu",
     description="Buildout recipe for creating a Zope instance",
@@ -27,37 +27,42 @@
         "Framework :: Zope :: 4",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: Zope Public License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=find_packages('src'),
     include_package_data=True,
     package_dir={'': 'src'},
     namespace_packages=['plone', 'plone.recipe'],
+    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
     install_requires=[
         'zc.buildout',
         'setuptools',
         'six',
         'zc.recipe.egg',
         'Zope >= 4.0b1',
         'ZODB >= 5.1.1',
         'ZEO',
         'waitress >= 1.2.0',
         'Paste',
+        'python-dotenv'
     ],
     extras_require={
         'test': [
             'zope.testrunner',
+            'sentry-sdk',
         ],
         'sentry': [
             'sentry-sdk',
         ]
     },
     zip_safe=False,
     entry_points={
```

### Comparing `plone.recipe.zope2instance-6.8.3/README.rst` & `plone.recipe.zope2instance-6.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
   recipe = plone.recipe.zope2instance
   user = admin:admin
   http-address = 8080
   eggs = my.distribution
   zcml = my.distribution
 
 .. ATTENTION::
-   This release is targeted at Plone 5.2, ZODB 5, Zope 4, and Python 2.7, 3.6 or 3.7.
-   If you are using this recipe with earlier versions, you should use one of the releases from the 4.x series.
+   This release is targeted at Plone 5.2, ZODB 5, Zope 4 and Zope 5, and
+   Python 2.7 and 3.5-3.9. If you are using this recipe with earlier versions,
+   you should use one of the releases from the 4.x series.
 
 
 .. contents:: **Contents**
 
 
 Options
 =======
```

### Comparing `plone.recipe.zope2instance-6.8.3/CHANGES.rst` & `plone.recipe.zope2instance-6.9.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.9.0 (2021-03-22)
+------------------
+
+New features:
+
+
+- Make any ctl script python-env aware
+  [sneridagh] (#162)
+- Added support for Python 3.9 and restored support for Python 3.5 (needed for Zope 4)
+  [dataflake] (#164)
+
+
+Bug fixes:
+
+
+- Fixed ``$PYTHONSTARTUP`` file support for the ``debug`` command under Python 3
+  [dataflake] (#167)
+
+
 6.8.3 (2021-02-17)
 ------------------
 
 Bug fixes:
 
 
 - Fix windows `wsgi.ini` to have a configurable listen address.
```

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/PKG-INFO` & `plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.recipe.zope2instance
-Version: 6.8.3
+Version: 6.9.0
 Summary: Buildout recipe for creating a Zope instance
 Home-page: https://github.com/plone/plone.recipe.zope2instance
 Author: Hanno Schlichting
 Author-email: hanno@hannosch.eu
 License: ZPL 2.1
 Description: Introduction
         ============
@@ -31,16 +31,17 @@
           recipe = plone.recipe.zope2instance
           user = admin:admin
           http-address = 8080
           eggs = my.distribution
           zcml = my.distribution
         
         .. ATTENTION::
-           This release is targeted at Plone 5.2, ZODB 5, Zope 4, and Python 2.7, 3.6 or 3.7.
-           If you are using this recipe with earlier versions, you should use one of the releases from the 4.x series.
+           This release is targeted at Plone 5.2, ZODB 5, Zope 4 and Zope 5, and
+           Python 2.7 and 3.5-3.9. If you are using this recipe with earlier versions,
+           you should use one of the releases from the 4.x series.
         
         
         .. contents:: **Contents**
         
         
         Options
         =======
@@ -794,14 +795,33 @@
         .. You should *NOT* be adding new change log entries to this file.
            You should create a file in the news directory instead.
            For helpful instructions, please see:
            https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
         
         .. towncrier release notes start
         
+        6.9.0 (2021-03-22)
+        ------------------
+        
+        New features:
+        
+        
+        - Make any ctl script python-env aware
+          [sneridagh] (#162)
+        - Added support for Python 3.9 and restored support for Python 3.5 (needed for Zope 4)
+          [dataflake] (#164)
+        
+        
+        Bug fixes:
+        
+        
+        - Fixed ``$PYTHONSTARTUP`` file support for the ``debug`` command under Python 3
+          [dataflake] (#167)
+        
+        
         6.8.3 (2021-02-17)
         ------------------
         
         Bug fixes:
         
         
         - Fix windows `wsgi.ini` to have a configurable listen address. 
@@ -2214,13 +2234,16 @@
 Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Provides-Extra: test
 Provides-Extra: sentry
```

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone.recipe.zope2instance.egg-info/SOURCES.txt` & `plone.recipe.zope2instance-6.9.0/src/plone.recipe.zope2instance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/ctl.py` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/ctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 Actions are commands like "start", "stop" and "status". If -i is specified or
 no action is specified on the command line, a "shell" interpreting actions
 typed interactively is started. Use the action "help" to find out about
 available actions.
 """
 
+from dotenv import load_dotenv
 from pkg_resources import iter_entry_points
 from time import sleep
 from waitress.wasyncore import dispatcher
 from ZConfig.loader import SchemaLoader
 from zdaemon.zdctl import ZDCmd, ZDCtlOptions
 from zdaemon.zdoptions import ZDOptions
 from Zope2.Startup.options import ConditionalSchemaParser
@@ -791,19 +792,23 @@
     In contrast to foreground this does not turn on debug mode.""")
 
     def do_debug(self, arg):
         # `-c` disables the PYTHONSTARTUP feature; load it explicitly
         interactive_startup = (
             "import os;"
             "os.path.exists(os.environ.get('PYTHONSTARTUP', '')) "
-            "and execfile(os.environ['PYTHONSTARTUP']); del os;"
+            "and %s; del os;"
         )
+        if six.PY2:
+            exec_call = "execfile(os.environ['PYTHONSTARTUP'])"
+        else:
+            exec_call = "exec(open(os.environ['PYTHONSTARTUP']).read())"
         cmdline = self.get_startup_cmd(
             self.options.python,
-            interactive_startup,
+            interactive_startup % exec_call,
             pyflags='-i',
         )
         print('Starting debugger (the name "app" is bound to the top-level '
               'Zope object)')
         os.system(cmdline)
 
     def help_debug(self):
@@ -938,21 +943,29 @@
     """Customized entry point for launching Zope without forking other processes
     """
 
     if '--wsgi' in args or '-w' in args:
         options = WSGICtlOptions()
     else:
         options = ZServerCtlOptions()
+
     options.add(name="no_request", short="R", long="no-request", flag=1)
     options.add(name="no_login", short="L", long="no-login", flag=1)
     options.add(name="object_path", short="O:", long="object-path=")
     options.add(name="wsgi", short='w:', long='wsgi=')
     # Realize arguments and set documentation which is used in the -h option
     options.realize(args, doc=__doc__)
 
+    load_dotenv(os.path.join(options.directory, '..', '..', '.env'))
+
+    if (os.environ.get('PLONE_ENV')):
+        PLONE_ENV = os.environ.get('PLONE_ENV')
+        load_dotenv(os.path.join(options.directory,
+                                 '..', '..', '.env.{}'.format(PLONE_ENV)))
+
     # Run the right command depending on whether we have ZServer
     options.interpreter = os.path.join(options.directory, 'bin', 'interpreter')
     if sys.platform == 'win32':
         options.interpreter += '-script.py'
 
     if options.wsgi is not None and \
        options.wsgi.lower() in ('off', 'false', '0'):
```

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_beforestorage.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_beforestorage.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_blobstorage.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_blobstorage.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_zlibstorage.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_zlibstorage.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/wsgi.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/wsgi.rst`

 * *Files 1% similar despite different names*

```diff
@@ -446,23 +446,19 @@
     ... user = me:me
     ... sentry_dsn = https://f00ba4ba2@my.sentry.server/9999
     ... ''' % options)
 
 Let's run it::
 
     >>> output = system(join('bin', 'buildout'))
-    >>> "Uninstalling instance" in output
-    True
-
-    >>> "Installing instance" in output
-    True
-
-    >>> WINDOWS or "Generated script" in output
-    True
-
+    >>> if "Uninstalling instance" not in output or "Installing instance" not in output:
+    ...    print(output)
+    >>> if not WINDOWS and "Generated script" not in output:
+    ...     print(output)
+    
 The buildout has updated our INI file:
 
     >>> instance = os.path.join(sample_buildout, 'parts', 'instance')
     >>> with open(os.path.join(instance, 'etc', 'wsgi.ini')) as fd:
     ...     wsgi_ini = fd.read()
     >>> print(wsgi_ini)
     [server:main]
```

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_tempstorage_off.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_tempstorage_off.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/test_docs.py` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/test_wsgischema.py` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/test_wsgischema.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_demostorage.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_demostorage.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_zeostorage.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_zeostorage.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_zserver.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_zserver.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_base.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_base.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/tests/zope2instance_relstorage.rst` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/tests/zope2instance_relstorage.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/make.py` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/make.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/skel4/etc/site.zcml` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/skel4/etc/site.zcml`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/recipe.py` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/recipe.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/sentry.py` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/sentry.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zope2instance-6.8.3/src/plone/recipe/zope2instance/wsgischema.xml` & `plone.recipe.zope2instance-6.9.0/src/plone/recipe/zope2instance/wsgischema.xml`

 * *Files identical despite different names*

