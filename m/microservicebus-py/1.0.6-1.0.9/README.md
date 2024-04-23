# Comparing `tmp/microservicebus-py-1.0.6.tar.gz` & `tmp/microservicebus-py-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-1.0.6.tar", last modified: Tue Jan 30 19:53:35 2024, max compression
+gzip compressed data, was "microservicebus-py-1.0.9.tar", last modified: Tue Apr 23 11:22:45 2024, max compression
```

## Comparing `microservicebus-py-1.0.6.tar` & `microservicebus-py-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2024-01-30 19:53:35.572837 microservicebus-py-1.0.6/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       18 2023-10-14 17:57:25.000000 microservicebus-py-1.0.6/MANIFEST.in
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2024-01-30 19:53:35.570835 microservicebus-py-1.0.6/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-1.0.6/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2024-01-30 19:53:35.389708 microservicebus-py-1.0.6/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2024-01-30 19:53:35.000000 microservicebus-py-1.0.6/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      513 2024-01-30 19:53:35.000000 microservicebus-py-1.0.6/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2024-01-30 19:53:35.000000 microservicebus-py-1.0.6/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2024-01-30 19:53:35.000000 microservicebus-py-1.0.6/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2024-01-30 19:53:35.000000 microservicebus-py-1.0.6/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2024-01-30 19:53:35.574246 microservicebus-py-1.0.6/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-10-14 17:55:13.000000 microservicebus-py-1.0.6/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2024-01-30 19:53:35.558326 microservicebus-py-1.0.6/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-1.0.6/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     7587 2023-11-27 13:25:43.000000 microservicebus-py-1.0.6/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4851 2024-01-21 18:26:08.000000 microservicebus-py-1.0.6/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    36774 2024-01-30 19:48:05.000000 microservicebus-py-1.0.6/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6688 2024-01-21 18:20:42.000000 microservicebus-py-1.0.6/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      775 2024-01-30 19:43:23.000000 microservicebus-py-1.0.6/src/package.json
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-1.0.6/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4676 2023-11-09 13:12:43.000000 microservicebus-py-1.0.6/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      822 2023-11-08 22:07:59.000000 microservicebus-py-1.0.6/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-1.0.6/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      215 2024-01-30 18:34:05.000000 microservicebus-py-1.0.6/src/updateMsb.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5169 2024-01-30 18:33:13.000000 microservicebus-py-1.0.6/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-1.0.6/src/vpn_helper.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1221 2023-09-19 11:22:46.000000 microservicebus-py-1.0.6/src/watchdog_service.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2024-04-23 11:22:45.912746 microservicebus-py-1.0.9/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       18 2023-10-14 17:57:25.000000 microservicebus-py-1.0.9/MANIFEST.in
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2024-04-23 11:22:45.905722 microservicebus-py-1.0.9/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-1.0.9/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2024-04-23 11:22:45.567181 microservicebus-py-1.0.9/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2024-04-23 11:22:45.000000 microservicebus-py-1.0.9/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      513 2024-04-23 11:22:45.000000 microservicebus-py-1.0.9/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2024-04-23 11:22:45.000000 microservicebus-py-1.0.9/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2024-04-23 11:22:45.000000 microservicebus-py-1.0.9/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2024-04-23 11:22:45.000000 microservicebus-py-1.0.9/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2024-04-23 11:22:45.915069 microservicebus-py-1.0.9/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-10-14 17:55:13.000000 microservicebus-py-1.0.9/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2024-04-23 11:22:45.880066 microservicebus-py-1.0.9/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-1.0.9/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     7587 2023-11-27 13:25:43.000000 microservicebus-py-1.0.9/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4916 2024-04-23 10:51:29.000000 microservicebus-py-1.0.9/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    36827 2024-04-23 10:50:57.000000 microservicebus-py-1.0.9/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6688 2024-01-21 18:20:42.000000 microservicebus-py-1.0.9/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      775 2024-04-23 11:20:23.000000 microservicebus-py-1.0.9/src/package.json
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-1.0.9/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4676 2023-11-09 13:12:43.000000 microservicebus-py-1.0.9/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      822 2023-11-08 22:07:59.000000 microservicebus-py-1.0.9/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-1.0.9/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      215 2024-02-17 13:26:04.000000 microservicebus-py-1.0.9/src/updateMsb.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5523 2024-04-23 10:55:02.000000 microservicebus-py-1.0.9/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-1.0.9/src/vpn_helper.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1221 2023-09-19 11:22:46.000000 microservicebus-py-1.0.9/src/watchdog_service.py
```

### Comparing `microservicebus-py-1.0.6/PKG-INFO` & `microservicebus-py-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 1.0.6
+Version: 1.0.9
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-1.0.6/README.md` & `microservicebus-py-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-1.0.9/microservicebus_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 1.0.6
+Version: 1.0.9
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-1.0.6/microservicebus_py.egg-info/SOURCES.txt` & `microservicebus-py-1.0.9/microservicebus_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/setup.py` & `microservicebus-py-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/axians.py` & `microservicebus-py-1.0.9/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/base_service.py` & `microservicebus-py-1.0.9/src/base_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/logger_service.py` & `microservicebus-py-1.0.9/src/logger_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     format='%(asctime)s: %(message)s',
     encoding='utf-8',
     level=logging.WARNING
 )
 
 class Logger(BaseService):
     def __init__(self, id, queue):
