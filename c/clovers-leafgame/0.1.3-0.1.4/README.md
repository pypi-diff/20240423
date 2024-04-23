# Comparing `tmp/clovers_leafgame-0.1.3.tar.gz` & `tmp/clovers_leafgame-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.3.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.4.tar", max compression
```

## Comparing `clovers_leafgame-0.1.3.tar` & `clovers_leafgame-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-15 02:23:00.888180 clovers_leafgame-0.1.3/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      682 2024-04-16 00:16:47.844659 clovers_leafgame-0.1.3/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4000 2024-04-16 13:40:14.090678 clovers_leafgame-0.1.3/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5568 2024-04-16 13:05:38.537666 clovers_leafgame-0.1.3/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-15 02:23:00.889680 clovers_leafgame-0.1.3/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1151 2024-04-16 00:26:16.638079 clovers_leafgame-0.1.3/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6480 2024-04-16 12:19:33.503496 clovers_leafgame-0.1.3/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14540 2024-04-16 00:25:10.170581 clovers_leafgame-0.1.3/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      347 2024-04-16 00:17:06.391821 clovers_leafgame-0.1.3/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    44533 2024-04-17 03:48:34.369878 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-15 07:55:35.192417 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8794 2024-04-16 00:25:10.463080 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-15 02:23:00.894179 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12802 2024-04-16 00:25:10.251581 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      447 2024-04-16 00:17:40.700801 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-02-25 09:48:38.954877 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-02-25 09:48:38.955377 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-13 05:59:32.008464 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0      933 2024-04-17 03:48:34.370378 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-03-28 05:01:34.333218 clovers_leafgame-0.1.3/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    18175 2024-04-17 03:48:34.371378 clovers_leafgame-0.1.3/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      457 2024-04-16 09:18:01.778879 clovers_leafgame-0.1.3/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12220 2024-04-16 00:24:21.794820 clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-04-16 00:19:07.783118 clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-15 02:23:00.897679 clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-03-20 09:21:29.211881 clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4516 2024-04-15 09:58:44.129537 clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3958 2024-04-17 03:48:34.371878 clovers_leafgame-0.1.3/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-15 02:23:00.898679 clovers_leafgame-0.1.3/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-15 09:04:34.774669 clovers_leafgame-0.1.3/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-15 11:17:50.623418 clovers_leafgame-0.1.3/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-03-15 10:15:49.531286 clovers_leafgame-0.1.3/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-15 07:17:11.700550 clovers_leafgame-0.1.3/LICENSE
--rw-r--r--   0        0        0      428 2024-04-17 04:24:07.341088 clovers_leafgame-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    18355 2024-04-15 11:14:25.199623 clovers_leafgame-0.1.3/README.md
--rw-r--r--   0        0        0    18184 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-15 02:23:00.888180 clovers_leafgame-0.1.4/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-16 00:16:47.844659 clovers_leafgame-0.1.4/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4000 2024-04-16 13:40:14.090678 clovers_leafgame-0.1.4/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5568 2024-04-16 13:05:38.537666 clovers_leafgame-0.1.4/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-15 02:23:00.889680 clovers_leafgame-0.1.4/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-16 00:26:16.638079 clovers_leafgame-0.1.4/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6480 2024-04-16 12:19:33.503496 clovers_leafgame-0.1.4/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14551 2024-04-23 13:53:09.577894 clovers_leafgame-0.1.4/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-16 00:17:06.391821 clovers_leafgame-0.1.4/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44539 2024-04-17 09:36:06.166199 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-15 07:55:35.192417 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8755 2024-04-23 13:54:15.236319 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-15 02:23:00.894179 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-16 00:25:10.251581 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-16 00:17:40.700801 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-02-25 09:48:38.952874 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-02-25 09:48:38.953876 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-02-25 09:48:38.954376 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-02-25 09:48:38.954877 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-02-25 09:48:38.955377 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-02-25 09:48:38.955878 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-13 05:59:32.008464 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0      933 2024-04-17 03:48:34.370378 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-03-28 05:01:34.333218 clovers_leafgame-0.1.4/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18177 2024-04-23 13:51:57.075986 clovers_leafgame-0.1.4/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-16 09:18:01.778879 clovers_leafgame-0.1.4/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    12241 2024-04-23 13:50:43.306529 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-16 00:19:07.783118 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-15 02:23:00.897679 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-03-20 09:21:29.211881 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4516 2024-04-15 09:58:44.129537 clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3958 2024-04-17 03:48:34.371878 clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-15 02:23:00.898679 clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-15 09:04:34.774669 clovers_leafgame-0.1.4/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-15 11:17:50.623418 clovers_leafgame-0.1.4/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-03-15 10:15:49.531286 clovers_leafgame-0.1.4/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-15 07:17:11.700550 clovers_leafgame-0.1.4/LICENSE
+-rw-r--r--   0        0        0      428 2024-04-23 13:53:54.885214 clovers_leafgame-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    18355 2024-04-15 11:14:25.199623 clovers_leafgame-0.1.4/README.md
+-rw-r--r--   0        0        0    18184 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.4/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/config.py` & `clovers_leafgame-0.1.4/clovers_leafgame/config.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.4/clovers_leafgame/core/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.4/clovers_leafgame/core/data.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/item.py` & `clovers_leafgame-0.1.4/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/main.py` & `clovers_leafgame-0.1.4/clovers_leafgame/main.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.4/clovers_leafgame/manager.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/account/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 @Check().superuser().at().check
 async def _(event: Event):
     user_id = event.user_id
     group_id = event.group_id
     user, account = manager.locate_account(event.at[0], group_id)
     confirm = "".join(str(random.randint(0, 9)) for _ in range(4))
 
