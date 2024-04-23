# Comparing `tmp/nonebot_plugin_helpwithpic-1.3.1.tar.gz` & `tmp/nonebot_plugin_helpwithpic-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helpwithpic-1.3.1.tar", last modified: Mon Apr 22 08:39:32 2024, max compression
+gzip compressed data, was "nonebot_plugin_helpwithpic-1.4.tar", last modified: Mon Apr 22 09:05:58 2024, max compression
```

## Comparing `nonebot_plugin_helpwithpic-1.3.1.tar` & `nonebot_plugin_helpwithpic-1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44288 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/draw_contect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/hwp_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44288 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:05:58.001829 nonebot_plugin_helpwithpic-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44233 2024-04-22 09:05:58.001829 nonebot_plugin_helpwithpic-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:05:57.997829 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/draw_contect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/hwp_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:05:58.001829 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44233 2024-04-22 09:05:57.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 09:05:57.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:05:57.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 09:05:57.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 09:05:57.000000 nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-22 09:05:54.000000 nonebot_plugin_helpwithpic-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:05:58.001829 nonebot_plugin_helpwithpic-1.4/setup.cfg
```

### Comparing `nonebot_plugin_helpwithpic-1.3.1/LICENSE` & `nonebot_plugin_helpwithpic-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/PKG-INFO` & `nonebot_plugin_helpwithpic-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helpwithpic
-Version: 1.3.1
+Version: 1.4
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -686,15 +686,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
 Requires-Dist: httpx
 Requires-Dist: aiohttp
-Requires-Dist: nonebot-plugin-send-anything-anywhere
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

### Comparing `nonebot_plugin_helpwithpic-1.3.1/README.md` & `nonebot_plugin_helpwithpic-1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/__init__.py` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/config.py` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
     #superusers: Set[str] = set() 以后可能会内置权限检查器，现在用不到
     hwp_font: Optional[str] = None
     hwp_custom_bg: List[str] = []
     version: str = "Unknow"
     hwp_commandstart :str = "#"
     hwp_nickname:str ="本BOT的帮助文档"
     hwp_text:str =  "你想要的,我们都没有(不是\n不知道写啥了"
-    hwp_version:str="HelpWithPic-Beta1.3.1"
+    hwp_version:str="HelpWithPic-Beta1.4"
 
 config: config_hwp = config_hwp.parse_obj(get_driver().config.dict())
 #本插件由 cubstaryow 编写
```

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/draw.py` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/draw_contect.py` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/draw_contect.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/jsondata.py` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/plugins_data.py` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helpwithpic
-Version: 1.3.1
+Version: 1.4
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -686,15 +686,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
 Requires-Dist: httpx
 Requires-Dist: aiohttp
-Requires-Dist: nonebot-plugin-send-anything-anywhere
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

### Comparing `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt` & `nonebot_plugin_helpwithpic-1.4/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.3.1/pyproject.toml` & `nonebot_plugin_helpwithpic-1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-helpwithpic"
-version = "1.3.1"
+version = "1.4"
 description = "nonebot插件-动态帮助图片制作"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -16,14 +16,13 @@
 ]
 
 dependencies = [
   "nonebot-adapter-onebot",
   "nonebot2",
   "httpx",
   "aiohttp",
-  "nonebot-plugin-send-anything-anywhere",
   "pil_utils",
   "pillow"
 ]
 
 [project.urls]
 repository = "https://github.com/cubstaryow/nonebot-plugin-HelpWithPic"
```

