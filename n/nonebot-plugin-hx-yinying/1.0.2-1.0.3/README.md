# Comparing `tmp/nonebot-plugin-hx-yinying-1.0.2.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.2.tar", last modified: Mon Apr 22 13:45:25 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.3.tar", last modified: Mon Apr 22 21:13:23 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.0.2.tar` & `nonebot-plugin-hx-yinying-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 13:45:25.003872 nonebot-plugin-hx-yinying-1.0.2/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4083 2024-04-22 13:45:25.008884 nonebot-plugin-hx-yinying-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3643 2024-04-22 08:30:49.000000 nonebot-plugin-hx-yinying-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 13:45:24.925827 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    12196 2024-04-22 13:20:39.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    32062 2024-04-22 13:44:32.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      396 2024-04-22 13:19:10.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:45:24.992760 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     4083 2024-04-22 13:45:24.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-22 13:45:24.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 13:45:24.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2024-04-22 13:45:24.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-22 13:45:24.000000 nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-22 13:45:25.033874 nonebot-plugin-hx-yinying-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-22 13:13:01.000000 nonebot-plugin-hx-yinying-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:13:23.846971 nonebot-plugin-hx-yinying-1.0.3/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4083 2024-04-22 21:13:23.846971 nonebot-plugin-hx-yinying-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3643 2024-04-22 08:30:49.000000 nonebot-plugin-hx-yinying-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 21:13:23.736576 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    19380 2024-04-22 21:04:06.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    41996 2024-04-22 21:12:22.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      396 2024-04-22 21:13:07.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:13:23.834269 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     4083 2024-04-22 21:13:23.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-22 21:13:23.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 21:13:23.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-04-22 21:13:23.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-22 21:13:23.000000 nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-22 21:13:23.846971 nonebot-plugin-hx-yinying-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-22 21:13:17.000000 nonebot-plugin-hx-yinying-1.0.3/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.0.2/LICENSE` & `nonebot-plugin-hx-yinying-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.2/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.2
+Version: 1.0.3
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.3 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.0.2/README.md` & `nonebot-plugin-hx-yinying-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -- coding: utf-8 --**
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent ,MessageSegment ,Message
-from nonebot.adapters.onebot.v11 import MessageSegment as MS
-from nonebot.matcher import Matcher
 from html import unescape
-from typing import Dict, List, Literal, Union
-import os,httpx, json, datetime, time, requests
+from typing import List
+import os,httpx, json, time, requests
 from .config import Config
 from nonebot import get_plugin_config, logger, require
-from datetime import datetime
 hx_config = get_plugin_config(Config)
 from pathlib import Path
 require("nonebot_plugin_localstore")
 import nonebot_plugin_localstore as store
 
 
 if hx_config.hx_path == None:
@@ -103,26 +100,38 @@
     nick = info["nickname"]
     if nick is None:
         nick = None
     else:
         nick = nick
     return nick
 
-#全局发送消息函数，发送消息直接await就行
-async def send_msg(matcher, event, content):
-    if hx_config.hx_reply == True:
-        await matcher.send(MessageSegment.reply(event.message_id) + content)
+
+#结果消息函数，发送消息直接await就行
+async def send_msg_reject(matcher, event, content):
+    config_global = config_in_global()
+    reply_config = json_get(config_global,"reply")
+    if reply_config == True:
+        await matcher.reject(MessageSegment.reply(event.message_id) + content)
     else:
