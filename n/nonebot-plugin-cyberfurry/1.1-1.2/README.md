# Comparing `tmp/nonebot_plugin_cyberfurry-1.1.tar.gz` & `tmp/nonebot_plugin_cyberfurry-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cyberfurry-1.1.tar", last modified: Mon Apr 22 08:09:36 2024, max compression
+gzip compressed data, was "nonebot_plugin_cyberfurry-1.2.tar", last modified: Tue Apr 23 08:13:48 2024, max compression
```

## Comparing `nonebot_plugin_cyberfurry-1.1.tar` & `nonebot_plugin_cyberfurry-1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/callapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurrymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43856 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 08:09:36.000000 nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 08:09:28.000000 nonebot_plugin_cyberfurry-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:09:36.398002 nonebot_plugin_cyberfurry-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:13:48.449279 nonebot_plugin_cyberfurry-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43964 2024-04-23 08:13:48.449279 nonebot_plugin_cyberfurry-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:13:48.445279 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/callapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberfurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberfurrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:13:48.445279 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43964 2024-04-23 08:13:48.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-23 08:13:48.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:13:48.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 08:13:48.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 08:13:48.000000 nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-23 08:13:44.000000 nonebot_plugin_cyberfurry-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:13:48.449279 nonebot_plugin_cyberfurry-1.2/setup.cfg
```

### Comparing `nonebot_plugin_cyberfurry-1.1/LICENSE` & `nonebot_plugin_cyberfurry-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/PKG-INFO` & `nonebot_plugin_cyberfurry-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.1
+Version: 1.2
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,14 +684,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
+Requires-Dist: nonebot-plugin-localstore
 Requires-Dist: aiohttp
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -763,20 +764,22 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-若未配置此插件将不会工作!!!!
+若未配置必填项此插件将不会工作!!!!
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
+| cubplugin_datadir | 否 | "" | 插件数据文件夹 |
+
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
```

### Comparing `nonebot_plugin_cyberfurry-1.1/README.md` & `nonebot_plugin_cyberfurry-1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,22 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-若未配置此插件将不会工作!!!!
+若未配置必填项此插件将不会工作!!!!
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
+| cubplugin_datadir | 否 | "" | 插件数据文件夹 |
+
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
```

#### html2text {}

```diff
@@ -11,16 +11,17 @@
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cyberfurry pdm pdm add nonebot-plugin-cyberfurry
 poetry poetry add nonebot-plugin-cyberfurry conda conda install nonebot-plugin-
 cyberfurry æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_cyberfurry"] ##
 âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
-è¥æªéç½®æ­¤æä»¶å°ä¸ä¼å·¥ä½!!!! | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | |:-----:|:----:|:----:|:----:| | cf_appid | æ¯ | æ  | APIçappid |
-| cf_token | æ¯ | æ  | APIçtoken | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ |
-æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /
-chat /cf /yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å
-| å¦ | ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
+è¥æªéç½®å¿å¡«é¡¹æ­¤æä»¶å°ä¸ä¼å·¥ä½!!!! | éç½®é¡¹ | å¿å¡« |
+é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | cf_appid | æ¯ | æ  |
+APIçappid | | cf_token | æ¯ | æ  | APIçtoken | | cubplugin_datadir | å¦
+| "" | æä»¶æ°æ®æä»¶å¤¹ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /chat /cf /
+yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å | å¦ |
+ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
 è®¾å®ä½¿ç¨çyinyingæ¨¡å,æ³¨æ,æ­¤ä¸ºä¸ªäººéç½® | | cfå½åæ¨¡å |
 ç¾¤å | å¦ | ä»»æ | æ¥çå½åæ¨¡å | | cfè®¾å® furåå­ furç§æ |
 ç¾¤å | å¦ | ä»»æ | è®¾å®ä¼ å¥yinyingçèªèº«è®¾å® |
