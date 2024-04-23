# Comparing `tmp/idc_index_data-18.0.0.tar.gz` & `tmp/idc_index_data-18.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idc_index_data-18.0.0.tar", last modified: Thu Apr 11 02:25:44 2024, max compression
+gzip compressed data, was "idc_index_data-18.0.1.tar", last modified: Tue Apr 23 20:17:21 2024, max compression
```

## Comparing `idc_index_data-18.0.0.tar` & `idc_index_data-18.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      125 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.gitattributes
--rw-r--r--   0        0        0     2858 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1089 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2217 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      313 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/workflows/keep-alive.yml
--rw-r--r--   0        0        0     2264 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.gitignore
--rw-r--r--   0        0        0     2338 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1352 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/CMakeLists.txt
--rw-r--r--   0        0        0     1054 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/LICENSE
--rw-r--r--   0        0        0     2293 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/README.md
--rw-r--r--   0        0        0      849 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/docs/conf.py
--rw-r--r--   0        0        0      201 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/docs/index.md
--rw-r--r--   0        0        0     5359 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/noxfile.py
--rw-r--r--   0        0        0     4198 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/pyproject.toml
--rw-r--r--   0        0        0     5034 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/scripts/python/idc_index_data_manager.py
--rwxr-xr-x   0        0        0     2653 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/scripts/python/update_idc_index_version.py
--rw-r--r--   0        0        0     1349 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/scripts/sql/idc_index.sql
--rw-r--r--   0        0        0     1058 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/src/idc_index_data/__init__.py
--rw-r--r--   0        0        0       49 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/src/idc_index_data/_version.pyi
--rw-r--r--   0        0        0        0 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/src/idc_index_data/py.typed
--rw-r--r--   0        0        0     1206 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/tests/test_package.py
--rw-r--r--   0        0        0     5431 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.gitattributes
+-rw-r--r--   0        0        0     2858 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1089 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2217 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      313 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.github/workflows/keep-alive.yml
+-rw-r--r--   0        0        0     2264 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.gitignore
+-rw-r--r--   0        0        0     2338 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1352 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1054 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/LICENSE
+-rw-r--r--   0        0        0     2293 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/README.md
+-rw-r--r--   0        0        0      849 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/docs/conf.py
+-rw-r--r--   0        0        0      201 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/docs/index.md
+-rw-r--r--   0        0        0     5359 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/noxfile.py
+-rw-r--r--   0        0        0     4198 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5034 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/scripts/python/idc_index_data_manager.py
+-rwxr-xr-x   0        0        0     2653 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/scripts/python/update_idc_index_version.py
+-rw-r--r--   0        0        0     1404 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/scripts/sql/idc_index.sql
+-rw-r--r--   0        0        0     1058 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/src/idc_index_data/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/src/idc_index_data/_version.pyi
+-rw-r--r--   0        0        0        0 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/src/idc_index_data/py.typed
+-rw-r--r--   0        0        0     1206 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/tests/test_package.py
+-rw-r--r--   0        0        0     5431 2024-04-23 20:17:21.000000 idc_index_data-18.0.1/PKG-INFO
```

### Comparing `idc_index_data-18.0.0/.github/CONTRIBUTING.md` & `idc_index_data-18.0.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/.github/matchers/pylint.json` & `idc_index_data-18.0.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/.github/workflows/cd.yml` & `idc_index_data-18.0.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/.github/workflows/ci.yml` & `idc_index_data-18.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/.gitignore` & `idc_index_data-18.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/.pre-commit-config.yaml` & `idc_index_data-18.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/CMakeLists.txt` & `idc_index_data-18.0.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/LICENSE` & `idc_index_data-18.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/README.md` & `idc_index_data-18.0.1/README.md`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/docs/conf.py` & `idc_index_data-18.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/noxfile.py` & `idc_index_data-18.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/pyproject.toml` & `idc_index_data-18.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "requests"
 ]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "idc-index-data"
-version = "18.0.0"
+version = "18.0.1"
 authors = [
   { name = "Andrey Fedorov", email = "andrey.fedorov@gmail.com" },
   { name = "Vamsi Thiriveedhi", email = "vthiriveedhi@mgh.harvard.edu" },
   { name = "Jean-Christophe Fillion-Robin", email = "jchris.fillionr@kitware.com" },
 ]
 description = "ImagingDataCommons index to query and download data."
 readme = "README.md"
```

### Comparing `idc_index_data-18.0.0/scripts/python/idc_index_data_manager.py` & `idc_index_data-18.0.1/scripts/python/idc_index_data_manager.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/scripts/python/update_idc_index_version.py` & `idc_index_data-18.0.1/scripts/python/update_idc_index_version.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/scripts/sql/idc_index.sql` & `idc_index_data-18.0.1/scripts/sql/idc_index.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 SELECT
   # collection level attributes
   ANY_VALUE(collection_id) AS collection_id,
+  ANY_VALUE(analysis_result_id) AS analysis_result_id,
   ANY_VALUE(PatientID) AS PatientID,
   SeriesInstanceUID,
   ANY_VALUE(StudyInstanceUID) AS StudyInstanceUID,
   ANY_VALUE(source_DOI) AS source_DOI,
   # patient level attributes
   ANY_VALUE(PatientAge) AS PatientAge,
   ANY_VALUE(PatientSex) AS PatientSex,
```

### Comparing `idc_index_data-18.0.0/src/idc_index_data/__init__.py` & `idc_index_data-18.0.1/src/idc_index_data/__init__.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/tests/test_package.py` & `idc_index_data-18.0.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-18.0.0/PKG-INFO` & `idc_index_data-18.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idc-index-data
-Version: 18.0.0
+Version: 18.0.1
 Summary: ImagingDataCommons index to query and download data.
 Author-Email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 License: Copyright 2024 Andrey Fedorov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

