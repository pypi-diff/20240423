# Comparing `tmp/domolibrary_execution-0.0.1.tar.gz` & `tmp/domolibrary_execution-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary_execution-0.0.1.tar", last modified: Fri Apr 19 18:27:27 2024, max compression
+gzip compressed data, was "domolibrary_execution-0.0.4.tar", last modified: Mon Apr 22 21:41:26 2024, max compression
```

## Comparing `domolibrary_execution-0.0.1.tar` & `domolibrary_execution-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 18:27:27.512351 domolibrary_execution-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/MANIFEST.in
--rw-r--r--   0 codespace  (1000) codespace  (1000)      749 2024-04-19 18:27:27.512351 domolibrary_execution-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 18:27:27.508351 domolibrary_execution-0.0.1/domolibrary_execution/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6799 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/FactoryAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/FactoryUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9926 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/_modidx.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/process.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2812 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/domolibrary_execution/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 18:27:27.512351 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      749 2024-04-19 18:27:27.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      602 2024-04-19 18:27:27.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:27:27.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-19 18:27:27.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-04-19 18:27:27.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-19 18:27:27.000000 domolibrary_execution-0.0.1/domolibrary_execution.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      890 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-19 18:27:27.512351 domolibrary_execution-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.4/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 21:41:26.580376 domolibrary_execution-0.0.4/domolibrary_execution/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5469 2024-04-22 21:40:45.000000 domolibrary_execution-0.0.4/domolibrary_execution/FactoryAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/FactoryUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8738 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/_modidx.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/domolibrary_execution/core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/process.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      602 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-04-22 21:36:26.000000 domolibrary_execution-0.0.4/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/setup.py
```

### Comparing `domolibrary_execution-0.0.1/LICENSE` & `domolibrary_execution-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution/FactoryUser.py` & `domolibrary_execution-0.0.4/domolibrary_execution/FactoryUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution/_modidx.py` & `domolibrary_execution-0.0.4/domolibrary_execution/_modidx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': '',
                 'doc_baseurl': '/domolibrary_execution',
                 'doc_host': 'https://.github.io',
                 'git_url': 'https://github.com//domolibrary_execution',
                 'lib_path': 'domolibrary_execution'},
