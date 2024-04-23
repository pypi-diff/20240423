# Comparing `tmp/democrite-0.2.2.223.tar.gz` & `tmp/democrite-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democrite-0.2.2.223.tar", last modified: Thu Jan 18 23:01:26 2024, max compression
+gzip compressed data, was "democrite-4.1.1.tar", last modified: Tue Apr 23 19:20:30 2024, max compression
```

## Comparing `democrite-0.2.2.223.tar` & `democrite-4.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-18 23:01:26.430223 democrite-0.2.2.223/
--rw-r--r--   0 vsts      (1001) docker     (127)     2468 2024-01-18 23:01:26.430223 democrite-0.2.2.223/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1928 2024-01-18 23:00:53.000000 democrite-0.2.2.223/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-18 23:01:26.430223 democrite-0.2.2.223/democrite.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2468 2024-01-18 23:01:26.000000 democrite-0.2.2.223/democrite.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-01-18 23:01:26.000000 democrite-0.2.2.223/democrite.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-18 23:01:26.000000 democrite-0.2.2.223/democrite.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-01-18 23:01:26.000000 democrite-0.2.2.223/democrite.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    10073 2024-01-18 23:00:53.000000 democrite-0.2.2.223/democrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-01-18 23:01:15.000000 democrite-0.2.2.223/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-01-18 23:01:26.430223 democrite-0.2.2.223/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 19:20:30.183455 democrite-4.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2463 2024-04-23 19:20:30.179455 democrite-4.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1928 2024-04-23 19:20:18.000000 democrite-4.1.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 19:20:30.179455 democrite-4.1.1/democrite.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2463 2024-04-23 19:20:30.000000 democrite-4.1.1/democrite.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-04-23 19:20:30.000000 democrite-4.1.1/democrite.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-23 19:20:30.000000 democrite-4.1.1/democrite.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-04-23 19:20:30.000000 democrite-4.1.1/democrite.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    10432 2024-04-23 19:20:18.000000 democrite-4.1.1/democrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      533 2024-04-23 19:20:26.000000 democrite-4.1.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-23 19:20:30.183455 democrite-4.1.1/setup.cfg
```

### Comparing `democrite-0.2.2.223/PKG-INFO` & `democrite-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: democrite
-Version: 0.2.2.223
+Version: 4.1.1
 Summary: Library use to construct VGrain to democrite servers
 Author-email: Nexai <info@nexai.net>
 Project-URL: Homepage, https://github.com/Nexai-net/democrite
 Project-URL: Issues, https://github.com/Nexai-net/democrite/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 Democrite
```

### Comparing `democrite-0.2.2.223/README.md` & `democrite-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `democrite-0.2.2.223/democrite.egg-info/PKG-INFO` & `democrite-4.1.1/democrite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: democrite
-Version: 0.2.2.223
+Version: 4.1.1
 Summary: Library use to construct VGrain to democrite servers
 Author-email: Nexai <info@nexai.net>
 Project-URL: Homepage, https://github.com/Nexai-net/democrite
 Project-URL: Issues, https://github.com/Nexai-net/democrite/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 Democrite
```

### Comparing `democrite-0.2.2.223/democrite.py` & `democrite-4.1.1/democrite.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import base64
 import socket
 import struct
 import codecs
 import concurrent.futures
 
 from abc import ABC, abstractmethod 
-from asyncio.windows_events import NULL
+# from asyncio.windows_events import NULL
 
 class LogLevel:
     """
     Defines logging severity levels.
     """
 
     Trace = 0,
@@ -52,24 +52,25 @@
 class _messageType:
     USER = 0
     SYSTEM = 1
     PING = 2
     PONG = 3
 
 class _remoteCommandServer:
-    def __init__(self, port:int, callback):
+    def __init__(self, port:int, serverIp:str, callback):
         self._port = port
+        self._serverIP = serverIp
         self._callback = callback
         self._executor = concurrent.futures.ThreadPoolExecutor()
 
     def __private__sendResponse_with_message_type(self, id:str, result: str, messageType: _messageType):
         finalData = struct.pack("!B", messageType)
         finalData += codecs.utf_8_encode(id)[0] 
 
-        if(result != NULL):
+        if(result is not None):
             finalData += codecs.utf_8_encode(result)[0] 
 
         fullFinalData = struct.pack("H", len(finalData)) + finalData
         self._socket.send(fullFinalData)
 
     def __private__executeCommand_async(self, msgid:str, compressedCmd:str):
         result = self._callback(compressedCmd)
@@ -79,15 +80,15 @@
         self.__private__sendResponse_with_message_type(id, result, messageType)
 
     def run(self):
         if (hasattr(self, '_socket')):
             return
 
         self._socket = socket.socket(socket.AddressFamily.AF_INET, socket.SocketKind.SOCK_STREAM);
