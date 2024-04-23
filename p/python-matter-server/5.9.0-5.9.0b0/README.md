# Comparing `tmp/python-matter-server-5.9.0.tar.gz` & `tmp/python-matter-server-5.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-5.9.0.tar", last modified: Thu Mar 28 19:32:10 2024, max compression
+gzip compressed data, was "python-matter-server-5.9.0b0.tar", last modified: Thu Mar  7 22:24:18 2024, max compression
```

## Comparing `python-matter-server-5.9.0.tar` & `python-matter-server-5.9.0b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.974574 python-matter-server-5.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-03-28 19:32:10.974574 python-matter-server-5.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.966574 python-matter-server-5.9.0/matter_server/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.966574 python-matter-server-5.9.0/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29249 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.966574 python-matter-server-5.9.0/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/models/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.970574 python-matter-server-5.9.0/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.970574 python-matter-server-5.9.0/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.970574 python-matter-server-5.9.0/matter_server/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-28 19:32:08.000000 python-matter-server-5.9.0/matter_server/dashboard/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.970574 python-matter-server-5.9.0/matter_server/dashboard/js/
--rw-r--r--   0 runner    (1001) docker     (127)    23240 2024-03-28 19:32:08.000000 python-matter-server-5.9.0/matter_server/dashboard/js/dialog-box-BgwoG2-2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-03-28 19:32:08.000000 python-matter-server-5.9.0/matter_server/dashboard/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    66796 2024-03-28 19:32:08.000000 python-matter-server-5.9.0/matter_server/dashboard/js/matter-dashboard-app-DK7p6YeT.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.970574 python-matter-server-5.9.0/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    59147 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.974574 python-matter-server-5.9.0/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/helpers/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/helpers/custom_web_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-28 19:31:54.000000 python-matter-server-5.9.0/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-03-28 19:31:59.000000 python-matter-server-5.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:10.974574 python-matter-server-5.9.0/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-28 19:32:10.000000 python-matter-server-5.9.0/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:32:10.974574 python-matter-server-5.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.119835 python-matter-server-5.9.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-03-07 22:24:18.119835 python-matter-server-5.9.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29228 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/models/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-07 22:24:15.000000 python-matter-server-5.9.0b0/matter_server/dashboard/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.111835 python-matter-server-5.9.0b0/matter_server/dashboard/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    23240 2024-03-07 22:24:15.000000 python-matter-server-5.9.0b0/matter_server/dashboard/js/dialog-box-3QS-wG6x.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-03-07 22:24:15.000000 python-matter-server-5.9.0b0/matter_server/dashboard/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66271 2024-03-07 22:24:15.000000 python-matter-server-5.9.0b0/matter_server/dashboard/js/matter-dashboard-app-BEx4IuJn.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.115835 python-matter-server-5.9.0b0/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59063 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.115835 python-matter-server-5.9.0b0/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/helpers/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/helpers/custom_web_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-07 22:24:02.000000 python-matter-server-5.9.0b0/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-07 22:24:04.000000 python-matter-server-5.9.0b0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:24:18.115835 python-matter-server-5.9.0b0/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-03-07 22:24:18.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-07 22:24:18.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 22:24:18.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-07 22:24:18.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 22:24:17.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-07 22:24:18.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-07 22:24:18.000000 python-matter-server-5.9.0b0/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 22:24:18.119835 python-matter-server-5.9.0b0/setup.cfg
```

### Comparing `python-matter-server-5.9.0/LICENSE` & `python-matter-server-5.9.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/PKG-INFO` & `python-matter-server-5.9.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 5.9.0
+Version: 5.9.0b0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -16,31 +16,31 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: dacite
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.3.2
+Requires-Dist: home-assistant-chip-clusters==2024.2.2
 Provides-Extra: server
-Requires-Dist: home-assistant-chip-core==2024.3.2; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.2.2; extra == "server"
 Requires-Dist: cryptography==42.0.5; extra == "server"
 Requires-Dist: zeroconf==0.131.0; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.2.6; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
-Requires-Dist: mypy==1.9.0; extra == "test"
-Requires-Dist: pre-commit==3.7.0; extra == "test"
+Requires-Dist: mypy==1.8.0; extra == "test"
+Requires-Dist: pre-commit==3.6.2; extra == "test"
 Requires-Dist: pre-commit-hooks==4.5.0; extra == "test"
 Requires-Dist: pylint==3.1.0; extra == "test"
-Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: pytest-asyncio==0.23.6; extra == "test"
+Requires-Dist: pytest==8.1.0; extra == "test"
+Requires-Dist: pytest-asyncio==0.23.5; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
-Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.3.4; extra == "test"
+Requires-Dist: pytest-cov==4.1.0; extra == "test"
+Requires-Dist: ruff==0.3.0; extra == "test"
 Requires-Dist: safety==3.0.1; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
```

### Comparing `python-matter-server-5.9.0/README.md` & `python-matter-server-5.9.0b0/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/client/client.py` & `python-matter-server-5.9.0b0/matter_server/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Matter Client implementation."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
 import logging
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, Final, Optional, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, Final, Optional, cast
 import uuid
 
 from aiohttp import ClientSession
 from chip.clusters import Objects as Clusters
 from chip.clusters.Types import NullValue
 
 from matter_server.common.errors import ERROR_MAP, NodeNotExists
@@ -59,16 +58,16 @@
 class MatterClient:
     """Manage a Matter server over WebSockets."""
 
     def __init__(self, ws_server_url: str, aiohttp_session: ClientSession):
         """Initialize the Client class."""
         self.connection = MatterClientConnection(ws_server_url, aiohttp_session)
         self.logger = logging.getLogger(__package__)
-        self._nodes: dict[int, MatterNode] = {}
-        self._result_futures: dict[str, asyncio.Future] = {}
+        self._nodes: Dict[int, MatterNode] = {}
+        self._result_futures: Dict[str, asyncio.Future] = {}
         self._subscribers: dict[str, list[Callable[[EventType, Any], None]]] = {}
         self._stop_called: bool = False
         self._loop: asyncio.AbstractEventLoop | None = None
 
     @property
     def server_info(self) -> ServerInfoMessage | None:
         """Return info of the server we're currently connected to."""
