# Comparing `tmp/domolibrary_execution-0.0.4.tar.gz` & `tmp/domolibrary_execution-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary_execution-0.0.4.tar", last modified: Mon Apr 22 21:41:26 2024, max compression
+gzip compressed data, was "domolibrary_execution-0.0.5.tar", last modified: Mon Apr 22 23:17:10 2024, max compression
```

## Comparing `domolibrary_execution-0.0.4.tar` & `domolibrary_execution-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/MANIFEST.in
--rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 21:41:26.580376 domolibrary_execution-0.0.4/domolibrary_execution/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5469 2024-04-22 21:40:45.000000 domolibrary_execution-0.0.4/domolibrary_execution/FactoryAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/FactoryUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8738 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/_modidx.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/domolibrary_execution/core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/process.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-04-22 21:40:46.000000 domolibrary_execution-0.0.4/domolibrary_execution/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      602 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 21:41:26.000000 domolibrary_execution-0.0.4/domolibrary_execution.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-04-22 21:36:26.000000 domolibrary_execution-0.0.4/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-22 21:41:26.584376 domolibrary_execution-0.0.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 23:17:10.094812 domolibrary_execution-0.0.5/domolibrary_execution/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6798 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/FactoryAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5474 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/FactoryJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/FactoryUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10634 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/_modidx.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/domolibrary_execution/core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/process.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      642 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-04-22 23:16:42.000000 domolibrary_execution-0.0.5/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/setup.py
```

### Comparing `domolibrary_execution-0.0.4/LICENSE` & `domolibrary_execution-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.4/PKG-INFO` & `domolibrary_execution-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary_execution
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution/FactoryAuth.py` & `domolibrary_execution-0.0.5/domolibrary_execution/FactoryJupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_FactoryJupyer.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_FactoryJupyter.ipynb.
 
 # %% auto 0
 __all__ = ['export_jupyter_instance_accounts', 'Factory_ExportJupyterAccounts']
 
-# %% ../nbs/00_FactoryJupyer.ipynb 1
+# %% ../nbs/00_FactoryJupyter.ipynb 1
 from domolibrary_extensions.utils.factory import (
     factory_function,
     FactoryLogs, 
     FactoryResponse, FactoryConfig, FactoryMessage)
 
 import domolibrary.client.DomoAuth as dmda
 
 
-# %% ../nbs/00_FactoryJupyer.ipynb 2
+# %% ../nbs/00_FactoryJupyter.ipynb 2
 import os 
 import httpx
 from dataclasses import dataclass, field
 from typing import List, Callable
 
 import domolibrary.classes.DomoJupyter as dmdj
 import domolibrary.classes.DomoAccount as dmac
 import domolibrary_extensions.pgp as depg
 import domolibrary_extensions.utils.convert as decv
 import domolibrary_execution.utils as dxut
 