-  'syms': { 'domolibrary_execution.FactoryAuth': { 'domolibrary_execution.FactoryAuth.Config_DomoJupyterToDomoAccount': ( 'factoryauth.html#config_domojupytertodomoaccount',
-                                                                                                                          'domolibrary_execution/FactoryAuth.py'),
-                                                   'domolibrary_execution.FactoryAuth.Config_GenerateConfigAuth': ( 'factoryauth.html#config_generateconfigauth',
-                                                                                                                    'domolibrary_execution/FactoryAuth.py'),
-                                                   'domolibrary_execution.FactoryAuth.Config_UpsertDomoAccount': ( 'factoryauth.html#config_upsertdomoaccount',
-                                                                                                                   'domolibrary_execution/FactoryAuth.py'),
-                                                   'domolibrary_execution.FactoryAuth.generate_config_auth': ( 'factoryauth.html#generate_config_auth',
-                                                                                                               'domolibrary_execution/FactoryAuth.py'),
-                                                   'domolibrary_execution.FactoryAuth.get_domoaccount': ( 'factoryauth.html#get_domoaccount',
-                                                                                                          'domolibrary_execution/FactoryAuth.py'),
-                                                   'domolibrary_execution.FactoryAuth.upsert_domoaccount': ( 'factoryauth.html#upsert_domoaccount',
-                                                                                                             'domolibrary_execution/FactoryAuth.py')},
+  'syms': { 'domolibrary_execution.FactoryAuth': { 'domolibrary_execution.FactoryAuth.Factory_ExportJupyterAccounts': ( 'factoryjupyer.html#factory_exportjupyteraccounts',
+                                                                                                                        'domolibrary_execution/FactoryAuth.py'),
+                                                   'domolibrary_execution.FactoryAuth.export_jupyter_instance_accounts': ( 'factoryjupyer.html#export_jupyter_instance_accounts',
+                                                                                                                           'domolibrary_execution/FactoryAuth.py')},
             'domolibrary_execution.FactoryUser': { 'domolibrary_execution.FactoryUser.Config_GenerateUserAccessToken': ( 'factoryuser.html#config_generateuseraccesstoken',
                                                                                                                          'domolibrary_execution/FactoryUser.py'),
                                                    'domolibrary_execution.FactoryUser.UpsertGroupConfig': ( 'factoryuser.html#upsertgroupconfig',
                                                                                                             'domolibrary_execution/FactoryUser.py'),
                                                    'domolibrary_execution.FactoryUser.UpsertRoleConfig': ( 'factoryuser.html#upsertroleconfig',
                                                                                                            'domolibrary_execution/FactoryUser.py'),
                                                    'domolibrary_execution.FactoryUser.UpsertUserConfig': ( 'factoryuser.html#upsertuserconfig',
```

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution/core.py` & `domolibrary_execution-0.0.4/domolibrary_execution/core.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution/process.py` & `domolibrary_execution-0.0.4/domolibrary_execution/process.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution/utils.py` & `domolibrary_execution-0.0.4/domolibrary_execution/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,46 +12,53 @@
 from operator import itemgetter
 
 import json
 from typing import Callable
 
 import domolibrary.client.DomoAuth as dmda
 
-# %% ../nbs/00_utils.ipynb 4
+# %% ../nbs/00_utils.ipynb 3
 def which_environment():
     return urllib_parse.urlparse(os.environ.get('DOMO_HOSTNAME')).netloc.replace('.domo.com', '')
     
 
-# %% ../nbs/00_utils.ipynb 6
+# %% ../nbs/00_utils.ipynb 4
 def read_domo_jupyter_account(account_name,
                               domojupyter_fn : Callable,
-                              is_abstract: bool = False,):
+                              is_abstract: bool = False,
+                              is_dict : bool = True
+                            
+                             ):
 
     account_properties = domojupyter_fn.get_account_property_keys(account_name)
 
     creds = {
         prop: domojupyter_fn.get_account_property_value(account_name, prop)
         for prop in account_properties
     }
 
     if not is_abstract:
         return creds
 
+    creds = creds['credentials']
+    
+    if not is_dict:
+        return creds.strip()
+    
     return json.loads(
-        creds["credentials"]
-    )  # converts credentials string into a dictionary
-
+        creds
+    )
 
-# %% ../nbs/00_utils.ipynb 7
+# %% ../nbs/00_utils.ipynb 5
 def remove_asterix(text):
     if text == '' or text == '********':
         return None
     return text
 
-# %% ../nbs/00_utils.ipynb 8
+# %% ../nbs/00_utils.ipynb 6
 async def domojupyter_to_domoauth(
     account_name,
     instance,
     domojupyter_fn: Callable,
     is_abstract: bool,
     is_test: bool = True
 ) -> dict:
```

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution.egg-info/PKG-INFO` & `domolibrary_execution-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: domolibrary-execution
-Version: 0.0.1
+Name: domolibrary_execution
+Version: 0.0.4
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,10 +13,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: fastcore
+Requires-Dist: pandas
+Requires-Dist: domolibrary
+Requires-Dist: domolibrary_extensions
 Provides-Extra: dev
 
 pip install domolibrary_executio
```

### Comparing `domolibrary_execution-0.0.1/domolibrary_execution.egg-info/SOURCES.txt` & `domolibrary_execution-0.0.4/domolibrary_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.1/settings.ini` & `domolibrary_execution-0.0.4/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domolibrary_execution
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = %(repo)s
@@ -34,10 +34,10 @@
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = 
 
 ### Optional ###
-# requirements = fastcore pandas
+requirements = fastcore pandas domolibrary domolibrary_extensions
 # dev_requirements = 
 # console_scripts =
```

### Comparing `domolibrary_execution-0.0.1/setup.py` & `domolibrary_execution-0.0.4/setup.py`

 * *Files identical despite different names*

