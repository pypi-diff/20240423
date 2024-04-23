# Comparing `tmp/nonebot_plugin_cyberfurry-1.0.tar.gz` & `tmp/nonebot_plugin_cyberfurry-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cyberfurry-1.0.tar", last modified: Mon Apr 22 07:56:37 2024, max compression
+gzip compressed data, was "nonebot_plugin_cyberfurry-1.1.tar", last modified: Mon Apr 22 08:09:36 2024, max compression
```

## Comparing `nonebot_plugin_cyberfurry-1.0.tar` & `nonebot_plugin_cyberfurry-1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:56:37.039976 nonebot_plugin_cyberfurry-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-04-22 07:56:37.039976 nonebot_plugin_cyberfurry-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:56:37.035976 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/callapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberfurry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberfurrymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:56:37.035976 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-04-22 07:56:37.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 07:56:37.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:56:37.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 07:56:37.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 07:56:37.000000 nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 07:56:33.000000 nonebot_plugin_cyberfurry-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:56:37.039976 nonebot_plugin_cyberfurry-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/callapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/setup.cfg
```

### Comparing `nonebot_plugin_cyberfurry-1.0/LICENSE` & `nonebot_plugin_cyberfurry-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/PKG-INFO` & `nonebot_plugin_cyberfurry-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.0
+Version: 1.1
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_cyberfurry-1.0/README.md` & `nonebot_plugin_cyberfurry-1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/__init__.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/callapi.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/callapi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberfurry.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberfurrymodel.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurrymodel.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberhistory.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberhistory.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/cyberinit.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberinit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 
 from nonebot.adapters.onebot.v11 import (
    Bot ,MessageSegment
 )
 from nonebot.matcher import Matcher
 from .cyberfurry import *
-from nonebot.adapters.telegram.event import MessageEvent as TGevent
+
 from nonebot.adapters.onebot.v11 import MessageEvent as obV11event
 from nonebot.params import CommandArg
 from nonebot import on_command
+try:
+    from nonebot.adapters.telegram.event import MessageEvent as TGevent
+except:
+    TGevent = obV11event
 
 MessageEvent = TGevent | obV11event
 
 run = on_command(
     "/chat",
     aliases={"/yy","/cf"} ,
     priority=25
```

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/data_source.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/jsondata.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry/plugins_data.py` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/PKG-INFO` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.0
+Version: 1.1
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_cyberfurry-1.0/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt` & `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.0/pyproject.toml` & `nonebot_plugin_cyberfurry-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-cyberfurry"
-version = "1.0"
+version = "1.1"
 description = "nonebot插件 cyberfurry-与赛博狼狼对话吧~"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

