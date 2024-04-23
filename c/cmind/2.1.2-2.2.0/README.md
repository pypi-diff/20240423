# Comparing `tmp/cmind-2.1.2.tar.gz` & `tmp/cmind-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-2.1.2.tar", last modified: Wed Apr 17 14:59:01 2024, max compression
+gzip compressed data, was "cmind-2.2.0.tar", last modified: Tue Apr 23 18:02:44 2024, max compression
```

## Comparing `cmind-2.1.2.tar` & `cmind-2.2.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-17 14:58:51.000000 cmind-2.1.2/LICENSE.CK.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-17 14:58:51.000000 cmind-2.1.2/LICENSE.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-17 14:59:01.517098 cmind-2.1.2/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9978 2024-04-17 14:58:51.000000 cmind-2.1.2/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    28106 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.507098 cmind-2.1.2/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3958 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/repo/automation/ckx/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/ckx/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/ckx/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/ckx/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/repo/README-extra.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    38649 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    25274 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    42753 2024-04-17 14:58:51.000000 cmind-2.1.2/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-17 14:59:01.517098 cmind-2.1.2/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1293 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-17 14:59:01.000000 cmind-2.1.2/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-17 14:59:01.517098 cmind-2.1.2/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2927 2024-04-17 14:58:51.000000 cmind-2.1.2/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.541275 cmind-2.2.0/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-23 17:59:41.000000 cmind-2.2.0/LICENSE.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-23 18:02:44.541275 cmind-2.2.0/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11260 2024-04-23 17:59:41.000000 cmind-2.2.0/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    28644 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3958 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/ckx/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/ckx/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/ckx/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/ckx/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.541275 cmind-2.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.541275 cmind-2.2.0/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/README-extra.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    38748 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    25437 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47067 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1279 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-23 18:02:44.541275 cmind-2.2.0/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2913 2024-04-23 17:59:41.000000 cmind-2.2.0/setup.py
```

### Comparing `cmind-2.1.2/LICENSE.CK.md` & `cmind-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/PKG-INFO` & `cmind-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.1.2
+Version: 2.2.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.CK.md
 License-File: LICENSE.md
 
 [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
 [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
 [![Downloads](https://static.pepy.tech/badge/cmind)](https://pepy.tech/project/cmind)
 
@@ -222,17 +221,40 @@
 
 
 Please check the [**Getting Started Guide**](https://github.com/mlcommons/ck/blob/master/docs/getting-started.md) 
 to understand how CM automation recipes work, how to use them to automate your own projects,
 and how to implement and share new automations in your public or private projects.
 
 
+### Documentation
+
+**We plan to rewrite and simplify the CM documentation and tutorials based on user feedback in Q2 2024 - please stay tuned for more details**.
+
+* [News](../docs/news.md)
+* [Getting Started Guide and FAQ](../docs/getting-started.md)
+  * [Common CM interface to run MLPerf inference benchmarks](../docs/mlperf/inference)
+  * [Common CM interface to re-run experiments from ML and Systems papers including MICRO'23 and the Student Cluster Competition @ SuperComputing'23](../docs/tutorials/common-interface-to-reproduce-research-projects.md)
+  * [Other CM tutorials]../(docs/tutorials)
+* [Full documentation](../docs/README.md)
+
+
 ### License
 
 [Apache 2.0](LICENSE.md)
 
 ### Copyright
 
 2022-2024 [MLCommons](https://mlcommons.org)
 
+### Get in touch
+
+Collective Mind workflow automation framework and Collective Knowledge Playground are being developed 
+by the [MLCommons Task Force on Automation and Reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
+as a community effort. Volunteers are very welcome to help with this community project!
+
+### Acknowledgments
+
+CK and CM are community projects based on the feedback from our users and MLCommons members.
+We would like to thank all [collaborators and contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md) 
+for their support, fruitful discussions, and useful feedback!
```

### Comparing `cmind-2.1.2/README.md` & `cmind-2.2.0/cmind.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: cmind
+Version: 2.2.0
+Summary: cmind
+Home-page: https://github.com/mlcommons/ck
+Author: Grigori Fursin
+Author-email: Grigori.Fursin@cTuning.org
+License: Apache 2.0
+Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
 [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
 [![Downloads](https://static.pepy.tech/badge/cmind)](https://pepy.tech/project/cmind)
 
 [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
 [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
@@ -208,15 +221,40 @@
 
 
 Please check the [**Getting Started Guide**](https://github.com/mlcommons/ck/blob/master/docs/getting-started.md) 
 to understand how CM automation recipes work, how to use them to automate your own projects,
 and how to implement and share new automations in your public or private projects.
 
 
+### Documentation
+
+**We plan to rewrite and simplify the CM documentation and tutorials based on user feedback in Q2 2024 - please stay tuned for more details**.
+
+* [News](../docs/news.md)
+* [Getting Started Guide and FAQ](../docs/getting-started.md)
+  * [Common CM interface to run MLPerf inference benchmarks](../docs/mlperf/inference)
+  * [Common CM interface to re-run experiments from ML and Systems papers including MICRO'23 and the Student Cluster Competition @ SuperComputing'23](../docs/tutorials/common-interface-to-reproduce-research-projects.md)
+  * [Other CM tutorials]../(docs/tutorials)
+* [Full documentation](../docs/README.md)
+
+
 ### License
 
 [Apache 2.0](LICENSE.md)
 
 ### Copyright
 
 2022-2024 [MLCommons](https://mlcommons.org)
 
+### Get in touch
+
+Collective Mind workflow automation framework and Collective Knowledge Playground are being developed 
+by the [MLCommons Task Force on Automation and Reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
+as a community effort. Volunteers are very welcome to help with this community project!
+
+### Acknowledgments
+
+CK and CM are community projects based on the feedback from our users and MLCommons members.
+We would like to thank all [collaborators and contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md) 
+for their support, fruitful discussions, and useful feedback! 
+
+
```

### Comparing `cmind-2.1.2/cmind/artifact.py` & `cmind-2.2.0/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/automation.py` & `cmind-2.2.0/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/cli.py` & `cmind-2.2.0/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/config.py` & `cmind-2.2.0/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/core.py` & `cmind-2.2.0/cmind/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,14 +580,24 @@
         if artifact != '':
             # Parse artifact
             r = parse_cm_object_and_check_current_dir(self, artifact)
             if r['return'] >0 : return r
 
             i['parsed_artifact'] = r['cm_object']
 
+        # Check min CM version requirement
+        min_cm_version = automation_meta.get('min_cm_version','').strip()
+        if min_cm_version != '':
+            from cmind import __version__ as current_cm_version
+            comparison = utils.compare_versions(current_cm_version, min_cm_version)
+            if comparison < 0:
+                return {'return':1, 'error':'CM automation requires CM version >= {} while current CM version is {} - please update using "pip install cmind -U"'.format(min_cm_version, current_cm_version)}
+
+
+
         # Call automation action
         action_addr=getattr(initialized_automation, action)
 
         r = action_addr(i)
 
         # Check if need to save index
         if self.use_index and self.index.updated:
```

### Comparing `cmind-2.1.2/cmind/index.py` & `cmind-2.2.0/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/net.py` & `cmind-2.2.0/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/automation/README.md` & `cmind-2.2.0/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/automation/module.py` & `cmind-2.2.0/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/automation/module_dummy.py` & `cmind-2.2.0/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/automation/module_misc.py` & `cmind-2.2.0/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/ckx/README.md` & `cmind-2.2.0/cmind/repo/automation/ckx/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/ckx/module.py` & `cmind-2.2.0/cmind/repo/automation/ckx/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/core/README.md` & `cmind-2.2.0/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/core/module.py` & `cmind-2.2.0/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/repo/README.md` & `cmind-2.2.0/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repo/automation/repo/module.py` & `cmind-2.2.0/cmind/repo/automation/repo/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -986,15 +986,16 @@
         artifact_found_in_current_path = False
 
         if found:
             for reverse in [False, True]:
                 r=utils.find_file_in_current_directory_or_above([self.cmind.cfg['file_cmeta']+'.json', 
                                                                  self.cmind.cfg['file_cmeta']+'.yaml'],
                                                                  path_to_start = path,
-                                                                 reverse = reverse)
+                                                                 reverse = reverse,
+                                                                 path_to_stop = path_to_repo_real)
                 if r['return']>0: return r
 
                 artifact_found = r['found']
                 artifact_found_in_current_path = r.get('found_in_current_path', False)
 
                 rr['artifact_found'] = artifact_found
```

### Comparing `cmind-2.1.2/cmind/repo.py` & `cmind-2.2.0/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-2.1.2/cmind/repos.py` & `cmind-2.2.0/cmind/repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
                             r = utils.match_objects(existing_uid, existing_alias, d_uid, d_alias)
                             if r['return']>0: return r
                             match = r['match']
 
                             if match:
                                 if d.get('conflict', False):
-                                    return {'return':1, 'error':'Can\'t install this repository because it conflicts with the already installed one ({}) - you may need to remove it to proceed (cm rm repo {} --all)'.format(d_alias,d_alias)}
+                                    return {'return':1, 'error':'Can\'t install this repository because it conflicts with the already installed one ({}) - you may need to remove it to proceed (cm rm repo {})'.format(d_alias,d_alias)}
 
                                 d['matched'] = True
 
                                 break
 
                                     
                 # Check if has missing deps on other CM repos
@@ -293,15 +293,15 @@
         Clone or pull CM repository
 
         Args:
             alias (str): CM repository alias
             (url) (str): Git repository URL
             (branch) (str): Git repository branch
             (checkout) (str): Git repository checkout
-           (checkout_only) (bool): only checkout existing repo
+            (checkout_only) (bool): only checkout existing repo
             (depth) (int): Git repository depth
             (console) (bool): if True, print some info to console
             (desc) (str): optional repository description
             (prefix) (str): sub-directory to be used inside this CM repository to store artifacts
             (path_to_repo) (str): force path to repo (useful to pull imported repos with non-standard path)
             (checkout_only) (bool): only checkout Git repository but don't pull
             (skip_zip_parent_dir) (bool): skip parent dir in CM ZIP repo (useful when 
@@ -348,15 +348,18 @@
 
         cur_dir = os.getcwd()
 
         clone=False
 
         download=True if url.find('.zip')>0 else False
 
-        if not checkout_only:
+        if checkout_only:
+            if not os.path.isdir(path_to_repo):
+                return {'return':1, 'error':'Trying to checkout repo "{}" that was not pulled'.format(alias)}
+        else:
             if download:
                 # If CM repo already exists
                 if os.path.isdir(path_to_repo):
                     return {'return':1, 'error':'repository is already installed'}
 
                 os.makedirs(path_to_repo)
```

### Comparing `cmind-2.1.2/cmind/utils.py` & `cmind-2.2.0/cmind/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,45 @@
         return save_json(file_name, meta, sort_keys, encoding = encoding)
     elif file_name.endswith('.yaml'):
         return save_yaml(file_name, meta, sort_keys, encoding = encoding)
 
     return {'return':ERROR_UNKNOWN_FILE_EXTENSION, 'error':'unknown file extension'}
 
 ###########################################################################
+def safe_load_json(path, file_name='', encoding='utf8'):
+    """
+    Load JSON file if exists, otherwise return empty dict
+
+    Args:    
+       (CM input dict):
+
+       file_name (str): file name
+       (encoding) (str): file encoding ('utf8' by default)
+
+    Returns:
+       (CM return dict):
+
+       * return (int): return code == 0 if no error and >0 if error
+       * (error) (str): error string if return>0
+
+       * meta (dict): meta from the file
+
+    """
+
+    path_to_file = os.path.join(path, file_name) if file_name == '' or path != file_name else path
+
+    meta = {}
+
+    r = load_json(path_to_file, check_if_exists=True, encoding=encoding)
+    if r['return'] == 0:
+        meta = r['meta']
+
+    return {'return':0, 'meta': meta}
+
+###########################################################################
 def load_json(file_name, check_if_exists = False, encoding='utf8'):
     """
     Load JSON file.
 
     Args:    
        (CM input dict):
 
@@ -169,16 +200,15 @@
 
     with open(file_name, encoding=encoding) as jf:
         try:
             meta = json.load(jf)
         except Exception as e:
             return {'return':4, 'error': format(e)}
 
-    return {'return':0,
-            'meta': meta}
+    return {'return':0, 'meta': meta}
 
 ###########################################################################
 def save_json(file_name, meta={}, indent=2, sort_keys=True, encoding = 'utf8'):
     """
     Save meta to JSON file.
 
     Args:    
@@ -962,22 +992,24 @@
 
     api = string[line1+1:line_comment2+3]
 
     return {'return':0, 'api':api}
 
 
 ###########################################################################
-def find_file_in_current_directory_or_above(file_names, path_to_start = None, reverse = False):
+def find_file_in_current_directory_or_above(file_names, path_to_start = None, 
+        reverse = False, path_to_stop = None):
     """
     Find file(s) in the current directory or above.
 
     Args:
        file_names (list): files to find
        (path_to_start) (str): path to start; use current directory if None
        (reverse) (bool): if True search recursively in current directory and below.
+       (path_to_stop) (str): path to stop search (usually path to found repo)
 
     Returns:
        (CM return dict):
 
        * return (int): return code == 0 if no error and >0 if error
        * (error) (str): error string if return>0
 
@@ -1020,22 +1052,25 @@
               if not d.startswith('.'):
                   test_dir = os.path.join(current_path, d)
                   if os.path.isdir(test_dir):
                       new_path = test_dir
                       break
 
           if new_path == '':
-              break        
+              break
 
        else:
           new_path = os.path.dirname(current_path)
 
           if new_path == current_path:
               break
 
+          if path_to_stop != None and new_path == path_to_stop:
+              break
+
        found_in_current_path = False
 
        current_path = new_path
 
     r = {'return':0, 'found': found}
 
     if found:
@@ -1627,7 +1662,123 @@
 
     ex = e[1]
 
     os.chmod(p, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
     f(p)
 
     return
+
+##############################################################################
+def debug_here(module_path, host='localhost', port=5678, text='', env={}, env_debug_uid=''):
+    import os
+
+    if env_debug_uid!='':
+        if len(env)==0:
+            env = os.environ
+        x = env.get('CM_TMP_DEBUG_UID', '').strip()
+        if x.lower() != env_debug_uid.lower():
+            class dummy:
+               def breakpoint(self):
+                   return
+
+            return dummy()
+
+    workplace = os.path.dirname(module_path)
+
+    print ('~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~')
+    print ('Adding remote debug breakpoint ...')
+    if text != '':
+        print (text)
+
+    print ('')
+    import debugpy
+    debugpy.listen(port)
+
+    print ('')
+    print ('Waiting for debugger to attach ...')
+    print ('')
+    print ('Further actions for Visual Studio Code:')
+    print ('  Open Python file in VS to set breakpoint: {}'.format(module_path))
+    print ('  File -> Add Folder to Workplace: {}'.format(workplace))
+    print ('  Run -> Add configuration -> Python Debugger -> Remote attach -> {} -> {}'.format(host, port))
+    print ('     Сhange "remoteRoot" to ${workspaceFolder}')
+    print ('  Set breakpoint ...')
+    print ('  Run -> Start Debugging (or press F5) ...')
+    print ('')
+
+    debugpy.wait_for_client()
+
+    # Go up outside this function to continue debugging (F11 in VS)
+    return debugpy
+
+##############################################################################
+def compare_versions(version1, version2):
+    """
+    Compare versions
+
+    Args:    
+
+       version1 (str): version 1
+       version2 (str): version 2
+
+    Returns:
+       comparison (int):  1 - version 1 > version 2
+                          0 - version 1 == version 2
+                         -1 - version 1 < version 2
+    """
+
+    l_version1 = version1.split('.')
+    l_version2 = version2.split('.')
+
+    # 3.9.6 vs 3.9
+    # 3.9 vs 3.9.6
+
+    i_version1 = [int(v) if v.isdigit() else v for v in l_version1]
+    i_version2 = [int(v) if v.isdigit() else v for v in l_version2]
+
+    comparison = 0
+
+    for index in range(max(len(i_version1), len(i_version2))):
+        v1 = i_version1[index] if index < len(i_version1) else 0
+        v2 = i_version2[index] if index < len(i_version2) else 0
+
+        if v1 > v2:
+            comparison = 1
+            break
+        elif v1 < v2:
+            comparison = -1
+            break
+
+    return comparison
+
+##############################################################################
+def check_if_true_yes_on(env, key):
+    """
+    Universal check if str(env.get(key, '')).lower() in ['true', 'yes', 'on']:
+
+    Args:    
+
+       env (dict): dictionary
+       key (str): key
+
+    Returns:
+       True if str(env.get(key, '')).lower() in ['true', 'yes', 'on']:
+    """
+
+    return str(env.get(key, '')).lower() in ['true', 'yes', 'on']
+
+##############################################################################
+def check_if_none_false_no_off(env, key):
+    """
+    Universal check if str(env.get(key, '')).lower() in ['false', 'no', 'off']:
+
+    Args:    
+
+       env (dict): dictionary
+       key (str): key
+
+    Returns:
+       True if str(env.get(key, '')).lower() in ['false', 'no', 'off']:
+    """
+
+    return str(env.get(key, '')).lower() in ['none', 'false', 'no', 'off']
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmind-2.1.2/cmind.egg-info/PKG-INFO` & `cmind-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: cmind
-Version: 2.1.2
-Summary: cmind
-Home-page: https://github.com/mlcommons/ck
-Author: Grigori Fursin
-Author-email: Grigori.Fursin@cTuning.org
-License: Apache 2.0
-Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.CK.md
-License-File: LICENSE.md
-
 [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
 [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
 [![Downloads](https://static.pepy.tech/badge/cmind)](https://pepy.tech/project/cmind)
 
 [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
 [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
@@ -222,17 +208,38 @@
 
 
 Please check the [**Getting Started Guide**](https://github.com/mlcommons/ck/blob/master/docs/getting-started.md) 
 to understand how CM automation recipes work, how to use them to automate your own projects,
 and how to implement and share new automations in your public or private projects.
 
 
+### Documentation
+
+**We plan to rewrite and simplify the CM documentation and tutorials based on user feedback in Q2 2024 - please stay tuned for more details**.
+
+* [News](../docs/news.md)
+* [Getting Started Guide and FAQ](../docs/getting-started.md)
+  * [Common CM interface to run MLPerf inference benchmarks](../docs/mlperf/inference)
+  * [Common CM interface to re-run experiments from ML and Systems papers including MICRO'23 and the Student Cluster Competition @ SuperComputing'23](../docs/tutorials/common-interface-to-reproduce-research-projects.md)
+  * [Other CM tutorials]../(docs/tutorials)
+* [Full documentation](../docs/README.md)
+
+
 ### License
 
 [Apache 2.0](LICENSE.md)
 
 ### Copyright
 
 2022-2024 [MLCommons](https://mlcommons.org)
 
+### Get in touch
+
+Collective Mind workflow automation framework and Collective Knowledge Playground are being developed 
+by the [MLCommons Task Force on Automation and Reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
+as a community effort. Volunteers are very welcome to help with this community project!
 
+### Acknowledgments
 
+CK and CM are community projects based on the feedback from our users and MLCommons members.
+We would like to thank all [collaborators and contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md) 
+for their support, fruitful discussions, and useful feedback!
```

### Comparing `cmind-2.1.2/cmind.egg-info/SOURCES.txt` & `cmind-2.2.0/cmind.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.CK.md
 LICENSE.md
 README.md
 setup.py
 cmind/__init__.py
 cmind/__main__.py
 cmind/artifact.py
 cmind/automation.py
```

### Comparing `cmind-2.1.2/setup.py` & `cmind-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 import re
 
-from setuptools import find_packages, setup, convert_path
+from setuptools import find_packages, setup
 
 try:
     from setuptools.command.install import install
 except ImportError:
     from distutils.command.install import install
 
 # Get version
```