```

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/__init__.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/callapi.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/callapi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurry.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberfurry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberfurrymodel.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberfurrymodel.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberhistory.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberhistory.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/cyberinit.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/cyberinit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/data_source.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/jsondata.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/jsondata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 from loguru import logger
-from .plugins_data import initdata,wdata,rdata,driver
+from .plugins_data import initdata,wdata,rdata,driver,data_dir
 import os
 from datetime import datetime
 jsonname = "cyberfurry.json"
 txtdir = "cyberfurry"
 bashdata = {
     "status":1,
     "qqname":{},
     "usermodel":{},
     "userdata":{},
     "userchat":{}
 }
 initdata(jsonname,bashdata)
-if not os.path.isdir("plugins_data/"+txtdir):
-    os.mkdir("plugins_data/"+txtdir)
+txt_dir =  data_dir / txtdir
+if not os.path.isdir(txt_dir):
+    os.mkdir(txt_dir)
 
 def writehistory(
     chat_id:str,
     text:str
 ):
     data = chat_id.split("-")
-    file_path="plugins_data/"+txtdir+f"/{data[1]}"
+    file_path=txt_dir+f"/{data[1]}"
     if not os.path.isdir(file_path):
         os.mkdir(file_path)
     with open(file_path+"/"+data[-1]+".txt",'a') as f:
         f.write(text)
 
 def gethistorylist(
     user_id:str
 ):
-    file_path="plugins_data/"+txtdir+f"/{user_id}/"
+    file_path=txt_dir+f"/{user_id}/"
     filelist = os.listdir(file_path)
     flist = []
     for name in filelist:
         flist.append(name.split(".")[0])
     if len(flist)>=5:
         return flist[-5:].sort()
     else:
         return flist.sort()
 
 def gethistorytxt(
     user_id:str,
     filename:str
 ):
-    file_path="plugins_data/"+txtdir+f"/{user_id}"
+    file_path=txt_dir+f"/{user_id}"
     filelist = os.listdir(file_path)
     if filename+".txt" in filelist:
-        return os.getcwd()+"/"+file_path+"/"+filename+".txt"
+        return file_path+"/"+filename+".txt"
     else:
         return False
 
 def getdate():
     now = datetime.now() # current date and time
     date_time = now.strftime("%y%m%d")
     return (date_time)
```

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry/plugins_data.py` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry/plugins_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 from pathlib import Path
-#from util.config import *
+from .config import config
 from nonebot import get_driver
 import os
 import json
 from nonebot.log import logger
 driver = get_driver()
-# 插件数据代理
+if config.cubplugin_datadir=="":
+    from nonebot import require
+    require("nonebot_plugin_localstore")
+    import nonebot_plugin_localstore as store
+    # 插件数据代理
+    data_dir = store.get_data_dir("cubplugins")
 
-path_name="plugins_data"
-dir_path = Path(Path(path_name)).absolute()
-
-if dir_path.is_dir():
-    logger.opt(colors=True).debug(f"\033[1;36;43m[plugin_data]\033[0m根目录正常-\<{path_name}\>")
+    logger.warning("未配置自定义数据文件夹,将使用localstore路径->"+str(data_dir))
 else:
-    #os.mkdir(path_name)
-    os.mkdir(dir_path)
-    logger.opt(colors=True).debug(f"\033[1;36;43m[plugin_data]\033[0m初始化根目录\<{path_name}\>")
+    path_name=config.cubplugin_datadir
+    data_dir = Path(Path(path_name)).absolute()
+    logger.debug("已配置自定义数据文件夹!->"+str(data_dir))
+
+    if data_dir.is_dir():
+        logger.opt(colors=True).debug(f"[plugin_data]\033[0m根目录正常-\<{path_name}\>")
+    else:
+        #os.mkdir(path_name)
+        os.mkdir(data_dir)
+        logger.opt(colors=True).debug(f"[plugin_data]\033[0m初始化根目录\<{path_name}\>")
 
 def initdata(
     conf_name,
     bashdata:dict={"status":1}
 ):
-    conf_path = Path(dir_path / conf_name).absolute()
+    conf_path = Path(data_dir / conf_name).absolute()
     config_init(conf_path,conf_name,"plugin_data",bashdata)
     return True
 
 def rdata(
     conf_name
 ):
-    conf_path = Path(dir_path / conf_name).absolute()
+    conf_path = Path(data_dir / conf_name).absolute()
     with open(conf_path, "r", encoding="utf-8") as f:
         data = json.loads(f.read())
     return data
 
 def wdata(
     conf_name:str,
     data:dict
 ):
-    conf_path = Path(dir_path / conf_name).absolute()
+    conf_path = Path(data_dir / conf_name).absolute()
     with open(conf_path, "w", encoding="utf-8") as f:
         f.write(json.dumps(data, indent=4,ensure_ascii=False))
     return True
 
 def config_init(
     _path_ ,
     conf_name:str ,
@@ -52,8 +60,9 @@
         logger.opt(colors=True).debug(f"\033[1;36;43m[util]\033[0m>>><W>{module_name}</>>>>{conf_name}-OK!")
     else:
         logger.opt(colors=True).debug(f"\033[1;36;43m[util]\033[0m>>><W>{module_name}</>>>>Create-{conf_name}!")
         with open(_path_, "w", encoding="utf-8") as f:
             f.write(json.dumps(data, indent=4))
             f.close()
 
-#本插件由 cubstaryow 编写
+#本插件由 cubstaryow 编写
+# plugins_data 为 cubplugins_util.plugins_data 移植
```

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/PKG-INFO` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.1
+Version: 1.2
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,14 +684,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
+Requires-Dist: nonebot-plugin-localstore
 Requires-Dist: aiohttp
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-cyberfurry/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -763,20 +764,22 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-若未配置此插件将不会工作!!!!
+若未配置必填项此插件将不会工作!!!!
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
+| cubplugin_datadir | 否 | "" | 插件数据文件夹 |
+
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
```

### Comparing `nonebot_plugin_cyberfurry-1.1/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt` & `nonebot_plugin_cyberfurry-1.2/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.1/pyproject.toml` & `nonebot_plugin_cyberfurry-1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-cyberfurry"
-version = "1.1"
+version = "1.2"
 description = "nonebot插件 cyberfurry-与赛博狼狼对话吧~"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -14,12 +14,13 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 dependencies = [
   "nonebot-adapter-onebot",
   "nonebot2",
+  "nonebot-plugin-localstore",
   "aiohttp"
 ]
 
 [project.urls]
 repository = "https://github.com/cubstaryow/nonebot-plugin-cyberfurry"
```

