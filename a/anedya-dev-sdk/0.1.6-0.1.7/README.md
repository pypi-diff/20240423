# Comparing `tmp/anedya_dev_sdk-0.1.6.tar.gz` & `tmp/anedya_dev_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anedya_dev_sdk-0.1.6.tar", last modified: Fri Apr 19 11:59:23 2024, max compression
+gzip compressed data, was "anedya_dev_sdk-0.1.7.tar", last modified: Tue Apr 23 08:39:43 2024, max compression
```

## Comparing `anedya_dev_sdk-0.1.6.tar` & `anedya_dev_sdk-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.6/LICENSE
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.6/MANIFEST.in
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.6/README.md
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/setup.cfg
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.6/setup.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.410248 anedya_dev_sdk-0.1.6/src/
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.410248 anedya_dev_sdk-0.1.6/src/anedya/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-04-18 07:34:23.000000 anedya_dev_sdk-0.1.6/src/anedya/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4298 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/anedya.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/src/anedya/client/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.6/src/anedya/client/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3435 2024-04-18 07:09:53.000000 anedya_dev_sdk-0.1.6/src/anedya/client/bindDevice.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1165 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/client/callbacks.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.6/src/anedya/client/certs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     5390 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/client/commandsUpdate.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2244 2024-04-18 10:28:59.000000 anedya_dev_sdk-0.1.6/src/anedya/client/mqttHandlers.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3417 2024-04-18 07:17:54.000000 anedya_dev_sdk-0.1.6/src/anedya/client/submitData.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2973 2024-04-19 11:55:17.000000 anedya_dev_sdk-0.1.6/src/anedya/client/submitLogs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3167 2024-04-18 07:17:21.000000 anedya_dev_sdk-0.1.6/src/anedya/client/timeSync.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4524 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1710 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/errors.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     3449 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.6/src/anedya/models.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.6/src/anedya/transaction.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      714 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/requires.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-19 11:59:23.000000 anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-19 11:59:23.414248 anedya_dev_sdk-0.1.6/tests/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.6/tests/test_config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.6/tests/test_core.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.7/LICENSE
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.7/MANIFEST.in
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.7/README.md
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/setup.cfg
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.7/setup.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-23 08:39:43.330270 anedya_dev_sdk-0.1.7/src/
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/src/anedya/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      474 2024-04-23 06:17:16.000000 anedya_dev_sdk-0.1.7/src/anedya/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4348 2024-04-23 08:27:32.000000 anedya_dev_sdk-0.1.7/src/anedya/anedya.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/src/anedya/client/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.7/src/anedya/client/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3435 2024-04-18 07:09:53.000000 anedya_dev_sdk-0.1.7/src/anedya/client/bindDevice.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1165 2024-04-23 07:20:28.000000 anedya_dev_sdk-0.1.7/src/anedya/client/callbacks.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.7/src/anedya/client/certs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4825 2024-04-23 08:27:11.000000 anedya_dev_sdk-0.1.7/src/anedya/client/commandsNext.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     6449 2024-04-23 08:22:21.000000 anedya_dev_sdk-0.1.7/src/anedya/client/commandsUpdate.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2245 2024-04-23 05:56:43.000000 anedya_dev_sdk-0.1.7/src/anedya/client/mqttHandlers.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3417 2024-04-18 07:17:54.000000 anedya_dev_sdk-0.1.7/src/anedya/client/submitData.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2973 2024-04-19 11:55:17.000000 anedya_dev_sdk-0.1.7/src/anedya/client/submitLogs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3167 2024-04-18 07:17:21.000000 anedya_dev_sdk-0.1.7/src/anedya/client/timeSync.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4524 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.7/src/anedya/config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1710 2024-04-19 11:55:25.000000 anedya_dev_sdk-0.1.7/src/anedya/errors.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     5502 2024-04-23 07:57:34.000000 anedya_dev_sdk-0.1.7/src/anedya/models.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.7/src/anedya/transaction.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-23 08:39:43.000000 anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      748 2024-04-23 08:39:43.000000 anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-23 08:39:43.000000 anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-23 08:39:43.000000 anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/requires.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-23 08:39:43.000000 anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-23 08:39:43.334271 anedya_dev_sdk-0.1.7/tests/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.7/tests/test_config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.7/tests/test_core.py
```

### Comparing `anedya_dev_sdk-0.1.6/LICENSE` & `anedya_dev_sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/PKG-INFO` & `anedya_dev_sdk-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-python
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-python
```

### Comparing `anedya_dev_sdk-0.1.6/README.md` & `anedya_dev_sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/setup.cfg` & `anedya_dev_sdk-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = anedya-dev-sdk
-version = 0.1.6
+version = 0.1.7
 url = https://github.com/anedyaio/anedya-dev-sdk-python
 author = Anedya Systems
 author_email = support@anedya.io
 description = Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 long_description = file: README.md
 requires_python = ">=3.7"
 dependencies = ["requests","paho-mqtt>=2.0.0"]