-        self.debug = True
+        self.debug = False
         super(Logger, self).__init__(id, queue)
 
     async def Start(self):
-        await self.Debug("Started.")
-
         self.settings = self.get_settings()
+        self.debug = self.settings["debug"]
+        await self.Debug(f"Started. Debug: {self.debug}")
         sb_namespace = self.settings["sbNamespace"]
         trackingHubName = self.settings["trackingHubName"]
         self.tracking_uri = f"https://{sb_namespace}.servicebus.windows.net/{trackingHubName}/messages?timeout=60"
 
         while True:
             await asyncio.sleep(0.1)
     async def msb_signed_in(self, args):
```

### Comparing `microservicebus-py-1.0.6/src/msb_handler.py` & `microservicebus-py-1.0.9/src/msb_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
                             if enabled_config["value"] == False:
                                 continue
                             
                             organization_id = sign_in_response["organizationId"]
                             file_name = pythonActivity["userData"]["type"].replace("_py", ".py")
 
                             uri = f"{self.base_uri}/api/Scripts/{organization_id}/{file_name}" if pythonActivity["userData"]["isCustom"] == True else f"{self.base_uri}/api/Scripts/00000000-0000-0000-0000-000000000001/{file_name}"
-
+                            asyncio.run(self.Debug(f"isCustom: {pythonActivity["userData"]["isCustom"]}"))
                             bind_to_version = pythonActivity["userData"]["bindToVersion"]
                             script_version = pythonActivity["userData"]["version"]
 
                             if bind_to_version == True:
                                 uri = f"{uri}/{script_version}"
 
                             service_file = requests.get(uri, allow_redirects=True, verify=False)
@@ -488,15 +488,14 @@
 
     def not_implemented(self, event_handler):
         asyncio.run(self.ThrowError(
             f'SignalR event handler \033[93m"{event_handler}"\033[0m is not implemented in the Python Node'))
 
     def ping_response(self, conn_id):
         try:
-            asyncio.run(self.Debug(f"Ping request"))
             settings = self.get_settings()
             self.connection.send("pingResponse", [ settings["nodeName"], socket.gethostname(), "Online", conn_id, False])
             asyncio.run(self.Debug("Ping response"))
         except Exception as e:
             asyncio.run(self.Debug(f"Error in ping_response: {e}"))
     
     def connected(self):
@@ -781,15 +780,15 @@
             asyncio.run(self.Debug(f"downloading file ({file_name}) to {directory}"))
             urllib.request.urlretrieve(uri, f"/{directory}/{file_name}")
             asyncio.run(self.Debug(f"download complete"))
             message = f"{file_name} has successfully been saved in ${directory} on ${node_name}."
             self.connection.send("notify", [connId, message, "INFO"])
 
         except Exception as ex:
-            asyncio.run(self.ThrowError(f"Error in msb.start: {e}"))
+            asyncio.run(self.ThrowError(f"Error in msb.start: {ex}"))
     # endregion
     # region Service callbacks
     async def request_connectionstring(self, message):
         action = message.message[0]["action"]     
         await self.SubmitAction(message.source, action, self.settings["receiveConnectionString"])
     async def terminal_output(self, message):
         connectionId = message.message[0]["connectionId"]
```

### Comparing `microservicebus-py-1.0.6/src/orchestrator_service.py` & `microservicebus-py-1.0.9/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/package.json` & `microservicebus-py-1.0.9/src/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'1.0.9'"}*

