# Comparing `tmp/ovos-PHAL-rediscamera-0.0.0a2.tar.gz` & `tmp/ovos-PHAL-rediscamera-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-rediscamera-0.0.0a2.tar", last modified: Wed Feb 28 03:53:06 2024, max compression
+gzip compressed data, was "ovos-PHAL-rediscamera-0.0.0a3.tar", last modified: Tue Apr 23 21:23:02 2024, max compression
```

## Comparing `ovos-PHAL-rediscamera-0.0.0a2.tar` & `ovos-PHAL-rediscamera-0.0.0a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 03:53:06.133165 ovos-PHAL-rediscamera-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-28 03:53:06.133165 ovos-PHAL-rediscamera-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-28 03:52:59.000000 ovos-PHAL-rediscamera-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 03:53:06.129165 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-28 03:52:59.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-28 03:52:59.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-28 03:52:59.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-28 03:53:02.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 03:53:06.129165 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-28 03:53:05.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-28 03:53:06.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 03:53:05.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-28 03:53:05.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-28 03:53:05.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 03:53:05.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 03:53:05.000000 ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 03:53:06.133165 ovos-PHAL-rediscamera-0.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2952 2024-02-28 03:52:59.000000 ovos-PHAL-rediscamera-0.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:23:02.236630 ovos-PHAL-rediscamera-0.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-23 21:23:02.236630 ovos-PHAL-rediscamera-0.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-23 21:22:54.000000 ovos-PHAL-rediscamera-0.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:23:02.236630 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-23 21:22:54.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 21:22:54.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-23 21:22:54.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 21:22:58.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:23:02.236630 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-23 21:23:01.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 21:23:02.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:23:01.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 21:23:01.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 21:23:01.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 21:23:01.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:23:01.000000 ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:23:02.240630 ovos-PHAL-rediscamera-0.0.0a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2952 2024-04-23 21:22:54.000000 ovos-PHAL-rediscamera-0.0.0a3/setup.py
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/PKG-INFO` & `ovos-PHAL-rediscamera-0.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-rediscamera
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: Expose OVOS cameras to IOT frameworks
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-rediscamera
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/README.md` & `ovos-PHAL-rediscamera-0.0.0a3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,30 +11,48 @@
 
 You can find dedicated redis documentation elsewhere, the easiest way to get started is with docker
 
 `docker run -p 6379:6379 --name redis -d redis`
 
 ## Configuration
 
+### Redis
+
+for voice and face recognition a companion Redis server needs to be running
+
+This is where buffers for mic and camera data are stored, allowing access to remote cameras/mic data from several devices
+
+a OVOS skill can then access a specific camera/microphone by id by retrieving the feed from redis
+
+Redis access is configured globally for all OVOS components in `mycroft.conf`
+
+```json
+{
+  "redis": {
+    "host": "my-redis.cloud.redislabs.com",
+    "port": 6379,
+    "username": "default",
+    "password": "secret",
+    "ssl": true,
+    "ssl_certfile": "./redis_user.crt",
+    "ssl_keyfile": "./redis_user_private.key",
+    "ssl_ca_certs": "./redis_ca.pem"
+  }
+}
+```
+
+### Plugin
+
 ```javascript
 {
   "PHAL": {
     "ovos-PHAL-rediscamera": {
       "device_name": "my_phal_device",
       "camera_index": 0,
-      "serve_mjpeg": false, // serve a mjpeg camera stream at http://0.0.0.0:5000/video_feed
-      "host": "my-redis.cloud.redislabs.com",
-      // below are all optional redis options
-      "port": 6379,
-      "username": "default", // use your Redis user. More info https://redis.io/docs/management/security/acl/
-      "password": "secret", // use your Redis password
-      "ssl": true,
-      "ssl_certfile": "./redis_user.crt",
-      "ssl_keyfile": "./redis_user_private.key",
-      "ssl_ca_certs": "./redis_ca.pem"
+      "serve_mjpeg": false // serve a mjpeg camera stream at http://0.0.0.0:5000/video_feed
     }
   }
 }
 ```
 
 ## Home Assistant
 
@@ -63,12 +81,12 @@
         """Retrieve Numpy array from Redis camera 'self.name' """
         encoded = self.r.get(self.name)
         h, w = struct.unpack('>II', encoded[:8])
         a = np.frombuffer(encoded, dtype=np.uint8, offset=8).reshape(h, w, 3)
         return a
 
 
