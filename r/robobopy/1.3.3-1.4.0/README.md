# Comparing `tmp/robobopy-1.3.3.tar.gz` & `tmp/robobopy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robobopy-1.3.3.tar", last modified: Mon Jan 29 12:55:05 2024, max compression
+gzip compressed data, was "robobopy-1.4.0.tar", last modified: Tue Apr 23 13:32:08 2024, max compression
```

## Comparing `robobopy-1.3.3.tar` & `robobopy-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 12:55:05.624815 robobopy-1.3.3/
--rw-rw-rw-   0        0        0     7817 2023-10-02 12:30:58.000000 robobopy-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      864 2024-01-29 12:55:05.623304 robobopy-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-10-02 12:30:58.000000 robobopy-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-01-29 12:55:05.625819 robobopy-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1483 2024-01-29 12:45:06.000000 robobopy-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-29 12:55:05.536315 robobopy-1.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-01-29 12:55:05.550859 robobopy-1.3.3/src/robobopy/
--rw-rw-rw-   0        0        0    40540 2024-01-29 09:00:28.000000 robobopy-1.3.3/src/robobopy/Robobo.py
--rw-rw-rw-   0        0        0     4047 2023-11-09 13:01:58.000000 robobopy-1.3.3/src/robobopy/State.py
--rw-rw-rw-   0        0        0        0 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 12:55:05.591750 robobopy-1.3.3/src/robobopy/processors/
--rw-rw-rw-   0        0        0     1012 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/processors/AbstractProcessor.py
--rw-rw-rw-   0        0        0     2915 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/processors/PTProcessor.py
--rw-rw-rw-   0        0        0     2865 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/processors/RobProcessor.py
--rw-rw-rw-   0        0        0     2224 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/processors/SmartphoneProcessor.py
--rw-rw-rw-   0        0        0     2462 2024-01-29 09:01:06.000000 robobopy-1.3.3/src/robobopy/processors/SoundProcessor.py
--rw-rw-rw-   0        0        0     1989 2023-11-09 12:42:55.000000 robobopy-1.3.3/src/robobopy/processors/SpeechProcessor.py
--rw-rw-rw-   0        0        0    12218 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/processors/VisionProcessor.py
--rw-rw-rw-   0        0        0        0 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/processors/__init__.py
--rw-rw-rw-   0        0        0    16210 2024-01-29 09:00:53.000000 robobopy-1.3.3/src/robobopy/remotelib.py
-drwxrwxrwx   0        0        0        0 2024-01-29 12:55:05.621304 robobopy-1.3.3/src/robobopy/utils/
--rw-rw-rw-   0        0        0      501 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Acceleration.py
--rw-rw-rw-   0        0        0      990 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Blob.py
--rw-rw-rw-   0        0        0      221 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/BlobColor.py
--rw-rw-rw-   0        0        0      326 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Color.py
--rw-rw-rw-   0        0        0      138 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/ConnectionState.py
--rw-rw-rw-   0        0        0     1434 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/DetectedObject.py
--rw-rw-rw-   0        0        0      538 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Emotions.py
--rw-rw-rw-   0        0        0      808 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Face.py
--rw-rw-rw-   0        0        0      621 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/IR.py
--rw-rw-rw-   0        0        0      800 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/LED.py
--rw-rw-rw-   0        0        0     2086 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Lanes.py
--rw-rw-rw-   0        0        0      715 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Lines.py
--rw-rw-rw-   0        0        0      919 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Message.py
--rw-rw-rw-   0        0        0      864 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Note.py
--rw-rw-rw-   0        0        0     1274 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Orientation.py
--rw-rw-rw-   0        0        0     2123 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/QRCode.py
--rw-rw-rw-   0        0        0      436 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Sounds.py
--rw-rw-rw-   0        0        0      318 2023-11-09 13:02:56.000000 robobopy-1.3.3/src/robobopy/utils/Speech.py
--rw-rw-rw-   0        0        0      273 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/StatusFrequency.py
--rw-rw-rw-   0        0        0     1773 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Tag.py
--rw-rw-rw-   0        0        0     2561 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Tap.py
--rw-rw-rw-   0        0        0      204 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/Wheels.py
--rw-rw-rw-   0        0        0        0 2023-10-02 12:30:58.000000 robobopy-1.3.3/src/robobopy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 12:55:05.580230 robobopy-1.3.3/src/robobopy.egg-info/
--rw-rw-rw-   0        0        0      864 2024-01-29 12:55:05.000000 robobopy-1.3.3/src/robobopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1326 2024-01-29 12:55:05.000000 robobopy-1.3.3/src/robobopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 12:55:05.000000 robobopy-1.3.3/src/robobopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-01-29 12:55:05.000000 robobopy-1.3.3/src/robobopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-29 12:55:05.000000 robobopy-1.3.3/src/robobopy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 13:32:08.897848 robobopy-1.4.0/
+-rw-rw-rw-   0        0        0     7817 2023-10-02 12:30:58.000000 robobopy-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      864 2024-04-23 13:32:08.897848 robobopy-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-10-02 12:30:58.000000 robobopy-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:32:08.897848 robobopy-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1483 2024-04-23 13:29:21.000000 robobopy-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:32:08.820740 robobopy-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 13:32:08.836765 robobopy-1.4.0/src/robobopy/
+-rw-rw-rw-   0        0        0    40726 2024-04-23 13:22:32.000000 robobopy-1.4.0/src/robobopy/Robobo.py
+-rw-rw-rw-   0        0        0     4047 2023-11-09 13:01:58.000000 robobopy-1.4.0/src/robobopy/State.py
+-rw-rw-rw-   0        0        0        0 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:32:08.866311 robobopy-1.4.0/src/robobopy/processors/
+-rw-rw-rw-   0        0        0     1012 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/processors/AbstractProcessor.py
+-rw-rw-rw-   0        0        0     2915 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/processors/PTProcessor.py
+-rw-rw-rw-   0        0        0     2865 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/processors/RobProcessor.py
+-rw-rw-rw-   0        0        0     2224 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/processors/SmartphoneProcessor.py
+-rw-rw-rw-   0        0        0     2462 2024-01-29 09:01:06.000000 robobopy-1.4.0/src/robobopy/processors/SoundProcessor.py
+-rw-rw-rw-   0        0        0     1989 2023-11-09 12:42:55.000000 robobopy-1.4.0/src/robobopy/processors/SpeechProcessor.py
+-rw-rw-rw-   0        0        0    12218 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/processors/VisionProcessor.py
+-rw-rw-rw-   0        0        0        0 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/processors/__init__.py
+-rw-rw-rw-   0        0        0    17129 2024-04-23 13:22:32.000000 robobopy-1.4.0/src/robobopy/remotelib.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:32:08.896848 robobopy-1.4.0/src/robobopy/utils/
+-rw-rw-rw-   0        0        0      501 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Acceleration.py
+-rw-rw-rw-   0        0        0      990 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Blob.py
+-rw-rw-rw-   0        0        0      221 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/BlobColor.py
+-rw-rw-rw-   0        0        0      326 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Color.py
+-rw-rw-rw-   0        0        0      138 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/ConnectionState.py
+-rw-rw-rw-   0        0        0     1434 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/DetectedObject.py
+-rw-rw-rw-   0        0        0      538 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Emotions.py
+-rw-rw-rw-   0        0        0      808 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Face.py
+-rw-rw-rw-   0        0        0      621 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/IR.py
+-rw-rw-rw-   0        0        0      800 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/LED.py
+-rw-rw-rw-   0        0        0     2086 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Lanes.py
+-rw-rw-rw-   0        0        0      715 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Lines.py
+-rw-rw-rw-   0        0        0      919 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Message.py
+-rw-rw-rw-   0        0        0      864 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Note.py
+-rw-rw-rw-   0        0        0     1274 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Orientation.py
+-rw-rw-rw-   0        0        0     2123 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/QRCode.py
+-rw-rw-rw-   0        0        0      436 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Sounds.py
+-rw-rw-rw-   0        0        0      318 2023-11-09 13:02:56.000000 robobopy-1.4.0/src/robobopy/utils/Speech.py
+-rw-rw-rw-   0        0        0      273 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/StatusFrequency.py
+-rw-rw-rw-   0        0        0     1773 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Tag.py
+-rw-rw-rw-   0        0        0     2561 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Tap.py
+-rw-rw-rw-   0        0        0      204 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/Wheels.py
+-rw-rw-rw-   0        0        0        0 2023-10-02 12:30:58.000000 robobopy-1.4.0/src/robobopy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:32:08.856789 robobopy-1.4.0/src/robobopy.egg-info/
+-rw-rw-rw-   0        0        0      864 2024-04-23 13:32:08.000000 robobopy-1.4.0/src/robobopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1326 2024-04-23 13:32:08.000000 robobopy-1.4.0/src/robobopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:32:08.000000 robobopy-1.4.0/src/robobopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 13:32:08.000000 robobopy-1.4.0/src/robobopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-23 13:32:08.000000 robobopy-1.4.0/src/robobopy.egg-info/top_level.txt
```

### Comparing `robobopy-1.3.3/LICENSE` & `robobopy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/PKG-INFO` & `robobopy-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robobopy
-Version: 1.3.3
+Version: 1.4.0
 Summary: Robobo remote control library
 Author: The Robobo Project
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robobopy-1.3.3/setup.py` & `robobopy-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="robobopy",                     # This is the name of the package
-    version="1.3.3",                        # The initial release version
+    version="1.4.0",                        # The initial release version
     author="The Robobo Project",                     # Full name of the author
     authore_email='info@theroboboproject.com',
     description="Robobo remote control library",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     repository_url="https://github.com/mintforpeople/robobo.py",
     #packages=setuptools.find_packages(),    # List of all python modules to be installed
