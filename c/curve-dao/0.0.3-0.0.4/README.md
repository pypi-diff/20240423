# Comparing `tmp/curve_dao-0.0.3.tar.gz` & `tmp/curve_dao-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curve_dao-0.0.3.tar", last modified: Tue Apr 23 17:05:19 2024, max compression
+gzip compressed data, was "curve_dao-0.0.4.tar", last modified: Tue Apr 23 17:15:06 2024, max compression
```

## Comparing `curve_dao-0.0.3.tar` & `curve_dao-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:05:19.483233 curve_dao-0.0.3/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1959 2024-04-23 17:05:19.482936 curve_dao-0.0.3/PKG-INFO
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1060 2024-04-23 15:39:50.000000 curve_dao-0.0.3/README.md
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:05:19.479518 curve_dao-0.0.3/curve_dao/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      593 2024-04-23 16:49:54.000000 curve_dao-0.0.3/curve_dao/__init__.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1415 2024-04-23 16:43:33.000000 curve_dao-0.0.3/curve_dao/addresses.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      859 2024-04-23 15:20:16.000000 curve_dao-0.0.3/curve_dao/ipfs.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1277 2024-04-23 15:20:16.000000 curve_dao-0.0.3/curve_dao/simulate.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1470 2024-04-23 15:20:16.000000 curve_dao-0.0.3/curve_dao/vote_utils.py
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:05:19.482582 curve_dao-0.0.3/curve_dao.egg-info/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1959 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/PKG-INFO
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      297 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/SOURCES.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)        1 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/dependency_links.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       45 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/requires.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       10 2024-04-23 17:05:19.000000 curve_dao-0.0.3/curve_dao.egg-info/top_level.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1192 2024-04-23 17:05:10.000000 curve_dao-0.0.3/pyproject.toml
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       38 2024-04-23 17:05:19.483288 curve_dao-0.0.3/setup.cfg
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:15:06.466174 curve_dao-0.0.4/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1933 2024-04-23 17:15:06.465969 curve_dao-0.0.4/PKG-INFO
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1060 2024-04-23 15:39:50.000000 curve_dao-0.0.4/README.md
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:15:06.462703 curve_dao-0.0.4/curve_dao/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      593 2024-04-23 16:49:54.000000 curve_dao-0.0.4/curve_dao/__init__.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1415 2024-04-23 16:43:33.000000 curve_dao-0.0.4/curve_dao/addresses.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      859 2024-04-23 15:20:16.000000 curve_dao-0.0.4/curve_dao/ipfs.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1277 2024-04-23 15:20:16.000000 curve_dao-0.0.4/curve_dao/simulate.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1470 2024-04-23 15:20:16.000000 curve_dao-0.0.4/curve_dao/vote_utils.py
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 17:15:06.465746 curve_dao-0.0.4/curve_dao.egg-info/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1933 2024-04-23 17:15:06.000000 curve_dao-0.0.4/curve_dao.egg-info/PKG-INFO
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      297 2024-04-23 17:15:06.000000 curve_dao-0.0.4/curve_dao.egg-info/SOURCES.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)        1 2024-04-23 17:15:06.000000 curve_dao-0.0.4/curve_dao.egg-info/dependency_links.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       34 2024-04-23 17:15:06.000000 curve_dao-0.0.4/curve_dao.egg-info/requires.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       10 2024-04-23 17:15:06.000000 curve_dao-0.0.4/curve_dao.egg-info/top_level.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1172 2024-04-23 17:14:57.000000 curve_dao-0.0.4/pyproject.toml
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       38 2024-04-23 17:15:06.466319 curve_dao-0.0.4/setup.cfg
```

### Comparing `curve_dao-0.0.3/PKG-INFO` & `curve_dao-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: curve-dao
-Version: 0.0.3
+Version: 0.0.4
 Summary: DAO governance tools for CurveDAO.
 Author-email: FiddyResearch <fiddyresearch@gmail.com>
 Maintainer-email: FiddyResearch <fiddyresearch@gmail.com>
 License: AGPL-3.0-only License
 Project-URL: Homepage, https://pypi.org/project/curve-dao/
 Project-URL: GitHub, https://github.com/bout3fiddy/curve-dao
 Project-URL: Changelog, https://github.com/bout3fiddy/curve-dao/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/bout3fiddy/curve-dao/issues
 Keywords: ethereum,smart-contracts,evm,vyper,curve-finance,dao,defi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: titanoboa>=0.1.9
-Requires-Dist: py-evm<0.10.0
+Requires-Dist: titanoboa>=0.1.10b1
 Requires-Dist: requests
 Requires-Dist: rich
 
 # Curve DAO Operations
 
 This repository contains tools, written in python, for Curve DAO operations. The goal is to provide a simple command-line interface that allows veCRV holders to create and decode on-chain executable proposals, and simple scripts to produce analytics on governance in the Curve DAO.
```

### Comparing `curve_dao-0.0.3/README.md` & `curve_dao-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.3/curve_dao/__init__.py` & `curve_dao-0.0.4/curve_dao/__init__.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.3/curve_dao/addresses.py` & `curve_dao-0.0.4/curve_dao/addresses.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.3/curve_dao/ipfs.py` & `curve_dao-0.0.4/curve_dao/ipfs.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.3/curve_dao/simulate.py` & `curve_dao-0.0.4/curve_dao/simulate.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.3/curve_dao/vote_utils.py` & `curve_dao-0.0.4/curve_dao/vote_utils.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.3/curve_dao.egg-info/PKG-INFO` & `curve_dao-0.0.4/curve_dao.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: curve-dao
-Version: 0.0.3
+Version: 0.0.4
 Summary: DAO governance tools for CurveDAO.
 Author-email: FiddyResearch <fiddyresearch@gmail.com>
 Maintainer-email: FiddyResearch <fiddyresearch@gmail.com>
 License: AGPL-3.0-only License
 Project-URL: Homepage, https://pypi.org/project/curve-dao/
 Project-URL: GitHub, https://github.com/bout3fiddy/curve-dao
 Project-URL: Changelog, https://github.com/bout3fiddy/curve-dao/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/bout3fiddy/curve-dao/issues
 Keywords: ethereum,smart-contracts,evm,vyper,curve-finance,dao,defi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: titanoboa>=0.1.9
-Requires-Dist: py-evm<0.10.0
+Requires-Dist: titanoboa>=0.1.10b1
 Requires-Dist: requests
 Requires-Dist: rich
 
 # Curve DAO Operations
 
 This repository contains tools, written in python, for Curve DAO operations. The goal is to provide a simple command-line interface that allows veCRV holders to create and decode on-chain executable proposals, and simple scripts to produce analytics on governance in the Curve DAO.
```

### Comparing `curve_dao-0.0.3/pyproject.toml` & `curve_dao-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curve-dao"
-version = "0.0.3"
+version = "0.0.4"
 description = "DAO governance tools for CurveDAO."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.10"
 license = {text = "AGPL-3.0-only License"}
 keywords = ["ethereum", "smart-contracts", "evm", "vyper", "curve-finance", "dao", "defi"]
 authors = [
     {name = "FiddyResearch", email = "fiddyresearch@gmail.com"},
@@ -16,16 +16,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 # Requirements
 dependencies = [
-    "titanoboa >= 0.1.9",
-    "py-evm < 0.10.0",
+    "titanoboa >= 0.1.10b1",
     "requests",
     "rich",
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
```

