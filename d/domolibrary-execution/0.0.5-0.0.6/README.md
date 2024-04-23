# Comparing `tmp/domolibrary_execution-0.0.5.tar.gz` & `tmp/domolibrary_execution-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary_execution-0.0.5.tar", last modified: Mon Apr 22 23:17:10 2024, max compression
+gzip compressed data, was "domolibrary_execution-0.0.6.tar", last modified: Tue Apr 23 17:19:29 2024, max compression
```

## Comparing `domolibrary_execution-0.0.5.tar` & `domolibrary_execution-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/MANIFEST.in
--rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 23:17:10.094812 domolibrary_execution-0.0.5/domolibrary_execution/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6798 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/FactoryAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5474 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/FactoryJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/FactoryUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10634 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/_modidx.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/domolibrary_execution/core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/process.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-04-22 23:16:49.000000 domolibrary_execution-0.0.5/domolibrary_execution/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      642 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-22 23:17:09.000000 domolibrary_execution-0.0.5/domolibrary_execution.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-04-22 23:16:42.000000 domolibrary_execution-0.0.5/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-22 23:17:10.102812 domolibrary_execution-0.0.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-23 17:19:29.477883 domolibrary_execution-0.0.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.6/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-23 17:19:29.477883 domolibrary_execution-0.0.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.6/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-23 17:19:29.473883 domolibrary_execution-0.0.6/domolibrary_execution/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6798 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/FactoryAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5679 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/FactoryJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/FactoryUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10634 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/_modidx.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.6/domolibrary_execution/core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/process.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-04-23 17:19:26.000000 domolibrary_execution-0.0.6/domolibrary_execution/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-23 17:19:29.477883 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      860 2024-04-23 17:19:29.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      642 2024-04-23 17:19:29.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-23 17:19:29.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-23 17:19:29.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-23 17:19:29.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:19:29.000000 domolibrary_execution-0.0.6/domolibrary_execution.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-04-23 17:19:13.000000 domolibrary_execution-0.0.6/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-23 17:19:29.477883 domolibrary_execution-0.0.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.6/setup.py
```

### Comparing `domolibrary_execution-0.0.5/LICENSE` & `domolibrary_execution-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/PKG-INFO` & `domolibrary_execution-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary_execution
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/FactoryAuth.py` & `domolibrary_execution-0.0.6/domolibrary_execution/FactoryAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/FactoryJupyter.py` & `domolibrary_execution-0.0.6/domolibrary_execution/FactoryJupyter.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,17 +47,18 @@
         domo_jupyter_workspace = await dmdj.DomoJupyterWorkspace.get_current_workspace(
             auth=auth, debug_api=debug_api, session=session
         )
         step.is_success = True
         step.message = "workspace config retrieved"
 
     except Exception as e:
-        step.message = e
+        message = f"no workspace retrieved - {e}"
+        step.message = message
         step.is_success = False
-        res.response = "no workspace"
+        res.response = message
         return res
 
     # STEP - get workspace accounts
     step = FactoryMessage(stage="get workspace accounts", is_success=False)
     res.add_message(step)
     domo_accounts = None
 
@@ -67,23 +68,24 @@
             debug_api = debug_api,
         )
         step.is_success = True
         step.message = f"{len(domo_accounts)} accounts retrieved"
 
     except Exception as e:
         step.is_success = False
-        step.message = "no accounts retrieved"
-        res.response = "no accounts"
+        message = f"no accounts retrieved {e}" 
+        step.message = message
+        res.response = message
         return res
 
     if len(domo_accounts) == 0:
-        step.message = "no accounts to export"
+        message =  "no accounts to export"
+        step.message = message
         step.is_success = True
-
-        res.response = "no accounts to export"
+        res.response = message
         return res
 
     # STEP - handle pgp key
     step = FactoryMessage(stage="handle pgp key", is_success=False)
     res.add_message(step)
 
     pgp_key = None
@@ -94,16 +96,17 @@
         pgp_key = depg.generate_pgpy_key(pgp_blob=pgp_blob)
 
         step.is_success = True
         step.message = "pgp key generated"
 
     except Exception as e:
         step.is_success = False
-        step.message = e
-        res.response = "no pgp blob"
+        message = f"no pgp blob - {e}"
+        step.message = message
+        res.response = message
         return res
 
     # STEP - EXPORT ACCOUNTS
     step = FactoryMessage(stage="export accounts", is_success=False)
     res.add_message(step)
 
     def export_account(export_folder, domo_account, res):
@@ -111,15 +114,15 @@
         step = FactoryMessage(
             stage=f"export accounts - {account_name}", is_success=False
         )
         res.add_message(step)
 
         try:
             config = dxut.read_domo_jupyter_account(
-                domo_account.alias, domojupyter_fn=dj
+                domo_account.alias, domojupyter_fn=domojupyter_fn
             )
             step.message = "read domojupyter_account"
 
             obj = domo_account.config._from_json(config).to_json()
             obj.update(
                 {"account_id": domo_account.id, "domo_instance": auth.domo_instance}
             )
@@ -132,15 +135,16 @@
             output_path = step.message = depg.pgpy_encrypt(
                 pgp_key=pgp_key, data=obj, output_path=export_path
             )
             step.is_success = True
             return output_path
 
         except Exception as e:
-            step.message = e
+            message = f"unable to export {account_name} - {e}"
+            step.message = message
             step.is_success = False
             return False
 
     export_folder = os.path.join(export_folder, "accounts")
 
     export_ls = [
         export_account(
```

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/FactoryUser.py` & `domolibrary_execution-0.0.6/domolibrary_execution/FactoryUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/_modidx.py` & `domolibrary_execution-0.0.6/domolibrary_execution/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/core.py` & `domolibrary_execution-0.0.6/domolibrary_execution/core.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/process.py` & `domolibrary_execution-0.0.6/domolibrary_execution/process.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution/utils.py` & `domolibrary_execution-0.0.6/domolibrary_execution/utils.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution.egg-info/PKG-INFO` & `domolibrary_execution-0.0.6/domolibrary_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary-execution
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.5/domolibrary_execution.egg-info/SOURCES.txt` & `domolibrary_execution-0.0.6/domolibrary_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.5/settings.ini` & `domolibrary_execution-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domolibrary_execution
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = %(repo)s
```

### Comparing `domolibrary_execution-0.0.5/setup.py` & `domolibrary_execution-0.0.6/setup.py`

 * *Files identical despite different names*

