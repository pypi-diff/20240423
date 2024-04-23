# Comparing `tmp/uptycs-py-0.0.2.tar.gz` & `tmp/uptycs-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptycs-py-0.0.2.tar", last modified: Mon Aug  7 14:41:59 2023, max compression
+gzip compressed data, was "uptycs-py-0.0.3.tar", last modified: Tue Apr 23 04:31:01 2024, max compression
```

## Comparing `uptycs-py-0.0.2.tar` & `uptycs-py-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2023-08-07 14:41:59.717604 uptycs-py-0.0.2/
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     1067 2023-04-04 12:00:29.000000 uptycs-py-0.0.2/LICENSE
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     1389 2023-08-07 14:41:59.717604 uptycs-py-0.0.2/PKG-INFO
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      940 2023-08-07 14:38:04.000000 uptycs-py-0.0.2/README.md
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      790 2023-08-07 14:41:15.000000 uptycs-py-0.0.2/pyproject.toml
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      357 2023-08-07 14:41:59.717604 uptycs-py-0.0.2/setup.cfg
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      823 2023-08-07 14:41:44.000000 uptycs-py-0.0.2/setup.py
-drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2023-08-07 14:41:59.713604 uptycs-py-0.0.2/src/
-drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2023-08-07 14:41:59.713604 uptycs-py-0.0.2/src/uptycs_py/
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      262 2023-08-07 13:34:20.000000 uptycs-py-0.0.2/src/uptycs_py/__init__.py
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)    45833 2023-08-07 14:19:45.000000 uptycs-py-0.0.2/src/uptycs_py/upt_api.py
-drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2023-08-07 14:41:59.717604 uptycs-py-0.0.2/uptycs_py.egg-info/
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     1389 2023-08-07 14:41:59.000000 uptycs-py-0.0.2/uptycs_py.egg-info/PKG-INFO
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      266 2023-08-07 14:41:59.000000 uptycs-py-0.0.2/uptycs_py.egg-info/SOURCES.txt
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)        1 2023-08-07 14:41:59.000000 uptycs-py-0.0.2/uptycs_py.egg-info/dependency_links.txt
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)       22 2023-08-07 14:41:59.000000 uptycs-py-0.0.2/uptycs_py.egg-info/requires.txt
--rw-rw-r--   0 cgadde    (1000) cgadde    (1000)       10 2023-08-07 14:41:59.000000 uptycs-py-0.0.2/uptycs_py.egg-info/top_level.txt
+drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2024-04-23 04:31:01.734732 uptycs-py-0.0.3/
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     1067 2023-04-04 12:00:29.000000 uptycs-py-0.0.3/LICENSE
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     3087 2024-04-23 04:31:01.734732 uptycs-py-0.0.3/PKG-INFO
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     1202 2024-04-23 03:47:30.000000 uptycs-py-0.0.3/README.md
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      790 2024-04-23 03:43:46.000000 uptycs-py-0.0.3/pyproject.toml
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      357 2024-04-23 04:31:01.734732 uptycs-py-0.0.3/setup.cfg
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      823 2024-04-23 03:43:26.000000 uptycs-py-0.0.3/setup.py
+drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2024-04-23 04:31:01.714732 uptycs-py-0.0.3/src/
+drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2024-04-23 04:31:01.730732 uptycs-py-0.0.3/src/uptycs_py/
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      262 2023-08-07 13:34:20.000000 uptycs-py-0.0.3/src/uptycs_py/__init__.py
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)    45833 2023-08-07 14:19:45.000000 uptycs-py-0.0.3/src/uptycs_py/upt_api.py
+drwxrwxr-x   0 cgadde    (1000) cgadde    (1000)        0 2024-04-23 04:31:01.730732 uptycs-py-0.0.3/uptycs_py.egg-info/
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)     3087 2024-04-23 04:31:01.000000 uptycs-py-0.0.3/uptycs_py.egg-info/PKG-INFO
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)      266 2024-04-23 04:31:01.000000 uptycs-py-0.0.3/uptycs_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)        1 2024-04-23 04:31:01.000000 uptycs-py-0.0.3/uptycs_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)       22 2024-04-23 04:31:01.000000 uptycs-py-0.0.3/uptycs_py.egg-info/requires.txt
+-rw-rw-r--   0 cgadde    (1000) cgadde    (1000)       10 2024-04-23 04:31:01.000000 uptycs-py-0.0.3/uptycs_py.egg-info/top_level.txt
```

### Comparing `uptycs-py-0.0.2/LICENSE` & `uptycs-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uptycs-py-0.0.2/README.md` & `uptycs-py-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,7 +20,20 @@
   UptAlertRule()   - Get or Create an alert rule
   UptAssets()      - Show/update assets registered in Uptycs, add/remove tags from assets
   UptEventRule()   - Get or Create an event rule
   UptLkpTable()    - Get or Create a lookup table (typically for whitelists/blacklists)
   UptQueryGlobal() - Run a query against global (flight recorder)
   UptQueryRt()     - Run a query against realtime
 ```
+
+Test sample:
+
+```
+import sys
+import uptycs_py
+
+keyfile = sys.argv[1]
+myauth = uptycs_py.UptApiAuth(keyfile)
+myasset = uptycs_py.UptAssets(myauth)
+print("Total number of assets %s " % len(myasset.items))
+print(myasset.get_id_from_hostname('test_host_name'))
+```
```

### Comparing `uptycs-py-0.0.2/pyproject.toml` & `uptycs-py-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uptycs-py"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Julian Wayte", email="jwayte@uptycs.com" },
   { name="Serge Teren", email="steren@uptycs.com" },
 ]
 maintainers = [
   { name="Chandrasekhar", email="cgadde@uptycs.com" },
   { name="Alan Koshy", email="akoshy@uptycs.com" },
```

### Comparing `uptycs-py-0.0.2/setup.py` & `uptycs-py-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='uptycs-py',
-     version='0.0.2',
-     author="Julian Waite",
+     version='0.0.3',
+     author="Julian Wayte",
      author_email="jwayte@uptycs.com",
      description="Uptycs API helper library (for Python 3)",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/Uptycs/uptycs-py",
      install_requires=[
         'requests',
```

### Comparing `uptycs-py-0.0.2/src/uptycs_py/upt_api.py` & `uptycs-py-0.0.3/src/uptycs_py/upt_api.py`

 * *Files identical despite different names*

