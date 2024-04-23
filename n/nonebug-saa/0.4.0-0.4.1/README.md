# Comparing `tmp/nonebug_saa-0.4.0.tar.gz` & `tmp/nonebug_saa-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebug_saa-0.4.0.tar", max compression
+gzip compressed data, was "nonebug_saa-0.4.1.tar", max compression
```

## Comparing `nonebug_saa-0.4.0.tar` & `nonebug_saa-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      175 2023-11-21 12:45:50.988739 nonebug_saa-0.4.0/README.md
--rw-r--r--   0        0        0     1448 2024-02-08 05:14:06.016224 nonebug_saa-0.4.0/nonebug_saa/__init__.py
--rw-r--r--   0        0        0     1675 2024-02-08 05:14:06.016714 nonebug_saa-0.4.0/nonebug_saa/fixtures.py
--rw-r--r--   0        0        0     1208 2024-02-08 05:14:06.020034 nonebug_saa-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 nonebug_saa-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      175 2023-11-21 12:45:50.988739 nonebug_saa-0.4.1/README.md
+-rw-r--r--   0        0        0     1537 2024-04-23 07:17:48.716194 nonebug_saa-0.4.1/nonebug_saa/__init__.py
+-rw-r--r--   0        0        0     1675 2024-02-08 05:14:06.016714 nonebug_saa-0.4.1/nonebug_saa/fixtures.py
+-rw-r--r--   0        0        0     1208 2024-04-23 07:17:58.881657 nonebug_saa-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 nonebug_saa-0.4.1/PKG-INFO
```

### Comparing `nonebug_saa-0.4.0/nonebug_saa/__init__.py` & `nonebug_saa-0.4.1/nonebug_saa/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     msg: Union["MessageFactory", "AggregatedMessageFactory"],
     bot: Bot,
     *,
     target: Optional["PlatformTarget"] = None,
     event: Optional[Event] = None,
     at_sender: bool = False,
     reply: bool = False,
+    exception: Optional[Exception] = None,
 ):
     require("nonebot_plugin_saa")
 
     from nonebot_plugin_saa import MessageFactory, extract_target
 
     if not target and not event:
         raise RuntimeError("either target or event should be supplied")
@@ -38,18 +39,20 @@
                 "message_factory": msg,
                 "target": target,
                 "event": event,
                 "at_sender": at_sender,
                 "reply": reply,
             },
             None,
+            exception,
         )
     else:
         ctx.should_call_api(
             "_saa_send_aggreagated_msg",
             {
                 "aggregated_message_factory": msg,
                 "target": target,
                 "event": event,
             },
             None,
+            exception,
         )
```

### Comparing `nonebug_saa-0.4.0/nonebug_saa/fixtures.py` & `nonebug_saa-0.4.1/nonebug_saa/fixtures.py`

 * *Files identical despite different names*

### Comparing `nonebug_saa-0.4.0/pyproject.toml` & `nonebug_saa-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebug-saa"
-version = "0.4.0"
+version = "0.4.1"
 description = "A nonebug helper for nonebot-plugin-send-anything-anything"
 authors = ["felinae98 <me@felinae98.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MountainDash/nonebug-saa"
 packages = [{ include = "nonebug_saa" }]
 repository = "https://github.com/MountainDash/nonebug-saa"
```

### Comparing `nonebug_saa-0.4.0/PKG-INFO` & `nonebug_saa-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebug-saa
-Version: 0.4.0
+Version: 0.4.1
 Summary: A nonebug helper for nonebot-plugin-send-anything-anything
 Home-page: https://github.com/MountainDash/nonebug-saa
 License: MIT
 Author: felinae98
 Author-email: me@felinae98.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
```

