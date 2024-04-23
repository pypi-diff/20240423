# Comparing `tmp/nonebot-plugin-osuverify-0.1.1.tar.gz` & `tmp/nonebot_plugin_osuverify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-osuverify-0.1.1.tar", last modified: Tue Mar  5 09:45:37 2024, max compression
+gzip compressed data, was "nonebot_plugin_osuverify-0.1.2.tar", last modified: Tue Apr 23 16:22:34 2024, max compression
```

## Comparing `nonebot-plugin-osuverify-0.1.1.tar` & `nonebot_plugin_osuverify-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:45:37.756991 nonebot-plugin-osuverify-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-05 09:45:33.000000 nonebot-plugin-osuverify-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-05 09:45:37.756991 nonebot-plugin-osuverify-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-05 09:45:33.000000 nonebot-plugin-osuverify-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:45:37.752991 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify/
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-05 09:45:33.000000 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 09:45:37.752991 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-05 09:45:37.000000 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-05 09:45:37.000000 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 09:45:37.000000 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-05 09:45:37.000000 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-05 09:45:37.000000 nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 09:45:37.756991 nonebot-plugin-osuverify-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-05 09:45:33.000000 nonebot-plugin-osuverify-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:22:34.925968 nonebot_plugin_osuverify-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-23 16:22:31.000000 nonebot_plugin_osuverify-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-23 16:22:34.925968 nonebot_plugin_osuverify-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-23 16:22:31.000000 nonebot_plugin_osuverify-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:22:34.925968 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify/
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-23 16:22:31.000000 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:22:34.925968 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-23 16:22:34.000000 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-23 16:22:34.000000 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:22:34.000000 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 16:22:34.000000 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 16:22:34.000000 nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:22:34.925968 nonebot_plugin_osuverify-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-23 16:22:31.000000 nonebot_plugin_osuverify-0.1.2/setup.py
```

### Comparing `nonebot-plugin-osuverify-0.1.1/LICENSE` & `nonebot_plugin_osuverify-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-osuverify-0.1.1/PKG-INFO` & `nonebot_plugin_osuverify-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-osuverify
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通过osu!账号审核入群功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.1.2 Summary:
 éè¿osu!è´¦å·å®¡æ ¸å¥ç¾¤åè½ Home-page: https://github.com/mas-alone/
 nonebot-plugin-sayoroll Author: A M D Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: httpx>=0.23.3 Requires-Dist: nonebot2>=2.0.0rc3 Requires-Dist:
 nonebot-adapter-onebot>=2.0.0b1
```

### Comparing `nonebot-plugin-osuverify-0.1.1/README.md` & `nonebot_plugin_osuverify-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify/__init__.py` & `nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from nonebot.adapters.onebot.v11.bot import Bot
 from nonebot.adapters.onebot.v11.event import GroupRequestEvent
 from nonebot.adapters.onebot.v11.message import MessageSegment
 
 
 __plugin_meta__ = PluginMetadata(
     name='osu!入群验证',
+    type='application',
     description='osu!账户自动审批入群申请！',
-    usage="",
+    homepage='https://github.com/mas-alone/nonebot-plugin-sayoroll',
+    usage="通过判断用户入群的答案，通过osu! api查询用户名验证入群",
     config={},
     extra={}
 )
 
 join_group = on_request(
     priority=1,
     block=True
```

### Comparing `nonebot-plugin-osuverify-0.1.1/nonebot_plugin_osuverify.egg-info/PKG-INFO` & `nonebot_plugin_osuverify-0.1.2/nonebot_plugin_osuverify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-osuverify
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通过osu!账号审核入群功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.1.2 Summary:
 éè¿osu!è´¦å·å®¡æ ¸å¥ç¾¤åè½ Home-page: https://github.com/mas-alone/
 nonebot-plugin-sayoroll Author: A M D Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: httpx>=0.23.3 Requires-Dist: nonebot2>=2.0.0rc3 Requires-Dist:
 nonebot-adapter-onebot>=2.0.0b1
```

### Comparing `nonebot-plugin-osuverify-0.1.1/setup.py` & `nonebot_plugin_osuverify-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-osuverify",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.1",  # 程序版本
+    version="0.1.2",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="通过osu!账号审核入群功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

