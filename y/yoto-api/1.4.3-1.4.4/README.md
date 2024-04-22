# Comparing `tmp/yoto_api-1.4.3.tar.gz` & `tmp/yoto_api-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.4.3.tar", last modified: Sun Apr 21 21:03:25 2024, max compression
+gzip compressed data, was "yoto_api-1.4.4.tar", last modified: Mon Apr 22 22:20:10 2024, max compression
```

## Comparing `yoto_api-1.4.3.tar` & `yoto_api-1.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:03:25.310051 yoto_api-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 21:02:58.000000 yoto_api-1.4.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-21 21:02:58.000000 yoto_api-1.4.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 21:02:58.000000 yoto_api-1.4.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 21:02:58.000000 yoto_api-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 21:02:58.000000 yoto_api-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-21 21:03:25.310051 yoto_api-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-21 21:02:58.000000 yoto_api-1.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 21:02:58.000000 yoto_api-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:03:25.310051 yoto_api-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-21 21:03:18.000000 yoto_api-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:03:25.306051 yoto_api-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:02:58.000000 yoto_api-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-21 21:02:58.000000 yoto_api-1.4.3/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:03:25.306051 yoto_api-1.4.3/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    23506 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-21 21:02:58.000000 yoto_api-1.4.3/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:03:25.306051 yoto_api-1.4.3/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-21 21:03:25.000000 yoto_api-1.4.3/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-21 21:03:25.000000 yoto_api-1.4.3/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:03:25.000000 yoto_api-1.4.3/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:03:25.000000 yoto_api-1.4.3/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 21:03:25.000000 yoto_api-1.4.3/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 21:03:25.000000 yoto_api-1.4.3/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.985965 yoto_api-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 22:19:48.000000 yoto_api-1.4.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-22 22:19:48.000000 yoto_api-1.4.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 22:19:48.000000 yoto_api-1.4.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 22:19:48.000000 yoto_api-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 22:19:48.000000 yoto_api-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-22 22:20:10.985965 yoto_api-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 22:19:48.000000 yoto_api-1.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 22:19:48.000000 yoto_api-1.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:20:10.985965 yoto_api-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-22 22:20:04.000000 yoto_api-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.981965 yoto_api-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:48.000000 yoto_api-1.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 22:19:48.000000 yoto_api-1.4.4/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.981965 yoto_api-1.4.4/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23544 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 22:19:48.000000 yoto_api-1.4.4/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:20:10.985965 yoto_api-1.4.4/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 22:20:10.000000 yoto_api-1.4.4/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.4.3/CONTRIBUTING.rst` & `yoto_api-1.4.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.3/LICENSE` & `yoto_api-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.3/PKG-INFO` & `yoto_api-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.4.3/README.rst` & `yoto_api-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.3/setup.py` & `yoto_api-1.4.4/setup.py`

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
-    version="1.4.3",
+    version="1.4.4",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.4.3/yoto_api/Card.py` & `yoto_api-1.4.4/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.3/yoto_api/YotoAPI.py` & `yoto_api-1.4.4/yoto_api/YotoAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,18 @@
             )
             _LOGGER.debug(f"{DOMAIN} - MQTT Topic: {message.topic}")
             _LOGGER.debug(f"{DOMAIN} - MQTT QOS: {message.qos}")
             _LOGGER.debug(f"{DOMAIN} - MQTT Retain: {message.retain}")
             parts = message.topic.split("/")
             base, device, topic = parts
             if topic == "status":
-                self._parse_status_message(str(message.payload.decode('utf-8')), )
+                self._parse_status_message(
+                    str(message.payload.decode("utf-8")),
+                )
+
         #             mqtt.CallbackAPIVersion.VERSION1,
         client = mqtt.Client(
             client_id="DASH" + deviceId,
             transport="websockets",
         )
         client.username_pw_set(
             username=deviceId + "?x-amz-customauthorizer-name=" + self.MQTT_AUTH_NAME,
```

### Comparing `yoto_api-1.4.3/yoto_api/YotoManager.py` & `yoto_api-1.4.4/yoto_api/YotoManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.library: list = {}
         self.mqtt_client = None
 
     def initialize(self) -> None:
         self.token: Token = self.api.login(self.username, self.password)
         self.update_players_status()
         self.update_cards()
-        self.connect_to_events()
+        # self.connect_to_events()
 
     def update_players_status(self) -> None:
         # Updates the data with current player data.
         self.api.update_players(self.token, self.players)
 
     def connect_to_events(self) -> None:
         for player in self.players.values():
```

### Comparing `yoto_api-1.4.3/yoto_api/YotoPlayer.py` & `yoto_api-1.4.4/yoto_api/YotoPlayer.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.4.3/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.4.4/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

