# Comparing `tmp/yoto_api-1.7.1.tar.gz` & `tmp/yoto_api-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.1.tar", last modified: Tue Apr 23 14:11:04 2024, max compression
+gzip compressed data, was "yoto_api-1.7.2.tar", last modified: Tue Apr 23 14:58:57 2024, max compression
```

## Comparing `yoto_api-1.7.1.tar` & `yoto_api-1.7.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.320131 yoto_api-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 14:10:38.000000 yoto_api-1.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 14:10:38.000000 yoto_api-1.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 14:10:38.000000 yoto_api-1.7.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 14:10:38.000000 yoto_api-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 14:10:38.000000 yoto_api-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 14:11:04.320131 yoto_api-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 14:10:38.000000 yoto_api-1.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:10:38.000000 yoto_api-1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:11:04.320131 yoto_api-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 14:10:57.000000 yoto_api-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.316131 yoto_api-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:38.000000 yoto_api-1.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 14:10:38.000000 yoto_api-1.7.1/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.320131 yoto_api-1.7.1/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27096 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.320131 yoto_api-1.7.1/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:58:57.336571 yoto_api-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 14:58:32.000000 yoto_api-1.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 14:58:32.000000 yoto_api-1.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 14:58:32.000000 yoto_api-1.7.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 14:58:32.000000 yoto_api-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 14:58:32.000000 yoto_api-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-23 14:58:57.336571 yoto_api-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 14:58:32.000000 yoto_api-1.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 14:58:32.000000 yoto_api-1.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:58:57.336571 yoto_api-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 14:58:50.000000 yoto_api-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:58:57.332571 yoto_api-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:58:32.000000 yoto_api-1.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 14:58:32.000000 yoto_api-1.7.2/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:58:57.336571 yoto_api-1.7.2/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27737 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 14:58:32.000000 yoto_api-1.7.2/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:58:57.336571 yoto_api-1.7.2/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-23 14:58:57.000000 yoto_api-1.7.2/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 14:58:57.000000 yoto_api-1.7.2/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:58:57.000000 yoto_api-1.7.2/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:58:57.000000 yoto_api-1.7.2/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 14:58:57.000000 yoto_api-1.7.2/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 14:58:57.000000 yoto_api-1.7.2/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.1/CONTRIBUTING.rst` & `yoto_api-1.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.1/LICENSE` & `yoto_api-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.1/PKG-INFO` & `yoto_api-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pytz
 Requires-Dist: requests
 Requires-Dist: paho-mqtt
+Requires-Dist: re
 
 Introduction
 ============
 
 Early days of this API. Plan is to use this for home assistant. So far basic device data comes back including online.   The library of cards is also populated.  Pause command functions.  Not other commands work yet.
 
 Credit
```

### Comparing `yoto_api-1.7.1/README.rst` & `yoto_api-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.1/setup.py` & `yoto_api-1.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.1",
+    version="1.7.2",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.1/yoto_api/Card.py` & `yoto_api-1.7.2/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.1/yoto_api/YotoAPI.py` & `yoto_api-1.7.2/yoto_api/YotoAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API Methods"""
 
 import requests
 import logging
 import datetime
+import re
 import paho.mqtt.client as mqtt
 
 from datetime import timedelta
 import pytz
 from .const import DOMAIN, LIGHT_COLORS, POWER_SOURCE
 from .Token import Token
 from .Card import Card
@@ -81,20 +82,18 @@
             deviceId = self.get_child_value(item, "deviceId")
             players[deviceId].name = self.get_child_value(item, "name")
             players[deviceId].device_type = self.get_child_value(item, "deviceType")
             players[deviceId].online = self.get_child_value(item, "online")
 
             # Should we call here or make this a separate call from YM?  This could help us reduce API calls.
             player_status_response = self._get_device_status(token, deviceId)
-            players[deviceId].last_updated_at = self.get_child_value(
-                player_status_response, "updatedAt"
+            players[deviceId].last_updated_at = self._parse_datetime(
+                self.get_child_value(player_status_response, "updatedAt"), pytz.utc
             )
-            if self.get_child_value(
-                player_status_response, "activeCard"
-            ) is not "none":
+            if self.get_child_value(player_status_response, "activeCard") != "none":
                 players[deviceId].is_playing = True
             else:
                 players[deviceId].is_playing = False
             players[deviceId].active_card = self.get_child_value(
                 player_status_response, "activeCard"
             )
             players[deviceId].ambient_light_sensor_reading = self.get_child_value(
@@ -129,20 +128,20 @@
             )
             players[deviceId].wifi_strength = self.get_child_value(
                 player_status_response, "wifiStrength"
             )
             players[deviceId].playing_source = self.get_child_value(
                 player_status_response, "playingSource"
             )
-            players[deviceId].night_light_mode = LIGHT_COLORS[self.get_child_value(
-                player_status_response, "nightlightMode"
-            )]
-            players[deviceId].plugged_in = POWER_SOURCE[self.get_child_value(
-                player_status_response, "powerSource"
-            )]
+            players[deviceId].night_light_mode = LIGHT_COLORS[
+                self.get_child_value(player_status_response, "nightlightMode")
+            ]
+            players[deviceId].plugged_in = POWER_SOURCE[
+                self.get_child_value(player_status_response, "powerSource")
+            ]
 
     def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
         for item in response["cards"]:
             if self.get_child_value(item, "cardId") not in library:
                 card: Card = Card(
                     id=self.get_child_value(item, "cardId"),
@@ -558,14 +557,32 @@
             except Exception:
                 try:
                     value = value[int(x)]
                 except Exception:
                     value = None
         return value
 
+    def _parse_datetime(self, value, timezone) -> datetime.datetime:
+        if value is None:
+            return datetime.datetime(2000, 1, 1, tzinfo=timezone)
+
+        value = (
+            value.replace("-", "").replace("T", "").replace(":", "").replace("Z", "")
+        )
+        m = re.match(r"(\d{4})(\d{2})(\d{2})(\d{2})(\d{2})(\d{2})", value)
+        return datetime.datetime(
+            year=int(m.group(1)),
+            month=int(m.group(2)),
+            day=int(m.group(3)),
+            hour=int(m.group(4)),
+            minute=int(m.group(5)),
+            second=int(m.group(6)),
+            tzinfo=timezone,
+        )
+
 
 ######Endpoints:
 
 # api.yotoplay.com/device-v2/devices/mine
 # api.yotoplay.com/device-v2/$deviceid/status
 # api.yotoplay.com/media/displayIcons/user/me
 # api.yotoplay.com/user/details
```

### Comparing `yoto_api-1.7.1/yoto_api/YotoManager.py` & `yoto_api-1.7.2/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.1/yoto_api/YotoPlayer.py` & `yoto_api-1.7.2/yoto_api/YotoPlayer.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.1/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.7.2/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pytz
 Requires-Dist: requests
 Requires-Dist: paho-mqtt
+Requires-Dist: re
 
 Introduction
 ============
 
 Early days of this API. Plan is to use this for home assistant. So far basic device data comes back including online.   The library of cards is also populated.  Pause command functions.  Not other commands work yet.
 
 Credit
```