-        await matcher.send(content, at_sender=hx_config.hx_reply_at)
+        reply_at = json_get(config_global,"reply_at")
+        await matcher.reject(content, at_sender=reply_at)
+
 
 #创建用户文件夹
 def create_dir_usr(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
+#json转义防止爆炸（）
+def json_replace(text) -> str:
+    text = text.replace('\n','\\n')
+    text = text.replace('\t','\\t')
+    text = text.replace("'","\\'")
+    text = text.replace('"','\\"')
+    return text
 
 #初始化log记录
 def log_in()-> str:
     try:
         if os.path.exists(f"{log_dir}/chat/all_log.json"):
             with open(f'{log_dir}/chat/all_log.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
@@ -157,25 +166,27 @@
 #用户输入
 def user_in(id, text):
     data = log_in()
     if f'{id}' in data: 
         id_log = data[f'{id}']['log']
         package = {}
         package['rule'] = 'user'
-        package['msg'] = f'{text}'
+        text_r = json_replace(text)
+        package['msg'] = f'{text_r}'
         id_log.append(package)
         data[f'{id}']['log'] = id_log
         with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
             json.dump(data,file)
     else : 
         package = {}
         log = {}
         history_package = []
         package['rule'] = 'user'
-        package['msg'] = f'{text}'
+        text_r = json_replace(text)
+        package['msg'] = f'{text_r}'
         history_package.append(package)
         log['log'] = history_package
         dt = time.time()
         t = int(dt)
         log['time'] = t
         data[f'{id}'] = log
         with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
@@ -184,45 +195,99 @@
 #AI输出
 def ai_out(id, text):
     data = log_in()
     if f'{id}' in data: 
         id_log = data[f'{id}']['log']
         package = {}
         package['rule'] = 'ai'
-        package['msg'] = f'{text}'
+        text_r = json_replace(text)
+        package['msg'] = f'{text_r}'
         id_log.append(package)
         data[f'{id}']['log'] = id_log
         with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
             json.dump(data,file)
     else : 
         package = {}
         log = {}
         history_package = []
         package['rule'] = 'ai'
-        package['msg'] = f'{text}'
+        text_r = json_replace(text)
+        package['msg'] = f'{text_r}'
         history_package.append(package)
         log['log'] = history_package
         dt = time.time()
         t = int(dt)
         log['time'] = t
         data[f'{id}'] = log
         with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
             json.dump(data,file)
 
+#载入本地保存的easycyber预设(一些情况下失败时不会清空，请找到专业人员修复)
+def easycyber_in(cybernick,json_1) -> str:
+    try:
+        if os.path.exists(f"{log_dir}/config/easycyber.json"):
+            with open(f'{log_dir}/config/easycyber.json','r',encoding='utf-8') as file:
+                json_data = json.load(file)
+                if cybernick in json_data or not json_1 or not cybernick:
+                    back = json_data
+                else:
+                    dt = time.time()
+                    t = int(dt)
+                    dw = int(len(json_data) + 1)
+                    package_easycyberfurry = json_1
+                    package_easycyberfurry["create_time"] = t
+                    package_easycyberfurry["last_update"] = t
+                    package_easycyberfurry["public"] = False
+                    package_easycyberfurry["id"] = dw
+                    json_data[f"{cybernick}"] = package_easycyberfurry
+                    with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                        json.dump(json_data,file)
+                    back = json_data
+        else:
+            create_dir_usr(f"{log_dir}/config")
+            with open(f'{log_dir}/config/easycyber.json','w',encoding='utf-8') as file:
+                dt = time.time()
+                t = int(dt)
+                global_easycyberfurry = {}
+                package_easycyberfurry = {}
+                package_easycyberfurry["cfNickname"] = "Hx"
+                package_easycyberfurry["cfSpecies"] = "龙狼"
+                package_easycyberfurry["cfConAge"] = "child"
+                package_easycyberfurry["cfConStyle"] = "sentiment"
+                package_easycyberfurry["cfStory"] = "相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。"
+                package_easycyberfurry["create_by"] = 3485462167
+                package_easycyberfurry["create_time"] = t
+                package_easycyberfurry["last_update"] = t
+                package_easycyberfurry["public"] = True
+                package_easycyberfurry["id"] = 0
+                global_easycyberfurry["Hx"] = package_easycyberfurry
+                packages_easycyberfurry = json_1
+                packages_easycyberfurry["create_time"] = t
+                packages_easycyberfurry["last_update"] = t
+                packages_easycyberfurry["public"] = True
+                packages_easycyberfurry["id"] = 1
+                global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
+                json.dump(global_easycyberfurry,file)
+                back = global_easycyberfurry
+    except Exception as e:
+            logger.error(f"加载本地cyberfurry预设时失败！，请不要随意修改bot插件本地文件。。。。！")
+            logger.warning("你要为你的行为负责，来自不知名开发者")
+            logger.warning(f"报错捕获{e}")
+            back = False
+    return back
+
 #载入全局本地配置
 def config_in_global() -> str:
     try:
         if os.path.exists(f"{log_dir}/config/config_global.json"):
             with open(f'{log_dir}/config/config_global.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 back = json_data
         else:
             create_dir_usr(f"{log_dir}/config")
-            logger.error(f"加载全局配置时失败！，请不要随意修改bot插件本地文件,现已重置所有群聊配置")
-            logger.warning("你要为你的行为负责，来自不知名开发者")
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json_data = {}
                 global_cyberfurry = {}
                 global_easycyberfurry = {}
                 black_user = []
                 black_group = []
                 black_world = []
@@ -246,26 +311,30 @@
                 package_easycyberfurry["create_time"] = 1713710000
                 package_easycyberfurry["last_update"] = 1713710923
                 package_easycyberfurry["public"] = True
                 package_easycyberfurry["id"] = 0
                 global_easycyberfurry["Hx"] = package_easycyberfurry
                 json_data['global_switch'] = True
                 json_data['limit'] = 12
+                json_data['at_reply'] = True
                 json_data['reply'] = False
                 json_data['reply_at'] = False
                 json_data['private'] = True
                 json_data['blacklist_user'] = black_user
                 json_data['blacklist_group'] = black_group
                 json_data['blacklist_world'] = black_world
                 json_data['cyberfurry'] = global_cyberfurry
                 json_data['easycyberfurry'] = global_easycyberfurry
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
             create_dir_usr(f"{log_dir}/config")
+            logger.error(f"加载全局配置时失败！，请不要随意修改bot插件本地文件,现已重置所有群聊配置")
+            logger.warning("你要为你的行为负责，来自不知名开发者")
+            logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json_data = {}
                 global_cyberfurry = {}
                 global_easycyberfurry = {}
                 black_user = []
                 black_group = []
                 black_world = []
@@ -338,14 +407,15 @@
                 id_package['last_chattime'] = t
                 json_data[f"{groupid}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
             logger.error(f"加载群聊{groupid}配置时失败！，请不要随意修改bot插件本地文件,现已重置所有群聊配置")
             logger.warning("你要为你的行为负责，来自不知名开发者")
+            logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
                 dt = time.time()
                 t = int(dt)
                 json_data = {}
                 id_package = {}
                 id_package['use_model'] = "yinyingllm-v2"
                 id_package['chat_alltimes'] = 0
@@ -358,31 +428,32 @@
 
 #载入个人本地配置
 def config_in_user(id,nick) -> str:
     try:
         if os.path.exists(f"{log_dir}/config/config_user.json"):
             with open(f'{log_dir}/config/config_user.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
-                if id in json_data:
+                if id in json_data or not nick:
                     back = json_data
                 else:
                     dt = time.time()
                     t = int(dt)
                     id_package = {}
                     id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
                     id_package['character_in'] = True
                     id_package['private_model'] = "yinyingllm-v2"
                     id_package['chat_alltimes'] = 0
                     id_package['times'] = 1
                     id_package['time'] = 1713710000
                     id_package['first_chattime'] = t
                     id_package['last_chattime'] = t
                     json_data[f"{id}"] = id_package
-                    json.dump(json_data,file)
-                    back = json_data
+                    with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                        json.dump(json_data,file)
+                        back = json_data
         else:
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
                 dt = time.time()
                 t = int(dt)
                 json_data = {}
                 id_package = {}
@@ -396,14 +467,15 @@
                 id_package['last_chattime'] = t
                 json_data[f"{id}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
             logger.error(f"加载用户{id}配置时失败！，请不要随意修改bot插件本地文件,现已重置所有用户配置")
             logger.warning("你要为你的行为负责，来自不知名开发者")
+            logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
                 dt = time.time()
                 t = int(dt)
                 json_data = {}
                 id_package = {}
                 id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
                 id_package['character_in'] = True
@@ -466,33 +538,41 @@
                 user_id=3485462167,
                 nickname="AAA星佑批发（幻歆限定）",
                 content=Message("合并消息时出错！"),
             )
         ]
     return msg_list
 
+#全局配置卡片构建
 async def get_config_global() -> List[MessageSegment]:
     config = config_in_global()
     msg_list = []
     try:
         reply = config["reply"]
         reply_at = config["reply_at"]
         global_switch = config["global_switch"]
         private = config["private"]
         limit = config["limit"]
+        at_reply = config["at_reply"]
         msg_list.append(
                 MessageSegment.node_custom(
                 user_id=3202123263,
                 nickname="AAA星佑批发（Hx限定）",
                 content=Message(f"全局开启状态:{global_switch}"),                    
                 ))
         msg_list.append(
                 MessageSegment.node_custom(
                 user_id=3202123263,
                 nickname="AAA星佑批发（Hx限定）",
+                content=Message(f"bot被艾特或回复是否回应:{at_reply}"),                    
+                ))
+        msg_list.append(
+                MessageSegment.node_custom(
+                user_id=3202123263,
+                nickname="AAA星佑批发（Hx限定）",
                 content=Message(f"对话回复开启状态:{reply}"),                    
                 ))
         msg_list.append(
                 MessageSegment.node_custom(
                 user_id=3202123263,
                 nickname="AAA星佑批发（Hx限定）",
                 content=Message(f"回复艾特开启状态:{reply_at}\n请注意：该配置项和对话回复冲突，当对话回复开启时，该配置项无效！"),                    
@@ -526,15 +606,15 @@
         ]
     return msg_list
 
 #检测对话次数
 def chat_times(id,nick) -> int:
     data = log_in()
     history = data[f"{id}"]['log']
-    times = len(history)/2
+    times = int(len(history)/2 + 0.5)
     limit = json_get(config_in_global(),"limit")
     config = config_in_user(id,nick)
     if times >= limit:
         dt = time.time()
         t = int(dt)
         data[f'{id}']['time'] = t
         data[f"{id}"]['log'] = []
@@ -609,83 +689,173 @@
     packages_data['appId'] = f'{hx_config.yinying_appid}'
     user_config = config_in_user(id,nick)
     group_config = config_in_group(groupid)
     id_config = json_get(user_config,id)
     group_config = json_get(group_config,groupid)
     character = json_get(id_config,"character")
     time = json_get(id_config,"time")
-    model = json_get(group_config,"use_model")
+    model_group = json_get(group_config,"use_model")
     try:
-        if model == None or model == "yinyingllm-v2":
-            logger.warning("找不到配置里的yinying_model或你设置的模型为yinyingllm-v2,将使用默认模型llm2")
-            packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
-            packages_data['model'] = 'yinyingllm-v2'
-            package = {}
-            package['nickName'] = f'{nick}'
-            package['furryCharacter'] = f'{character}'
-            allvariables.update(package)
-            packages_data['variables'] = allvariables
-            packages_data['message'] = f'{text}'
-        elif model == "yinyingllm-v1":
-            packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v1'
-            package = {}
-            package['nickName'] = f'{nick}'
-            package['furryCharacter'] = f'{character}'
-            allvariables.update(package)
-            packages_data['variables'] = allvariables
-            packages_data['message'] = f'{text}'
-        elif model == "yinyingllm-v3":
-            packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v3'
-            package = {}
-            package['nickName'] = f'{nick}'
-            package['furryCharacter'] = f'{character}'
-            allvariables.update(package)
-            packages_data['variables'] = allvariables
-            packages_data['message'] = f'{text}'
-        elif model == "cyberfurry-001":
-            packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-cyberfurry-001'
-            packages_data['model'] = 'cyberfurry-001'
-            packages_data['systemPrompt'] = "你的名字叫Hx"
-            packages_data['message'] = f'{text}'
-        elif model == "easycyberfurry-001":
-            packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-            packages_data['model'] = 'easycyberfurry-001'
-            characterSet = {}
-            package = {}
-            package['nickName'] = f'{nick}'
-            package['furryCharacter'] = f'{character}'
-            allvariables.update(package)
-            new_package = {}
-            new_package['cfNickname'] = '幻歆'
-            new_package['cfSpecies'] = '龙狼'
-            new_package['cfConAge'] = 'child'
-            new_package['cfConStyle'] = 'social_anxiety'
-            new_package['cfStory'] = '由幻歆创造'
-            characterSet.update(new_package)
-            packages_data['variables'] = allvariables
-            packages_data['characterSet'] = characterSet
-            packages_data['message'] = f'{text}'
+        if not model_group or groupid == None:
+            model = json_get(id_config,"private_model")
+            if model == None or model == "yinyingllm-v2":
+                logger.warning("找不到配置里的yinying_model或你设置的模型为yinyingllm-v2,将使用默认模型llm2")
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
+                packages_data['model'] = 'yinyingllm-v2'
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
+                packages_data['message'] = f'{text}'
+            elif model == "yinyingllm-v1":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v1'
+                packages_data['message'] = f'{text}'
+            elif model == "yinyingllm-v3":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v3'
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
+                packages_data['message'] = f'{text}'
+            elif model == "cyberfurry-001":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-cyberfurry-001'
+                packages_data['model'] = 'cyberfurry-001'
+                packages_data['systemPrompt'] = "你的名字叫Hx"
+                packages_data['message'] = f'{text}'
+            elif model == "easycyberfurry-001":
+                if json_get(id_config,"character_in") == True or not json_get(id_config,"character_in"):
+                    logger.warning("okokok1")
+                    packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
+                    packages_data['model'] = 'easycyberfurry-001'
+                    characterSet = {}
+                    package = {}
+                    package['nickName'] = f'{nick}'
+                    package['furryCharacter'] = f'{character}'
+                    allvariables.update(package)
+                    new_package = {}
+                    new_package['cfNickname'] = 'Hx'
+                    new_package['cfSpecies'] = '龙狼'
+                    new_package['cfConAge'] = 'child'
+                    new_package['cfConStyle'] = 'social_anxiety'
+                    new_package['cfStory'] = '你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。'
+                    characterSet.update(new_package)
+                    packages_data['variables'] = allvariables
+                    packages_data['characterSet'] = characterSet
+                    packages_data['message'] = f'{text}'
+                else:
+                    logger.warning("okokok2")
+                    promte_model = json_get(id_config,"character_in")
+                    promte = json_get(easycyber_in(promte_model,False),f"{promte_model}")
+                    if not promte:
+                        packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
+                        packages_data['model'] = 'easycyberfurry-001'
+                        characterSet = {}
+                        package = {}
+                        package['nickName'] = f'{nick}'
+                        package['furryCharacter'] = f'{character}'
+                        allvariables.update(package)
+                        new_package = {}
+                        new_package['cfNickname'] = 'Hx'
+                        new_package['cfSpecies'] = '龙狼'
+                        new_package['cfConAge'] = 'child'
+                        new_package['cfConStyle'] = 'social_anxiety'
+                        new_package['cfStory'] = '你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。'
+                        characterSet.update(new_package)
+                        packages_data['variables'] = allvariables
+                        packages_data['characterSet'] = characterSet
+                        packages_data['message'] = f'{text}'
+                    else:
+                        logger.warning("okokok3")
+                        packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
+                        packages_data['model'] = 'easycyberfurry-001'
+                        package = {}
+                        package['nickName'] = f'{nick}'
+                        package['furryCharacter'] = f'{character}'
+                        allvariables.update(package)
+                        new_package = {}
+                        new_package['cfNickname'] = f"{promte['cfNickname']}"
+                        new_package['cfSpecies'] = f"{promte['cfSpecies']}"
+                        new_package['cfConAge'] = f"{promte['cfConAge']}"
+                        new_package['cfConStyle'] = f"{promte['cfConStyle']}"
+                        new_package['cfStory'] = f"{promte['cfStory']}"
+                        characterSet.update(new_package)
+                        packages_data['variables'] = allvariables
+                        packages_data['characterSet'] = characterSet
+                        packages_data['message'] = f'{text}'
+            else:
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
+                package = {}
+                package['nick'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
+                packages_data['message'] = f'{text}'
         else:
-            logger.warning("找不到该模型！将使用默认模型llm2")
-            packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
-            package = {}
-            package['nick'] = f'{nick}'
-            package['furryCharacter'] = f'{character}'
-            allvariables.update(package)
-            packages_data['variables'] = allvariables
-            packages_data['message'] = f'{text}'
+            logger.warning(f"{model_group}")
+            model = model_group
+            if model == None or model == "yinyingllm-v2":
+                logger.warning("找不到配置里的yinying_model或你设置的模型为yinyingllm-v2,将使用默认模型llm2")
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
+                packages_data['model'] = 'yinyingllm-v2'
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
+                packages_data['message'] = f'{text}'
+            elif model == "yinyingllm-v1":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v1'
+                packages_data['message'] = f'{text}'
+            elif model == "yinyingllm-v3":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v3'
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
+                packages_data['message'] = f'{text}'
+            elif model == "cyberfurry-001":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-cyberfurry-001'
+                packages_data['model'] = 'cyberfurry-001'
+                packages_data['systemPrompt'] = "你的名字叫Hx"
+                packages_data['message'] = f'{text}'
+            elif model == "easycyberfurry-001":
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
+                packages_data['model'] = 'easycyberfurry-001'
+                characterSet = {}
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                new_package = {}
+                new_package['cfNickname'] = 'Hx'
+                new_package['cfSpecies'] = '龙狼'
+                new_package['cfConAge'] = 'child'
+                new_package['cfConStyle'] = 'social_anxiety'
+                new_package['cfStory'] = '你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。'
+                characterSet.update(new_package)
+                packages_data['variables'] = allvariables
+                packages_data['characterSet'] = characterSet
+                packages_data['message'] = f'{text}'
+            else:
+                logger.warning("找不到该模型！将使用默认模型llm2")
+                packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
+                package = {}
+                package['nick'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
+                packages_data['message'] = f'{text}'
     except Exception as e:
             logger.error("严重错误，构建data失败！")
             json_data = False
     return packages_data
 
-def get_chatfubar() -> str:
-    return True
-
-
 #全局发送消息函数，发送消息直接await就行
 async def send_msg(matcher, event, content):
     config_global = config_in_global()
     reply_config = json_get(config_global,"reply")
     if reply_config == True:
         await matcher.send(MessageSegment.reply(event.message_id) + content)
     else:
@@ -707,42 +877,36 @@
             back_msg = f"json解析报错！\n返回结果：{e}"
             return back_msg
     try:
         times = chat_times(id,nick)
         limit = json_get(config_in_global(),"limit")
         if times >= limit or times == 0:
             msg = back['choices'][0]['message']['content']
-            text0 = msg.replace("\n","\\n")
-            text1 = text0.replace("'","\\'")
-            text = text1.replace('"','')
-            ai_out(id,text)
+            ai_out(id,json_replace(text))
             back_msg = f"{msg}\n[对话次数达到上限，即将清空缓存.]"
         else:
             msg = back['choices'][0]['message']['content']
-            text0 = msg.replace("\n","\\n")
-            text1 = text0.replace("'","\\'")
-            text = text1.replace('"','')
-            ai_out(id,text)
+            ai_out(id,json_replace(text))
             back_msg = f"{msg}\n[{times}|{limit}]"
     except Exception as e:
         back_msg = f"{back}\n\n{osu}\n\n未知错误，错误定位于#主要构建函数。"
     return back_msg
 
 #获取回复（被艾特）
 async def get_answer_at(matcher, event, bot):
     text = unescape(await gen_chat_text(event, bot))
-    if  text == "" or text is None or text == "/hx" or text == "/chat":
+    if  text == "" or text is None or text == "！d" or text == "/！d":
         msg = "诶唔，你叫我是有什么事嘛？"
         await send_msg(matcher,event,msg)
     else:
         try:
             groupid = get_groupid(event)
             id = get_id(event)
             nick = await get_nick(bot,event)
-            user_in(id,text)
+            user_in(id,json_replace(text))
             back_msg = str(await yinying(groupid,id,text,nick))
             msg = back_msg.replace("\\n","\n")
             await send_msg(matcher,event,msg)
         except httpx.HTTPError as e:
             back_msg = f"请求接口报错！\n返回结果：{e}"
             await send_msg(matcher, event, back_msg)
 
@@ -750,15 +914,15 @@
 async def get_answer_ml(matcher, event ,bot ,msg):
     text = msg.extract_plain_text()
     if not text == "" or text == None:
         try:
             groupid = get_groupid(event)
             id = get_id(event)
             nick = await get_nick(bot,event)
-            user_in(id,text)
+            user_in(id,json_replace(text))
             back_msg = str(await yinying(groupid,id,text,nick))
             msg = back_msg.replace("\\n","\n")
             await send_msg(matcher,event,msg)
         except httpx.HTTPError as e:
             back_msg = f"请求接口报错！\n返回结果：{e}"
             await send_msg(matcher, event, back_msg)
     else:
```

### Comparing `nonebot-plugin-hx-yinying-1.0.2/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.2
+Version: 1.0.3
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.3 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.0.2/setup.py` & `nonebot-plugin-hx-yinying-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.0.2",
+    version="1.0.3",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

