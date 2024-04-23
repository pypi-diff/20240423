# Comparing `tmp/auditor-htcondor-collector-0.4.0.tar.gz` & `tmp/auditor-htcondor-collector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auditor-htcondor-collector-0.4.0.tar", last modified: Mon Feb  5 14:26:41 2024, max compression
+gzip compressed data, was "auditor-htcondor-collector-0.5.0.tar", last modified: Tue Apr 23 14:03:12 2024, max compression
```

## Comparing `auditor-htcondor-collector-0.4.0.tar` & `auditor-htcondor-collector-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.275563 auditor-htcondor-collector-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-05 14:26:41.275563 auditor-htcondor-collector-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 14:26:41.275563 auditor-htcondor-collector-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.271563 auditor-htcondor-collector-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.275563 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/state_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-05 14:26:28.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.275563 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-05 14:26:41.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-05 14:26:41.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 14:26:41.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-05 14:26:41.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-05 14:26:41.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 14:26:41.000000 auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:03:12.671757 auditor-htcondor-collector-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 14:03:12.671757 auditor-htcondor-collector-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:03:12.671757 auditor-htcondor-collector-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:03:12.667757 auditor-htcondor-collector-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:03:12.667757 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/state_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-23 14:03:03.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:03:12.671757 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 14:03:12.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 14:03:12.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:03:12.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 14:03:12.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 14:03:12.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 14:03:12.000000 auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/top_level.txt
```

### Comparing `auditor-htcondor-collector-0.4.0/PKG-INFO` & `auditor-htcondor-collector-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: auditor-htcondor-collector
-Version: 0.4.0
+Version: 0.5.0
 Summary: AUDITOR collector for aggregating data from the HTCondor batch system
 Project-URL: documentation, https://alu-schumacher.github.io/AUDITOR/#htcondor-collector
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: python-auditor==0.4.0
+Requires-Dist: python-auditor==0.5.0
 Provides-Extra: build
-Requires-Dist: build==1.0.3; extra == "build"
-Requires-Dist: setuptools==69.0.3; extra == "build"
+Requires-Dist: build==1.2.1; extra == "build"
+Requires-Dist: setuptools==69.2.0; extra == "build"
 
 # HTCondor Collector
 
 Documentation of the HTCondor collector is available on the [AUDITOR website](https://alu-schumacher.github.io/AUDITOR/#htcondor-collector).
```

### Comparing `auditor-htcondor-collector-0.4.0/pyproject.toml` & `auditor-htcondor-collector-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
-requires = ["setuptools==69.0.3"]
+requires = ["setuptools==69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {""= "src"}
 packages = ["auditor_htcondor_collector"]
 
 [project]
 name = "auditor-htcondor-collector"
 description = "AUDITOR collector for aggregating data from the HTCondor batch system"
-version = "0.4.0"
+version = "0.5.0"
 requires-python = ">=3.8"
 dependencies = [
     "pyyaml==6.0.1",
-    "python-auditor==0.4.0"
+    "python-auditor==0.5.0"
 ]
 readme = "README.md"
 
 [project.optional-dependencies]
 build = [
-      "build==1.0.3",
-      "setuptools==69.0.3",
+      "build==1.2.1",
+      "setuptools==69.2.0",
 ]
 
 [project.scripts]
 auditor-htcondor-collector = "auditor_htcondor_collector.main:main"
 
 [project.urls]
 documentation = "https://alu-schumacher.github.io/AUDITOR/#htcondor-collector"
```

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/cli.py` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/cli.py`

 * *Files identical despite different names*

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/collector.py` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/collector.py`

 * *Files identical despite different names*

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/config.py` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/config.py`

 * *Files identical despite different names*

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/exceptions.py` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/exceptions.py`

 * *Files identical despite different names*

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/state_db.py` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/state_db.py`

 * *Files identical despite different names*

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector/utils.py` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector/utils.py`

 * *Files identical despite different names*

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/PKG-INFO` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: auditor-htcondor-collector
-Version: 0.4.0
+Version: 0.5.0
 Summary: AUDITOR collector for aggregating data from the HTCondor batch system
 Project-URL: documentation, https://alu-schumacher.github.io/AUDITOR/#htcondor-collector
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: python-auditor==0.4.0
+Requires-Dist: python-auditor==0.5.0
 Provides-Extra: build
-Requires-Dist: build==1.0.3; extra == "build"
-Requires-Dist: setuptools==69.0.3; extra == "build"
+Requires-Dist: build==1.2.1; extra == "build"
+Requires-Dist: setuptools==69.2.0; extra == "build"
 
 # HTCondor Collector
 
 Documentation of the HTCondor collector is available on the [AUDITOR website](https://alu-schumacher.github.io/AUDITOR/#htcondor-collector).
```

### Comparing `auditor-htcondor-collector-0.4.0/src/auditor_htcondor_collector.egg-info/SOURCES.txt` & `auditor-htcondor-collector-0.5.0/src/auditor_htcondor_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

