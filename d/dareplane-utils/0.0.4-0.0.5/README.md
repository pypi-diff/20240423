# Comparing `tmp/dareplane_utils-0.0.4.tar.gz` & `tmp/dareplane_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dareplane_utils-0.0.4.tar", last modified: Mon Jan 15 13:18:23 2024, max compression
+gzip compressed data, was "dareplane_utils-0.0.5.tar", last modified: Tue Apr 23 18:28:24 2024, max compression
```

## Comparing `dareplane_utils-0.0.4.tar` & `dareplane_utils-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.989871 dareplane_utils-0.0.4/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     1069 2023-06-06 11:52:12.000000 dareplane_utils-0.0.4/LICENSE
--rw-r--r--   0 matthias.dold   (502) staff       (20)     3930 2024-01-15 13:18:23.989680 dareplane_utils-0.0.4/PKG-INFO
--rw-r--r--   0 matthias.dold   (502) staff       (20)     3605 2024-01-11 12:12:16.000000 dareplane_utils-0.0.4/README.md
--rw-r--r--   0 matthias.dold   (502) staff       (20)      522 2024-01-15 13:17:26.000000 dareplane_utils-0.0.4/pyproject.toml
--rw-r--r--   0 matthias.dold   (502) staff       (20)       38 2024-01-15 13:18:23.989913 dareplane_utils-0.0.4/setup.cfg
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.986785 dareplane_utils-0.0.4/src/
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.986984 dareplane_utils-0.0.4/src/dareplane_utils/
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.988328 dareplane_utils-0.0.4/src/dareplane_utils/default_server/
--rw-r--r--   0 matthias.dold   (502) staff       (20)        0 2023-06-06 11:52:12.000000 dareplane_utils-0.0.4/src/dareplane_utils/default_server/__init__.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     4295 2024-01-15 13:15:40.000000 dareplane_utils-0.0.4/src/dareplane_utils/default_server/functions.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)    12676 2024-01-15 13:15:40.000000 dareplane_utils-0.0.4/src/dareplane_utils/default_server/server.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.988767 dareplane_utils-0.0.4/src/dareplane_utils/logging/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     1378 2024-01-15 13:11:11.000000 dareplane_utils-0.0.4/src/dareplane_utils/logging/logger.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     4024 2023-09-22 08:32:16.000000 dareplane_utils-0.0.4/src/dareplane_utils/logging/server.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)      767 2023-06-06 11:52:12.000000 dareplane_utils-0.0.4/src/dareplane_utils/logging/ujson_socket_handler.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.988908 dareplane_utils-0.0.4/src/dareplane_utils/stream_watcher/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     6192 2023-06-06 11:52:12.000000 dareplane_utils-0.0.4/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.989493 dareplane_utils-0.0.4/src/dareplane_utils.egg-info/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     3930 2024-01-15 13:18:23.000000 dareplane_utils-0.0.4/src/dareplane_utils.egg-info/PKG-INFO
--rw-r--r--   0 matthias.dold   (502) staff       (20)      678 2024-01-15 13:18:23.000000 dareplane_utils-0.0.4/src/dareplane_utils.egg-info/SOURCES.txt
--rw-r--r--   0 matthias.dold   (502) staff       (20)        1 2024-01-15 13:18:23.000000 dareplane_utils-0.0.4/src/dareplane_utils.egg-info/dependency_links.txt
--rw-r--r--   0 matthias.dold   (502) staff       (20)       16 2024-01-15 13:18:23.000000 dareplane_utils-0.0.4/src/dareplane_utils.egg-info/top_level.txt
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-01-15 13:18:23.989309 dareplane_utils-0.0.4/tests/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     2541 2023-06-06 11:52:12.000000 dareplane_utils-0.0.4/tests/test_default_server_process_book_keeping.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     2124 2023-06-06 11:52:12.000000 dareplane_utils-0.0.4/tests/test_default_server_thread_book_keeping.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     4120 2023-06-07 19:54:43.000000 dareplane_utils-0.0.4/tests/test_logging_server_client_communication.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.758080 dareplane_utils-0.0.5/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     1069 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/LICENSE
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     3995 2024-04-23 18:28:24.757894 dareplane_utils-0.0.5/PKG-INFO
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     3670 2024-04-23 18:24:44.000000 dareplane_utils-0.0.5/README.md
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      522 2024-04-23 18:27:30.000000 dareplane_utils-0.0.5/pyproject.toml
+-rw-r--r--   0 matthias.dold   (502) staff       (20)       38 2024-04-23 18:28:24.758127 dareplane_utils-0.0.5/setup.cfg
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.754707 dareplane_utils-0.0.5/src/
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.754974 dareplane_utils-0.0.5/src/dareplane_utils/
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.756306 dareplane_utils-0.0.5/src/dareplane_utils/default_server/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)        0 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/src/dareplane_utils/default_server/__init__.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     4295 2024-01-15 13:15:40.000000 dareplane_utils-0.0.5/src/dareplane_utils/default_server/functions.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)    12801 2024-04-23 17:44:11.000000 dareplane_utils-0.0.5/src/dareplane_utils/default_server/server.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.756622 dareplane_utils-0.0.5/src/dareplane_utils/general/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     6827 2024-04-13 14:51:34.000000 dareplane_utils-0.0.5/src/dareplane_utils/general/ringbuffer.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      777 2024-04-09 14:20:21.000000 dareplane_utils-0.0.5/src/dareplane_utils/general/time.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757014 dareplane_utils-0.0.5/src/dareplane_utils/logging/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     1559 2024-01-19 11:17:32.000000 dareplane_utils-0.0.5/src/dareplane_utils/logging/logger.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     5739 2024-04-23 17:29:50.000000 dareplane_utils-0.0.5/src/dareplane_utils/logging/server.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      767 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/src/dareplane_utils/logging/ujson_socket_handler.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757140 dareplane_utils-0.0.5/src/dareplane_utils/stream_watcher/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     4955 2024-04-12 09:08:14.000000 dareplane_utils-0.0.5/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757690 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     3995 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/PKG-INFO
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      756 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias.dold   (502) staff       (20)        1 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias.dold   (502) staff       (20)       16 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/top_level.txt
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757519 dareplane_utils-0.0.5/tests/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     2541 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/tests/test_default_server_process_book_keeping.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     2124 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/tests/test_default_server_thread_book_keeping.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     4120 2023-06-07 19:54:43.000000 dareplane_utils-0.0.5/tests/test_logging_server_client_communication.py
```

### Comparing `dareplane_utils-0.0.4/LICENSE` & `dareplane_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.4/PKG-INFO` & `dareplane_utils-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dareplane_utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Default utilities for the dareplane platform
 Author-email: Matthias Dold <matthias.dold@gmx.net>
 Project-URL: homepage, https://github.com/matthiasdold/dareplane-pyutils
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -108,7 +108,11 @@
 
 ## The above is using the following implementation
     def unfold_buffer(self):
         return np.vstack(
             [self.buffer[self.curr_i :], self.buffer[: self.curr_i]]
         )
 ```
+
+## TODO
+
+- [ ] channel names are only initialized on connection
```

