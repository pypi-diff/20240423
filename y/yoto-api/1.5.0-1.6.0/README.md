# Comparing `tmp/yoto_api-1.5.0.tar.gz` & `tmp/yoto_api-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.5.0.tar", last modified: Tue Apr 23 01:47:50 2024, max compression
+gzip compressed data, was "yoto_api-1.6.0.tar", last modified: Tue Apr 23 02:31:18 2024, max compression
```

## Comparing `yoto_api-1.5.0.tar` & `yoto_api-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.756072 yoto_api-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 01:47:23.000000 yoto_api-1.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 01:47:23.000000 yoto_api-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 01:47:23.000000 yoto_api-1.5.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 01:47:23.000000 yoto_api-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 01:47:23.000000 yoto_api-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 01:47:50.756072 yoto_api-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 01:47:23.000000 yoto_api-1.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 01:47:23.000000 yoto_api-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:47:50.756072 yoto_api-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 01:47:44.000000 yoto_api-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.752072 yoto_api-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:23.000000 yoto_api-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 01:47:23.000000 yoto_api-1.5.0/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.756072 yoto_api-1.5.0/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    26356 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 01:47:23.000000 yoto_api-1.5.0/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:47:50.756072 yoto_api-1.5.0/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:47:50.000000 yoto_api-1.5.0/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:31:18.839016 yoto_api-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 02:30:55.000000 yoto_api-1.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 02:30:55.000000 yoto_api-1.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 02:30:55.000000 yoto_api-1.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 02:30:55.000000 yoto_api-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 02:30:55.000000 yoto_api-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 02:31:18.839016 yoto_api-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 02:30:55.000000 yoto_api-1.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 02:30:55.000000 yoto_api-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:31:18.839016 yoto_api-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 02:31:12.000000 yoto_api-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:31:18.839016 yoto_api-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:30:55.000000 yoto_api-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 02:30:55.000000 yoto_api-1.6.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:31:18.839016 yoto_api-1.6.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26850 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 02:30:55.000000 yoto_api-1.6.0/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:31:18.839016 yoto_api-1.6.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 02:31:18.000000 yoto_api-1.6.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 02:31:18.000000 yoto_api-1.6.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:31:18.000000 yoto_api-1.6.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:31:18.000000 yoto_api-1.6.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 02:31:18.000000 yoto_api-1.6.0/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 02:31:18.000000 yoto_api-1.6.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.5.0/CONTRIBUTING.rst` & `yoto_api-1.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.5.0/LICENSE` & `yoto_api-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.5.0/PKG-INFO` & `yoto_api-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.5.0/README.rst` & `yoto_api-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.5.0/setup.py` & `yoto_api-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.5.0",
+    version="1.6.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.5.0/yoto_api/Card.py` & `yoto_api-1.6.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.5.0/yoto_api/YotoAPI.py` & `yoto_api-1.6.0/yoto_api/YotoAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,23 @@
             deviceId = self.get_child_value(item, "deviceId")
             players[deviceId].name = self.get_child_value(item, "name")
             players[deviceId].device_type = self.get_child_value(item, "deviceType")
             players[deviceId].online = self.get_child_value(item, "online")
             players[deviceId].last_updated_at = datetime.datetime.now(pytz.utc)
             # Should we call here or make this a separate call from YM?  This could help us reduce API calls.
             player_status_response = self._get_device_status(token, deviceId)
-            if self.get_child_value(player_status_response, "activeCard") == "none":
-                players[deviceId].active_card = ""
+            if self.get_child_value(
+                player_status_response, "activeCard"
+            ) is not "none":
+                players[deviceId].is_playing = True
             else:
-                players[deviceId].active_card = self.get_child_value(
-                    player_status_response, "activeCard"
-                )
+                players[deviceId].is_playing = False
+            players[deviceId].active_card = self.get_child_value(
+                player_status_response, "activeCard"
+            )
             players[deviceId].ambient_light_sensor_reading = self.get_child_value(
                 player_status_response, "ambientLightSensorReading"
             )
             players[deviceId].battery_level_percentage = self.get_child_value(
                 player_status_response, "batteryLevelPercentage"
             )
             players[deviceId].night_mode_on = self.get_child_value(
@@ -117,14 +120,23 @@
             )
             players[deviceId].audio_device_connected = self.get_child_value(
                 player_status_response, "isAudioDeviceConnected"
             )
             players[deviceId].firmware_version = self.get_child_value(
                 player_status_response, "firmwareVersion"
             )
+            players[deviceId].wifi_strength = self.get_child_value(
+                player_status_response, "wifiStrength"
+            )
+            players[deviceId].playing_source = self.get_child_value(
+                player_status_response, "playingSource"
+            )
+            players[deviceId].night_light_mode = self.get_child_value(
+                player_status_response, "nightlightMode"
+            )
 
     def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
         for item in response["cards"]:
             if self.get_child_value(item, "cardId") not in library:
                 card: Card = Card(
                     id=self.get_child_value(item, "cardId"),
```

### Comparing `yoto_api-1.5.0/yoto_api/YotoManager.py` & `yoto_api-1.6.0/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.5.0/yoto_api/YotoPlayer.py` & `yoto_api-1.6.0/yoto_api/YotoPlayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,27 @@
     name: str = None
     device_type: str = None
     online: bool = None
     last_updated_at: datetime.datetime = None
 
     # Status API
     active_card: str = None
+    is_playing: bool = None
+    playing_source: str = None
     ambient_light_sensor_reading: int = None
     battery_level_percentage: int = None
     night_mode_on: bool = None
     user_volume: int = None
     system_volume: int = None
     temperature_celcius: int = None
     bluetooth_audio_connected: bool = None
     charging: bool = None
     audio_device_connected: bool = None
     firmware_version: str = None
+    wifi_strength: int = None
 
 
 # {'devices': [{'deviceId': 'XXXX', 'name': 'Yoto Player', 'description': 'nameless.limit', 'online': False, 'releaseChannel': 'general', 'deviceType': 'v3', 'deviceFamily': 'v3', 'deviceGroup': '', 'hasUserGivenName': False}]}
 # Device Status API: {'activeCard': 'none', 'ambientLightSensorReading': 0, 'averageDownloadSpeedBytesSecond': 0, 'batteryLevelPercentage': 100, 'buzzErrors': 0, 'cardInsertionState': 2, 'dayMode': 0, 'deviceId': 'XXXX', 'errorsLogged': 210, 'firmwareVersion': 'v2.17.5', 'freeDiskSpaceBytes': 30250544, 'isAudioDeviceConnected': False, 'isBackgroundDownloadActive': False, 'isBluetoothAudioConnected': False, 'isCharging': False, 'isOnline': True, 'networkSsid': 'XXXX', 'nightlightMode': '0x000000', 'playingSource': 0, 'powerCapabilities': '0x02', 'powerSource': 2, 'systemVolumePercentage': 47, 'taskWatchdogTimeoutCount': 0, 'temperatureCelcius': '20', 'totalDiskSpaceBytes': 31385600, 'updatedAt': '2024-04-23T01:26:19.927Z', 'uptime': 252342, 'userVolumePercentage': 50, 'utcOffsetSeconds': -21600, 'utcTime': 1713835609, 'wifiStrength': -61}
 # Mqtt response:
 
 {
```

### Comparing `yoto_api-1.5.0/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.6.0/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