```

### Comparing `robobopy-1.3.3/src/robobopy/Robobo.py` & `robobopy-1.4.0/src/robobopy/Robobo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,32 @@
 from robobopy.utils.Tap import Tap
 import time
 from copy import copy, deepcopy
 
 class Robobo:
 
 
-    def __init__(self, ip, robot_id=0):
+    def __init__(self, ip, robot_id=0, secure=False):
         """
         Creates a new Robobo library instance.
 
         :param ip: The IP address of the Robobo robot.
 
         :type ip: string
 
         :param robot_id: Sequential ID of robots. Only used in multi-robot scenarios in simulation.
 
         :type robot_id: int
+
+        :param secure: Use a secure websocket connection instead of the default one. Only works in local networks (192.68.xxx.xxx)
+
+        :type secure: bool
         """
 
-        self.rem = Remote(ip, robot_id)
+        self.rem = Remote(ip, robot_id, secure)
 
     def connect(self):
         """
         Establishes a remote connection with the Robobo indicated by the IP address associated to this instance.
         """
 
         self.rem.wsStartup()
```

### Comparing `robobopy-1.3.3/src/robobopy/State.py` & `robobopy-1.4.0/src/robobopy/State.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/AbstractProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/AbstractProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/PTProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/PTProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/RobProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/RobProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/SmartphoneProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/SmartphoneProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/SoundProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/SoundProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/SpeechProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/SpeechProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/processors/VisionProcessor.py` & `robobopy-1.4.0/src/robobopy/processors/VisionProcessor.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/remotelib.py` & `robobopy-1.4.0/src/robobopy/remotelib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import websocket
+import pathlib
+import ssl
 import threading
 import time
 import sys
 
 from robobopy.State import State
 from robobopy.processors.PTProcessor import PTProcessor
 from robobopy.processors.RobProcessor import RobProcessor
