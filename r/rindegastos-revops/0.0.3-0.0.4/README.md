# Comparing `tmp/rindegastos_revops-0.0.3.tar.gz` & `tmp/rindegastos_revops-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rindegastos_revops-0.0.3.tar", last modified: Tue Apr 23 19:05:26 2024, max compression
+gzip compressed data, was "rindegastos_revops-0.0.4.tar", last modified: Tue Apr 23 19:33:39 2024, max compression
```

## Comparing `rindegastos_revops-0.0.3.tar` & `rindegastos_revops-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,37 @@
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:05:26.025386 rindegastos_revops-0.0.3/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 19:05:26.025279 rindegastos_revops-0.0.3/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.3/README.md
--rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.3/pyproject.toml
--rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-23 19:05:26.025671 rindegastos_revops-0.0.3/setup.cfg
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:05:26.023497 rindegastos_revops-0.0.3/src/
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:05:26.025069 rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 19:05:26.000000 rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)      298 2024-04-23 19:05:26.000000 rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/SOURCES.txt
--rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 19:05:26.000000 rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/dependency_links.txt
--rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-23 19:05:26.000000 rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/requires.txt
--rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 19:05:26.000000 rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/top_level.txt
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:05:26.024821 rindegastos_revops-0.0.3/tests/
--rw-r--r--   0 joseizam   (501) staff       (20)     1007 2024-04-23 19:03:08.000000 rindegastos_revops-0.0.3/tests/test_hubspot_api_contacts.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.654469 rindegastos_revops-0.0.4/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 19:33:39.654377 rindegastos_revops-0.0.4/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.4/README.md
+-rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.4/pyproject.toml
+-rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-23 19:33:39.654821 rindegastos_revops-0.0.4/setup.cfg
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.648907 rindegastos_revops-0.0.4/src/
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.650096 rindegastos_revops-0.0.4/src/rindegastos_revops/
+-rw-r--r--   0 joseizam   (501) staff       (20)       26 2024-04-23 19:33:10.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.651126 rindegastos_revops-0.0.4/src/rindegastos_revops/data_engineering/
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 19:00:35.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/data_engineering/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.651302 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/
+-rw-r--r--   0 joseizam   (501) staff       (20)       71 2024-04-23 16:04:11.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.652252 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/helpers/
+-rw-r--r--   0 joseizam   (501) staff       (20)      104 2024-04-23 16:03:30.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/helpers/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      129 2024-04-23 16:54:01.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/helpers/dates.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      183 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/helpers/file_name.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      852 2024-04-23 16:16:16.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/helpers/hubspot.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     2025 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.652505 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/
+-rw-r--r--   0 joseizam   (501) staff       (20)       48 2024-04-23 16:03:05.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.652900 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/companies/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 16:01:55.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/companies/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     2592 2024-04-23 18:57:23.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/companies/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.653279 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/contacts/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 16:01:43.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     3303 2024-04-23 18:57:30.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/objects/contacts/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.653665 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/properties/
+-rw-r--r--   0 joseizam   (501) staff       (20)       23 2024-04-23 16:02:25.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/properties/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      800 2024-04-23 18:57:40.000000 rindegastos_revops-0.0.4/src/rindegastos_revops/hubspot_api/properties/read_all.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.654101 rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 19:33:39.000000 rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)     1141 2024-04-23 19:33:39.000000 rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/SOURCES.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 19:33:39.000000 rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/dependency_links.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-23 19:33:39.000000 rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/requires.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       19 2024-04-23 19:33:39.000000 rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/top_level.txt
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 19:33:39.653836 rindegastos_revops-0.0.4/tests/
+-rw-r--r--   0 joseizam   (501) staff       (20)     1007 2024-04-23 19:03:08.000000 rindegastos_revops-0.0.4/tests/test_hubspot_api_contacts.py
```

### Comparing `rindegastos_revops-0.0.3/PKG-INFO` & `rindegastos_revops-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.3/setup.cfg` & `rindegastos_revops-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rindegastos_revops
-version = 0.0.3
+version = 0.0.4
 author = Jose Izam
 author_email = jose.izam99@gmail.com
 description = Simple sdk for revops packages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joigmz/rindegastos_revops
 project_urls =
```

### Comparing `rindegastos_revops-0.0.3/src/rindegastos_revops.egg-info/PKG-INFO` & `rindegastos_revops-0.0.4/src/rindegastos_revops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.3/tests/test_hubspot_api_contacts.py` & `rindegastos_revops-0.0.4/tests/test_hubspot_api_contacts.py`

 * *Files identical despite different names*

