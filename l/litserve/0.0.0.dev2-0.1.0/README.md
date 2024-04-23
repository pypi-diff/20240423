# Comparing `tmp/litserve-0.0.0.dev2.tar.gz` & `tmp/litserve-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litserve-0.0.0.dev2.tar", last modified: Thu Mar  7 23:37:06 2024, max compression
+gzip compressed data, was "litserve-0.1.0.tar", last modified: Tue Apr 23 13:09:27 2024, max compression
```

## Comparing `litserve-0.0.0.dev2.tar` & `litserve-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:37:06.074189 litserve-0.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-07 23:37:06.074189 litserve-0.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 23:37:06.074189 litserve-0.0.0.dev2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4107 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:37:06.070189 litserve-0.0.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:37:06.070189 litserve-0.0.0.dev2/src/litserve/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/src/litserve/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/src/litserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/src/litserve/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-03-07 23:36:56.000000 litserve-0.0.0.dev2/src/litserve/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:37:06.074189 litserve-0.0.0.dev2/src/litserve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-07 23:37:06.000000 litserve-0.0.0.dev2/src/litserve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-07 23:37:06.000000 litserve-0.0.0.dev2/src/litserve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 23:37:06.000000 litserve-0.0.0.dev2/src/litserve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 23:37:06.000000 litserve-0.0.0.dev2/src/litserve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-07 23:37:06.000000 litserve-0.0.0.dev2/src/litserve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-07 23:37:06.000000 litserve-0.0.0.dev2/src/litserve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:09:27.535761 litserve-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-23 13:09:17.000000 litserve-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-23 13:09:17.000000 litserve-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-23 13:09:27.535761 litserve-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-04-23 13:09:17.000000 litserve-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 13:09:17.000000 litserve-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:09:27.535761 litserve-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4688 2024-04-23 13:09:17.000000 litserve-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:09:27.531761 litserve-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:09:27.531761 litserve-0.1.0/src/litserve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-23 13:09:17.000000 litserve-0.1.0/src/litserve/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-23 13:09:17.000000 litserve-0.1.0/src/litserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-23 13:09:17.000000 litserve-0.1.0/src/litserve/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-23 13:09:17.000000 litserve-0.1.0/src/litserve/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 13:09:17.000000 litserve-0.1.0/src/litserve/python_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-04-23 13:09:17.000000 litserve-0.1.0/src/litserve/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:09:27.535761 litserve-0.1.0/src/litserve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-23 13:09:27.000000 litserve-0.1.0/src/litserve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-23 13:09:27.000000 litserve-0.1.0/src/litserve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:09:27.000000 litserve-0.1.0/src/litserve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:09:27.000000 litserve-0.1.0/src/litserve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 13:09:27.000000 litserve-0.1.0/src/litserve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 13:09:27.000000 litserve-0.1.0/src/litserve.egg-info/top_level.txt
```

### Comparing `litserve-0.0.0.dev2/LICENSE` & `litserve-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litserve-0.0.0.dev2/MANIFEST.in` & `litserve-0.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `litserve-0.0.0.dev2/setup.py` & `litserve-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 #!/usr/bin/env python
+# Copyright The Lightning AI team.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import glob
 import os
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 
 from pkg_resources import parse_requirements
 from setuptools import find_packages, setup
```

