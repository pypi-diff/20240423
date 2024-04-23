# Comparing `tmp/pathling-6.6.0.dev0.tar.gz` & `tmp/pathling-7.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathling-6.6.0.dev0.tar", last modified: Sun Mar 17 01:21:08 2024, max compression
+gzip compressed data, was "pathling-7.0.0.dev0.tar", last modified: Tue Apr 23 02:06:36 2024, max compression
```

## Comparing `pathling-6.6.0.dev0.tar` & `pathling-7.0.0.dev0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.010260 pathling-6.6.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-03-17 01:21:08.010260 pathling-6.6.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.006260 pathling-6.6.0.dev0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.002260 pathling-6.6.0.dev0/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.006260 pathling-6.6.0.dev0/examples/data/bundles/
--rw-r--r--   0 runner    (1001) docker     (127)    86431 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json
--rw-r--r--   0 runner    (1001) docker     (127)    66676 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.006260 pathling-6.6.0.dev0/examples/data/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/data/resources/Condition.ndjson
--rw-r--r--   0 runner    (1001) docker     (127)    29641 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/data/resources/Patient.ndjson
--rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/designation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/display.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/encode_bundles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/encode_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1606 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/member_of.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1358 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/member_of_old.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/property_of.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4536 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/query.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/subsumes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/subsumes_old.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1347 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1310 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/examples/translate_old.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.006260 pathling-6.6.0.dev0/pathling/
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-17 01:21:03.000000 pathling-6.6.0.dev0/pathling/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)    21092 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/datasink.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/fhir.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/pathling/udfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.010260 pathling-6.6.0.dev0/pathling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-03-17 01:21:07.000000 pathling-6.6.0.dev0/pathling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-17 01:21:08.000000 pathling-6.6.0.dev0/pathling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 01:21:07.000000 pathling-6.6.0.dev0/pathling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-17 01:21:07.000000 pathling-6.6.0.dev0/pathling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-17 01:21:07.000000 pathling-6.6.0.dev0/pathling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-17 01:21:08.010260 pathling-6.6.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 01:21:08.010260 pathling-6.6.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/tests/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-03-17 01:18:06.000000 pathling-6.6.0.dev0/tests/test_udfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.388430 pathling-7.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-23 02:06:36.388430 pathling-7.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.384430 pathling-7.0.0.dev0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.380430 pathling-7.0.0.dev0/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.384430 pathling-7.0.0.dev0/examples/data/bundles/
+-rw-r--r--   0 runner    (1001) docker     (127)    86431 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json
+-rw-r--r--   0 runner    (1001) docker     (127)    66676 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.384430 pathling-7.0.0.dev0/examples/data/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/data/resources/Condition.ndjson
+-rw-r--r--   0 runner    (1001) docker     (127)    29641 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/data/resources/Patient.ndjson
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/designation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/encode_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/encode_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1606 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/member_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1358 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/member_of_old.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/property_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4537 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/subsumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/subsumes_old.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1347 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1310 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/examples/translate_old.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.388430 pathling-7.0.0.dev0/pathling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 02:06:31.000000 pathling-7.0.0.dev0/pathling/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/datasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/fhir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/pathling/udfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.388430 pathling-7.0.0.dev0/pathling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-23 02:06:36.000000 pathling-7.0.0.dev0/pathling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 02:06:36.000000 pathling-7.0.0.dev0/pathling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:06:36.000000 pathling-7.0.0.dev0/pathling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 02:06:36.000000 pathling-7.0.0.dev0/pathling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 02:06:36.000000 pathling-7.0.0.dev0/pathling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 02:06:36.388430 pathling-7.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:06:36.388430 pathling-7.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-04-23 02:04:06.000000 pathling-7.0.0.dev0/tests/test_udfs.py
```

### Comparing `pathling-6.6.0.dev0/LICENSE` & `pathling-7.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/PKG-INFO` & `pathling-7.0.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pathling
-Version: 6.6.0.dev0
+Version: 7.0.0.dev0
 Summary: Python API for Pathling
 Home-page: https://github.com/aehrc/pathling
 Author: Australian e-Health Research Centre, CSIRO
 Author-email: ontoserver-support@csiro.au
 License: Apache License, version 2.0
 Keywords: pathling,fhir,analytics,spark,standards,terminology
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyspark<3.5.0,>=3.4.0
+Requires-Dist: pyspark<3.6.0,>=3.5.0
 Requires-Dist: deprecated>=1.2.13
 
 Python API for Pathling
 =======================
 
 This is the Python API for [Pathling](https://pathling.csiro.au). It provides a 
 set of tools that aid the use of FHIR terminology services and FHIR data within
```

### Comparing `pathling-6.6.0.dev0/README.md` & `pathling-7.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json` & `pathling-7.0.0.dev0/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json` & `pathling-7.0.0.dev0/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/data/resources/Condition.ndjson` & `pathling-7.0.0.dev0/examples/data/resources/Condition.ndjson`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/data/resources/Patient.ndjson` & `pathling-7.0.0.dev0/examples/data/resources/Patient.ndjson`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/designation.py` & `pathling-7.0.0.dev0/examples/designation.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/display.py` & `pathling-7.0.0.dev0/examples/display.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/encode_bundles.py` & `pathling-7.0.0.dev0/examples/encode_bundles.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/encode_resources.py` & `pathling-7.0.0.dev0/examples/encode_resources.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/member_of.py` & `pathling-7.0.0.dev0/examples/member_of.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/member_of_old.py` & `pathling-7.0.0.dev0/examples/member_of_old.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/property_of.py` & `pathling-7.0.0.dev0/examples/property_of.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/query.py` & `pathling-7.0.0.dev0/examples/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 WAREHOUSE_DIR = os.path.join(TEMP_DIR, "warehouse")
 NDJSON_DIR_2 = os.path.join(TEMP_DIR, "ndjson")
 
 # Configure Hive, so that we can test out the tables functionality.
 spark = (
     SparkSession.builder.config(
         "spark.jars.packages",
-        f"au.csiro.pathling:library-runtime:{__java_version__},io.delta:delta-core_2.12:2.2.0",
+        f"au.csiro.pathling:library-runtime:{__java_version__},io.delta:delta-spark_2.12:3.1.0",
     )
     .config(
         "spark.sql.extensions",
         "io.delta.sql.DeltaSparkSessionExtension",
     )
     .config(
         "spark.sql.catalog.spark_catalog",
```

### Comparing `pathling-6.6.0.dev0/examples/subsumes.py` & `pathling-7.0.0.dev0/examples/subsumes.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/subsumes_old.py` & `pathling-7.0.0.dev0/examples/subsumes_old.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/translate.py` & `pathling-7.0.0.dev0/examples/translate.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/examples/translate_old.py` & `pathling-7.0.0.dev0/examples/translate_old.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/__init__.py` & `pathling-7.0.0.dev0/pathling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from .coding import Coding
 from .context import PathlingContext, StorageType
 from .core import Expression
 from .datasource import DataSources, DataSource
-from .fhir import MimeType, FhirVersion
+from .fhir import MimeType, Version
 from .functions import to_coding, to_snomed_coding, to_ecl_value_set
 from .query import ExtractQuery, AggregateQuery
 from .udfs import (
     member_of,
     translate,
     subsumes,
     subsumed_by,
@@ -32,15 +32,15 @@
     Equivalence,
 )
 
 __all__ = [
     "PathlingContext",
     "StorageType",
     "MimeType",
-    "FhirVersion",
+    "Version",
     "Coding",
     "member_of",
     "translate",
     "subsumes",
     "subsumed_by",
     "property_of",
     "display",
```

### Comparing `pathling-6.6.0.dev0/pathling/coding.py` & `pathling-7.0.0.dev0/pathling/coding.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/context.py` & `pathling-7.0.0.dev0/pathling/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 
 from deprecated import deprecated
 from py4j.java_gateway import JavaObject
 from pyspark.sql import DataFrame, SparkSession, Column
 from typing import Optional, Sequence, TYPE_CHECKING
 
 from pathling._version import (
-    __version__,
     __java_version__,
     __scala_version__,
     __delta_version__,
     __hadoop_version__,
 )
 from pathling.coding import Coding
-from pathling.fhir import MimeType, FhirVersion
+from pathling.fhir import MimeType
 
 if TYPE_CHECKING:
     from .datasource import DataSources
 
 __all__ = ["PathlingContext"]
 
 EQ_EQUIVALENT = "equivalent"
@@ -63,15 +62,14 @@
         """
         return self._spark
 
     @classmethod
     def create(
         cls,
         spark: Optional[SparkSession] = None,
-        fhir_version: Optional[str] = FhirVersion.R4,
         max_nesting_level: Optional[int] = 3,
         enable_extensions: Optional[bool] = False,
         enabled_open_types: Optional[Sequence[str]] = (
             "boolean",
             "code",
             "date",
             "dateTime",
@@ -121,15 +119,14 @@
 
         If a SparkSession is provided, it needs to include the Pathling library API JAR on its
         classpath. You can get the path for the JAR (which is bundled with the Python package)
         using the `pathling.etc.find_jar` method.
 
         :param spark: a pre-configured :class:`SparkSession` instance, use this if you need to
                control the way that the session is set up
-        :param fhir_version: the version of FHIR to use, defaults to R4
         :param max_nesting_level: controls the maximum depth of nested element data that is encoded
                upon import. This affects certain elements within FHIR resources that contain
                recursive references, e.g. `QuestionnaireResponse.item
                <https://hl7.org/fhir/R4/questionnaireresponse.html>`_.
         :param enable_extensions: enables support for FHIR extensions
         :param enabled_open_types: the list of types that are encoded within open types,
                such as extensions. This default list was taken from the data types that are common
@@ -183,39 +180,33 @@
         """
 
         def _new_spark_session():
             spark_builder = (
                 SparkSession.builder.config(
                     "spark.jars.packages",
                     f"au.csiro.pathling:library-runtime:{__java_version__},"
-                    f"io.delta:delta-core_{__scala_version__}:{__delta_version__},"
+                    f"io.delta:delta-spark_{__scala_version__}:{__delta_version__},"
                     f"org.apache.hadoop:hadoop-aws:{__hadoop_version__}",
                 )
                 .config(
                     "spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension"
                 )
                 .config(
                     "spark.sql.catalog.spark_catalog",
                     "org.apache.spark.sql.delta.catalog.DeltaCatalog",
                 )
             )
-            if __version__.endswith(".dev"):
-                spark_builder = spark_builder.config(
-                    "spark.jars.repositories",
-                    "https://oss.sonatype.org/content/repositories/snapshots",
-                )
             return spark_builder.getOrCreate()
 
         spark = spark or SparkSession.getActiveSession() or _new_spark_session()
         jvm = spark._jvm
 
         # Build an encoders configuration object from the provided parameters.
         encoders_config = (
             jvm.au.csiro.pathling.config.EncodingConfiguration.builder()
-            .fhirVersion(fhir_version)
             .maxNestingLevel(max_nesting_level)
             .enableExtensions(enable_extensions)
             .openTypes(jvm.java.util.HashSet(enabled_open_types))
             .build()
         )
 
         # Build a terminology client configuration object from the provided parameters.
```

### Comparing `pathling-6.6.0.dev0/pathling/core.py` & `pathling-7.0.0.dev0/pathling/core.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/datasink.py` & `pathling-7.0.0.dev0/pathling/datasink.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/datasource.py` & `pathling-7.0.0.dev0/pathling/datasource.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/fhir.py` & `pathling-7.0.0.dev0/pathling/fhir.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,13 @@
     Constants for FHIR encoding mime types.
     """
 
     FHIR_JSON: str = "application/fhir+json"
     FHIR_XML: str = "application/fhir+xml"
 
 
-class FhirVersion:
+class Version:
     """
     Constants for FHIR versions.
     """
 
-    R4: str = "4.0.1"
-    STU3: str = "3.0.2"
+    R4: str = "R4"
```

### Comparing `pathling-6.6.0.dev0/pathling/functions.py` & `pathling-7.0.0.dev0/pathling/functions.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/query.py` & `pathling-7.0.0.dev0/pathling/query.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling/udfs.py` & `pathling-7.0.0.dev0/pathling/udfs.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/pathling.egg-info/PKG-INFO` & `pathling-7.0.0.dev0/pathling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pathling
-Version: 6.6.0.dev0
+Version: 7.0.0.dev0
 Summary: Python API for Pathling
 Home-page: https://github.com/aehrc/pathling
 Author: Australian e-Health Research Centre, CSIRO
 Author-email: ontoserver-support@csiro.au
 License: Apache License, version 2.0
 Keywords: pathling,fhir,analytics,spark,standards,terminology
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyspark<3.5.0,>=3.4.0
+Requires-Dist: pyspark<3.6.0,>=3.5.0
 Requires-Dist: deprecated>=1.2.13
 
 Python API for Pathling
 =======================
 
 This is the Python API for [Pathling](https://pathling.csiro.au). It provides a 
 set of tools that aid the use of FHIR terminology services and FHIR data within
```

### Comparing `pathling-6.6.0.dev0/pathling.egg-info/SOURCES.txt` & `pathling-7.0.0.dev0/pathling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/setup.py` & `pathling-7.0.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,22 +52,21 @@
     author="Australian e-Health Research Centre, CSIRO",
     author_email="ontoserver-support@csiro.au",
     url="https://github.com/aehrc/pathling",
     keywords=["pathling", "fhir", "analytics", "spark", "standards", "terminology"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     license="Apache License, version 2.0",
-    python_requires=">=3.7",
-    install_requires=["pyspark>=3.4.0,<3.5.0", "deprecated>=1.2.13"],
+    python_requires=">=3.8",
+    install_requires=["pyspark>=3.5.0,<3.6.0", "deprecated>=1.2.13"],
     include_package_data=True,
     data_files=[
         ("share/pathling/examples", glob.glob("examples/*.py")),
         (
             "share/pathling/examples/data/resources",
             glob.glob("examples/data/resources/*.ndjson"),
         ),
```

### Comparing `pathling-6.6.0.dev0/tests/test_datasource.py` & `pathling-7.0.0.dev0/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/tests/test_encoders.py` & `pathling-7.0.0.dev0/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/tests/test_functions.py` & `pathling-7.0.0.dev0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/tests/test_query.py` & `pathling-7.0.0.dev0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pathling-6.6.0.dev0/tests/test_udfs.py` & `pathling-7.0.0.dev0/tests/test_udfs.py`

 * *Files identical despite different names*