```

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/anedya.py` & `anedya_dev_sdk-0.1.7/src/anedya/anedya.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,10 +101,11 @@
         self._mqttclient.disconnect()
         return
 
     from .client.bindDevice import bind_device
     from .client.submitData import submit_data
     from .client.submitLogs import submit_logs
     from .client.commandsUpdate import update_command_status
+    from .client.commandsNext import next_command
     from .client.timeSync import get_time
     from .client.mqttHandlers import _onconnect_handler, _ondisconnect_handler
     from .client.callbacks import _error_callback, _response_callback, _command_callback
```

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/bindDevice.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/bindDevice.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/callbacks.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/callbacks.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/certs.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/certs.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/mqttHandlers.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/mqttHandlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         topic_prefix = "$anedya/device/" + str(self._config._deviceID)
         # Connection is successful, subscribe to the error and response topics.
         self._mqttclient.subscribe(
             topic=topic_prefix + "/errors", qos=0)
         self._mqttclient.subscribe(
             topic=topic_prefix + "/response", qos=0)
         self._mqttclient.subscribe(
-            topic=topic_prefix + "/command", qos=0)
+            topic=topic_prefix + "/commands", qos=0)
         # Define all Callbacks for error and response
         # Callback for errors
         print("Adding Callbacks")
         self._mqttclient.message_callback_add(sub=topic_prefix + "/errors", callback=self._error_callback)
         # Callback for response
         self._mqttclient.message_callback_add(sub=topic_prefix + "/response", callback=self._response_callback)
         # Callback for command
```

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/submitData.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/submitData.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/submitLogs.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/submitLogs.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/client/timeSync.py` & `anedya_dev_sdk-0.1.7/src/anedya/client/timeSync.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/config.py` & `anedya_dev_sdk-0.1.7/src/anedya/config.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/errors.py` & `anedya_dev_sdk-0.1.7/src/anedya/errors.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya/transaction.py` & `anedya_dev_sdk-0.1.7/src/anedya/transaction.py`

 * *Files identical despite different names*

### Comparing `anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/PKG-INFO` & `anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-python
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-python
```

### Comparing `anedya_dev_sdk-0.1.6/src/anedya_dev_sdk.egg-info/SOURCES.txt` & `anedya_dev_sdk-0.1.7/src/anedya_dev_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/anedya/errors.py
 src/anedya/models.py
 src/anedya/transaction.py
 src/anedya/client/__init__.py
 src/anedya/client/bindDevice.py
 src/anedya/client/callbacks.py
 src/anedya/client/certs.py
+src/anedya/client/commandsNext.py
 src/anedya/client/commandsUpdate.py
 src/anedya/client/mqttHandlers.py
 src/anedya/client/submitData.py
 src/anedya/client/submitLogs.py
 src/anedya/client/timeSync.py
 src/anedya_dev_sdk.egg-info/PKG-INFO
 src/anedya_dev_sdk.egg-info/SOURCES.txt
```

### Comparing `anedya_dev_sdk-0.1.6/tests/test_config.py` & `anedya_dev_sdk-0.1.7/tests/test_config.py`

 * *Files identical despite different names*