-    @plugin.temp_handle(f"{confirm} {user_id} {group_id}", {"user_id", "group_id", "permission"})
+    @plugin.temp_handle(f"{confirm} {user_id} {group_id}", extra_args={"user_id", "group_id", "permission"})
     async def _(temp_event: Event, finish):
         if temp_event.user_id != user_id or temp_event.group_id != group_id:
             return
         finish()
         if temp_event.raw_command != confirm:
             return "【冻结】已取消。"
         bank = Counter()
```

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1043,21 +1043,21 @@
                         return session.end(tips)
                 else:
                     tips += "\n你增加了2滴血"
                     session.data[hp] += 2
                     session.data[hp] = min(session.data[hp], session.data["HP_MAX"])
             case "肾上腺素":
                 if len(event.args) < 2:
-                    return tips + "使用失败，你未指定对方的道具"
+                    return tips + "\n使用失败，你未指定对方的道具"
                 inner_prop_key = event.args[1]
                 if inner_prop_key == prop_key:
-                    return tips + "使用失败，目标不能是肾上腺素"
+                    return tips + "\n使用失败，目标不能是肾上腺素"
                 others_props = f"props{others_key}"
                 if inner_prop_key not in session.data[others_props]:
-                    return tips + f"使用失败，对方未持有道具{inner_prop_key}"
+                    return tips + f"\n使用失败，对方未持有道具{inner_prop_key}"
                 session.data[others_props].remove(inner_prop_key)
                 session.data[props].append(inner_prop_key)
                 return use(session, inner_prop_key)
             case "手机":
                 bullet = session.data["bullet"]
                 sum_bullet = len(bullet)
                 sum_real_bullet = sum(bullet)
```

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         return session
 
     def create(self, place: dict[str, Session]):
         def decorator(func: Callable[[Session, str], Coroutine]):
             async def wrapper(event: Event):
                 user_id = event.user_id
                 group_id = event.group_id
-                if (session := self.session_check(place, user_id)) and (tip := session.create_check(user_id)):
+                if (session := self.session_check(place, group_id)) and (tip := session.create_check(user_id)):
                     return tip
                 prop_name, n, arg = self.args_parse(event.args)
                 prop = manager.props_library.get(prop_name, GOLD)
                 user, account = manager.locate_account(user_id, group_id)
                 user.connect = group_id
                 bank = prop.locate_bank(user, account)
                 if n < 0:
@@ -221,17 +221,16 @@
 
         return decorator
 
     def action(self, place: dict[str, Session]):
         def decorator(func: Callable[[Event, Session], Coroutine]):
             async def wrapper(event: Event):
                 group_id = event.group_id or manager.data.user(event.user_id).connect