```

### Comparing `python-matter-server-5.9.0/matter_server/client/connection.py` & `python-matter-server-5.9.0b0/matter_server/client/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         assert self._ws_client
         ws_msg = await self._ws_client.receive()
 
         if ws_msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSED, WSMsgType.CLOSING):
             raise ConnectionClosed("Connection was closed.")
 
         if ws_msg.type == WSMsgType.ERROR:
-            raise ConnectionFailed
+            raise ConnectionFailed()
 
         if ws_msg.type != WSMsgType.TEXT:
             raise InvalidMessage(
                 f"Received non-Text message: {ws_msg.type}: {ws_msg.data}"
             )
 
         try:
```

### Comparing `python-matter-server-5.9.0/matter_server/client/exceptions.py` & `python-matter-server-5.9.0b0/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/client/models/clusters.py` & `python-matter-server-5.9.0b0/matter_server/client/models/clusters.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/client/models/device_types.py` & `python-matter-server-5.9.0b0/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/client/models/node.py` & `python-matter-server-5.9.0b0/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/common/errors.py` & `python-matter-server-5.9.0b0/matter_server/common/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Matter Exceptions."""
 
 from __future__ import annotations
 
+from typing import Type
+
 # mapping from error_code to Exception class
 ERROR_MAP: dict[int, type] = {}
 
 
 class MatterError(Exception):
     """Generic Matter exception."""
 
@@ -73,10 +75,10 @@
 
 class InvalidCommand(MatterError):
     """Error raised when there an unknown/invalid command is requested."""
 
     error_code = 9
 
 
-def exception_from_error_code(error_code: int) -> type[MatterError]:
+def exception_from_error_code(error_code: int) -> Type[MatterError]:
     """Return correct Exception class from error_code."""
     return ERROR_MAP.get(error_code, MatterError)
```

### Comparing `python-matter-server-5.9.0/matter_server/common/helpers/api.py` & `python-matter-server-5.9.0b0/matter_server/common/helpers/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Several helpers for the WebSockets API."""
 
 from __future__ import annotations
 
-from collections.abc import Callable, Coroutine
 from dataclasses import MISSING, dataclass
 import inspect
-from typing import Any, TypeVar, get_type_hints
+from typing import Any, Callable, Coroutine, TypeVar, get_type_hints
 
 from matter_server.common.helpers.util import parse_value
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 
 
 @dataclass