@@ -11,30 +13,35 @@
 from robobopy.processors.SmartphoneProcessor import SmartphoneProcessor
 from robobopy.processors.SoundProcessor import SoundProcessor
 from robobopy.processors.SpeechProcessor import SpeechProcessor
 from robobopy.utils.ConnectionState import ConnectionState
 
 
 class Remote:
-    def __init__(self, ip, robot_id=0):
+    def __init__(self, ip, robot_id=0, secure=False):
         self.ip = ip
         self.robot_id = robot_id
+        self.secure = secure
+        self.ssl_context = None
         self.ws = None
         self.password = ""
         self.state = State()
         self.processors = {"PT": PTProcessor(self.state),
                            "ROB": RobProcessor(self.state),
                            "PHONE": SmartphoneProcessor(self.state),
                            "SOUND": SoundProcessor(self.state),
                            "SPEECH" : SpeechProcessor(self.state),
                            "VISION": VisionProcessor(self.state)}
 
         self.wsDaemon = None
         self.connectionState = ConnectionState.DISCONNECTED
 
+        self.ssl_context = None
+        self.localhost_pem = None
+
         self.wheelsLastTime = 0
         self.panLastTime = 0
         self.tiltLastTime = 0
 
         self.timeout = 10
 
     def filterMovement(self, speed, axis):