-                if not (session := self.session_check(place, group_id)):
-                    return
-                if session.game.name != self.name:
+                session = place.get(group_id)
+                if not session or session.game.name != self.name:
                     return
                 user_id = event.user_id
                 if tip := session.action_check(user_id):
                     return tip
                 return await func(event, session)
 
             return wrapper
```

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/market/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return f"重置正在冷却中，结束时间：{time.strftime('%H:%M:%S', time.localtime(revolution_time + revolt_cd))}"
     ranklist: list[tuple[Account, int]] = []
     sum_wealths = 0
     for account_id in group.accounts_map.values():
         account = manager.data.account_dict[account_id]
         n = account.bank[GOLD.id]
         if account.bank[GOLD.id] >= gini_filter_gold:
-            ranklist.append(account, n)
+            ranklist.append((account, n))
         sum_wealths += n
     if sum_wealths < company_public_gold:
         return f"本群金币（{sum_wealths}）小于{company_public_gold}，未满足重置条件。"
     gini = gini_coef([x[1] for x in ranklist])
     if gini < revolt_gini:
         return f"当前基尼系数为{round(gini,3)}，未满足重置条件。"
     ranklist = heapq.nlargest(10, ranklist, key=lambda x: x[1])
```

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,26 +203,26 @@
     if prop.deal(bank, -1):
         return f"使用失败，你未持有{prop.name}"
     group_id = event.group_id
     folders = {f.name: f for f in manager.backup_path.iterdir() if f.is_dir()}
     tip = "请输入你要回档的日期:\n" + "\n".join(folders.keys())
     key = f"{user_id} {group_id}"
 
-    @plugin.temp_handle(key, {"user_id", "group_id"}, 30)
+    @plugin.temp_handle(key, extra_args={"user_id", "group_id"})
     @Check().locate(user_id, group_id).check
     async def _(event: Event, finish):
         date = event.raw_command
         folder = folders.get(date)
         if not folder:
             return tip
         files = {f.stem.split()[1].replace("-", ":"): f for f in folder.iterdir() if f.is_file()}
         tip2 = "请输入你要回档的时间:\n" + "\n".join(files.keys())
         finish()
 
-        @plugin.temp_handle(key, {"user_id", "group_id"}, 30)
+        @plugin.temp_handle(key, extra_args={"user_id", "group_id"})
         @Check().locate(user_id, group_id).check
         async def _(event: Event, finish):
             clock = event.raw_command
             file = files.get(clock)
             if not file:
                 return tip2
             manager.data.cancel_user(user_id)
@@ -247,15 +247,15 @@
         return f"使用失败，你没有足够的{prop.name}"
     group_id = event.group_id
 
     def ten_times_bank(bank: Counter):
         for k in bank.keys():
             bank[k] *= 10
 
-    @plugin.temp_handle(f"{user_id} {group_id}", {"user_id", "group_id"}, 30)
+    @plugin.temp_handle(f"{user_id} {group_id}", extra_args={"user_id", "group_id"})
     async def _(event_1: Event, finish):
         if event_1.user_id != user_id or event_1.group_id != group_id:
             return
         finish()
         if event_1.raw_command == "取消":
             return "恶魔轮盘已取消"
         if event_1.raw_command != "开枪":
```

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/prop/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.4/clovers_leafgame/modules/task/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/output.py` & `clovers_leafgame-0.1.4/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.4/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/LICENSE` & `clovers_leafgame-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/README.md` & `clovers_leafgame-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.3/PKG-INFO` & `clovers_leafgame-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
-Requires-Dist: clovers[linecard,tools] (>=0.1.2,<0.2.0)
+Requires-Dist: clovers[linecard,tools] (>=0.1.3,<0.2.0)
 Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 # clovers_leafgame
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.3 Summary: Author:
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.4 Summary: Author:
 KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers
-[linecard,tools] (>=0.1.2,<0.2.0) Requires-Dist: mplfinance
+[linecard,tools] (>=0.1.3,<0.2.0) Requires-Dist: mplfinance
 (>=0.12.10b0,<0.13.0) Requires-Dist: pydantic (>=2.7.0,<3.0.0) Description-
 Content-Type: text/markdown # clovers_leafgame _â¨ æ¹èª
 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian)
 å [nonebot_plugin_horserace](https://github.com/shinianj/
 nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
                     [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ pip ```bash pip install clovers_leafgame ``` poetry ```bash
```