-# %% ../nbs/00_FactoryJupyer.ipynb 3
+# %% ../nbs/00_FactoryJupyter.ipynb 3
 @factory_function(config_id_col="jupyter_instance_name")
 async def export_jupyter_instance_accounts(
     res: FactoryResponse,
     config: FactoryConfig,
     logs: FactoryLogs,
     debug_api: bool = False,
     session: httpx.AsyncClient = None,
@@ -161,15 +161,15 @@
 
     step.is_success = True
     step.message = f"successfully export {len(export_ls)} accounts"
 
     res.response = f"accounts exported to {export_folder}"
     return res
 
-# %% ../nbs/00_FactoryJupyer.ipynb 4
+# %% ../nbs/00_FactoryJupyter.ipynb 4
 @dataclass
 class Factory_ExportJupyterAccounts(FactoryConfig):
     auth : dmda.DomoAuth
     domojupyter_fn : Callable = None
     jupyter_instance_name : str = None
     pgp_account_name :str = None
     export_folder :str = './EXPORT/'
```

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution/FactoryUser.py` & `domolibrary_execution-0.0.5/domolibrary_execution/FactoryUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution/_modidx.py` & `domolibrary_execution-0.0.5/domolibrary_execution/_modidx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': '',
                 'doc_baseurl': '/domolibrary_execution',
                 'doc_host': 'https://.github.io',
                 'git_url': 'https://github.com//domolibrary_execution',
                 'lib_path': 'domolibrary_execution'},
-  'syms': { 'domolibrary_execution.FactoryAuth': { 'domolibrary_execution.FactoryAuth.Factory_ExportJupyterAccounts': ( 'factoryjupyer.html#factory_exportjupyteraccounts',
-                                                                                                                        'domolibrary_execution/FactoryAuth.py'),
-                                                   'domolibrary_execution.FactoryAuth.export_jupyter_instance_accounts': ( 'factoryjupyer.html#export_jupyter_instance_accounts',
-                                                                                                                           'domolibrary_execution/FactoryAuth.py')},
+  'syms': { 'domolibrary_execution.FactoryAuth': { 'domolibrary_execution.FactoryAuth.Config_DomoJupyterToDomoAccount': ( 'factoryauth.html#config_domojupytertodomoaccount',
+                                                                                                                          'domolibrary_execution/FactoryAuth.py'),
+                                                   'domolibrary_execution.FactoryAuth.Config_GenerateConfigAuth': ( 'factoryauth.html#config_generateconfigauth',
+                                                                                                                    'domolibrary_execution/FactoryAuth.py'),
+                                                   'domolibrary_execution.FactoryAuth.Config_UpsertDomoAccount': ( 'factoryauth.html#config_upsertdomoaccount',
+                                                                                                                   'domolibrary_execution/FactoryAuth.py'),
+                                                   'domolibrary_execution.FactoryAuth.generate_config_auth': ( 'factoryauth.html#generate_config_auth',
+                                                                                                               'domolibrary_execution/FactoryAuth.py'),
+                                                   'domolibrary_execution.FactoryAuth.get_domoaccount': ( 'factoryauth.html#get_domoaccount',
+                                                                                                          'domolibrary_execution/FactoryAuth.py'),
+                                                   'domolibrary_execution.FactoryAuth.upsert_domoaccount': ( 'factoryauth.html#upsert_domoaccount',
+                                                                                                             'domolibrary_execution/FactoryAuth.py')},
+            'domolibrary_execution.FactoryJupyter': { 'domolibrary_execution.FactoryJupyter.Factory_ExportJupyterAccounts': ( 'factoryjupyter.html#factory_exportjupyteraccounts',
+                                                                                                                              'domolibrary_execution/FactoryJupyter.py'),
+                                                      'domolibrary_execution.FactoryJupyter.export_jupyter_instance_accounts': ( 'factoryjupyter.html#export_jupyter_instance_accounts',
+                                                                                                                                 'domolibrary_execution/FactoryJupyter.py')},
             'domolibrary_execution.FactoryUser': { 'domolibrary_execution.FactoryUser.Config_GenerateUserAccessToken': ( 'factoryuser.html#config_generateuseraccesstoken',
                                                                                                                          'domolibrary_execution/FactoryUser.py'),
                                                    'domolibrary_execution.FactoryUser.UpsertGroupConfig': ( 'factoryuser.html#upsertgroupconfig',
                                                                                                             'domolibrary_execution/FactoryUser.py'),
                                                    'domolibrary_execution.FactoryUser.UpsertRoleConfig': ( 'factoryuser.html#upsertroleconfig',
                                                                                                            'domolibrary_execution/FactoryUser.py'),
                                                    'domolibrary_execution.FactoryUser.UpsertUserConfig': ( 'factoryuser.html#upsertuserconfig',
```

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution/core.py` & `domolibrary_execution-0.0.5/domolibrary_execution/core.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution/process.py` & `domolibrary_execution-0.0.5/domolibrary_execution/process.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution/utils.py` & `domolibrary_execution-0.0.5/domolibrary_execution/utils.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution.egg-info/PKG-INFO` & `domolibrary_execution-0.0.5/domolibrary_execution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary-execution
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.4/domolibrary_execution.egg-info/SOURCES.txt` & `domolibrary_execution-0.0.5/domolibrary_execution.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 domolibrary_execution/FactoryAuth.py
+domolibrary_execution/FactoryJupyter.py
 domolibrary_execution/FactoryUser.py
 domolibrary_execution/__init__.py
 domolibrary_execution/_modidx.py
 domolibrary_execution/core.py
 domolibrary_execution/process.py
 domolibrary_execution/utils.py
 domolibrary_execution.egg-info/PKG-INFO
```

### Comparing `domolibrary_execution-0.0.4/settings.ini` & `domolibrary_execution-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domolibrary_execution
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = %(repo)s
```

### Comparing `domolibrary_execution-0.0.4/setup.py` & `domolibrary_execution-0.0.5/setup.py`

 * *Files identical despite different names*

