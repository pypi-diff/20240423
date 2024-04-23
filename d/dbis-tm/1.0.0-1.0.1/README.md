# Comparing `tmp/dbis_tm-1.0.0.tar.gz` & `tmp/dbis_tm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis_tm-1.0.0.tar", last modified: Tue Apr 16 11:31:06 2024, max compression
+gzip compressed data, was "dbis_tm-1.0.1.tar", last modified: Tue Apr 23 13:15:22 2024, max compression
```

## Comparing `dbis_tm-1.0.0.tar` & `dbis_tm-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      704 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-04-16 11:15:29.000000 dbis_tm-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/src/dbis_tm/
--rw-rw-rw-   0 root         (0) root         (0)    40325 2024-04-14 14:39:41.000000 dbis_tm-1.0.0/src/dbis_tm/Generate.py
--rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-09 10:37:55.000000 dbis_tm-1.0.0/src/dbis_tm/Generate_Tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    24508 2024-04-09 10:37:55.000000 dbis_tm-1.0.0/src/dbis_tm/Solution_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    12780 2024-04-09 12:17:44.000000 dbis_tm-1.0.0/src/dbis_tm/TM.py
--rw-rw-rw-   0 root         (0) root         (0)    13595 2024-04-09 10:42:22.000000 dbis_tm-1.0.0/src/dbis_tm/TMCheck.py
--rw-rw-rw-   0 root         (0) root         (0)    25050 2024-04-09 10:42:22.000000 dbis_tm-1.0.0/src/dbis_tm/TMSolver.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-08 12:03:38.000000 dbis_tm-1.0.0/src/dbis_tm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/src/dbis_tm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      704 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5181 2024-04-09 10:53:52.000000 dbis_tm-1.0.0/tests/test_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     6708 2024-04-09 10:53:52.000000 dbis_tm-1.0.0/tests/test_perfomance.py
--rw-rw-rw-   0 root         (0) root         (0)    15382 2024-04-09 10:53:52.000000 dbis_tm-1.0.0/tests/test_ub10Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)    36807 2024-04-09 12:17:44.000000 dbis_tm-1.0.0/tests/test_ub10TM.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:15:22.536826 dbis_tm-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-04-23 13:15:22.536826 dbis_tm-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 13:15:22.536826 dbis_tm-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:15:22.532826 dbis_tm-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:15:22.532826 dbis_tm-1.0.1/src/dbis_tm/
+-rw-rw-rw-   0 root         (0) root         (0)    40325 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/src/dbis_tm/Generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/src/dbis_tm/Generate_Tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    24508 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/src/dbis_tm/Solution_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    12780 2024-04-09 12:17:44.000000 dbis_tm-1.0.1/src/dbis_tm/TM.py
+-rw-rw-rw-   0 root         (0) root         (0)    13595 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/src/dbis_tm/TMCheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    25050 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/src/dbis_tm/TMSolver.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-08 12:03:38.000000 dbis_tm-1.0.1/src/dbis_tm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:15:22.536826 dbis_tm-1.0.1/src/dbis_tm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-04-23 13:15:22.000000 dbis_tm-1.0.1/src/dbis_tm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-23 13:15:22.000000 dbis_tm-1.0.1/src/dbis_tm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 13:15:22.000000 dbis_tm-1.0.1/src/dbis_tm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-23 13:15:22.000000 dbis_tm-1.0.1/src/dbis_tm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 13:15:22.000000 dbis_tm-1.0.1/src/dbis_tm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:15:22.536826 dbis_tm-1.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5181 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/tests/test_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6708 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/tests/test_perfomance.py
+-rw-rw-rw-   0 root         (0) root         (0)    15382 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/tests/test_ub10Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)    36807 2024-04-23 13:10:59.000000 dbis_tm-1.0.1/tests/test_ub10TM.py
```

### Comparing `dbis_tm-1.0.0/PKG-INFO` & `dbis_tm-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbis-tm
-Version: 1.0.0
+Version: 1.0.1
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-tm
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: graphviz~=0.20.1
-Requires-Dist: dbis-exc-manager~=0.3
+Requires-Dist: dbis-exc-manager~=1.0
 Provides-Extra: test
 Requires-Dist: black==23.12.1; extra == "test"
 Provides-Extra: build
 Requires-Dist: twine==4.*; extra == "build"
 Requires-Dist: build==1.*; extra == "build"
```

### Comparing `dbis_tm-1.0.0/pyproject.toml` & `dbis_tm-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name="dbis-tm"
-version='1.0.0'
+version='1.0.1'
 description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 
 authors = [
 	{ name = "DBIS i5 RWTH Aachen", email = "dbis-vl@dbis.rwth-aachen.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11"
 ]
 
 dependencies = [
 	"graphviz~=0.20.1",
-	"dbis-exc-manager~=0.3"
+	"dbis-exc-manager~=1.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "black==23.12.1"
 ]
 build = [
```

### Comparing `dbis_tm-1.0.0/src/dbis_tm/Generate.py` & `dbis_tm-1.0.1/src/dbis_tm/Generate.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/src/dbis_tm/Generate_Tasks.py` & `dbis_tm-1.0.1/src/dbis_tm/Generate_Tasks.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/src/dbis_tm/Solution_generator.py` & `dbis_tm-1.0.1/src/dbis_tm/Solution_generator.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/src/dbis_tm/TM.py` & `dbis_tm-1.0.1/src/dbis_tm/TM.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/src/dbis_tm/TMCheck.py` & `dbis_tm-1.0.1/src/dbis_tm/TMCheck.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/src/dbis_tm/TMSolver.py` & `dbis_tm-1.0.1/src/dbis_tm/TMSolver.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/src/dbis_tm.egg-info/PKG-INFO` & `dbis_tm-1.0.1/src/dbis_tm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbis-tm
-Version: 1.0.0
+Version: 1.0.1
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-tm
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: graphviz~=0.20.1
-Requires-Dist: dbis-exc-manager~=0.3
+Requires-Dist: dbis-exc-manager~=1.0
 Provides-Extra: test
 Requires-Dist: black==23.12.1; extra == "test"
 Provides-Extra: build
 Requires-Dist: twine==4.*; extra == "build"
 Requires-Dist: build==1.*; extra == "build"
```

### Comparing `dbis_tm-1.0.0/tests/test_generator.py` & `dbis_tm-1.0.1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/tests/test_perfomance.py` & `dbis_tm-1.0.1/tests/test_perfomance.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/tests/test_ub10Scorer.py` & `dbis_tm-1.0.1/tests/test_ub10Scorer.py`

 * *Files identical despite different names*

### Comparing `dbis_tm-1.0.0/tests/test_ub10TM.py` & `dbis_tm-1.0.1/tests/test_ub10TM.py`

 * *Files identical despite different names*