@@ -73,25 +80,38 @@
         def on_close(ws, status_code, msg):
             self.connectionState = ConnectionState.DISCONNECTED
             if (status_code != None):
                 print(f"### closed connection [{status_code}] {msg} ###")
             else:
                 print("### closed connection ###")
         
-        port = 40404 + (self.robot_id * 10)
-
-        self.ws = websocket.WebSocketApp('ws://' + self.ip + ":" + str(port),
-                                         on_message=on_message,
-                                         on_error=on_error,
-                                         on_close=on_close)
+        if not self.secure:
+            port = 40404 + (self.robot_id * 10)
+            self.ws = websocket.WebSocketApp('ws://' + self.ip + ":" + str(port),
+                                            on_message=on_message,
+                                            on_error=on_error,
+                                            on_close=on_close)
+        else:
+            self.ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+            localhost_pem = pathlib.Path(__file__).with_name("local_network_cert.pem")
+            self.ssl_context.load_verify_locations(localhost_pem)
+
+            port = 44304 + (self.robot_id * 10)
+            self.ws = websocket.WebSocketApp('wss://' + self.ip + ":" + str(port),
+                                            on_message=on_message,
+                                            on_error=on_error,
+                                            on_close=on_close)
 
         self.ws.on_open = on_open
 
         def runWS():
-            self.ws.run_forever()
+            if self.secure:
+                self.ws.run_forever(sslopt={'context': self.ssl_context})
+            else:
+                self.ws.run_forever()
 
         self.wsDaemon = threading.Thread(target=runWS, name='wsDaemon')
         self.wsDaemon.setDaemon(True)
         self.wsDaemon.start()
 
         print("Connecting")
         self.connectionState = ConnectionState.CONNECTING
```

### Comparing `robobopy-1.3.3/src/robobopy/utils/Blob.py` & `robobopy-1.4.0/src/robobopy/utils/Blob.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/DetectedObject.py` & `robobopy-1.4.0/src/robobopy/utils/DetectedObject.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Emotions.py` & `robobopy-1.4.0/src/robobopy/utils/Emotions.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Face.py` & `robobopy-1.4.0/src/robobopy/utils/Face.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/IR.py` & `robobopy-1.4.0/src/robobopy/utils/IR.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/LED.py` & `robobopy-1.4.0/src/robobopy/utils/LED.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Lanes.py` & `robobopy-1.4.0/src/robobopy/utils/Lanes.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Lines.py` & `robobopy-1.4.0/src/robobopy/utils/Lines.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Message.py` & `robobopy-1.4.0/src/robobopy/utils/Message.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Note.py` & `robobopy-1.4.0/src/robobopy/utils/Note.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Orientation.py` & `robobopy-1.4.0/src/robobopy/utils/Orientation.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/QRCode.py` & `robobopy-1.4.0/src/robobopy/utils/QRCode.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Tag.py` & `robobopy-1.4.0/src/robobopy/utils/Tag.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy/utils/Tap.py` & `robobopy-1.4.0/src/robobopy/utils/Tap.py`

 * *Files identical despite different names*

### Comparing `robobopy-1.3.3/src/robobopy.egg-info/PKG-INFO` & `robobopy-1.4.0/src/robobopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robobopy
-Version: 1.3.3
+Version: 1.4.0
 Summary: Robobo remote control library
 Author: The Robobo Project
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robobopy-1.3.3/src/robobopy.egg-info/SOURCES.txt` & `robobopy-1.4.0/src/robobopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