```diff
@@ -18,9 +18,9 @@
     "long_description": "",
     "long_description_content_type": "text/markdown",
     "name": "microservicebus-py",
     "packages": [
         "src"
     ],
     "url": "https://github.com/axians/microservicebus-py",
-    "version": "1.0.6"
+    "version": "1.0.9"
 }
```

### Comparing `microservicebus-py-1.0.6/src/rauc_handler.py` & `microservicebus-py-1.0.9/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/start.py` & `microservicebus-py-1.0.9/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/terminal_service.py` & `microservicebus-py-1.0.9/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/utils.py` & `microservicebus-py-1.0.9/src/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,22 @@
     return ip
 
 def getHwAddr(ifname):
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     info = fcntl.ioctl(s.fileno(), 0x8927,  struct.pack('256s', bytes(ifname, 'utf-8')[:15]))
     return ':'.join('%02x' % b for b in info[18:24])
 
-def check_version():
+def check_version(msb_dir):
     try:
         # Check if directory exists
-        msb_dir = f"{os.environ['HOME']}/msb-py"
+        if(msb_dir == ""):
+            msb_dir = f"{os.environ['HOME']}/msb-py"
+        
         if os.path.isdir(msb_dir) == False:
-            return
+            return False
 
         print("")
         print("*********************************************")
         print (f"current dir: {os.path.dirname(os.path.abspath(__file__))}")
         currentDirectory = os.path.dirname(os.path.abspath(__file__));
         preferedVersion = "latest"
         currentVersion = ""
@@ -30,24 +32,24 @@
         if os.path.exists(msb_settings_path):
             with open(msb_settings_path) as f:
                 settings = json.load(f)
                 preferedVersion = settings["coreVersion"]
                 print(f"preferedVersion: {preferedVersion}")
         else:
             print(f"{preferedVersion} does not exist")
-            return
+            return False
         
         with open(f"{currentDirectory}/package.json") as f:
             settings = json.load(f)
             currentVersion = settings["version"]
             print(f"currentVersion: {currentVersion}")
 
         if preferedVersion == "ignore":
             print("IGNORING VERSION")
-            return
+            return False
         elif preferedVersion == "latest":
             gitUri = "https://api.github.com/repos/axians/microservicebus-py/releases/latest"
             response = urllib.request.urlopen(gitUri)
             data = response.read()
             encoding = response.info().get_content_charset('utf-8')
             latest_release = json.loads(data.decode(encoding))
             preferedVersion = latest_release["tag_name"]
@@ -58,15 +60,15 @@
             gitUri = f"https://api.github.com/repos/axians/microservicebus-py/releases"
             response = urllib.request.urlopen(gitUri)
             data = response.read()
             encoding = response.info().get_content_charset('utf-8')
             releases = json.loads(data.decode(encoding))
             filtered = [x for x in releases if x['tag_name'] == preferedVersion]
             if len(filtered) == 0:
-                return
+                return False
             release = releases[0]
             tarball_url = release["tarball_url"]
             response = requests.get(tarball_url, stream=True)
 
             if response.status_code == 200:
                 install_dir = f"{currentDirectory}/../install"
                 if os.path.exists(f"{currentDirectory}/../install"):
@@ -100,10 +102,25 @@
                     os.remove(f"{currentDirectory}/{filename}")
 
                 for filename in os.listdir(f"{currentDirectory}/../src_new"):
                     print(f"\tCopying {filename}")
                     shutil.copyfile(f"{currentDirectory}/../src_new/{filename}", f"{currentDirectory}/{filename}")
                 #os.rename(f"{currentDirectory}/../src_new", f"{currentDirectory}")
                 print("Successfully updated")
+                return True
     
     except Exception as e:
-        print(f"Failed to update version: {e}")
+        print(f"Failed to update version: {e}")
+        return False
+
+def red(str):
+    return f"\033[1;31m{str}\033[0m"
+
+def green(str):
+    return f"\033[1;32m{str}\033[0m"
+
+def yellow(str):
+    return f"\033[1;33m{str}\033[0m"
+
+def purple(str):
+    return f"\033[95m{str}\033[0m"
+
```

### Comparing `microservicebus-py-1.0.6/src/vpn_helper.py` & `microservicebus-py-1.0.9/src/vpn_helper.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-1.0.6/src/watchdog_service.py` & `microservicebus-py-1.0.9/src/watchdog_service.py`

 * *Files identical despite different names*