### Comparing `dareplane_utils-0.0.4/README.md` & `dareplane_utils-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,7 +98,11 @@
 
 ## The above is using the following implementation
     def unfold_buffer(self):
         return np.vstack(
             [self.buffer[self.curr_i :], self.buffer[: self.curr_i]]
         )
 ```
+
+## TODO
+
+- [ ] channel names are only initialized on connection
```

### Comparing `dareplane_utils-0.0.4/pyproject.toml` & `dareplane_utils-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dareplane_utils"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{name="Matthias Dold", email="matthias.dold@gmx.net"}]
 description = "Default utilities for the dareplane platform"
 readme ="README.md"
 requires-python = ">=3.10"
 
 [project.urls]
 "homepage" = "https://github.com/matthiasdold/dareplane-pyutils"
```

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils/default_server/functions.py` & `dareplane_utils-0.0.5/src/dareplane_utils/default_server/functions.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils/default_server/server.py` & `dareplane_utils-0.0.5/src/dareplane_utils/default_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,40 +69,17 @@
                 )
                 raise err
 
             self.current_conn = current_conn
             self.current_conn.sendall(f"Connected to {self.name}\n".encode())
             while not self.listen_stop_event.is_set():
                 try:
-                    msg = self.current_conn.recv(1024)
+                    msg = self.current_conn.recv(2048)
                     if msg:
-                        self.logger.info(f"Received: {msg}")
-                        # interpret the message
-
-                        # Default functionality which should always be there
-                        # and the same for all servers
-                        is_default_command = self.default_msg_interpretation(
-                            msg
-                        )
-
-                        # if not a default command, check the pcmommand map
-                        if not is_default_command:
-                            msg = msg.replace(b"\r\n", b"")
-                            # common start byte, would lead to an error in decode otherwise # noqa
-                            msg = msg.replace(b"\xc2", b"")
-                            # Ignore blanks -> e.g. accidental return in telnet
-                            if (
-                                msg != b""
-                                and msg.decode("ascii").split("|")[0]
-                                in self.pcommand_map.keys()
-                            ):
-                                self.msg_interpretation(msg)
-
-                            else:
-                                self.logger.warning(f"Unknown pcomm in {msg=}")
+                        self.handle_msg(msg)
 
                 except socket.timeout as err:
                     self.logger.info(f"Caugth timeout error {err=}")
 
                 except KeyboardInterrupt as _:
                     self.logger.info(
                         "Received KeyboardInterrupt - stopping the server"
@@ -115,14 +92,47 @@
                 except Exception as err:
                     self.logger.error(f"Caught error {err=}")
                     self.is_listening = False
                     raise err
 
         self.is_listening = False
 
+    def handle_msg(self, msg: str):
+        """interpret the message"""
+
+        self.logger.info(f"Received: {msg}")
+        # Check if msg is concatenation of multiple commands, happends if
+        # processing of a single command takes to long so multiple commands
+        # end up at the socket
+        if b";" in msg:
+            for pc in msg.split(b";"):
+                if pc != b"":
+                    self.handle_msg(pc)
+        else:
+
+            # Default functionality which should always be there
+            # and the same for all servers
+            is_default_command = self.default_msg_interpretation(msg)
+
+            # if not a default command, check the pcmommand map
+            if not is_default_command:
+                msg = msg.replace(b"\r\n", b"")
+                # common start byte, would lead to an error in decode otherwise # noqa
+                msg = msg.replace(b"\xc2", b"")
+                # Ignore blanks -> e.g. accidental return in telnet
+                if (
+                    msg != b""
+                    and msg.decode("ascii").split("|")[0]
+                    in self.pcommand_map.keys()
+                ):
+                    self.msg_interpretation(msg)
+
+                else:
+                    self.logger.warning(f"Unknown pcomm in {msg=}")
+
     def default_msg_interpretation(self, msg: str) -> bool:
         """This contains the default interpretation"""
         if (
             msg == b"STOP\r\n"
             or msg == b"STOP"
             or msg == b"STOP|\r\n"
             or msg == b"STOP|"
```

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils/logging/logger.py` & `dareplane_utils-0.0.5/src/dareplane_utils/logging/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import logging
 import logging.config
 
 default_dareplane_config = {
     "version": 1,
     "formatters": {
-        "dareplane_standard": {
+        "dareplane_standard_color": {
             "()": "colorlog.ColoredFormatter",
             "format": "%(log_color)s%(asctime)s - %(name)s - %(levelname)s - %(reset)s %(white)s%(message)s",
-        }
+        },
+        "dareplane_standard": {
+            "format": "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+        },
     },
     "handlers": {
         "console": {
             "class": "logging.StreamHandler",
-            "formatter": "dareplane_standard",
+            "formatter": "dareplane_standard_color",
         },
         "socket": {
+            "formatter": "dareplane_standard",
             "class": "dareplane_utils.logging.ujson_socket_handler.UJsonSocketHandler",
             "host": "localhost",
             "port": 9020,
         },
     },
     "root": {
         "handlers": ["console", "socket"],
```

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils/logging/ujson_socket_handler.py` & `dareplane_utils-0.0.5/src/dareplane_utils/logging/ujson_socket_handler.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py` & `dareplane_utils-0.0.5/src/dareplane_utils/general/ringbuffer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,194 @@
-import pylsl
-import logging
-import xmltodict
-
+# A simple numpy ring buffer for data + timestamps
+# This was abstracted from the StreamWatcher class, as it is often useful on its own
 import numpy as np
 
 from dareplane_utils.logging.logger import get_logger
 
 logger = get_logger(__name__)
 
-# ch = logging.StreamHandler()
-# ch.setFormatter(logging.Formatter("%(levelname)s - %(asctime)s - %(message)s"))
-# logger.addHandler(ch)
-# logger.setLevel(10)
-#
-#
-
-
-class StreamWatcherNotConnected(ValueError):
-    pass
-
-
-def get_streams_names() -> list[str]:
-    """Get a list of all available lsl stream names.
-
-    Returns
-    -------
-    streams : list[str]
-        names of all available LSL streams
 
+class RingBuffer:
     """
 
-    return [s.name() for s in pylsl.resolve_streams()]
-
-
-def pylsl_xmlelement_to_dict(inf: pylsl.pylsl.StreamInfo) -> dict:
-    """
-    The pylsl XMLElement is hard to investigate -> cast to a dict for
-    simplicity
+    Attributes
+    ----------
+    buffer : np.ndarray
+        the data buffer
+    buffer_t : np.ndarray
+        the time buffer
+    last_t : float
+        latest time stamp
+    curr_i : int
+        index of the latest data point int the buffer
+    logger : logging.Logger
+        the logger used for warnings and debug messages
     """
-    return xmltodict.parse(inf.as_xml())
-
-
-def get_channel_names(inf: pylsl.pylsl.StreamInfo) -> list[str]:
-    d = pylsl_xmlelement_to_dict(inf)
-
-    # By adding to the xml meta data structure of LSL, if we only add one
-    # channel, the data will be a dict instead of a list of dicts
-
-    try:
-        if isinstance(d["info"]["desc"]["channels"]["channel"], dict):
-            return [d["info"]["desc"]["channels"]["channel"]["label"]]
-        else:
-            return [
-                ch_inf["label"]
-                for ch_inf in d["info"]["desc"]["channels"]["channel"]
-            ]
-    except TypeError as err:
-        return [f"ch_{i + 1}" for i in range(inf.channel_count())]
-
-
-class StreamWatcher:
-    def __init__(
-        self,
-        name: str = "",
-        buffer_size_s: float = 2,
-        logger: logging.Logger = logger,
-    ):
-        """
-        Parameters
-        ----------
-        name : str
-            Name tag to identify the manager -> could be same as the LSL stream
-            it should be watching
-        buffer_size_s : float
-            the data buffer size in seconds
-        """
-        self.name = name
-        self.buffer_size_s = buffer_size_s
-        self.stream = None
-        self.inlet = None
-
-        # Set after connection
-        self.n_buffer: int = 0
-        self.buffer_t: np.ndarray = np.asarray([])
-        self.buffer: np.ndarray = np.asarray([])
-        self.last_t: float = 0
-        self.curr_i: int = 0
-        self.samples: list[list[float]] = []
-        self.times: list[float] = []
-        self.n_new: int = 0
-
-        self.logger = logger
-
-    def connect_to_stream(self, identifier: dict | None = None):
-        """
-        Either use the self.name or a provided identifier dict to hook up
-        with an LSL stream, they should coincide
-        """
-        if identifier:
-            name = identifier["name"]
-            self.name = name
-        else:
-            name = self.name
-
-        self.streams = pylsl.resolve_byprop("name", name)
-        if len(self.streams) > 1:
-            print(f"Selecting stream by {name=} was ambigous - taking first")
-
-        self.inlet = pylsl.StreamInlet(self.streams[0])
-
-        self.channel_names = get_channel_names(self.inlet.info())
-
-        self._init_buffer()
-
-        # The first update call will return empty, so do it here already
-        self.update()
-
-    def _init_buffer(self):
-        if self.streams is None or self.inlet is None:
-            raise StreamWatcherNotConnected(
-                "StreamWatcher seems not connected, did you call"
-                " connect_to_stream() on it?"
-            )
-
-        # set a default value for irregular streams
-        if self.streams[0].nominal_srate() == 0:
-            n_samples = 1000
-        else:
-            n_samples = int(
-                self.streams[0].nominal_srate() * self.buffer_size_s
-            )
-
-        self.n_buffer = n_samples
 
+    def __init__(self, shape: tuple[int, int], dtype: type = np.float32):
         # Using numpy buffers
-        self.buffer = np.empty((n_samples, len(self.channel_names)))
-        self.buffer_t = np.empty(n_samples)
+        self.buffer = np.empty((shape[0], shape[1]), dtype=dtype)
+        self.buffer_t = np.empty(shape[0])
         self.last_t = 0  # last time stamp
         self.curr_i = 0
+        self.logger = logger
 
-    def add_samples(self, samples: list, times: list):
+    def legacy_add_samples(self, samples: list, times: list):
         if len(samples) > 0 and len(times) > 0:
-            if len(samples) > self.n_buffer:
+            buffer_size = self.buffer.shape[0]
+            if len(samples) > buffer_size:
                 self.logger.warning(
                     "Received more data than fitting into the"
                     " buffer. Will only add data to fill buffer"
                     " once with the latest data"
                 )
-
-                samples = samples[-self.n_buffer :]
-                times = times[-self.n_buffer :]
-
+                samples = samples[-buffer_size:]
+                times = times[-buffer_size:]
             # make it a ring buffer with FIFO
             old_i = self.curr_i
-
-            self.curr_i = (self.curr_i + len(samples)) % self.n_buffer
+            self.curr_i = (self.curr_i + len(samples)) % buffer_size
             # self.logger.debug(f"{old_i=}, {self.curr_i=}, {len(samples)=}")
-
             # plain forward fill
             if old_i < self.curr_i:
                 self.buffer[old_i : self.curr_i] = samples
                 self.buffer_t[old_i : self.curr_i] = times
             # fill buffer up
             elif self.curr_i == 0:
                 self.buffer[old_i:] = samples
                 self.buffer_t[old_i:] = times
-
             # split needed -> start over at beginning
             else:
                 self.logger.debug("Splitting data to add as buffer is full")
-                nfull = self.n_buffer - old_i
+                nfull = buffer_size - old_i
                 self.buffer[old_i:] = samples[:nfull]
                 self.buffer_t[old_i:] = times[:nfull]
-
                 self.buffer[: self.curr_i] = samples[nfull:]
                 self.buffer_t[: self.curr_i] = times[nfull:]
 
             self.last_t = times[-1]
 
-    def update(self):
-        """Look for new data and update the buffer"""
-        samples, times = self.inlet.pull_chunk()
-        self.add_samples(samples, times)
-        self.samples = samples
-        self.n_new += len(samples)
-
     def unfold_buffer(self):
         return np.vstack(
             [self.buffer[self.curr_i :], self.buffer[: self.curr_i]]
         )
 
     def unfold_buffer_t(self):
         # Do hstack here as the time buffer will be of dim (n,1) anyways
         return np.hstack(
             [self.buffer_t[self.curr_i :], self.buffer_t[: self.curr_i]]
         )
 
-    def disconnect(self):
-        """TODO to be implemented"""
-        pass
+    def get_insert_slices(self, len_samples: int) -> tuple[slice, slice, int]:
+        """Get slices mapping data from the samples to the buffer
+
+        Parameters
+        ----------
+        len_samples : int
+            number of samples to add
+
+        Returns
+        -------
+        tuple[list[slice], list[slice], int]
+
+        """
+        old_i = self.curr_i
+        new_i = (self.curr_i + len_samples) % self.buffer.shape[0]
+
+        if old_i < new_i:
+            return [slice(old_i, new_i)], [slice(0, len_samples)], new_i
+        elif new_i == 0:
+            return [slice(old_i, None)], [slice(0, len_samples)], new_i
+        else:
+            nfull = self.buffer.shape[0] - old_i
+            return (
+                [slice(old_i, None), slice(0, new_i)],
+                [slice(0, nfull), slice(nfull, None)],
+                new_i,
+            )
+
+    def add_samples(self, samples: list, times: list):
+        if len(samples) > 0 and len(times) > 0:
+            buffer_size = self.buffer.shape[0]
+            if len(samples) > buffer_size:
+                self.logger.warning(
+                    "Received more data than fitting into the"
+                    " buffer. Will only add data to fill buffer"
+                    " once with the latest data"
+                )
+                samples = samples[-buffer_size:]
+                times = times[-buffer_size:]
+            # make it a ring buffer with FIFO
+            slice_buffer, slice_samples, self.curr_i = self.get_insert_slices(
+                len(samples)
+            )
+            if len(slice_buffer) > 1:
+                self.logger.debug("Splitting data to add as buffer is full")
+                self.buffer[slice_buffer[0]] = samples[slice_samples[0]]
+                self.buffer_t[slice_buffer[0]] = times[slice_samples[0]]
+                self.buffer[slice_buffer[1]] = samples[slice_samples[1]]
+                self.buffer_t[slice_buffer[1]] = times[slice_samples[1]]
+
+            else:
+                self.buffer[slice_buffer[0]] = samples[slice_samples[0]]
+                self.buffer_t[slice_buffer[0]] = times[slice_samples[0]]
+
+            self.last_t = times[-1]
 
 
 if __name__ == "__main__":
-    sw = StreamWatcher("mock_EEG_stream")
-    sw.connect_to_stream()
+
+    x = np.random.rand(500_000, 5)
+    rb = RingBuffer((20_000, 5))
+    rb.add_samples(x[:1500], np.arange(1500))
+
+    np.random.seed(42)
+    inc = (np.random.rand(10) * 1000).astype(int)
+    ts = [np.arange(i) for i in inc]
+
+    def test_foo():
+        i = 0
+        for ic, t in zip(inc, ts):
+            rb.legacy_add_samples(x[i : i + ic], t)
+            i += ic
+
+    def test_foo_new():
+        i = 0
+        for ic, t in zip(inc, ts):
+            rb.add_samples(x[i : i + ic], t)
+            i += ic
+
+    # %timeit test_foo_new()
+    # %timeit test_foo()
+
+    # %timeit test_foo()
+    # --> old version without using get_insert_slices and using if statements
+    # In [18]:     %timeit test_foo()
+    # 15.5 µs ± 86.7 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    #
+    # New version is slower for a few 100 inserts, but up to 50% faster for smaller number of samples to add
+    # %timeit test_foo_new()
+    # 18.8 µs ± 35.4 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    #
+    # Also for a few 1000 inserts, speed is the same
+    #     #In [62]:     %timeit test_foo_new()
+    # 56 µs ± 1.03 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    #
+    # In [63]:     %timeit test_foo()
+    # 53.3 µs ± 1.21 µs per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    #
+    # In [64]: inc
+    # Out[64]: array([3745, 9507, 7319, 5986, 1560, 1559,  580, 8661, 6011, 7080])
+
+    #
+    # %timeit a=slice(5, 2000) --> ~40ns for defining as slice
+    #
+    # Select with slice vs index
+    # s = slice(5, 2000)
+    # idx = np.arange(5, 2000)
+    # %timeit x[s] --> 75ns
+    # %timeit x[idx] --> 17us!!!
+    #
+    #
+    #
+    # In [5]: %timeit rb.unfold_buffer()
+    # 8.3 µs ± 79.7 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    #
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils.egg-info/PKG-INFO` & `dareplane_utils-0.0.5/src/dareplane_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dareplane_utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Default utilities for the dareplane platform
 Author-email: Matthias Dold <matthias.dold@gmx.net>
 Project-URL: homepage, https://github.com/matthiasdold/dareplane-pyutils
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -108,7 +108,11 @@
 
 ## The above is using the following implementation
     def unfold_buffer(self):
         return np.vstack(
             [self.buffer[self.curr_i :], self.buffer[: self.curr_i]]
         )
 ```
+
+## TODO
+
+- [ ] channel names are only initialized on connection
```

### Comparing `dareplane_utils-0.0.4/src/dareplane_utils.egg-info/SOURCES.txt` & `dareplane_utils-0.0.5/src/dareplane_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 src/dareplane_utils.egg-info/PKG-INFO
 src/dareplane_utils.egg-info/SOURCES.txt
 src/dareplane_utils.egg-info/dependency_links.txt
 src/dareplane_utils.egg-info/top_level.txt
 src/dareplane_utils/default_server/__init__.py
 src/dareplane_utils/default_server/functions.py
 src/dareplane_utils/default_server/server.py
+src/dareplane_utils/general/ringbuffer.py
+src/dareplane_utils/general/time.py
 src/dareplane_utils/logging/logger.py
 src/dareplane_utils/logging/server.py
 src/dareplane_utils/logging/ujson_socket_handler.py
 src/dareplane_utils/stream_watcher/lsl_stream_watcher.py
 tests/test_default_server_process_book_keeping.py
 tests/test_default_server_thread_book_keeping.py
 tests/test_logging_server_client_communication.py
```

### Comparing `dareplane_utils-0.0.4/tests/test_default_server_process_book_keeping.py` & `dareplane_utils-0.0.5/tests/test_default_server_process_book_keeping.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.4/tests/test_default_server_thread_book_keeping.py` & `dareplane_utils-0.0.5/tests/test_default_server_thread_book_keeping.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.4/tests/test_logging_server_client_communication.py` & `dareplane_utils-0.0.5/tests/test_logging_server_client_communication.py`

 * *Files identical despite different names*

