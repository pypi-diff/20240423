# Comparing `tmp/casm-0.4.tar.gz` & `tmp/casm-0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casm-0.4.tar", last modified: Tue Apr 23 15:34:57 2024, max compression
+gzip compressed data, was "casm-0.4a1.tar", last modified: Wed Dec 13 16:20:54 2023, max compression
```

## Comparing `casm-0.4.tar` & `casm-0.4a1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/
--rw-r--r--   0 root         (0) root         (0)    18431 2023-11-28 14:52:30.000000 casm-0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      652 2024-04-23 15:34:57.667701 casm-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       31 2023-11-28 14:52:30.000000 casm-0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm/
--rw-r--r--   0 root         (0) root         (0)      392 2023-11-29 19:21:28.000000 casm-0.4/casm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm/cmds/
--rw-r--r--   0 root         (0) root         (0)     3345 2023-12-13 16:58:42.000000 casm-0.4/casm/cmds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm/cmds/modify/
--rw-r--r--   0 root         (0) root         (0)      426 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/modify/__init__.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/modify/assemble.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-12-12 17:20:02.000000 casm-0.4/casm/cmds/modify/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm/cmds/podman/
--rw-r--r--   0 root         (0) root         (0)      756 2023-12-02 16:05:35.000000 casm-0.4/casm/cmds/podman/__init__.py
--rw-r--r--   0 root         (0) root         (0)      544 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman/system.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm/cmds/podman_compose/
--rw-r--r--   0 root         (0) root         (0)      338 2023-12-02 14:38:43.000000 casm-0.4/casm/cmds/podman_compose/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/down.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/exec.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/logs.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/pause.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/pull.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/restart.py
--rw-r--r--   0 root         (0) root         (0)      720 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/start.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/stop.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/unpause.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-12-11 15:07:49.000000 casm-0.4/casm/cmds/podman_compose/up.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-12-12 17:20:02.000000 casm-0.4/casm/cmds/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm/utils/
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-23 15:34:02.000000 casm-0.4/casm/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4707 2023-12-13 15:59:15.000000 casm-0.4/casm/utils/assemble.py
--rw-r--r--   0 root         (0) root         (0)    15251 2023-12-13 15:36:13.000000 casm-0.4/casm/utils/compose.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-12-02 15:46:00.000000 casm-0.4/casm/utils/podman.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-12-02 15:38:29.000000 casm-0.4/casm/utils/podman_compose.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-12-02 09:09:24.000000 casm-0.4/casm/utils/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:34:57.667701 casm-0.4/casm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      652 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      970 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 15:34:57.000000 casm-0.4/casm.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     1019 2024-04-23 15:34:57.667701 casm-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       72 2023-11-28 16:16:02.000000 casm-0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:54.122975 casm-0.4a1/
+-rwxrwxrwx   0 root         (0) root         (0)    18431 2023-11-28 14:52:30.000000 casm-0.4a1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      654 2023-12-13 16:20:54.126523 casm-0.4a1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-11-28 14:52:30.000000 casm-0.4a1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:52.529586 casm-0.4a1/casm/
+-rwxrwxrwx   0 root         (0) root         (0)      392 2023-11-29 19:21:28.000000 casm-0.4a1/casm/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:52.756972 casm-0.4a1/casm/cmds/
+-rwxrwxrwx   0 root         (0) root         (0)     3369 2023-12-13 16:20:36.000000 casm-0.4a1/casm/cmds/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:52.890807 casm-0.4a1/casm/cmds/modify/
+-rwxrwxrwx   0 root         (0) root         (0)      426 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/modify/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      312 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/modify/assemble.py
+-rwxrwxrwx   0 root         (0) root         (0)     2156 2023-12-12 17:20:02.000000 casm-0.4a1/casm/cmds/modify/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:53.035936 casm-0.4a1/casm/cmds/podman/
+-rwxrwxrwx   0 root         (0) root         (0)      756 2023-12-02 16:05:35.000000 casm-0.4a1/casm/cmds/podman/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      544 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman/system.py
+-rwxrwxrwx   0 root         (0) root         (0)     1972 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman/systemd.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:53.740484 casm-0.4a1/casm/cmds/podman_compose/
+-rwxrwxrwx   0 root         (0) root         (0)      338 2023-12-02 14:38:43.000000 casm-0.4a1/casm/cmds/podman_compose/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      719 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/down.py
+-rwxrwxrwx   0 root         (0) root         (0)     1768 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/exec.py
+-rwxrwxrwx   0 root         (0) root         (0)     1073 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/logs.py
+-rwxrwxrwx   0 root         (0) root         (0)      728 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/pause.py
+-rwxrwxrwx   0 root         (0) root         (0)      726 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/pull.py
+-rwxrwxrwx   0 root         (0) root         (0)      732 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/restart.py
+-rwxrwxrwx   0 root         (0) root         (0)      720 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/start.py
+-rwxrwxrwx   0 root         (0) root         (0)      714 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/stop.py
+-rwxrwxrwx   0 root         (0) root         (0)      740 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/unpause.py
+-rwxrwxrwx   0 root         (0) root         (0)      729 2023-12-11 15:07:49.000000 casm-0.4a1/casm/cmds/podman_compose/up.py
+-rwxrwxrwx   0 root         (0) root         (0)     3372 2023-12-12 17:20:02.000000 casm-0.4a1/casm/cmds/service.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:54.069351 casm-0.4a1/casm/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      695 2023-12-13 16:19:23.000000 casm-0.4a1/casm/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4707 2023-12-13 15:59:15.000000 casm-0.4a1/casm/utils/assemble.py
+-rwxrwxrwx   0 root         (0) root         (0)    15251 2023-12-13 15:36:13.000000 casm-0.4a1/casm/utils/compose.py
+-rwxrwxrwx   0 root         (0) root         (0)     2116 2023-12-02 15:46:00.000000 casm-0.4a1/casm/utils/podman.py
+-rwxrwxrwx   0 root         (0) root         (0)     2825 2023-12-02 15:38:29.000000 casm-0.4a1/casm/utils/podman_compose.py
+-rwxrwxrwx   0 root         (0) root         (0)      697 2023-12-02 09:09:24.000000 casm-0.4a1/casm/utils/yaml.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-13 16:20:52.690326 casm-0.4a1/casm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      654 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      970 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       70 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-12-13 16:20:52.000000 casm-0.4a1/casm.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)     1004 2023-12-13 16:20:54.138501 casm-0.4a1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-11-28 16:16:02.000000 casm-0.4a1/setup.py
```

### Comparing `casm-0.4/LICENSE` & `casm-0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `casm-0.4/PKG-INFO` & `casm-0.4a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casm
-Version: 0.4
+Version: 0.4a1
 Summary: container assembler
 Home-page: https://github.com/podboy/casm
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/podboy/casm
 Project-URL: Bug Tracker, https://github.com/podboy/casm/issues
```

