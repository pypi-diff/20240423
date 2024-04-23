# Comparing `tmp/curve_dao-0.0.2.tar.gz` & `tmp/curve_dao-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curve_dao-0.0.2.tar", last modified: Tue Apr 23 17:02:07 2024, max compression
+gzip compressed data, was "curve_dao-0.0.3.tar", last modified: Tue Apr 23 17:05:19 2024, max compression
```

## Comparing `curve_dao-0.0.2.tar` & `curve_dao-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:02:07.764166 curve_dao-0.0.2/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1959 2024-04-23 17:02:07.763828 curve_dao-0.0.2/PKG-INFO
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1060 2024-04-23 15:39:50.000000 curve_dao-0.0.2/README.md
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:02:07.760608 curve_dao-0.0.2/curve_dao/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      593 2024-04-23 16:49:54.000000 curve_dao-0.0.2/curve_dao/__init__.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1415 2024-04-23 16:43:33.000000 curve_dao-0.0.2/curve_dao/addresses.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      859 2024-04-23 15:20:16.000000 curve_dao-0.0.2/curve_dao/ipfs.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1277 2024-04-23 15:20:16.000000 curve_dao-0.0.2/curve_dao/simulate.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1470 2024-04-23 15:20:16.000000 curve_dao-0.0.2/curve_dao/vote_utils.py
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:02:07.763496 curve_dao-0.0.2/curve_dao.egg-info/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1959 2024-04-23 17:02:07.000000 curve_dao-0.0.2/curve_dao.egg-info/PKG-INFO
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      297 2024-04-23 17:02:07.000000 curve_dao-0.0.2/curve_dao.egg-info/SOURCES.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)        1 2024-04-23 17:02:07.000000 curve_dao-0.0.2/curve_dao.egg-info/dependency_links.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       45 2024-04-23 17:02:07.000000 curve_dao-0.0.2/curve_dao.egg-info/requires.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       10 2024-04-23 17:02:07.000000 curve_dao-0.0.2/curve_dao.egg-info/top_level.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1190 2024-04-23 17:01:25.000000 curve_dao-0.0.2/pyproject.toml
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       38 2024-04-23 17:02:07.764237 curve_dao-0.0.2/setup.cfg
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:05:19.483233 curve_dao-0.0.3/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1959 2024-04-23 17:05:19.482936 curve_dao-0.0.3/PKG-INFO
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1060 2024-04-23 15:39:50.000000 curve_dao-0.0.3/README.md
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:05:19.479518 curve_dao-0.0.3/curve_dao/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      593 2024-04-23 16:49:54.000000 curve_dao-0.0.3/curve_dao/__init__.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1415 2024-04-23 16:43:33.000000 curve_dao-0.0.3/curve_dao/addresses.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      859 2024-04-23 15:20:16.000000 curve_dao-0.0.3/curve_dao/ipfs.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1277 2024-04-23 15:20:16.000000 curve_dao-0.0.3/curve_dao/simulate.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1470 2024-04-23 15:20:16.000000 curve_dao-0.0.3/curve_dao/vote_utils.py
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:05:19.482582 curve_dao-0.0.3/curve_dao.egg-info/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1959 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/PKG-INFO
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      297 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/SOURCES.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)        1 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/dependency_links.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       45 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/requires.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       10 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/top_level.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1192 2024-04-23 17:05:10.000000 curve_dao-0.0.3/pyproject.toml
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       38 2024-04-23 17:05:19.483288 curve_dao-0.0.3/setup.cfg
```

### Comparing `curve_dao-0.0.2/PKG-INFO` & `curve_dao-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curve-dao
-Version: 0.0.2
+Version: 0.0.3
 Summary: DAO governance tools for CurveDAO.
 Author-email: FiddyResearch <fiddyresearch@gmail.com>
 Maintainer-email: FiddyResearch <fiddyresearch@gmail.com>
 License: AGPL-3.0-only License
 Project-URL: Homepage, https://pypi.org/project/curve-dao/
 Project-URL: GitHub, https://github.com/bout3fiddy/curve-dao
 Project-URL: Changelog, https://github.com/bout3fiddy/curve-dao/blob/main/CHANGELOG.md
```

### Comparing `curve_dao-0.0.2/README.md` & `curve_dao-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.2/curve_dao/__init__.py` & `curve_dao-0.0.3/curve_dao/__init__.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.2/curve_dao/addresses.py` & `curve_dao-0.0.3/curve_dao/addresses.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.2/curve_dao/ipfs.py` & `curve_dao-0.0.3/curve_dao/ipfs.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.2/curve_dao/simulate.py` & `curve_dao-0.0.3/curve_dao/simulate.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.2/curve_dao/vote_utils.py` & `curve_dao-0.0.3/curve_dao/vote_utils.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.2/curve_dao.egg-info/PKG-INFO` & `curve_dao-0.0.3/curve_dao.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curve-dao
-Version: 0.0.2
+Version: 0.0.3
 Summary: DAO governance tools for CurveDAO.
 Author-email: FiddyResearch <fiddyresearch@gmail.com>
 Maintainer-email: FiddyResearch <fiddyresearch@gmail.com>
 License: AGPL-3.0-only License
 Project-URL: Homepage, https://pypi.org/project/curve-dao/
 Project-URL: GitHub, https://github.com/bout3fiddy/curve-dao
 Project-URL: Changelog, https://github.com/bout3fiddy/curve-dao/blob/main/CHANGELOG.md
```

### Comparing `curve_dao-0.0.2/pyproject.toml` & `curve_dao-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curve-dao"
-version = "0.0.2"
+version = "0.0.3"
 description = "DAO governance tools for CurveDAO."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.10"
 license = {text = "AGPL-3.0-only License"}
 keywords = ["ethereum", "smart-contracts", "evm", "vyper", "curve-finance", "dao", "defi"]
 authors = [
     {name = "FiddyResearch", email = "fiddyresearch@gmail.com"},
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 # Requirements
 dependencies = [
     "titanoboa >= 0.1.9",
-    "py-evm<0.10.0",
+    "py-evm < 0.10.0",
     "requests",
     "rich",
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
```

