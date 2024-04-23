# Comparing `tmp/rindegastos_revops-0.0.1.tar.gz` & `tmp/rindegastos_revops-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rindegastos_revops-0.0.1.tar", last modified: Tue Apr 23 15:03:38 2024, max compression
+gzip compressed data, was "rindegastos_revops-0.0.2.tar", last modified: Tue Apr 23 18:31:51 2024, max compression
```

## Comparing `rindegastos_revops-0.0.1.tar` & `rindegastos_revops-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,33 @@
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 15:03:38.002195 rindegastos_revops-0.0.1/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 15:03:38.002116 rindegastos_revops-0.0.1/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.1/README.md
--rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.1/pyproject.toml
--rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-23 15:03:38.002457 rindegastos_revops-0.0.1/setup.cfg
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 15:03:38.000497 rindegastos_revops-0.0.1/src/
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 15:03:38.001898 rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 15:03:37.000000 rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)      263 2024-04-23 15:03:37.000000 rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/SOURCES.txt
--rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 15:03:37.000000 rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/dependency_links.txt
--rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-23 15:03:37.000000 rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/requires.txt
--rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 15:03:37.000000 rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/top_level.txt
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.264040 rindegastos_revops-0.0.2/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 18:31:51.263963 rindegastos_revops-0.0.2/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.2/README.md
+-rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.2/pyproject.toml
+-rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-23 18:31:51.264369 rindegastos_revops-0.0.2/setup.cfg
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.258057 rindegastos_revops-0.0.2/src/
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.258627 rindegastos_revops-0.0.2/src/hubspot_api/
+-rw-r--r--   0 joseizam   (501) staff       (20)       71 2024-04-23 16:04:11.000000 rindegastos_revops-0.0.2/src/hubspot_api/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.260266 rindegastos_revops-0.0.2/src/hubspot_api/helpers/
+-rw-r--r--   0 joseizam   (501) staff       (20)      104 2024-04-23 16:03:30.000000 rindegastos_revops-0.0.2/src/hubspot_api/helpers/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      129 2024-04-23 16:54:01.000000 rindegastos_revops-0.0.2/src/hubspot_api/helpers/dates.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      183 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.2/src/hubspot_api/helpers/file_name.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      852 2024-04-23 16:16:16.000000 rindegastos_revops-0.0.2/src/hubspot_api/helpers/hubspot.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     2025 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.2/src/hubspot_api/helpers/properties_selection.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.260592 rindegastos_revops-0.0.2/src/hubspot_api/objects/
+-rw-r--r--   0 joseizam   (501) staff       (20)       48 2024-04-23 16:03:05.000000 rindegastos_revops-0.0.2/src/hubspot_api/objects/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.261176 rindegastos_revops-0.0.2/src/hubspot_api/objects/companies/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 16:01:55.000000 rindegastos_revops-0.0.2/src/hubspot_api/objects/companies/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     2604 2024-04-23 17:00:21.000000 rindegastos_revops-0.0.2/src/hubspot_api/objects/companies/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.261674 rindegastos_revops-0.0.2/src/hubspot_api/objects/contacts/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 16:01:43.000000 rindegastos_revops-0.0.2/src/hubspot_api/objects/contacts/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     3315 2024-04-23 16:51:14.000000 rindegastos_revops-0.0.2/src/hubspot_api/objects/contacts/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.262316 rindegastos_revops-0.0.2/src/hubspot_api/properties/
+-rw-r--r--   0 joseizam   (501) staff       (20)       23 2024-04-23 16:02:25.000000 rindegastos_revops-0.0.2/src/hubspot_api/properties/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      804 2024-04-23 16:23:24.000000 rindegastos_revops-0.0.2/src/hubspot_api/properties/read_all.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.263757 rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-23 18:31:51.000000 rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)      807 2024-04-23 18:31:51.000000 rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/SOURCES.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-23 18:31:51.000000 rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/dependency_links.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-23 18:31:51.000000 rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/requires.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       12 2024-04-23 18:31:51.000000 rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/top_level.txt
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-23 18:31:51.263383 rindegastos_revops-0.0.2/tests/
+-rw-r--r--   0 joseizam   (501) staff       (20)      969 2024-04-23 16:55:12.000000 rindegastos_revops-0.0.2/tests/test_hubspot_api_contacts.py
```

### Comparing `rindegastos_revops-0.0.1/PKG-INFO` & `rindegastos_revops-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.1/setup.cfg` & `rindegastos_revops-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rindegastos_revops
-version = 0.0.1
+version = 0.0.2
 author = Jose Izam
 author_email = jose.izam99@gmail.com
 description = Simple sdk for revops packages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joigmz/rindegastos_revops
 project_urls =
```

### Comparing `rindegastos_revops-0.0.1/src/rindegastos_revops.egg-info/PKG-INFO` & `rindegastos_revops-0.0.2/src/rindegastos_revops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

