# Comparing `tmp/slalom_tapdance-0.9.10.dev51.tar.gz` & `tmp/slalom_tapdance-0.9.10.dev53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-0.9.10.dev51.tar", max compression
+gzip compressed data, was "slalom_tapdance-0.9.10.dev53.tar", max compression
```

## Comparing `slalom_tapdance-0.9.10.dev51.tar` & `slalom_tapdance-0.9.10.dev53.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-04-18 21:22:03.867293 slalom_tapdance-0.9.10.dev51/LICENSE
--rw-r--r--   0        0        0     1169 2024-04-18 21:22:18.227207 slalom_tapdance-0.9.10.dev51/pyproject.toml
--rw-r--r--   0        0        0      288 2024-04-18 21:22:03.871292 slalom_tapdance-0.9.10.dev51/tapdance/__init__.py
--rw-r--r--   0        0        0      696 2024-04-18 21:22:03.871292 slalom_tapdance-0.9.10.dev51/tapdance/cli.py
--rw-r--r--   0        0        0    15304 2024-04-18 21:22:03.875292 slalom_tapdance-0.9.10.dev51/tapdance/config.py
--rw-r--r--   0        0        0    13533 2024-04-18 21:22:03.875292 slalom_tapdance-0.9.10.dev51/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-04-18 21:22:03.875292 slalom_tapdance-0.9.10.dev51/tapdance/install_helper.py
--rw-r--r--   0        0        0    37111 2024-04-18 21:22:03.875292 slalom_tapdance-0.9.10.dev51/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-04-18 21:22:03.875292 slalom_tapdance-0.9.10.dev51/tapdance/states.py
--rw-r--r--   0        0        0    11787 2024-04-18 21:22:03.875292 slalom_tapdance-0.9.10.dev51/tapdance/syncs.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev51/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-23 20:32:51.193271 slalom_tapdance-0.9.10.dev53/LICENSE
+-rw-r--r--   0        0        0     1162 2024-04-23 20:33:09.929468 slalom_tapdance-0.9.10.dev53/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/cli.py
+-rw-r--r--   0        0        0    15304 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/config.py
+-rw-r--r--   0        0        0    13533 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/install_helper.py
+-rw-r--r--   0        0        0    37111 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/states.py
+-rw-r--r--   0        0        0    11787 2024-04-23 20:32:51.197271 slalom_tapdance-0.9.10.dev53/tapdance/syncs.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev53/PKG-INFO
```

### Comparing `slalom_tapdance-0.9.10.dev51/LICENSE` & `slalom_tapdance-0.9.10.dev53/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/pyproject.toml` & `slalom_tapdance-0.9.10.dev53/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "0.9.10-dev.51"
+version = "0.9.10-dev.53"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["AJ Steers <aj.steers@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
 
@@ -31,13 +31,13 @@
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 aws = ["boto3", "s3fs"]
 azure = ["azure-storage-blob", "azure-storage-file-datalake"]
 
 [tool.poetry.scripts]
-slalom-tapdance = "tapdance.cli:main"
+tapdance = "tapdance.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/cli.py` & `slalom_tapdance-0.9.10.dev53/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/config.py` & `slalom_tapdance-0.9.10.dev53/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/docker.py` & `slalom_tapdance-0.9.10.dev53/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/install_helper.py` & `slalom_tapdance-0.9.10.dev53/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/plans.py` & `slalom_tapdance-0.9.10.dev53/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/states.py` & `slalom_tapdance-0.9.10.dev53/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/tapdance/syncs.py` & `slalom_tapdance-0.9.10.dev53/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev51/PKG-INFO` & `slalom_tapdance-0.9.10.dev53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 0.9.10.dev51
+Version: 0.9.10.dev53
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: AJ Steers
 Author-email: aj.steers@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

