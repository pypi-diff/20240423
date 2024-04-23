# Comparing `tmp/democrite-4.1.2.tar.gz` & `tmp/democrite-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democrite-4.1.2.tar", last modified: Tue Apr 23 20:09:42 2024, max compression
+gzip compressed data, was "democrite-4.1.3.tar", last modified: Tue Apr 23 20:14:15 2024, max compression
```

## Comparing `democrite-4.1.2.tar` & `democrite-4.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 20:09:42.446449 democrite-4.1.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     2463 2024-04-23 20:09:42.446449 democrite-4.1.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1928 2024-04-23 20:09:33.000000 democrite-4.1.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 20:09:42.446449 democrite-4.1.2/democrite.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2463 2024-04-23 20:09:42.000000 democrite-4.1.2/democrite.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-04-23 20:09:42.000000 democrite-4.1.2/democrite.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-23 20:09:42.000000 democrite-4.1.2/democrite.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-04-23 20:09:42.000000 democrite-4.1.2/democrite.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    10502 2024-04-23 20:09:33.000000 democrite-4.1.2/democrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)      533 2024-04-23 20:09:39.000000 democrite-4.1.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-23 20:09:42.446449 democrite-4.1.2/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 20:14:15.348965 democrite-4.1.3/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2463 2024-04-23 20:14:15.348965 democrite-4.1.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1928 2024-04-23 20:14:07.000000 democrite-4.1.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 20:14:15.348965 democrite-4.1.3/democrite.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2463 2024-04-23 20:14:15.000000 democrite-4.1.3/democrite.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-04-23 20:14:15.000000 democrite-4.1.3/democrite.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-23 20:14:15.000000 democrite-4.1.3/democrite.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-04-23 20:14:15.000000 democrite-4.1.3/democrite.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    10502 2024-04-23 20:14:07.000000 democrite-4.1.3/democrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      533 2024-04-23 20:14:11.000000 democrite-4.1.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-23 20:14:15.348965 democrite-4.1.3/setup.cfg
```

### Comparing `democrite-4.1.2/PKG-INFO` & `democrite-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democrite
-Version: 4.1.2
+Version: 4.1.3
 Summary: Library use to construct VGrain to democrite servers
 Author-email: Nexai <info@nexai.net>
 Project-URL: Homepage, https://github.com/Nexai-net/democrite
 Project-URL: Issues, https://github.com/Nexai-net/democrite/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `democrite-4.1.2/README.md` & `democrite-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `democrite-4.1.2/democrite.egg-info/PKG-INFO` & `democrite-4.1.3/democrite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democrite
-Version: 4.1.2
+Version: 4.1.3
 Summary: Library use to construct VGrain to democrite servers
 Author-email: Nexai <info@nexai.net>
 Project-URL: Homepage, https://github.com/Nexai-net/democrite
 Project-URL: Issues, https://github.com/Nexai-net/democrite/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `democrite-4.1.2/democrite.py` & `democrite-4.1.3/democrite.py`

 * *Files identical despite different names*

### Comparing `democrite-4.1.2/pyproject.toml` & `democrite-4.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "democrite"
-version = "4.1.2"
+version = "4.1.3"
 authors = [
   { name="Nexai", email="info@nexai.net" },
 ]
 
 description = "Library use to construct VGrain to democrite servers"
 readme = "README.md"
 requires-python = ">=3.8"
```