```

### Comparing `python-matter-server-5.9.0/matter_server/common/helpers/json.py` & `python-matter-server-5.9.0b0/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/common/helpers/util.py` & `python-matter-server-5.9.0b0/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/common/models.py` & `python-matter-server-5.9.0b0/matter_server/common/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Models that are (serializeable) shared between server and client."""
 
 from __future__ import annotations
 
-from collections.abc import Callable
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
-from typing import Any
+from typing import Any, Callable
 
 # Enums and constants
 
 
 class EventType(Enum):
     """Enum with possible events sent from server to client."""
```

### Comparing `python-matter-server-5.9.0/matter_server/dashboard/index.html` & `python-matter-server-5.9.0b0/matter_server/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/dashboard/js/dialog-box-BgwoG2-2.js` & `python-matter-server-5.9.0b0/matter_server/dashboard/js/dialog-box-3QS-wG6x.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
     T as d,
     i as c,
     t as h,
     c as p,
     o as v,
     d as m,
     m as g
-} from "./matter-dashboard-app-DK7p6YeT.js";
+} from "./matter-dashboard-app-BEx4IuJn.js";
 const u = {
         dialog: [
             [
                 [{
                     transform: "translateY(-50px)"
                 }, {
                     transform: "translateY(0)"
```

### Comparing `python-matter-server-5.9.0/matter_server/dashboard/js/main.js` & `python-matter-server-5.9.0b0/matter_server/dashboard/js/main.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -154,26 +154,24 @@
     }
     fireEvent(e, t) {
         const s = this.eventListeners[e];
         if (s)
             for (const e of s) e()
     }
 }!async function() {
-    import("./matter-dashboard-app-DK7p6YeT.js").then((function(e) {
+    import("./matter-dashboard-app-BEx4IuJn.js").then((function(e) {
         return e.f
     }));
     let e = "";
-    if (location.href.includes(":5010")) {
+    if (location.href.includes(":5580")) e = "ws" + new URL("./ws", location.href).toString().substring(4);
+    else {
         let t = localStorage.getItem("matterURL");
         if (!t) {
             if (t = prompt("Enter Websocket URL to a running Matter Server", "ws://localhost:5580/ws"), !t) return void alert("Unable to connect without URL");
             localStorage.setItem("matterURL", t)
         }
         e = t
-    } else {
-        let t = window.location.origin + window.location.pathname;
-        t.endsWith("/") && (t = t.slice(0, -1)), e = t.replace("http", "ws") + "/ws", console.log(`Connecting to Matter Server API using url: ${e}`)
     }
     const t = new o(e),
         s = document.createElement("matter-dashboard-app");
     s.client = t, document.body.append(s)
 }();
```

### Comparing `python-matter-server-5.9.0/matter_server/dashboard/js/matter-dashboard-app-DK7p6YeT.js` & `python-matter-server-5.9.0b0/matter_server/dashboard/js/matter-dashboard-app-BEx4IuJn.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -333,49 +333,49 @@
     R = "?" + S,
     I = `<${R}>`,
     P = document,
     k = () => P.createComment(""),
     T = t => null === t || "object" != typeof t && "function" != typeof t,
     L = Array.isArray,
     N = "[ \t\n\f\r]",
-    M = /<(?:(!--|\/[^a-zA-Z])|(\/?[a-zA-Z][^>\s]*)|(\/?$))/g,
-    H = /-->/g,
-    z = />/g,
-    U = RegExp(`>|${N}(?:([^\\s"'>=/]+)(${N}*=${N}*(?:[^ \t\n\f\r"'\`<>=]|("|')|))|$)`, "g"),
-    O = /'/g,
+    z = /<(?:(!--|\/[^a-zA-Z])|(\/?[a-zA-Z][^>\s]*)|(\/?$))/g,
+    M = /-->/g,
+    U = />/g,
+    O = RegExp(`>|${N}(?:([^\\s"'>=/]+)(${N}*=${N}*(?:[^ \t\n\f\r"'\`<>=]|("|')|))|$)`, "g"),
+    H = /'/g,
     D = /"/g,
-    V = /^(?:script|style|textarea|title)$/i,
-    B = t => (e, ...i) => ({
+    B = /^(?:script|style|textarea|title)$/i,
+    V = t => (e, ...i) => ({
         _$litType$: t,
         strings: e,
         values: i
     }),
-    F = B(1),
-    j = B(2),
+    F = V(1),
+    j = V(2),
     q = Symbol.for("lit-noChange"),
     K = Symbol.for("lit-nothing"),
     W = new WeakMap,
     G = P.createTreeWalker(P, 129);
 
 function Z(t, e) {
     if (!Array.isArray(t) || !t.hasOwnProperty("raw")) throw Error("invalid template strings array");
     return void 0 !== C ? C.createHTML(e) : e
 }
 const Y = (t, e) => {
     const i = t.length - 1,
         s = [];
     let r, o = 2 === e ? "<svg>" : "",
-        n = M;
+        n = z;
     for (let e = 0; e < i; e++) {
         const i = t[e];
         let a, l, d = -1,
             c = 0;
-        for (; c < i.length && (n.lastIndex = c, l = n.exec(i), null !== l);) c = n.lastIndex, n === M ? "!--" === l[1] ? n = H : void 0 !== l[1] ? n = z : void 0 !== l[2] ? (V.test(l[2]) && (r = RegExp("</" + l[2], "g")), n = U) : void 0 !== l[3] && (n = U) : n === U ? ">" === l[0] ? (n = r ?? M, d = -1) : void 0 === l[1] ? d = -2 : (d = n.lastIndex - l[2].length, a = l[1], n = void 0 === l[3] ? U : '"' === l[3] ? D : O) : n === D || n === O ? n = U : n === H || n === z ? n = M : (n = U, r = void 0);
-        const h = n === U && t[e + 1].startsWith("/>") ? " " : "";
-        o += n === M ? i + I : d >= 0 ? (s.push(a), i.slice(0, d) + E + i.slice(d) + S + h) : i + S + (-2 === d ? e : h)
+        for (; c < i.length && (n.lastIndex = c, l = n.exec(i), null !== l);) c = n.lastIndex, n === z ? "!--" === l[1] ? n = M : void 0 !== l[1] ? n = U : void 0 !== l[2] ? (B.test(l[2]) && (r = RegExp("</" + l[2], "g")), n = O) : void 0 !== l[3] && (n = O) : n === O ? ">" === l[0] ? (n = r ?? z, d = -1) : void 0 === l[1] ? d = -2 : (d = n.lastIndex - l[2].length, a = l[1], n = void 0 === l[3] ? O : '"' === l[3] ? D : H) : n === D || n === H ? n = O : n === M || n === U ? n = z : (n = O, r = void 0);
+        const h = n === O && t[e + 1].startsWith("/>") ? " " : "";
+        o += n === z ? i + I : d >= 0 ? (s.push(a), i.slice(0, d) + E + i.slice(d) + S + h) : i + S + (-2 === d ? e : h)
     }
     return [Z(t, o + (t[i] || "<?>") + (2 === e ? "</svg>" : "")), s]
 };
 class J {
     constructor({
         strings: t,
         _$litType$: e
@@ -406,15 +406,15 @@
                                 strings: i,
                                 ctor: "." === n[1] ? it : "?" === n[1] ? st : "@" === n[1] ? rt : et
                             }), s.removeAttribute(t)
                         } else t.startsWith(S) && (a.push({
                             type: 6,
                             index: r
                         }), s.removeAttribute(t));
-                if (V.test(s.tagName)) {
+                if (B.test(s.tagName)) {
                     const t = s.textContent.split(S),
                         e = t.length - 1;
                     if (e > 0) {
                         s.textContent = A ? A.emptyScript : "";
                         for (let i = 0; i < e; i++) s.append(t[i], k()), G.nextNode(), a.push({
                             type: 2,
                             index: ++r
@@ -1135,68 +1135,68 @@
         for (const i of Tt) null == t || t.removeEventListener(i, this), null == e || e.addEventListener(i, this)
     }
 }
 t([ut({
     type: Boolean,
     reflect: !0
 })], Nt.prototype, "disabled", void 0), t([mt()], Nt.prototype, "hovered", void 0), t([mt()], Nt.prototype, "pressed", void 0), t([ft(".surface")], Nt.prototype, "mdRoot", void 0);
-const Mt = n`:host{display:flex;margin:auto;pointer-events:none}:host([disabled]){display:none}@media(forced-colors: active){:host{display:none}}:host,.surface{border-radius:inherit;position:absolute;inset:0;overflow:hidden}.surface{-webkit-tap-highlight-color:rgba(0,0,0,0)}.surface::before,.surface::after{content:"";opacity:0;position:absolute}.surface::before{background-color:var(--md-ripple-hover-color, var(--md-sys-color-on-surface, #1d1b20));inset:0;transition:opacity 15ms linear,background-color 15ms linear}.surface::after{background:radial-gradient(closest-side, var(--md-ripple-pressed-color, var(--md-sys-color-on-surface, #1d1b20)) max(100% - 70px, 65%), transparent 100%);transform-origin:center center;transition:opacity 375ms linear}.hovered::before{background-color:var(--md-ripple-hover-color, var(--md-sys-color-on-surface, #1d1b20));opacity:var(--md-ripple-hover-opacity, 0.08)}.pressed::after{opacity:var(--md-ripple-pressed-opacity, 0.12);transition-duration:105ms}/*# sourceMappingURL=ripple-styles.css.map */
+const zt = n`:host{display:flex;margin:auto;pointer-events:none}:host([disabled]){display:none}@media(forced-colors: active){:host{display:none}}:host,.surface{border-radius:inherit;position:absolute;inset:0;overflow:hidden}.surface{-webkit-tap-highlight-color:rgba(0,0,0,0)}.surface::before,.surface::after{content:"";opacity:0;position:absolute}.surface::before{background-color:var(--md-ripple-hover-color, var(--md-sys-color-on-surface, #1d1b20));inset:0;transition:opacity 15ms linear,background-color 15ms linear}.surface::after{background:radial-gradient(closest-side, var(--md-ripple-pressed-color, var(--md-sys-color-on-surface, #1d1b20)) max(100% - 70px, 65%), transparent 100%);transform-origin:center center;transition:opacity 375ms linear}.hovered::before{background-color:var(--md-ripple-hover-color, var(--md-sys-color-on-surface, #1d1b20));opacity:var(--md-ripple-hover-opacity, 0.08)}.pressed::after{opacity:var(--md-ripple-pressed-opacity, 0.12);transition-duration:105ms}/*# sourceMappingURL=ripple-styles.css.map */
 `;
-let Ht = class extends Nt {};
-Ht.styles = [Mt], Ht = t([ct("md-ripple")], Ht);
-const zt = Symbol.for(""),
-    Ut = t => {
-        if ((null == t ? void 0 : t.r) === zt) return null == t ? void 0 : t._$litStatic$
+let Mt = class extends Nt {};
+Mt.styles = [zt], Mt = t([ct("md-ripple")], Mt);
+const Ut = Symbol.for(""),
+    Ot = t => {
+        if ((null == t ? void 0 : t.r) === Ut) return null == t ? void 0 : t._$litStatic$
     },
-    Ot = (t, ...e) => ({
+    Ht = (t, ...e) => ({
         _$litStatic$: e.reduce(((e, i, s) => e + (t => {
             if (void 0 !== t._$litStatic$) return t._$litStatic$;
             throw Error(`Value passed to 'literal' function must be a 'literal' result: ${t}. Use 'unsafeStatic' to pass non-literal values, but\n            take care to ensure page security.`)
         })(i) + t[s + 1]), t[0]),
-        r: zt
+        r: Ut
     }),
     Dt = new Map,
-    Vt = (t => (e, ...i) => {
+    Bt = (t => (e, ...i) => {
         const s = i.length;
         let r, o;
         const n = [],
             a = [];
         let l, d = 0,
             c = !1;
         for (; d < s;) {
-            for (l = e[d]; d < s && void 0 !== (o = i[d], r = Ut(o));) l += r + e[++d], c = !0;
+            for (l = e[d]; d < s && void 0 !== (o = i[d], r = Ot(o));) l += r + e[++d], c = !0;
             d !== s && a.push(o), n.push(l), d++
         }
         if (d === s && n.push(e[s]), c) {
             const t = n.join("$$lit$$");
             void 0 === (e = Dt.get(t)) && (n.raw = n, Dt.set(t, e = n)), i = a
         }
         return t(e, ...i)
     })(F),
-    Bt = ["ariaAtomic", "ariaAutoComplete", "ariaBusy", "ariaChecked", "ariaColCount", "ariaColIndex", "ariaColSpan", "ariaCurrent", "ariaDisabled", "ariaExpanded", "ariaHasPopup", "ariaHidden", "ariaInvalid", "ariaKeyShortcuts", "ariaLabel", "ariaLevel", "ariaLive", "ariaModal", "ariaMultiLine", "ariaMultiSelectable", "ariaOrientation", "ariaPlaceholder", "ariaPosInSet", "ariaPressed", "ariaReadOnly", "ariaRequired", "ariaRoleDescription", "ariaRowCount", "ariaRowIndex", "ariaRowSpan", "ariaSelected", "ariaSetSize", "ariaSort", "ariaValueMax", "ariaValueMin", "ariaValueNow", "ariaValueText"];
+    Vt = ["ariaAtomic", "ariaAutoComplete", "ariaBusy", "ariaChecked", "ariaColCount", "ariaColIndex", "ariaColSpan", "ariaCurrent", "ariaDisabled", "ariaExpanded", "ariaHasPopup", "ariaHidden", "ariaInvalid", "ariaKeyShortcuts", "ariaLabel", "ariaLevel", "ariaLive", "ariaModal", "ariaMultiLine", "ariaMultiSelectable", "ariaOrientation", "ariaPlaceholder", "ariaPosInSet", "ariaPressed", "ariaReadOnly", "ariaRequired", "ariaRoleDescription", "ariaRowCount", "ariaRowIndex", "ariaRowSpan", "ariaSelected", "ariaSetSize", "ariaSort", "ariaValueMax", "ariaValueMin", "ariaValueNow", "ariaValueText"];
 
 function Ft(t) {
     return t.replace("aria", "aria-").replace(/Elements?/g, "").toLowerCase()
 }
 
 function jt(t) {
-    for (const e of Bt) t.createProperty(e, {
+    for (const e of Vt) t.createProperty(e, {
         attribute: Ft(e),
         reflect: !0
     });
     t.addInitializer((t => {
         const e = {
             hostConnected() {
                 t.setAttribute("role", "presentation")
             }
         };
         t.addController(e)
     }))
 }
-Bt.map(Ft);
+Vt.map(Ft);
 const qt = Symbol("internals"),
     Kt = Symbol("privateInternals");
 
 function Wt(t) {
     return class extends t {
         get[qt]() {
             return this[Kt] || (this[Kt] = this.attachInternals()), this[Kt]
@@ -1250,24 +1250,24 @@
     get labels() {
         return this[qt].labels
     }
     willUpdate() {
         this.href && (this.disabled = !1)
     }
     render() {
-        const t = this.href ? Ot`div` : Ot`button`,
+        const t = this.href ? Ht`div` : Ht`button`,
             {
                 ariaLabel: e,
                 ariaHasPopup: i,
                 ariaExpanded: s
             } = this,
             r = e && this.ariaLabelSelected,
             o = this.toggle ? this.selected : K;
         let n = K;
-        return this.href || (n = r && this.selected ? this.ariaLabelSelected : e), Vt`<${t}
+        return this.href || (n = r && this.selected ? this.ariaLabelSelected : e), Bt`<${t}
         class="icon-button ${It(this.getRenderClasses())}"
         id="button"
         aria-label="${n||K}"
         aria-haspopup="${!this.href&&i||K}"
         aria-expanded="${!this.href&&s||K}"
         aria-pressed="${o}"
         ?disabled="${!this.href&&this.disabled}"
@@ -1659,25 +1659,25 @@
     `)
     }
     renderListItem(t) {
         const e = "link" === this.type;
         let i;
         switch (this.type) {
             case "link":
-                i = Ot`a`;
+                i = Ht`a`;
                 break;
             case "button":
-                i = Ot`button`;
+                i = Ht`button`;
                 break;
             default:
-                i = Ot`li`
+                i = Ht`li`
         }
         const s = "text" !== this.type,
             r = e && this.target ? this.target : K;
-        return Vt`
+        return Bt`
       <${i}
         id="item"
         tabindex="${this.isDisabled||!s?-1:0}"
         ?disabled=${this.isDisabled}
         role="listitem"
         aria-selected=${this.ariaSelected||K}
         aria-checked=${this.ariaChecked||K}
@@ -1873,15 +1873,15 @@
     }
     _disconnect() {
         localStorage.removeItem("matterURL"), location.reload()
     }
 };
 
 function Pe(t, e, i) {
-    return import("./dialog-box-BgwoG2-2.js"), new Promise((t => {
+    return import("./dialog-box-3QS-wG6x.js"), new Promise((t => {
         const s = document.createElement("dialox-box");
         s.params = i, s.dialogResult = t, s.type = e, document.body.appendChild(s)
     }))
 }
 Ie.styles = n`
     :host {
       display: flex;
@@ -1936,17 +1936,16 @@
       color: var(--md-sys-color-on-surface);
     }
 
     .footer a {
       color: var(--md-sys-color-on-surface);
     }
   `, t([ut()], Ie.prototype, "nodes", void 0), Ie = t([ct("matter-dashboard")], Ie);
-const ke = (t, e) => Pe(0, "alert", e),
-    Te = (t, e) => Pe(0, "prompt", e);
-let Le = class extends lt {
+const ke = (t, e) => Pe(0, "alert", e);
+let Te = class extends lt {
     render() {
         return this.node ? F`
       <div class="header">
         <a href="#">
           <md-icon-button>
             <ha-svg-icon .path=${Ce}></ha-svg-icon>
           </md-icon-button>
@@ -1954,17 +1953,14 @@
 
         <div>Node ${this.node.node_id}</div>
         <div class="flex"></div>
         <div class="actions">
           <md-icon-button @click=${this._reinterview} title="Reinterview node">
             <ha-svg-icon .path=${"M12,3C17.5,3 22,6.58 22,11C22,15.42 17.5,19 12,19C10.76,19 9.57,18.82 8.47,18.5C5.55,21 2,21 2,21C4.33,18.67 4.7,17.1 4.75,16.5C3.05,15.07 2,13.13 2,11C2,6.58 6.5,3 12,3M17,12V10H15V12H17M13,12V10H11V12H13M9,12V10H7V12H9Z"}></ha-svg-icon>
           </md-icon-button>
-          <md-icon-button @click=${this._remove} title="Remove node">
-            <ha-svg-icon .path=${"M9,3V4H4V6H5V19A2,2 0 0,0 7,21H17A2,2 0 0,0 19,19V6H20V4H15V3H9M9,8H11V17H9V8M13,8H15V17H13V8Z"}></ha-svg-icon>
-          </md-icon-button>
         </div>
       </div>
       <div class="container">
         <pre>${JSON.stringify(this.node.data,void 0,2)}</pre>
       </div>
     ` : F`
         <p>Node not found!</p>
@@ -1972,46 +1968,33 @@
           @click=${()=>{history.back()}}
         >
           Back
         </button>
       `
     }
     async _reinterview() {
-        if (await Te(0, {
+        var t;
+        if (await (t = {
                 title: "Reinterview",
                 text: "Are you sure you want to reinterview this node?",
                 confirmText: "Reinterview"
-            })) try {
+            }, Pe(0, "prompt", t))) try {
             await this.client.interviewNode(this.node.node_id), ke(0, {
                 title: "Reinterview node",
                 text: "Success!"
-            }), location.reload()
-        } catch (t) {
-            ke(0, {
-                title: "Failed to reinterview node",
-                text: t.message
             })
-        }
-    }
-    async _remove() {
-        if (await Te(0, {
-                title: "Remove",
-                text: "Are you sure you want to remove this node?",
-                confirmText: "Remove"
-            })) try {
-            await this.client.removeNode(this.node.node_id), location.replace("#")
         } catch (t) {
             ke(0, {
-                title: "Failed to remove node",
+                title: "Failed to reinterview node",
                 text: t.message
             })
         }
     }
 };
-Le.styles = n`
+Te.styles = n`
     :host {
       display: block;
       background-color: var(--md-sys-color-background);
     }
 
     .header {
       background-color: var(--md-sys-color-primary);
@@ -2033,16 +2016,16 @@
     }
 
     .container {
       padding: 16px;
       max-width: 600px;
       margin: 0 auto;
     }
-  `, t([ut()], Le.prototype, "node", void 0), Le = t([ct("matter-node-view")], Le);
-let Ne = class extends lt {
+  `, t([ut()], Te.prototype, "node", void 0), Te = t([ct("matter-node-view")], Te);
+let Le = class extends lt {
     render() {
         return F`
       <div class="header">
         <a href="#">
           <md-icon-button>
             <ha-svg-icon .path=${Ce}></ha-svg-icon>
           </md-icon-button>
@@ -2054,15 +2037,15 @@
       </div>
       <div class="container">
         <pre>${JSON.stringify(this.client.serverInfo,void 0,2)}</pre>
       </div>
     `
     }
 };
-Ne.styles = n`
+Le.styles = n`
     :host {
       display: flex;
       background-color: var(--md-sys-color-background);
       box-sizing: border-box;
       flex-direction: column;
       min-height: 100vh;
     }
@@ -2088,16 +2071,16 @@
 
     .container {
       padding: 16px;
       max-width: 600px;
       margin: 0 auto;
       flex: 1;
     }
-  `, Ne = t([ct("matter-server-view")], Ne);
-let Me = class extends lt {
+  `, Le = t([ct("matter-server-view")], Le);
+let Ne = class extends lt {
     constructor() {
         super(...arguments), this._route = {
             prefix: "",
             path: ""
         }, this._state = "connecting"
     }
     firstUpdated(t) {
@@ -2132,14 +2115,14 @@
       .route=${this._route}
     ></matter-dashboard>`
     }
     _clearLocalStorage() {
         localStorage.removeItem("matterURL"), location.reload()
     }
 };
-t([mt()], Me.prototype, "_route", void 0), t([mt()], Me.prototype, "_state", void 0), Me = t([ct("matter-dashboard-app")], Me);
-var He = Object.freeze({
+t([mt()], Ne.prototype, "_route", void 0), t([mt()], Ne.prototype, "_state", void 0), Ne = t([ct("matter-dashboard-app")], Ne);
+var ze = Object.freeze({
     __proto__: null
 });
 export {
-    Pt as E, K as T, t as _, mt as a, It as b, Gt as c, qt as d, ft as e, He as f, n as i, Wt as m, ut as n, yt as o, jt as r, lt as s, ct as t, F as x
+    Pt as E, K as T, t as _, mt as a, It as b, Gt as c, qt as d, ft as e, ze as f, n as i, Wt as m, ut as n, yt as o, jt as r, lt as s, ct as t, F as x
 };
```

### Comparing `python-matter-server-5.9.0/matter_server/server/__main__.py` & `python-matter-server-5.9.0b0/matter_server/server/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,15 @@
     help="Directory where PAA root certificates are stored.",
 )
 
 args = parser.parse_args()
 
 
 def _setup_logging() -> None:
-    log_fmt = (
-        "%(asctime)s.%(msecs)03d (%(threadName)s) %(levelname)s [%(name)s] %(message)s"
-    )
+    log_fmt = "%(asctime)s (%(threadName)s) %(levelname)s [%(name)s] %(message)s"
     custom_level_style = {
         **coloredlogs.DEFAULT_LEVEL_STYLES,
         "chip_automation": {"color": "green", "faint": True},
         "chip_detail": {"color": "green", "faint": True},
         "chip_progress": {},
         "chip_error": {"color": "red"},
     }
```

### Comparing `python-matter-server-5.9.0/matter_server/server/client_handler.py` & `python-matter-server-5.9.0b0/matter_server/server/client_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Logic to handle a client connected over WebSockets."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
 from concurrent import futures
 from contextlib import suppress
 import logging
-from typing import TYPE_CHECKING, Any, Final
+from typing import TYPE_CHECKING, Any, Callable, Final
 
 from aiohttp import WSMsgType, web
 import async_timeout
 from chip.exceptions import ChipStackError
 
 from matter_server.common.helpers.json import json_dumps, json_loads
 from matter_server.common.models import EventType
@@ -184,15 +183,15 @@
     async def _run_handler(
         self, handler: APICommandHandler, msg: CommandMessage
     ) -> None:
         try:
             try:
                 args = parse_arguments(handler.signature, handler.type_hints, msg.args)
             except (TypeError, KeyError, ValueError) as err:
-                raise InvalidArguments from err
+                raise InvalidArguments() from err
             result = handler.target(**args)
             if asyncio.iscoroutine(result):
                 result = await result
             self._send_message(SuccessResultMessage(msg.message_id, result))
         except (ChipStackError, MatterError) as err:
             error_code = getattr(err, "error_code", MatterError.error_code)
             message_str = msg.command
```

### Comparing `python-matter-server-5.9.0/matter_server/server/const.py` & `python-matter-server-5.9.0b0/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/server/device_controller.py` & `python-matter-server-5.9.0b0/matter_server/server/device_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 # pylint: disable=too-many-lines
 
 from __future__ import annotations
 
 import asyncio
 from collections import deque
-from collections.abc import Callable, Iterable
 from datetime import datetime
 from functools import partial
 import logging
 from pathlib import Path
 from random import randint
 import time
-from typing import TYPE_CHECKING, Any, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, TypeVar, cast
 
 from chip.ChipDeviceCtrl import DeviceProxyWrapper
 from chip.clusters import Attribute, Objects as Clusters
 from chip.clusters.Attribute import ValueDecodeFailure
 from chip.clusters.ClusterObjects import ALL_ATTRIBUTES, ALL_CLUSTERS, Cluster
 from chip.exceptions import ChipStackError
 from chip.native import PyChipError
@@ -35,14 +34,15 @@
     NodeNotReady,
     NodeNotResolving,
 )
 from ..common.helpers.api import api_command
 from ..common.helpers.util import (
     create_attribute_path_from_attribute,
     dataclass_from_dict,
+    dataclass_to_dict,
     parse_attribute_path,
     parse_value,
 )
 from ..common.models import (
     APICommand,
     EventType,
     MatterNodeData,
@@ -842,19 +842,34 @@
         if prev_sub := self._subscriptions.get(node_id, None):
             node_logger.info("Unsubscribing from existing subscription.")
             await self._call_sdk(prev_sub.Shutdown)
             del self._subscriptions[node_id]
 
         loop = cast(asyncio.AbstractEventLoop, self.server.loop)
 
-        def attribute_updated(
+        # set-up the actual subscription
+
+        def attribute_updated_callback(
             path: Attribute.TypedAttributePath,
-            old_value: Any,
-            new_value: Any,
+            transaction: Attribute.SubscriptionTransaction,
         ) -> None:
+            self._node_last_seen[node_id] = time.time()
+            new_value = transaction.GetAttribute(path)
+            # failsafe: ignore ValueDecodeErrors
+            # these are set by the SDK if parsing the value failed miserably
+            if isinstance(new_value, ValueDecodeFailure):
+                return
+
+            attr_path = str(path.Path)
+            old_value = node.attributes.get(attr_path)
+
+            # return early if the value did not actually change at all
+            if old_value == new_value:
+                return
+
             node_logger.debug(
                 "Attribute updated: %s - old value: %s - new value: %s",
                 path,
                 old_value,
                 new_value,
             )
 
@@ -863,15 +878,17 @@
                 node.is_bridge
                 and path.Path.EndpointId == 0
                 and path.AttributeType == Clusters.Descriptor.Attributes.PartsList
             ):
                 endpoints_removed = set(old_value or []) - set(new_value)
                 endpoints_added = set(new_value) - set(old_value or [])
                 if endpoints_removed:
-                    self._handle_endpoints_removed(node_id, endpoints_removed)
+                    loop.call_soon_threadsafe(
+                        self._handle_endpoints_removed, node_id, endpoints_removed
+                    )
                 if endpoints_added:
                     loop.create_task(
                         self._handle_endpoints_added(node_id, endpoints_added)
                     )
                 return
 
             # work out if software version changed
@@ -879,47 +896,27 @@
                 path.AttributeType == Clusters.BasicInformation.softwareVersion
                 and new_value != old_value
             ):
                 # schedule a full interview of the node if the software version changed
                 loop.create_task(self.interview_node(node_id))
 
             # store updated value in node attributes
-            attr_path = str(path.Path)
             node.attributes[attr_path] = new_value
 
             # schedule save to persistent storage
-            self._write_node_state(node_id)
+            loop.call_soon_threadsafe(self._write_node_state, node_id)
 
             # This callback is running in the CHIP stack thread
-            self.server.signal_event(
+            loop.call_soon_threadsafe(
+                self.server.signal_event,
                 EventType.ATTRIBUTE_UPDATED,
                 # send data as tuple[node_id, attribute_path, new_value]
                 (node_id, attr_path, new_value),
             )
 
-        def attribute_updated_callback(
-            path: Attribute.TypedAttributePath,
-            transaction: Attribute.SubscriptionTransaction,
-        ) -> None:
-            self._node_last_seen[node_id] = time.time()
-            new_value = transaction.GetAttribute(path)
-            # failsafe: ignore ValueDecodeErrors
-            # these are set by the SDK if parsing the value failed miserably
-            if isinstance(new_value, ValueDecodeFailure):
-                return
-
-            attr_path = str(path.Path)
-            old_value = node.attributes.get(attr_path)
-
-            # return early if the value did not actually change at all
-            if old_value == new_value:
-                return
-
-            loop.call_soon_threadsafe(attribute_updated, path, old_value, new_value)
-
         def event_callback(
             data: Attribute.EventReadResult,
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             # pylint: disable=unused-argument
             assert loop is not None
             node_logger.debug(
@@ -1004,15 +1001,14 @@
             == Clusters.ThreadNetworkDiagnostics.Enums.RoutingRoleEnum.kSleepyEndDevice
         ):
             interval_ceiling = NODE_SUBSCRIPTION_CEILING_BATTERY_POWERED
         else:
             interval_ceiling = NODE_SUBSCRIPTION_CEILING_THREAD
         self._last_subscription_attempt[node_id] = 0
         async with self._get_node_lock(node_id):
-            # set-up the actual subscription
             sub: Attribute.SubscriptionTransaction = await self.chip_controller.Read(
                 node_id,
                 attributes="*",
                 events=[("*", 1)],
                 returnClusterObject=False,
                 reportInterval=(interval_floor, interval_ceiling),
                 fabricFiltered=False,
@@ -1184,15 +1180,16 @@
                 "Attempting to resolve node %s... (attempt %s of %s)",
                 node_id,
                 attempt,
                 retries,
             )
             time_start = time.time()
             async with self._get_node_lock(node_id):
-                return await self.chip_controller.GetConnectedDevice(
+                return await self._call_sdk(
+                    self.chip_controller.GetConnectedDeviceSync,
                     nodeid=node_id,
                     allowPASE=False,
                     timeoutMs=None,
                 )
         except ChipStackError as err:
             if attempt >= retries:
                 # when we're out of retries, raise NodeNotResolving
@@ -1343,15 +1340,15 @@
     def _write_node_state(self, node_id: int, force: bool = False) -> None:
         """Schedule the write of the current node state to persistent storage."""
         if node_id not in self._nodes:
             return  # guard
         node = self._nodes[node_id]
         self.server.storage.set(
             DATA_KEY_NODES,
-            value=node,
+            value=dataclass_to_dict(node),
             subkey=str(node_id),
             force=force,
         )
 
     async def _node_offline(self, node_id: int) -> None:
         """Mark node as offline."""
         # shutdown existing subscriptions
```

### Comparing `python-matter-server-5.9.0/matter_server/server/helpers/attributes.py` & `python-matter-server-5.9.0b0/matter_server/server/helpers/attributes.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/server/helpers/custom_web_runner.py` & `python-matter-server-5.9.0b0/matter_server/server/helpers/custom_web_runner.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-5.9.0b0/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/server/helpers/utils.py` & `python-matter-server-5.9.0b0/matter_server/server/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/server/server.py` & `python-matter-server-5.9.0b0/matter_server/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Implementation of a Websocket-based server to proxy Matter support (using CHIP SDK)."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
 from functools import partial
 import ipaddress
 import logging
 import os
 from pathlib import Path
 import traceback
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Callable, Set, cast
 import weakref
 
 from aiohttp import web
 
 from matter_server.server.helpers.custom_web_runner import MultiHostTCPSite
 
 from ..common.const import SCHEMA_VERSION
@@ -122,15 +121,15 @@
         # Initialize our (intermediate) device controller which keeps track
         # of Matter devices and their subscriptions.
         self.device_controller = MatterDeviceController(self)
         self.storage = StorageController(self)
         self.vendor_info = VendorInfo(self)
         # we dynamically register command handlers
         self.command_handlers: dict[str, APICommandHandler] = {}
-        self._subscribers: set[EventCallBackType] = set()
+        self._subscribers: Set[EventCallBackType] = set()
         self._register_api_commands()
 
     async def start(self) -> None:
         """Start running the Matter server."""
         self.logger.info("Starting the Matter Server...")
         # safety shield: make sure we use same clusters and core packages!
         if chip_clusters_version() != chip_core_version():
```

### Comparing `python-matter-server-5.9.0/matter_server/server/stack.py` & `python-matter-server-5.9.0b0/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/matter_server/server/storage.py` & `python-matter-server-5.9.0b0/matter_server/server/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Logic to handle storage of persistent data."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
-from pathlib import Path
-from typing import TYPE_CHECKING, Any, cast
+import os
+from typing import TYPE_CHECKING, Any, Dict, cast
 
 from ..common.helpers.json import JSON_DECODE_EXCEPTIONS, json_dumps, json_loads
 
 if TYPE_CHECKING:
     from .server import MatterServer
 
 LOGGER = logging.getLogger(__name__)
@@ -18,31 +18,26 @@
 
 class StorageController:
     """Controller that handles storage of persistent data."""
 
     def __init__(self, server: "MatterServer") -> None:
         """Initialize storage controller."""
         self.server = server
-        self._data: dict[str, Any] = {}
+        self._data: Dict[str, Any] = {}
         self._timer_handle: asyncio.TimerHandle | None = None
         self._save_lock: asyncio.Lock = asyncio.Lock()
 
     @property
-    def filename(self) -> Path:
+    def filename(self) -> str:
         """Return full path to (fabric-specific) storage file."""
-        return Path(
+        return os.path.join(
             self.server.storage_path,
             f"{self.server.device_controller.compressed_fabric_id}.json",
         )
 
-    @property
-    def filename_backup(self) -> Path:
-        """Return full path to (fabric-specific) storage backup file."""
-        return self.filename.with_suffix(".json.backup")
-
     async def start(self) -> None:
         """Async initialize of controller."""
         await self._load()
         LOGGER.debug("Started.")
 
     async def stop(self) -> None:
         """Handle logic on server stop."""
@@ -101,18 +96,19 @@
         self.set(key, value)
 
     async def _load(self) -> None:
         """Load data from persistent storage."""
         assert not self._data, "Already loaded"
 
         def _load() -> dict:
-            for filename in self.filename, self.filename_backup:
+            for filename in self.filename, f"{self.filename}.backup":
                 LOGGER.debug("Loading persistent settings from %s", filename)
                 try:
-                    with open(filename, "r", encoding="utf-8") as _file:
+                    _filename = os.path.join(self.server.storage_path, filename)
+                    with open(_filename, "r", encoding="utf-8") as _file:
                         return cast(dict, json_loads(_file.read()))
                 except FileNotFoundError:
                     pass
                 except JSON_DECODE_EXCEPTIONS:  # pylint: disable=catching-non-exception
                     LOGGER.error(
                         "Error while reading persistent storage file %s", filename
                     )
@@ -147,17 +143,20 @@
             )
 
     async def async_save(self) -> None:
         """Save persistent data to disk."""
         assert self.server.loop is not None
 
         def do_save() -> None:
+            filename_backup = f"{self.filename}.backup"
             # make backup before we write a new file
-            if self.filename.is_file():
-                self.filename.replace(self.filename_backup)
+            if os.path.isfile(self.filename):
+                if os.path.isfile(filename_backup):
+                    os.remove(filename_backup)
+                os.rename(self.filename, filename_backup)
 
             with open(self.filename, "w", encoding="utf-8") as _file:
                 _file.write(json_dumps(self._data))
             LOGGER.debug("Saved data to persistent storage")
 
         async with self._save_lock:
             await self.server.loop.run_in_executor(None, do_save)
```

### Comparing `python-matter-server-5.9.0/matter_server/server/vendor_info.py` & `python-matter-server-5.9.0b0/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-5.9.0/pyproject.toml` & `python-matter-server-5.9.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,43 +19,43 @@
 dependencies = [
     "aiohttp",
     "aiorun",
     "async-timeout",
     "coloredlogs",
     "dacite",
     "orjson",
-    "home-assistant-chip-clusters==2024.3.2",
+    "home-assistant-chip-clusters==2024.2.2",
 ]
 description = "Python Matter WebSocket Server"
 name = "python-matter-server"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "5.9.0"
+version = "5.9.0b0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 server = [
-    "home-assistant-chip-core==2024.3.2",
+    "home-assistant-chip-core==2024.2.2",
     "cryptography==42.0.5",
     "zeroconf==0.131.0",
 ]
 test = [
     "codespell==2.2.6",
     "isort==5.13.2",
-    "mypy==1.9.0",
-    "pre-commit==3.7.0",
+    "mypy==1.8.0",
+    "pre-commit==3.6.2",
     "pre-commit-hooks==4.5.0",
     "pylint==3.1.0",
-    "pytest==8.1.1",
-    "pytest-asyncio==0.23.6",
+    "pytest==8.1.0",
+    "pytest-asyncio==0.23.5",
     "pytest-aiohttp==1.0.5",
-    "pytest-cov==5.0.0",
-    "ruff==0.3.4",
+    "pytest-cov==4.1.0",
+    "ruff==0.3.0",
     "safety==3.0.1",
     "tomli==2.0.1",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
@@ -170,14 +170,15 @@
     "S101",
     "TD002",
     "TD003",
     "TD004",
     "COM812",
     "ISC001",
     "TCH003",
+    "UP035",
     "TCH002",
     "TID252",
     "N805",
     "EXE002",
     "T201",
     "ANN201",
     "UP032",
@@ -217,14 +218,15 @@
     "N818",
     "N815",
     "N801",
     "N813",
     "RUF012",
     "TCH001",
     "ANN102",
+    "RSE102",
     "B007",
     "SIM102",
     "C901",
     "PLR0911",
     "PLR0912",
     "SLF001",
     "RUF010",
@@ -238,14 +240,17 @@
     "TRY201",
     "A002",
     "DTZ003",
     "N803",
     "ARG002",
     "S104",
     "UP015",
+    "PTH113",
+    "PTH107",
+    "PTH104",
 ]
 select = [
     "ALL",
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
```

### Comparing `python-matter-server-5.9.0/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-5.9.0b0/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 5.9.0
+Version: 5.9.0b0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -16,31 +16,31 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: dacite
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.3.2
+Requires-Dist: home-assistant-chip-clusters==2024.2.2
 Provides-Extra: server
-Requires-Dist: home-assistant-chip-core==2024.3.2; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.2.2; extra == "server"
 Requires-Dist: cryptography==42.0.5; extra == "server"
 Requires-Dist: zeroconf==0.131.0; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.2.6; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
-Requires-Dist: mypy==1.9.0; extra == "test"
-Requires-Dist: pre-commit==3.7.0; extra == "test"
+Requires-Dist: mypy==1.8.0; extra == "test"
+Requires-Dist: pre-commit==3.6.2; extra == "test"
 Requires-Dist: pre-commit-hooks==4.5.0; extra == "test"
 Requires-Dist: pylint==3.1.0; extra == "test"
-Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: pytest-asyncio==0.23.6; extra == "test"
+Requires-Dist: pytest==8.1.0; extra == "test"
+Requires-Dist: pytest-asyncio==0.23.5; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
-Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.3.4; extra == "test"
+Requires-Dist: pytest-cov==4.1.0; extra == "test"
+Requires-Dist: ruff==0.3.0; extra == "test"
 Requires-Dist: safety==3.0.1; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
```

### Comparing `python-matter-server-5.9.0/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-5.9.0b0/python_matter_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 matter_server/common/const.py
 matter_server/common/errors.py
 matter_server/common/models.py
 matter_server/common/helpers/api.py
 matter_server/common/helpers/json.py
 matter_server/common/helpers/util.py
 matter_server/dashboard/index.html
-matter_server/dashboard/js/dialog-box-BgwoG2-2.js
+matter_server/dashboard/js/dialog-box-3QS-wG6x.js
 matter_server/dashboard/js/main.js
-matter_server/dashboard/js/matter-dashboard-app-DK7p6YeT.js
+matter_server/dashboard/js/matter-dashboard-app-BEx4IuJn.js
 matter_server/server/__init__.py
 matter_server/server/__main__.py
 matter_server/server/client_handler.py
 matter_server/server/const.py
 matter_server/server/device_controller.py
 matter_server/server/server.py
 matter_server/server/stack.py
```

