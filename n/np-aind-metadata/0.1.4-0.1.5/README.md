# Comparing `tmp/np_aind_metadata-0.1.4.tar.gz` & `tmp/np_aind_metadata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_aind_metadata-0.1.4.tar", last modified: Mon Apr 22 23:19:56 2024, max compression
+gzip compressed data, was "np_aind_metadata-0.1.5.tar", last modified: Tue Apr 23 00:07:15 2024, max compression
```

## Comparing `np_aind_metadata-0.1.4.tar` & `np_aind_metadata-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-22 23:19:53.000000 np_aind_metadata-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.427611 np_aind_metadata-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.431611 np_aind_metadata-0.1.4/src/np_aind_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.431611 np_aind_metadata-0.1.4/src/np_aind_metadata/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/init/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-22 23:19:50.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/np.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.431611 np_aind_metadata-0.1.4/src/np_aind_metadata/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-22 23:19:51.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/src/np_aind_metadata/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-22 23:19:50.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/src/np_aind_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:19:56.000000 np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:56.435611 np_aind_metadata-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_np.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-22 23:19:17.000000 np_aind_metadata-0.1.4/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.230375 np_aind_metadata-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-23 00:07:15.230375 np_aind_metadata-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-23 00:07:12.000000 np_aind_metadata-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 00:07:15.230375 np_aind_metadata-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.222375 np_aind_metadata-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.226375 np_aind_metadata-0.1.5/src/np_aind_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.226375 np_aind_metadata-0.1.5/src/np_aind_metadata/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/init/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.226375 np_aind_metadata-0.1.5/src/np_aind_metadata/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-23 00:07:09.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.226375 np_aind_metadata-0.1.5/src/np_aind_metadata/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/update/dynamic_routing_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/update/dynamic_routing_task_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/src/np_aind_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.230375 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-23 00:07:15.000000 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 00:07:15.000000 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:07:15.000000 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 00:07:15.000000 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 00:07:15.000000 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 00:07:15.000000 np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:07:15.230375 np_aind_metadata-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/tests/test_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/tests/test_np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 00:06:39.000000 np_aind_metadata-0.1.5/tests/test_storage.py
```

### Comparing `np_aind_metadata-0.1.4/LICENSE` & `np_aind_metadata-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/PKG-INFO` & `np_aind_metadata-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.4
+Version: 0.1.5
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.4/README.md` & `np_aind_metadata-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/pyproject.toml` & `np_aind_metadata-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dependencies = [
     "h5py>=3.10.0",
     "pyyaml>=6.0.1",
     "np-session>=0.6.40",
     "np-config>=0.4.27",
     "aind-metadata-mapper==0.6.2",
 ]
-version = "0.1.4"
+version = "0.1.5"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
@@ -207,14 +207,15 @@
 
 [tool.pdm.scripts]
 ruff = "ruff check src --fix-only"
 black = "black src"
 pytest = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'not onprem and not storage'"
 pytest-storage = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'storage'"
 pytest-onprem = "pytest --cov-report term-missing:skip-covered --cov-report=html -m 'onprem'"
+pytest-full = "pytest --cov-report term-missing:skip-covered --cov-report=html"
 mypy = "mypy src --install-types --non-interactive"
 log = "git-changelog -o CHANGELOG.md"
 dryrun = "pdm publish --repository testpypi --dry-run"
 post_init = "pdm install --plugins"
 
 [tool.pdm.scripts.test]
 composite = [
```

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/__init__.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/common.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/common.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/init/neuropixels_rig.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/init/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/np.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/np.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/np_codeocean.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/np_codeocean.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/scripts/main.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 modification_date_format_1 = "%Y/%m/%d"
 
 
 @cli.command()
 @click.argument("storage-directory", type=pathlib.Path)
 @click.argument(
     "rig-name",
-    type=common.RigName,
+    type=click.Choice(["NP1", "NP2", "NP3"]),
 )
 @click.option(
     "--date",
     help=(
         "Rig modification date. Supported formats:"
         f" {modification_date_format_0}, {modification_date_format_1}"
     ),
```

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/storage.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/storage.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/update/dynamic_routing_task.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/update/dynamic_routing_task_etl.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/update/dynamic_routing_task_etl.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata/utils.py` & `np_aind_metadata-0.1.5/src/np_aind_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/PKG-INFO` & `np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.4
+Version: 0.1.5
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.4/src/np_aind_metadata.egg-info/SOURCES.txt` & `np_aind_metadata-0.1.5/src/np_aind_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/tests/test_np_codeocean.py` & `np_aind_metadata-0.1.5/tests/test_np_codeocean.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.4/tests/test_storage.py` & `np_aind_metadata-0.1.5/tests/test_storage.py`

 * *Files identical despite different names*