### Comparing `casm-0.4/casm/cmds/__init__.py` & `casm-0.4a1/casm/cmds/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding:utf-8
 
 from errno import ENOENT
 import os
+from typing import List
 from typing import Optional
 from typing import Sequence
 
 from xarg import add_command
 from xarg import argp
 from xarg import commands
 from xarg import run_command
```

### Comparing `casm-0.4/casm/cmds/modify/template.py` & `casm-0.4a1/casm/cmds/modify/template.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman/__init__.py` & `casm-0.4a1/casm/cmds/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman/system.py` & `casm-0.4a1/casm/cmds/podman/system.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman/systemd.py` & `casm-0.4a1/casm/cmds/podman/systemd.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/down.py` & `casm-0.4a1/casm/cmds/podman_compose/down.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/exec.py` & `casm-0.4a1/casm/cmds/podman_compose/exec.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/logs.py` & `casm-0.4a1/casm/cmds/podman_compose/logs.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/pause.py` & `casm-0.4a1/casm/cmds/podman_compose/pause.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/pull.py` & `casm-0.4a1/casm/cmds/podman_compose/pull.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/restart.py` & `casm-0.4a1/casm/cmds/podman_compose/restart.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/start.py` & `casm-0.4a1/casm/cmds/podman_compose/start.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/stop.py` & `casm-0.4a1/casm/cmds/podman_compose/stop.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/unpause.py` & `casm-0.4a1/casm/cmds/podman_compose/unpause.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/podman_compose/up.py` & `casm-0.4a1/casm/cmds/podman_compose/up.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/cmds/service.py` & `casm-0.4a1/casm/cmds/service.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/utils/__init__.py` & `casm-0.4a1/casm/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 from .podman_compose import podman_compose_cmd
 from .yaml import safe_load_data
 from .yaml import safe_load_file
 
 __package_name__ = "casm"
 __prog_name__ = "casm"
 __prog_compose__ = f"{__prog_name__}-compose"
-__version__ = "0.4"
+__version__ = "0.4.alpha.1"
 
 URL_PROG = "https://github.com/podboy/casm"
```

### Comparing `casm-0.4/casm/utils/assemble.py` & `casm-0.4a1/casm/utils/assemble.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/utils/compose.py` & `casm-0.4a1/casm/utils/compose.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/utils/podman.py` & `casm-0.4a1/casm/utils/podman.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/utils/podman_compose.py` & `casm-0.4a1/casm/utils/podman_compose.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm/utils/yaml.py` & `casm-0.4a1/casm/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `casm-0.4/casm.egg-info/PKG-INFO` & `casm-0.4a1/casm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casm
-Version: 0.4
+Version: 0.4a1
 Summary: container assembler
 Home-page: https://github.com/podboy/casm
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/podboy/casm
 Project-URL: Bug Tracker, https://github.com/podboy/casm/issues
```

### Comparing `casm-0.4/casm.egg-info/SOURCES.txt` & `casm-0.4a1/casm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casm-0.4/setup.cfg` & `casm-0.4a1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 	Documentation = https://github.com/podboy/casm
 
 [options]
 zip_safe = True
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	makefile-help
-	xarg-python >= 1.5
+	xarg-python >= 1.0
 	podman_compose >= 1.0.6
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	casm = casm.cmds:main
 	cman = casm.cmds.podman:main
```

