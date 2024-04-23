# Comparing `tmp/nonebot_plugin_clovers-0.1.2.post2.tar.gz` & `tmp/nonebot_plugin_clovers-0.1.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_clovers-0.1.2.post2.tar", max compression
+gzip compressed data, was "nonebot_plugin_clovers-0.1.2.post3.tar", max compression
```

## Comparing `nonebot_plugin_clovers-0.1.2.post2.tar` & `nonebot_plugin_clovers-0.1.2.post3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.2.post2/LICENSE
--rw-r--r--   0        0        0     2332 2024-04-16 09:24:45.888724 nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/__init__.py
--rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/adapters/main.py
--rw-r--r--   0        0        0     1730 2024-04-15 11:51:19.416688 nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/adapters/qq.py
--rw-r--r--   0        0        0     3609 2024-04-15 11:51:16.127157 nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/adapters/v11.py
--rw-r--r--   0        0        0      252 2024-04-16 04:31:38.942676 nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/config.py
--rw-r--r--   0        0        0      420 2024-04-16 12:17:41.981999 nonebot_plugin_clovers-0.1.2.post2/pyproject.toml
--rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.2.post2/README.md
--rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.2.post2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.2.post3/LICENSE
+-rw-r--r--   0        0        0     2522 2024-04-20 03:42:50.974654 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/main.py
+-rw-r--r--   0        0        0     4240 2024-04-23 10:10:22.146061 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/onebot/v11.py
+-rw-r--r--   0        0        0     1732 2024-04-20 03:58:16.439239 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/qq.py
+-rw-r--r--   0        0        0      365 2024-04-20 03:23:59.271766 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/config.py
+-rw-r--r--   0        0        0      557 2024-04-23 17:15:09.977152 nonebot_plugin_clovers-0.1.2.post3/pyproject.toml
+-rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.2.post3/README.md
+-rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.2.post3/PKG-INFO
```

### Comparing `nonebot_plugin_clovers-0.1.2.post2/LICENSE` & `nonebot_plugin_clovers-0.1.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/__init__.py` & `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,26 +47,32 @@
 
 get_driver().on_startup(adapter.startup)
 
 main = on_message(priority=clovers_priority, block=False)
 
 
 def add_response(Bot, Event, adapter_method: AdapterMethod, adapter_key: str):
+    print(f"加载适配器：{adapter_key}")
     adapter.methods[adapter_key] = adapter_method
 
     @main.handle()
     async def _(matcher: Matcher, bot: Bot, event: Event):
         command = extract_command(event.get_plaintext())
         if await adapter.response(adapter_key, command, bot=bot, event=event):
             matcher.stop_propagation()
 
 
-from .adapters import qq
-from nonebot.adapters.qq import Bot as QQBot, MessageEvent as QQMsgEvent
+using_adapters = config_data.using_adapters
 
-add_response(QQBot, QQMsgEvent, qq.initializer(main), "QQ")
 
+if "nonebot.adapters.qq" in using_adapters:
+    from .adapters import qq
+    from nonebot.adapters.qq import Bot, MessageEvent
 
-from .adapters import v11
-from nonebot.adapters.onebot.v11 import Bot as v11Bot, MessageEvent as v11MsgEvent
+    add_response(Bot, MessageEvent, qq.initializer(main), "QQ")
 
-add_response(v11Bot, v11MsgEvent, v11.initializer(main), "v11")
+if "nonebot.adapters.onebot.v11" in using_adapters:
+
+    from .adapters.onebot import v11
+    from nonebot.adapters.onebot.v11 import Bot, MessageEvent
+
+    add_response(Bot, MessageEvent, v11.initializer(main), "onebot.v11".upper())
```

### Comparing `nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/adapters/main.py` & `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/adapters/qq.py` & `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/qq.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from clovers.core.adapter import AdapterMethod
 from clovers.core.plugin import Result
 from nonebot.matcher import Matcher
 from nonebot.adapters.qq import MessageEvent, Message, MessageSegment
 
 
 def initializer(main: type[Matcher]) -> AdapterMethod:
+
     method = AdapterMethod()
 
     @method.send("text")
     async def _(message: str):
         """发送纯文本"""
         await main.send(message)
```

### Comparing `nonebot_plugin_clovers-0.1.2.post2/nonebot_plugin_clovers/adapters/v11.py` & `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/onebot/v11.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,21 +26,24 @@
     @method.send("image")
     async def _(message: BytesIO, send: Callable[..., Coroutine] = main.send):
         """发送图片"""
         await send(MessageSegment.image(message))
 
     @method.send("list")
     async def _(message: list[Result], send: Callable[..., Coroutine] = main.send):
-        """发送图片文本混合信息"""
+        """发送图片文本混合信息，@信息在此发送"""
         msg = Message()
         for seg in message:
-            if seg.send_method == "text":
-                msg += seg.data
-            elif seg.send_method == "image":
-                msg += MessageSegment.image(seg.data)
+            match seg.send_method:
+                case "text":
+                    msg += seg.data
+                case "image":
+                    msg += MessageSegment.image(seg.data)
+                case "at":
+                    msg += MessageSegment.at(seg.data)
         await send(msg)
 
     @method.send("segmented")
     async def _(message: AsyncGenerator[Result, None], send: Callable[..., Coroutine] = main.send):
         """发送分段信息"""
         async for seg in message:
             await method.send_dict[seg.send_method](seg.data, send)
@@ -97,8 +100,19 @@
     async def _(bot: Bot) -> Callable[[int, Result], Coroutine]:
         async def send_group_message(group_id: int, result: Result):
             send = lambda message: bot.send_group_msg(group_id=group_id, message=message)
             await method.send_dict[result.send_method](result.data, send)
 
         return send_group_message
 
+    @method.kwarg("group_member_list")
+    async def _(bot: Bot, event: MessageEvent) -> None | list[dict]:
+        if not isinstance(event, GroupMessageEvent):
+            return None
+        info_list = await bot.get_group_member_list(group_id=event.group_id)
+        for user_info in info_list:
+            user_id = str(user_info["user_id"])
+            user_info["user_id"] = user_id
+            user_info["avatar"] = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
+        return info_list
+
     return method
```

### Comparing `nonebot_plugin_clovers-0.1.2.post2/README.md` & `nonebot_plugin_clovers-0.1.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2.post2/PKG-INFO` & `nonebot_plugin_clovers-0.1.2.post3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-clovers
-Version: 0.1.2.post2
+Version: 0.1.2.post3
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers (>=0.1.2,<0.2.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0)
-Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0)
+Provides-Extra: onebot
+Provides-Extra: qq
+Requires-Dist: clovers (>=0.1.4.post1,<0.2.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra == "onebot"
+Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq"
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
-Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.2.post2
+Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.2.post3
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: clovers (>=0.1.2,<0.2.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.4.3,<3.0.0) Requires-Dist: nonebot-adapter-qq
-(>=1.4.3,<2.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist:
-pydantic (>=2.7.0,<3.0.0) Description-Content-Type: text/markdown
+Python :: 3.11 Provides-Extra: onebot Provides-Extra: qq Requires-Dist: clovers
+(>=0.1.4.post1,<0.2.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ;
+extra == "onebot" Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra ==
+"qq" Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-Type: text/
+markdown
                                    _[_n_o_n_e_b_o_t_]
         # nonebot_plugin_clovers[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ æ¨èä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot_plugin_clovers ``` ä½¿ç¨åç®¡çå¨å®è£ pip ```bash
 pip install nonebot_plugin_clovers ``` poetry ```bash poetry add
 nonebot_plugin_clovers ``` æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
```

