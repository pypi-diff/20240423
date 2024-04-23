# Comparing `tmp/sonar_dummy_python_oss-0.1.0.93.tar.gz` & `tmp/sonar_dummy_python_oss-0.1.0a75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonar_dummy_python_oss-0.1.0.93.tar", max compression
+gzip compressed data, was "sonar_dummy_python_oss-0.1.0a75.tar", max compression
```

## Comparing `sonar_dummy_python_oss-0.1.0.93.tar` & `sonar_dummy_python_oss-0.1.0a75.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7652 2024-04-22 16:27:43.756991 sonar_dummy_python_oss-0.1.0.93/LICENSE
--rw-r--r--   0        0        0       77 2024-04-22 16:27:43.756991 sonar_dummy_python_oss-0.1.0.93/README.md
--rw-r--r--   0        0        0     1281 2024-04-22 16:27:51.097146 sonar_dummy_python_oss-0.1.0.93/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 16:27:43.756991 sonar_dummy_python_oss-0.1.0.93/src/sonar_dummy_python_oss/__init__.py
--rw-r--r--   0        0        0       43 2024-04-22 16:27:43.756991 sonar_dummy_python_oss-0.1.0.93/src/sonar_dummy_python_oss/example.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 sonar_dummy_python_oss-0.1.0.93/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-03-27 13:19:33.936545 sonar_dummy_python_oss-0.1.0a75/LICENSE
+-rw-r--r--   0        0        0       76 2024-03-27 13:19:33.936545 sonar_dummy_python_oss-0.1.0a75/README.md
+-rw-r--r--   0        0        0     1282 2024-03-27 13:19:44.228777 sonar_dummy_python_oss-0.1.0a75/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-27 13:19:33.936545 sonar_dummy_python_oss-0.1.0a75/src/sonar_dummy_python_oss/__init__.py
+-rw-r--r--   0        0        0       43 2024-03-27 13:19:33.936545 sonar_dummy_python_oss-0.1.0a75/src/sonar_dummy_python_oss/example.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 sonar_dummy_python_oss-0.1.0a75/PKG-INFO
```

### Comparing `sonar_dummy_python_oss-0.1.0.93/LICENSE` & `sonar_dummy_python_oss-0.1.0a75/LICENSE`

 * *Files identical despite different names*

### Comparing `sonar_dummy_python_oss-0.1.0.93/pyproject.toml` & `sonar_dummy_python_oss-0.1.0a75/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 authors = ['Jayadeep Kinavoor Madam <jayadeep.kinavoormadam@sonarsource.com>']
 classifiers = ['Environment :: Console', 'Intended Audience :: Developers', 'Operating System :: OS Independent', 'Programming Language :: Python', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'Programming Language :: Python :: 3.12', 'Topic :: Software Development :: Quality Assurance']
 description = 'A sample python project used for testing purposes'
 keywords = ['sonar', 'sonar-dummy']
 license = 'LGPL-3.0-only'
 name = 'sonar_dummy_python_oss'
 readme = 'README.md'
-version = '0.1.0.93'
+version = '0.1.0a.75'
 
 [tool.poetry.dependencies]
 python = '>=3.8'
 
 [[tool.poetry.packages]]
 from = 'src'
 include = 'sonar_dummy_python_oss'
```

### Comparing `sonar_dummy_python_oss-0.1.0.93/PKG-INFO` & `sonar_dummy_python_oss-0.1.0a75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonar_dummy_python_oss
-Version: 0.1.0.93
+Version: 0.1.0a75
 Summary: A sample python project used for testing purposes
 License: LGPL-3.0-only
 Keywords: sonar,sonar-dummy
 Author: Jayadeep Kinavoor Madam
 Author-email: jayadeep.kinavoormadam@sonarsource.com
 Requires-Python: >=3.8
 Classifier: Environment :: Console
@@ -19,10 +19,9 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/markdown
 
 # sonar-dummy-python-oss
-
 A sample python project used for testing purposes.
```

