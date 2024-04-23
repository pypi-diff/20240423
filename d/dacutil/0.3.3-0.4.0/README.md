# Comparing `tmp/dacutil-0.3.3.tar.gz` & `tmp/dacutil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dacutil-0.3.3.tar", max compression
+gzip compressed data, was "dacutil-0.4.0.tar", max compression
```

## Comparing `dacutil-0.3.3.tar` & `dacutil-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      723 2024-02-09 09:12:52.124549 dacutil-0.3.3/README.md
--rw-r--r--   0        0        0      456 2024-03-19 04:31:32.012959 dacutil-0.3.3/dacutil/__init__.py
--rw-r--r--   0        0        0     4985 2024-02-07 08:23:14.673797 dacutil-0.3.3/dacutil/addict.py
--rw-r--r--   0        0        0     4334 2024-03-19 06:02:26.465638 dacutil-0.3.3/dacutil/config.py
--rw-r--r--   0        0        0     4881 2024-03-19 04:49:01.770472 dacutil-0.3.3/dacutil/crypt.py
--rw-r--r--   0        0        0     2659 2023-12-22 07:20:50.710357 dacutil-0.3.3/dacutil/dateutil.py
--rw-r--r--   0        0        0     1537 2024-03-05 06:12:40.996347 dacutil-0.3.3/dacutil/strutil.py
--rw-r--r--   0        0        0     1256 2023-12-22 05:44:36.724417 dacutil-0.3.3/dacutil/thai_mod11.py
--rw-r--r--   0        0        0     1329 2023-12-22 05:44:20.003573 dacutil-0.3.3/dacutil/worker.py
--rw-r--r--   0        0        0      516 2024-03-19 04:46:44.925838 dacutil-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 dacutil-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      723 2024-02-09 09:12:52.124549 dacutil-0.4.0/README.md
+-rw-r--r--   0        0        0      456 2024-03-19 04:31:32.012959 dacutil-0.4.0/dacutil/__init__.py
+-rw-r--r--   0        0        0     4985 2024-02-07 08:23:14.673797 dacutil-0.4.0/dacutil/addict.py
+-rw-r--r--   0        0        0     4334 2024-03-19 06:02:26.465638 dacutil-0.4.0/dacutil/config.py
+-rw-r--r--   0        0        0     4881 2024-03-19 04:49:01.770472 dacutil-0.4.0/dacutil/crypt.py
+-rw-r--r--   0        0        0     2659 2023-12-22 07:20:50.710357 dacutil-0.4.0/dacutil/dateutil.py
+-rw-r--r--   0        0        0     1305 2024-04-23 05:11:48.225404 dacutil-0.4.0/dacutil/pyencryption.py
+-rw-r--r--   0        0        0     1537 2024-03-05 06:12:40.996347 dacutil-0.4.0/dacutil/strutil.py
+-rw-r--r--   0        0        0     1256 2023-12-22 05:44:36.724417 dacutil-0.4.0/dacutil/thai_mod11.py
+-rw-r--r--   0        0        0     1329 2023-12-22 05:44:20.003573 dacutil-0.4.0/dacutil/worker.py
+-rw-r--r--   0        0        0      542 2024-04-23 05:15:18.541452 dacutil-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 dacutil-0.4.0/PKG-INFO
```

### Comparing `dacutil-0.3.3/README.md` & `dacutil-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/addict.py` & `dacutil-0.4.0/dacutil/addict.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/config.py` & `dacutil-0.4.0/dacutil/config.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/crypt.py` & `dacutil-0.4.0/dacutil/crypt.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/dateutil.py` & `dacutil-0.4.0/dacutil/dateutil.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/strutil.py` & `dacutil-0.4.0/dacutil/strutil.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/thai_mod11.py` & `dacutil-0.4.0/dacutil/thai_mod11.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/dacutil/worker.py` & `dacutil-0.4.0/dacutil/worker.py`

 * *Files identical despite different names*

### Comparing `dacutil-0.3.3/pyproject.toml` & `dacutil-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dacutil"
-version = "0.3.3"
+version = "0.4.0"
 description = "For Data Analytic"
 authors = ["Attapon Thanawong <attapon_srem@hotmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
@@ -12,14 +12,15 @@
 pyarrow = ">=14.0.0"
 requests = ">=2.31.0"
 configobj = ">=5.0.0"
 pyyaml = ">=6.0.0"
 tomli = ">=2.0.0"
 cryptography = ">=41.0.0"
 pyrage = ">=1.1.0"
+pycryptodome = ">=3.17.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `dacutil-0.3.3/PKG-INFO` & `dacutil-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dacutil
-Version: 0.3.3
+Version: 0.4.0
 Summary: For Data Analytic
 Author: Attapon Thanawong
 Author-email: attapon_srem@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: configobj (>=5.0.0)
 Requires-Dist: cryptography (>=41.0.0)
 Requires-Dist: pandas (>=2.1.0)
 Requires-Dist: pyarrow (>=14.0.0)
+Requires-Dist: pycryptodome (>=3.17.0)
 Requires-Dist: pyrage (>=1.1.0)
 Requires-Dist: pyyaml (>=6.0.0)
 Requires-Dist: requests (>=2.31.0)
 Requires-Dist: tomli (>=2.0.0)
 Description-Content-Type: text/markdown
 
 # Data Analytic Utils
```

