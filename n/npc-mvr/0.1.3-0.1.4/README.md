# Comparing `tmp/npc-mvr-0.1.3.tar.gz` & `tmp/npc_mvr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc-mvr-0.1.3.tar", last modified: Tue Mar 26 16:39:19 2024, max compression
+gzip compressed data, was "npc_mvr-0.1.4.tar", last modified: Tue Apr 23 19:10:13 2024, max compression
```

## Comparing `npc-mvr-0.1.3.tar` & `npc_mvr-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-26 16:38:39.000000 npc-mvr-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-26 16:38:39.000000 npc-mvr-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-26 16:39:16.000000 npc-mvr-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/src/npc_mvr/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-26 16:38:39.000000 npc-mvr-0.1.3/src/npc_mvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20192 2024-03-26 16:39:12.000000 npc-mvr-0.1.3/src/npc_mvr/mvr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:38:39.000000 npc-mvr-0.1.3/src/npc_mvr/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/src/npc_mvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-26 16:39:19.000000 npc-mvr-0.1.3/src/npc_mvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-26 16:39:19.000000 npc-mvr-0.1.3/src/npc_mvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:39:19.000000 npc-mvr-0.1.3/src/npc_mvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 16:39:19.000000 npc-mvr-0.1.3/src/npc_mvr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 16:39:19.000000 npc-mvr-0.1.3/src/npc_mvr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:39:19.361718 npc-mvr-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 16:38:39.000000 npc-mvr-0.1.3/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-23 19:10:10.000000 npc_mvr-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/src/npc_mvr/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/src/npc_mvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35353 2024-04-23 19:10:07.000000 npc_mvr-0.1.4/src/npc_mvr/mvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/src/npc_mvr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/src/npc_mvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/tests/test_core.py
```

### Comparing `npc-mvr-0.1.3/LICENSE` & `npc_mvr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `npc-mvr-0.1.3/PKG-INFO` & `npc_mvr-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-mvr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for reading raw video data from MindScope Neuropixels experiments, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_mvr
 Project-URL: Issues, https://github.com/AllenInstitute/npc_mvr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `npc-mvr-0.1.3/README.md` & `npc_mvr-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `npc-mvr-0.1.3/pyproject.toml` & `npc_mvr-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "npc-io>=0.1.20",
     "npc-sync>=0.1.5",
     "opencv-python-headless>=4.9.0.80",
     "typing-extensions>=4.9.0",
 ]
-version = "0.1.3"
+version = "0.1.4"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `npc-mvr-0.1.3/src/npc_mvr/__init__.py` & `npc_mvr-0.1.4/src/npc_mvr/__init__.py`

 * *Files identical despite different names*

### Comparing `npc-mvr-0.1.3/src/npc_mvr.egg-info/PKG-INFO` & `npc_mvr-0.1.4/src/npc_mvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-mvr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for reading raw video data from MindScope Neuropixels experiments, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_mvr
 Project-URL: Issues, https://github.com/AllenInstitute/npc_mvr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

