# Comparing `tmp/pulumi_commandx-0.0.2a1713827595.tar.gz` & `tmp/pulumi_commandx-0.0.2a1713828252.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_commandx-0.0.2a1713827595.tar", last modified: Mon Apr 22 23:15:20 2024, max compression
+gzip compressed data, was "pulumi_commandx-0.0.2a1713828252.tar", last modified: Mon Apr 22 23:25:54 2024, max compression
```

## Comparing `pulumi_commandx-0.0.2a1713827595.tar` & `pulumi_commandx-0.0.2a1713828252.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:15:20.250343 pulumi_commandx-0.0.2a1713827595/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-22 23:15:20.246343 pulumi_commandx-0.0.2a1713827595/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:15:20.242343 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/
--rw-------   0 runner    (1001) docker     (127)     1253 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/_utilities.py
--rw-------   0 runner    (1001) docker     (127)     2738 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/provider.py
--rw-------   0 runner    (1001) docker     (127)      101 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:15:20.246343 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/
--rw-------   0 runner    (1001) docker     (127)      590 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108421 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14943 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14962 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/curl.py
--rw-------   0 runner    (1001) docker     (127)    15035 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15175 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14943 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14978 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14838 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/mv.py
--rw-------   0 runner    (1001) docker     (127)    91760 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14838 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/rm.py
--rw-------   0 runner    (1001) docker     (127)    14873 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/sed.py
--rw-------   0 runner    (1001) docker     (127)    15105 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14873 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/tar.py
--rw-------   0 runner    (1001) docker     (127)    14893 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/tee.py
--rw-------   0 runner    (1001) docker     (127)    14908 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:15:20.246343 pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-22 23:15:20.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-22 23:15:20.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:15:20.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 23:15:20.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:15:20.000000 pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      745 2024-04-22 23:15:11.000000 pulumi_commandx-0.0.2a1713827595/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:15:20.250343 pulumi_commandx-0.0.2a1713827595/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:25:54.863847 pulumi_commandx-0.0.2a1713828252/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-22 23:25:54.863847 pulumi_commandx-0.0.2a1713828252/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:25:54.859847 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/
+-rw-------   0 runner    (1001) docker     (127)     1253 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)     2738 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/provider.py
+-rw-------   0 runner    (1001) docker     (127)      101 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:25:54.863847 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108421 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14943 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14962 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15035 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15175 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14943 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14978 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14838 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91760 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14838 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14873 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15105 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14873 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14893 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14908 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:25:54.863847 pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-22 23:25:54.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-22 23:25:54.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:25:54.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 23:25:54.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:25:54.000000 pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      745 2024-04-22 23:25:48.000000 pulumi_commandx-0.0.2a1713828252/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:25:54.863847 pulumi_commandx-0.0.2a1713828252/setup.cfg
```

### Comparing `pulumi_commandx-0.0.2a1713827595/PKG-INFO` & `pulumi_commandx-0.0.2a1713828252/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_commandx
-Version: 0.0.2a1713827595
+Version: 0.0.2a1713828252
 Summary: A Pulumi component provider for creating statically typed `Command` resources.
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-commandx
 Keywords: pulumi,command,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_commandx-0.0.2a1713827595/README.md` & `pulumi_commandx-0.0.2a1713828252/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/__init__.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/_utilities.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/provider.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/__init__.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/_enums.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/_inputs.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/chmod.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/curl.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/etcdctl.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/hostnamectl.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/mkdir.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/mktemp.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/mv.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/outputs.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/rm.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/sed.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/systemctl.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/tar.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/tee.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx/remote/wget.py` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx/remote/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/PKG-INFO` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_commandx
-Version: 0.0.2a1713827595
+Version: 0.0.2a1713828252
 Summary: A Pulumi component provider for creating statically typed `Command` resources.
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-commandx
 Keywords: pulumi,command,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_commandx-0.0.2a1713827595/pulumi_commandx.egg-info/SOURCES.txt` & `pulumi_commandx-0.0.2a1713828252/pulumi_commandx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.0.2a1713827595/pyproject.toml` & `pulumi_commandx-0.0.2a1713828252/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_commandx"
   description = "A Pulumi component provider for creating statically typed `Command` resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.2a1713827595"
+  version = "0.0.2a1713828252"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-commandx"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

