# Comparing `tmp/yoto_api-1.4.4.tar.gz` & `tmp/yoto_api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.4.4.tar", last modified: Mon Apr 22 22:20:10 2024, max compression
+gzip compressed data, was "yoto_api-1.5.0.tar", last modified: Tue Apr 23 01:47:50 2024, max compression
```

## Comparing `yoto_api-1.4.4.tar` & `yoto_api-1.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.985965 yoto_api-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 22:19:48.000000 yoto_api-1.4.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-22 22:19:48.000000 yoto_api-1.4.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 22:19:48.000000 yoto_api-1.4.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 22:19:48.000000 yoto_api-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 22:19:48.000000 yoto_api-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-22 22:20:10.985965 yoto_api-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 22:19:48.000000 yoto_api-1.4.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 22:19:48.000000 yoto_api-1.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:20:10.985965 yoto_api-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-22 22:20:04.000000 yoto_api-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.981965 yoto_api-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:48.000000 yoto_api-1.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 22:19:48.000000 yoto_api-1.4.4/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.981965 yoto_api-1.4.4/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    23544 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.985965 yoto_api-1.4.4/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.756072 yoto_api-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 01:47:23.000000 yoto_api-1.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 01:47:23.000000 yoto_api-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 01:47:23.000000 yoto_api-1.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 01:47:23.000000 yoto_api-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 01:47:23.000000 yoto_api-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 01:47:50.756072 yoto_api-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 01:47:23.000000 yoto_api-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 01:47:23.000000 yoto_api-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:47:50.756072 yoto_api-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 01:47:44.000000 yoto_api-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.752072 yoto_api-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:23.000000 yoto_api-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 01:47:23.000000 yoto_api-1.5.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.756072 yoto_api-1.5.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26356 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.756072 yoto_api-1.5.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.4.4/CONTRIBUTING.rst` & `yoto_api-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.4/LICENSE` & `yoto_api-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.4/PKG-INFO` & `yoto_api-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.4.4
+Version: 1.5.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.4.4/README.rst` & `yoto_api-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.4/setup.py` & `yoto_api-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.4.4",
+    version="1.5.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.4.4/yoto_api/Card.py` & `yoto_api-1.5.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.4/yoto_api/YotoAPI.py` & `yoto_api-1.5.0/yoto_api/YotoAPI.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,52 @@
                 )
                 players[player.id] = player
             deviceId = self.get_child_value(item, "deviceId")
             players[deviceId].name = self.get_child_value(item, "name")
             players[deviceId].device_type = self.get_child_value(item, "deviceType")
             players[deviceId].online = self.get_child_value(item, "online")
             players[deviceId].last_updated_at = datetime.datetime.now(pytz.utc)
+            # Should we call here or make this a separate call from YM?  This could help us reduce API calls.
+            player_status_response = self._get_device_status(token, deviceId)
+            if self.get_child_value(player_status_response, "activeCard") == "none":
+                players[deviceId].active_card = ""
+            else:
+                players[deviceId].active_card = self.get_child_value(
+                    player_status_response, "activeCard"
+                )
+            players[deviceId].ambient_light_sensor_reading = self.get_child_value(
+                player_status_response, "ambientLightSensorReading"
+            )
+            players[deviceId].battery_level_percentage = self.get_child_value(
+                player_status_response, "batteryLevelPercentage"
+            )
+            players[deviceId].night_mode_on = self.get_child_value(
+                player_status_response, "dayMode"
+            )
+            players[deviceId].user_volume = self.get_child_value(
+                player_status_response, "userVolumePercentage"
+            )
+            players[deviceId].system_volume = self.get_child_value(
+                player_status_response, "systemVolumePercentage"
+            )
+            players[deviceId].temperature_celcius = self.get_child_value(
+                player_status_response, "temperatureCelcius"
+            )
+            players[deviceId].bluetooth_audio_connected = self.get_child_value(
+                player_status_response, "isBluetoothAudioConnected"
+            )
+            players[deviceId].charging = self.get_child_value(
+                player_status_response, "isCharging"
+            )
+            players[deviceId].audio_device_connected = self.get_child_value(
+                player_status_response, "isAudioDeviceConnected"
+            )
+            players[deviceId].firmware_version = self.get_child_value(
+                player_status_response, "firmwareVersion"
+            )
 
     def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
         for item in response["cards"]:
             if self.get_child_value(item, "cardId") not in library:
                 card: Card = Card(
                     id=self.get_child_value(item, "cardId"),
@@ -143,14 +181,23 @@
 
         headers = self._get_authenticated_headers(token)
 
         response = requests.get(url, headers=headers).json()
         _LOGGER.debug(f"{DOMAIN} - Get Devices Response: {response}")
         return response
 
+    def _get_device_status(self, token: Token, player_id: str) -> None:
+        url = self.BASE_URL + "/device-v2/" + player_id + "/status"
+
+        headers = self._get_authenticated_headers(token)
+
+        response = requests.get(url, headers=headers).json()
+        _LOGGER.debug(f"{DOMAIN} - Get Device Status Response: {response}")
+        return response
+
     def _get_cards(self, token: Token) -> dict:
         ############## ${BASE_URL}/card/family/library #############
         url = self.BASE_URL + "/card/family/library"
 
         headers = self._get_authenticated_headers(token)
 
         response = requests.get(url, headers=headers).json()
@@ -492,7 +539,22 @@
                 value = value[x]
             except Exception:
                 try:
                     value = value[int(x)]
                 except Exception:
                     value = None
         return value
+
+
+######Endpoints:
+
+# api.yotoplay.com/device-v2/devices/mine
+# api.yotoplay.com/device-v2/$deviceid/status
+# api.yotoplay.com/media/displayIcons/user/me
+# api.yotoplay.com/user/details
+# api.yotoplay.com/user/family/mine?allowStub=true
+# api.yotoplay.com/card/mine
+# api.yotoplay.com/card/mine/user/family/mine?allowStub=true
+# api.yotoplay.com/card/family/library
+# api.yotoplay.com/card/library/free
+# api.yotoplay.com/card/library/club
+# api.yotoplay.com/card/family/library
```

### Comparing `yoto_api-1.4.4/yoto_api/YotoManager.py` & `yoto_api-1.5.0/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.4/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.5.0/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.4.4
+Version: 1.5.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