-        self._socket.connect(("localhost", self._port));
+        self._socket.connect((self._serverIP, self._port));
 
         pkgSize = [] 
         while (True):
             
             pkgSizeArrayBytes = self._socket.recv(2)
 
             if (len(pkgSizeArrayBytes) < 2):
@@ -104,15 +105,15 @@
 
             msg = str()
             if (len(containerData) > 37):
                 msg = codecs.utf_8_decode(containerData[37:])[0]
                 # msg = base64.b64encode(msgDataStr)
 
             if (msgType == _messageType.PING):
-                self.__private__sendResponse_with_message_type(msgId, NULL, _messageType.PONG)
+                self.__private__sendResponse_with_message_type(msgId, None, _messageType.PONG)
                 continue
 
             if (msgType == _messageType.USER):
                 self._executor.submit(self.__private__executeCommand_async, msgId, msg)
                 continue
 
         print("Server Stopped")
@@ -213,63 +214,72 @@
 def execFunc(command=vgrainCommand, tools=vgrainTools): ...
 
 class vgrain:
     """ Base class of VGRain used execute democrite jobs"""
     
     def __init__(self, args: list[str]):
 
+        self._serverIP = "127.0.0.1"
+
         # Search in arguments the command information "--cmd:'CMD_JSON_BASE64'"
-        for arg in args:
+        argCopy = args.copy();
+        for arg in argCopy:
 
             if (arg.startswith("--cmd:'")):
                 remainLen = len(arg) - 1
                 self._command = arg[7:remainLen]
                 args.remove(arg)
 
             if (arg.startswith("--port:")):
                 remainLen = len(arg)
                 self._remotePort = int(arg[7:remainLen])
                 args.remove(arg)
 
+            if (arg.startswith("--server:")):
+                remainLen = len(arg)
+                self._serverIP = arg[9:remainLen]
+                args.remove(arg)
+
         self._arguments = args
+        print("ServerIp: " + self._serverIP + ":" + str(self._remotePort))
         
     def test(self, data, func: execFunc):
         """ Execute the command pass by argument to test """
         
         testCommandContainer = { 
             'FlowUid' : uuid.uuid4().hex, 
             'ExecutionId' : uuid.uuid4().hex, 
             'Content' : data 
         }
         
         formatCommand = self.__private_format_command(testCommandContainer)
         result, _ = self.__private_execute_command(formatCommand, func)
 
-        if (result != NULL):
+        if (result is not None):
             print("Result : " + json.dumps(result))
 
         print("Original Data : " + json.dumps(data))
 
     def execute(self, func: execFunc) -> None:
         """ Execute the command pass by command line arguments in oneshot """
 
-        if self._command == NULL:
+        if self._command is None:
             raise KeyError("Command not found, ensure the command is pass using --cmd:'CMD_JSON_BASE64'")
 
         response, cmd  = self.__private_execute_command(self._command, func)
         formatResponse = self.__private_format_command(response)
         print(cmd.get_execution_uid() + ":" + formatResponse)
 
     def run(self, func: execFunc):
         """ Run in background and process all command send """
         callback = lambda compressedMsg=str : self.__private_execute_command_and_format(compressedMsg, func)
-        self._remoteServer = _remoteCommandServer(self._remotePort, callback)
+        self._remoteServer = _remoteCommandServer(self._remotePort, self._serverIP, callback)
         self._remoteServer.run()
 
-    def __private_execute_command(self, compressCommand: str, func: execFunc) -> dict[str, any] | vgrainCommand:
+    def __private_execute_command(self, compressCommand: str, func: execFunc) -> dict[str, any]:
         """ Execute  compressCommand (UTF-8 Json in base64 ) """
 
         bytes = base64.b64decode(compressCommand)
         cmd = json.loads(bytes)
 
         vgrainCmd = vgrainCommand(cmd["FlowUid"], cmd["ExecutionId"], cmd["Content"])
 
@@ -303,10 +313,10 @@
     
     def __private_format_command(self, cmd) -> str:
         jsonValue = json.dumps(cmd);
         byte_data = jsonValue.encode('utf-8')
         formatCommand = base64.b64encode(byte_data);
         return codecs.utf_8_decode(formatCommand)[0]
     
-    def __private_execute_command_and_format(self, compressCommand: str, func: execFunc) -> dict[str, any] | vgrainCommand:
+    def __private_execute_command_and_format(self, compressCommand: str, func: execFunc) -> dict[str, any]:
         response, cmd  = self.__private_execute_command(compressCommand, func)
         return self.__private_format_command(response)
```

### Comparing `democrite-0.2.2.223/pyproject.toml` & `democrite-4.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "democrite"
-version = "0.2.2.223"
+version = "4.1.1"
 authors = [
   { name="Nexai", email="info@nexai.net" },
 ]
 
 description = "Library use to construct VGrain to democrite servers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Nexai-net/democrite"
```

