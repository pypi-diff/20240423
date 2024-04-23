# Comparing `tmp/clovers-0.1.2.tar.gz` & `tmp/clovers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.2.tar", max compression
+gzip compressed data, was "clovers-0.1.3.tar", max compression
```

## Comparing `clovers-0.1.2.tar` & `clovers-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-15 03:08:16.293727 clovers-0.1.2/clovers/__init__.py
--rw-r--r--   0        0        0     3748 2024-04-15 06:14:05.759745 clovers-0.1.2/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.2/clovers/core/config.py
--rw-r--r--   0        0        0     6393 2024-04-15 08:29:41.742919 clovers-0.1.2/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.2/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-15 08:45:36.432996 clovers-0.1.2/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.2/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.2/LICENSE
--rw-r--r--   0        0        0      645 2024-04-15 12:34:14.824383 clovers-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9681 2024-04-15 06:29:12.523168 clovers-0.1.2/README.md
--rw-r--r--   0        0        0    10038 1970-01-01 00:00:00.000000 clovers-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 12:37:36.317298 clovers-0.1.3/clovers/__init__.py
+-rw-r--r--   0        0        0     4306 2024-04-23 10:22:17.869713 clovers-0.1.3/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.3/clovers/core/config.py
+-rw-r--r--   0        0        0     6592 2024-04-23 10:21:00.375616 clovers-0.1.3/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.3/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-16 04:46:17.581644 clovers-0.1.3/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.3/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.3/LICENSE
+-rw-r--r--   0        0        0      645 2024-04-23 10:26:05.713483 clovers-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9681 2024-04-15 06:29:12.523168 clovers-0.1.3/README.md
+-rw-r--r--   0        0        0    10038 1970-01-01 00:00:00.000000 clovers-0.1.3/PKG-INFO
```

### Comparing `clovers-0.1.2/clovers/core/adapter.py` & `clovers-0.1.3/clovers/core/adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import traceback
 from collections.abc import Coroutine, Callable, Awaitable
 from .plugin import Plugin, Handle, Event
 
 
 class AdapterError(Exception):
     def __init__(self, message: str, data=None):
         super().__init__(message)
@@ -57,34 +58,48 @@
                 continue
             kwarg = method.kwarg_dict.get(key) or self.method.kwarg_dict.get(key)
             if not kwarg:
                 raise AdapterError(f"未定义kwarg[{key}]方法")
             kwargs_task.append(kwarg(**extra))
             extra_args.append(key)
         event.kwargs = {k: v for k, v in zip(extra_args, await asyncio.gather(*kwargs_task))}
+        for key in handle.get_extra_args:
+            if key in event.kwargs:
+                continue
+            kwarg = method.kwarg_dict.get(key) or self.method.kwarg_dict.get(key)
+            if not kwarg:
+                raise AdapterError(f"未定义kwarg[{key}]方法")
+            event.kwargs[key] = lambda: kwarg(**extra)
         result = await handle(event)
         if not result:
             return 0
         send_method = result.send_method
         send = method.send_dict.get(send_method) or self.method.send_dict.get(send_method)
         if not send:
             raise AdapterError(f"使用了未定义的 send 方法:{send_method}")
         await send(result.data, **extra)
         return 1
 
+    async def response_task_safe(self, *args):
+        try:
+            return await self.response_task(*args)
+        except:
+            traceback.print_exc()
+            return 0
+
     async def response(self, adapter: str, command: str, **extra) -> int:
         method = self.methods[adapter]
         task_list = []
         for plugin in self.plugins:
             if data := plugin(command):
-                task_list += [self.response_task(method, plugin.handles[key], event, extra) for key, event in data.items()]
+                task_list += [self.response_task_safe(method, plugin.handles[key], event, extra) for key, event in data.items()]
             if not plugin.temp_check():
                 continue
             event = Event(command, [])
-            task_list += [self.response_task(method, handle, event, extra) for _, handle in plugin.temp_handles.values()]
+            task_list += [self.response_task_safe(method, handle, event, extra) for _, handle in plugin.temp_handles.values()]
         return sum(await asyncio.gather(*task_list)) if task_list else 0
 
     async def startup(self):
         task_list = [task for plugin in self.plugins for task in plugin.startup_tasklist]
         self.wait_for.append(asyncio.gather(*task_list))
         self.wait_for += [task for plugin in self.plugins for task in plugin.shutdown_tasklist]
         self.plugins = [plugin for plugin in self.plugins if plugin.handles]
```

### Comparing `clovers-0.1.2/clovers/core/config.py` & `clovers-0.1.3/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.2/clovers/core/plugin.py` & `clovers-0.1.3/clovers/core/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,17 @@
         self.args = args
         self.kwargs: dict = {}
 
 
 class Handle:
     func: Callable[[Event], Coroutine[None, None, Result | None]]
 
-    def __init__(self, extra_args: Iterable[str]):
+    def __init__(self, extra_args: Iterable[str], get_extra_args: Iterable[str]):
         self.extra_args = extra_args
+        self.get_extra_args = get_extra_args
 
     async def __call__(self, event: Event):
         return await self.func(event)
 
 
 PluginCommands = str | set[str] | re.Pattern | None
 
@@ -80,41 +81,43 @@
         else:
             raise PluginError(f"指令：{commands} 类型错误：{type(commands)}")
 
     def handle(
         self,
         commands: PluginCommands,
         extra_args: Iterable[str] = [],
+        get_extra_args: Iterable[str] = [],
     ):
         def decorator(func: Callable[..., Coroutine]):
             key = len(self.handles)
             self.commands_register(commands, key)
-            handle = Handle(extra_args)
+            handle = Handle(extra_args, get_extra_args)
             handle.func = self.handle_warpper(func)
             self.handles[key] = handle
 
         return decorator
 
     def temp_handle(
         self,
         key: str,
-        extra_args: Iterable[str] = [],
         timeout: float | int = 30.0,
+        extra_args: Iterable[str] = [],
+        get_extra_args: Iterable[str] = [],
     ):
 
         def decorator(func: Callable[..., Coroutine]):
 
             def finish():
                 del self.temp_handles[key]
 
             async def wrapper(event: Event):
                 if result := await func(self.build_event(event), finish):
                     return self.build_result(result)
 
-            handle = Handle(extra_args)
+            handle = Handle(extra_args, get_extra_args)
             handle.func = wrapper
             self.temp_handles[key] = time.time() + timeout, handle
 
         return decorator
 
     def startup(self, func: Callable[[], Coroutine]):
         """注册一个启动任务"""
```

### Comparing `clovers-0.1.2/clovers/utils/library.py` & `clovers-0.1.3/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.2/clovers/utils/linecard.py` & `clovers-0.1.3/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.2/clovers/utils/tools.py` & `clovers-0.1.3/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.2/LICENSE` & `clovers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.2/pyproject.toml` & `clovers-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clovers"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = "^0.10.2"
```

### Comparing `clovers-0.1.2/README.md` & `clovers-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.2/PKG-INFO` & `clovers-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

