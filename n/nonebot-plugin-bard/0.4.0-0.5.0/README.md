# Comparing `tmp/nonebot_plugin_bard-0.4.0.tar.gz` & `tmp/nonebot_plugin_bard-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bard-0.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bard-0.5.0.tar", max compression
```

## Comparing `nonebot_plugin_bard-0.4.0.tar` & `nonebot_plugin_bard-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     2405 2024-04-09 04:54:21.516654 nonebot_plugin_bard-0.4.0/README.md
--rw-r--r--   0        0        0     6148 2024-04-09 05:38:23.977968 nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/.DS_Store
--rw-r--r--   0        0        0     5122 2024-04-09 05:32:14.247381 nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/__init__.py
--rw-r--r--   0        0        0      539 2024-04-09 04:54:21.517674 nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/config.py
--rw-r--r--   0        0        0   188156 2024-04-09 04:54:21.523269 nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/images/demo1.jpg
--rw-r--r--   0        0        0   120205 2024-04-09 04:54:21.525354 nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/images/demo2.jpg
--rw-r--r--   0        0        0   147000 2024-04-09 04:54:21.527614 nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/images/demo3.jpg
--rw-r--r--   0        0        0      550 2024-04-09 05:32:23.088675 nonebot_plugin_bard-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 nonebot_plugin_bard-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2405 2024-04-23 03:28:09.973333 nonebot_plugin_bard-0.5.0/README.md
+-rw-r--r--   0        0        0     5123 2024-04-23 03:26:35.474716 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/__init__.py
+-rw-r--r--   0        0        0      539 2024-04-23 03:26:54.720592 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/config.py
+-rw-r--r--   0        0        0   188156 2024-04-23 03:25:58.592485 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo1.jpg
+-rw-r--r--   0        0        0   120205 2024-04-23 03:25:58.593504 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo2.jpg
+-rw-r--r--   0        0        0   147000 2024-04-23 03:25:58.594370 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo3.jpg
+-rw-r--r--   0        0        0      525 2024-04-23 03:28:32.466457 nonebot_plugin_bard-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 nonebot_plugin_bard-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_bard-0.4.0/README.md` & `nonebot_plugin_bard-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/__init__.py` & `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, PrivateMessageEvent, MessageEvent, helpers , GROUP_OWNER , GROUP_ADMIN
 from nonebot.permission import SUPERUSER
 
 from nonebot.plugin import PluginMetadata
 
 from .config import Config, ConfigError
-from gemini_webapi import GeminiClient
+from .gemini_webapi import GeminiClient
 
 # require("nonebot_plugin_htmlrender")
 # from nonebot_plugin_htmlrender import md_to_pic
 
 __plugin_meta__ = PluginMetadata(
     name="谷歌Gemini Pro聊天",
     description="Nonebot框架下的谷歌Gemini Pro聊天插件，支持联网搜索和图片识别",
```

### Comparing `nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/config.py` & `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/images/demo1.jpg` & `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/images/demo2.jpg` & `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo2.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.4.0/nonebot_plugin_bard/images/demo3.jpg` & `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo3.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.4.0/pyproject.toml` & `nonebot_plugin_bard-0.5.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-bard"
-version = "0.4.0"
+version = "0.5.0"
 description = "A nonebot plugin for Bard"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = "^2.2.1"
 websocket-client = "^1.6.1"
-gemini_webapi = "^1.1.1"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
```

### Comparing `nonebot_plugin_bard-0.4.0/PKG-INFO` & `nonebot_plugin_bard-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bard
-Version: 0.4.0
+Version: 0.5.0
 Summary: A nonebot plugin for Bard
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gemini_webapi (>=1.1.1,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Requires-Dist: websocket-client (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bard Version: 0.4.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bard Version: 0.5.0 Summary: A
 nonebot plugin for Bard License: MIT Author: Alpaca Author-email:
 alpaca@bupt.edu.cn Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gemini_webapi (>=1.1.1,<2.0.0) Requires-Dist: nonebot-adapter-
-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Requires-
-Dist: websocket-client (>=1.6.1,<2.0.0) Description-Content-Type: text/markdown
+Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0rc3,<3.0.0) Requires-Dist: websocket-client (>=1.6.1,<2.0.0)
+Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                              # nonebot-plugin-bard
 # ä»ç» - æ¬æä»¶æ¯ééGoogle
 Geminiç½é¡µççèå¤©æºå¨äººæä»¶ï¼åå©Gemini
 Proçèç½è½ååå¤æ¨¡æè¯å«è½åå®ç°æ´åç¡®å°åå¤åå¾çè¯å«åå¤ç­åè½ã
 - æ ¸å¿ä»£ç æºäº[Gemini-API](https://github.com/HanaokaYuzu/Gemini-
```