-remote_cam = RedisCameraReader("laptop", "192.168.1.17")
+remote_cam = RedisCameraReader("laptop")
 while True:
     frame = remote_cam.get()
     # do stuff
 ```
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/__init__.py` & `ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import struct
 from threading import Thread, Event
 
 import cv2
 import redis
 from ovos_plugin_manager.templates.phal import PHALPlugin
 from ovos_utils import create_daemon
-
+from ovos_config import Configuration
 from ovos_PHAL_rediscamera.server import get_app
 
 
 class RedisStream(Thread):
-    def __init__(self, name, host, camera_index=0, port=6379, **kwargs):
+    def __init__(self, name, camera_index=0):
         super().__init__(daemon=True)
         self.stream = cv2.VideoCapture(camera_index)
         # Redis connection
-        kwargs = {k: v for k, v in kwargs.items()
-                  if k in ["username", "password", "ssl",
-                           "ssl_certfile", "ssl_keyfile", "ssl_ca_certs"]}
-        self.r = redis.Redis(host=host, port=port, **kwargs)
+        kwargs = Configuration().get("redis", {"host": "127.0.0.1", "port": 6379})
+        self.r = redis.Redis(**kwargs)
         self.r.ping()
-        self.name = name
+        self.name = "cam::" + name
         self.stopped = Event()
 
     def run(self):
         while not self.stopped.is_set():
             (self.grabbed, self.frame) = self.stream.read()
             h, w = self.frame.shape[:2]
             shape = struct.pack('>II', h, w)
@@ -34,17 +32,18 @@
     def stop(self):
         self.stopped.set()
 
 
 class PHALRedisCamera(PHALPlugin):
     def __init__(self, bus, name="phal_rediscamera", config=None):
         config = config or {}
-        if "host" not in config:
-            raise ValueError("redis2mjpeg server host not set in config")
-        self.sender = RedisStream(**config)
+        if "device_name" not in config:
+            raise ValueError("camera device_name not set in config")
+        self.sender = RedisStream(name=config["device_name"],
+                                  camera_index=config.get("camera_index", 0))
         super().__init__(bus, name, config or {})
         if config.get("serve_mjpeg"):
             self.server = create_daemon(self.serve_mjpeg)
         else:
             self.server = None
 
     def serve_mjpeg(self):
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/__main__.py` & `ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,21 @@
+import click
 from ovos_config import Configuration
 from ovos_utils import wait_for_exit_signal
-
 from ovos_utils.fakebus import FakeBus
+
 from ovos_PHAL_rediscamera import PHALRedisCamera
 
 
-def standalone_launch(conf = None):
-    conf = conf or Configuration().get("PHAL", {}).get("ovos-PHAL-rediscamera", {})
+@click.command()
+@click.option('--camera-id', type=str, help='Name of the device running the camera.')
+@click.option('--camera-index', default=0, type=int, help='Index of the camera to be used.')
+def standalone_launch(camera_id, camera_index):
+    conf = Configuration().get("PHAL", {}).get("ovos-PHAL-rediscamera", {})
+    conf.update({"camera_index": camera_index, "device_name": camera_id})
     s = PHALRedisCamera(bus=FakeBus(), config=conf)
-
     wait_for_exit_signal()
-    print("Redis server needs to be running")
+    s.shutdown()
 
 
 if __name__ == "__main__":
-    # TODO kwargs
-    conf = {
-        "camera_index": 0,
-        "name": "laptop",
-        "host": "192.168.1.17",
-        "serve_mjpeg": True
-    }
-    standalone_launch(conf)
+    standalone_launch()
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera/server.py` & `ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera/server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import struct
-
+import click
 import cv2
 import numpy as np
 import redis
-from flask import Flask, Response
+from ovos_config import Configuration
 
 
 class RedisCameraReader:
 
-    def __init__(self, name, host, port=6379,  **kwargs):
-        # Redis connection
-        kwargs = {k: v for k,v in kwargs.items()
-                  if k in ["username", "password", "ssl",
-                           "ssl_certfile", "ssl_keyfile", "ssl_ca_certs"]}
-        self.r = redis.Redis(host=host, port=port, **kwargs)
+    def __init__(self, device_name: str):
+        kwargs = Configuration().get("redis", {"host": "127.0.0.1", "port": 6379})
+        self.r = redis.Redis(**kwargs)
         self.r.ping()
-        self.name = name
+        self.name = "cam::" + device_name
 
     def get(self, name=None):
         """Retrieve Numpy array from Redis key 'n'"""
         encoded = self.r.get(name or self.name)
         h, w = struct.unpack('>II', encoded[:8])
         a = np.frombuffer(encoded, dtype=np.uint8, offset=8).reshape(h, w, 3)
         return a
 
 
 def get_app(**kwargs):
+    # imported here to make flask dependency optional
+    # mjpeg server is not the main purpose of the plugin
+    from flask import Flask, Response
+
     app = Flask(__name__)
 
     image_hub = RedisCameraReader(**kwargs)
 
     def _gen_frames(name=None):  # generate frame by frame from camera
         name = name or image_hub.name
         while True:
-            frame = image_hub.get(name)
+            frame = image_hub.get("cam::" + name)
             if frame is None:
                 continue
             try:
                 ret, jpeg = cv2.imencode('.jpg', frame)
                 yield (b'--frame\r\n'
                        b'Content-Type: image/jpeg\r\n\r\n' + jpeg.tobytes() + b'\r\n')
             except Exception as e:
@@ -50,19 +51,19 @@
     @app.route('/video_feed/<name>')
     def named_video_feed(name):
         return Response(_gen_frames(name), mimetype='multipart/x-mixed-replace; boundary=frame')
 
     return app
 
 
-def main():
-    # TODO kwargs
-    conf = {
-        "name": "redis2mjpeg",
-        "host": "192.168.1.17"
-    }
-    app = get_app(**conf)
+@click.command()
+@click.option('--camera-id', type=str, help='Name of the device running the camera.')
+@click.option('--camera-index', default=0, type=int, help='Index of the camera to be used.')
+def main(camera_id, camera_index):
+    """Launch the PHALRedisCamera with specified configurations."""
+    app = get_app(camera_index=camera_index,
+                  device_name=camera_id)
     app.run(host="0.0.0.0")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/ovos_PHAL_rediscamera.egg-info/PKG-INFO` & `ovos-PHAL-rediscamera-0.0.0a3/ovos_PHAL_rediscamera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-rediscamera
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: Expose OVOS cameras to IOT frameworks
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-rediscamera
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-rediscamera-0.0.0a2/setup.py` & `ovos-PHAL-rediscamera-0.0.0a3/setup.py`

 * *Files identical despite different names*

