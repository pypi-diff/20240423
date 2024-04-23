# Comparing `tmp/mo-sql-4.586.24095.tar.gz` & `tmp/mo_sql-4.600.24114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-sql-4.586.24095.tar", last modified: Thu Apr  4 12:58:46 2024, max compression
+gzip compressed data, was "mo_sql-4.600.24114.tar", last modified: Tue Apr 23 01:21:12 2024, max compression
```

## Comparing `mo-sql-4.586.24095.tar` & `mo_sql-4.600.24114.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:58:46.471593 mo-sql-4.586.24095/
--rw-rw-rw-   0        0        0    16725 2020-01-28 21:55:32.000000 mo-sql-4.586.24095/LICENSE
--rw-rw-rw-   0        0        0     1478 2024-04-04 12:58:46.471593 mo-sql-4.586.24095/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-01-20 19:08:03.000000 mo-sql-4.586.24095/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 12:58:46.471593 mo-sql-4.586.24095/mo_sql/
--rw-rw-rw-   0        0        0     7604 2024-03-21 02:38:31.000000 mo-sql-4.586.24095/mo_sql/__init__.py
--rw-rw-rw-   0        0        0     5460 2024-03-17 15:14:27.000000 mo-sql-4.586.24095/mo_sql/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:58:46.471593 mo-sql-4.586.24095/mo_sql.egg-info/
--rw-rw-rw-   0        0        0     1478 2024-04-04 12:58:46.000000 mo-sql-4.586.24095/mo_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-04 12:58:46.000000 mo-sql-4.586.24095/mo_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:58:46.000000 mo-sql-4.586.24095/mo_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-04-04 12:58:46.000000 mo-sql-4.586.24095/mo_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 12:58:46.000000 mo-sql-4.586.24095/mo_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 12:58:46.471593 mo-sql-4.586.24095/setup.cfg
--rw-rw-rw-   0        0        0     1468 2024-04-04 12:58:42.000000 mo-sql-4.586.24095/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 01:21:12.969454 mo_sql-4.600.24114/
+-rw-rw-rw-   0        0        0    16725 2020-01-28 21:55:32.000000 mo_sql-4.600.24114/LICENSE
+-rw-rw-rw-   0        0        0     1478 2024-04-23 01:21:12.969454 mo_sql-4.600.24114/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-01-20 19:08:03.000000 mo_sql-4.600.24114/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 01:21:12.956246 mo_sql-4.600.24114/mo_sql/
+-rw-rw-rw-   0        0        0     7604 2024-03-21 02:38:31.000000 mo_sql-4.600.24114/mo_sql/__init__.py
+-rw-rw-rw-   0        0        0     5460 2024-03-17 15:14:27.000000 mo_sql-4.600.24114/mo_sql/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 01:21:12.968240 mo_sql-4.600.24114/mo_sql.egg-info/
+-rw-rw-rw-   0        0        0     1478 2024-04-23 01:21:12.000000 mo_sql-4.600.24114/mo_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-23 01:21:12.000000 mo_sql-4.600.24114/mo_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 01:21:12.000000 mo_sql-4.600.24114/mo_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-23 01:21:12.000000 mo_sql-4.600.24114/mo_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 01:21:12.000000 mo_sql-4.600.24114/mo_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 01:21:12.970664 mo_sql-4.600.24114/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2024-04-23 01:21:08.000000 mo_sql-4.600.24114/setup.py
```

### Comparing `mo-sql-4.586.24095/LICENSE` & `mo_sql-4.600.24114/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-sql-4.586.24095/PKG-INFO` & `mo_sql-4.600.24114/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql
-Version: 4.586.24095
+Version: 4.600.24114
 Summary: More SQL!  For safely assembling SQL
 Home-page: https://github.com/klahnakoski/mo-sql
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.584.24095
+Requires-Dist: mo-dots==9.600.24114
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.584.24095
-Requires-Dist: mo-logs==8.584.24095
+Requires-Dist: mo-json==6.600.24114
+Requires-Dist: mo-logs==8.600.24114
 Provides-Extra: tests
-Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
+Requires-Dist: mo-testing>=7.585.24095; extra == "tests"
 
 # More SQL!
 
 A number of generator functions for type-safe SQL composition.
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/mo-sql/)
```

### Comparing `mo-sql-4.586.24095/mo_sql/__init__.py` & `mo_sql-4.600.24114/mo_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mo-sql-4.586.24095/mo_sql/utils.py` & `mo_sql-4.600.24114/mo_sql/utils.py`

 * *Files identical despite different names*

### Comparing `mo-sql-4.586.24095/mo_sql.egg-info/PKG-INFO` & `mo_sql-4.600.24114/mo_sql.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql
-Version: 4.586.24095
+Version: 4.600.24114
 Summary: More SQL!  For safely assembling SQL
 Home-page: https://github.com/klahnakoski/mo-sql
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.584.24095
+Requires-Dist: mo-dots==9.600.24114
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.584.24095
-Requires-Dist: mo-logs==8.584.24095
+Requires-Dist: mo-json==6.600.24114
+Requires-Dist: mo-logs==8.600.24114
 Provides-Extra: tests
-Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
+Requires-Dist: mo-testing>=7.585.24095; extra == "tests"
 
 # More SQL!
 
 A number of generator functions for type-safe SQL composition.
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/mo-sql/)
```

### Comparing `mo-sql-4.586.24095/setup.py` & `mo_sql-4.600.24114/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Topic :: Database","Topic :: Utilities","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More SQL!  For safely assembling SQL',
-    extras_require={"tests":["mo-testing>=7.562.24075"]},
+    extras_require={"tests":["mo-testing>=7.585.24095"]},
     include_package_data=True,
-    install_requires=["mo-dots==9.584.24095","mo-future==7.584.24095","mo-json==6.584.24095","mo-logs==8.584.24095"],
+    install_requires=["mo-dots==9.600.24114","mo-future==7.584.24095","mo-json==6.600.24114","mo-logs==8.600.24114"],
     license='MPL 2.0',
     long_description='# More SQL!\n\nA number of generator functions for type-safe SQL composition.\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/mo-sql/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/mo-sql.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-sql)\n\n## Summary',
     long_description_content_type='text/markdown',
     name='mo-sql',
     packages=["mo_sql"],
     url='https://github.com/klahnakoski/mo-sql',
-    version='4.586.24095'
+    version='4.600.24114'
 )
```

