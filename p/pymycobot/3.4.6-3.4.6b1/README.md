# Comparing `tmp/pymycobot-3.4.6.tar.gz` & `tmp/pymycobot-3.4.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.4.6.tar", last modified: Tue Apr 23 03:29:58 2024, max compression
+gzip compressed data, was "pymycobot-3.4.6b1.tar", last modified: Thu Apr 18 11:14:01 2024, max compression
```

## Comparing `pymycobot-3.4.6.tar` & `pymycobot-3.4.6b1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 03:29:58.033547 pymycobot-3.4.6/
--rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.6/LICENSE
--rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0    63942 2024-04-23 03:29:58.032549 pymycobot-3.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 03:29:57.990535 pymycobot-3.4.6/pymycobot/
--rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     2169 2024-04-23 03:13:04.000000 pymycobot-3.4.6/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.6/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    24941 2024-04-23 03:10:08.000000 pymycobot-3.4.6/pymycobot/common.py
--rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.6/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/error.py
--rw-rw-rw-   0        0        0    42593 2024-04-18 11:13:01.000000 pymycobot-3.4.6/pymycobot/generate.py
--rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.6/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.6/pymycobot/log.py
--rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.6/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mecharmsocket.py
--rw-rw-rw-   0        0        0     7695 2024-04-12 11:33:10.000000 pymycobot-3.4.6/pymycobot/mercury.py
--rw-rw-rw-   0        0        0    16855 2024-04-23 03:10:49.000000 pymycobot-3.4.6/pymycobot/mercury_api.py
--rw-rw-rw-   0        0        0     6460 2024-04-23 03:12:41.000000 pymycobot-3.4.6/pymycobot/mercurychassis.py
--rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.6/pymycobot/mercurysocket.py
--rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.6/pymycobot/myagv.py
--rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    16331 2024-04-22 09:53:52.000000 pymycobot-3.4.6/pymycobot/myarm_api.py
--rw-rw-rw-   0        0        0      273 2024-04-22 09:29:51.000000 pymycobot-3.4.6/pymycobot/myarmc.py
--rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.4.6/pymycobot/myarmm.py
--rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/myarmsocket.py
--rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0    85159 2024-04-18 01:28:43.000000 pymycobot-3.4.6/pymycobot/mycobotpro630.py
--rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.6/pymycobot/public.py
--rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.6/pymycobot/robot_limit.json
--rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.6/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.6/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 03:29:58.030546 pymycobot-3.4.6/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    63942 2024-04-23 03:29:57.000000 pymycobot-3.4.6/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1093 2024-04-23 03:29:57.000000 pymycobot-3.4.6/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 03:29:57.000000 pymycobot-3.4.6/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-23 03:29:57.000000 pymycobot-3.4.6/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-23 03:29:57.000000 pymycobot-3.4.6/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 03:29:58.033547 pymycobot-3.4.6/setup.cfg
--rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 03:29:58.029547 pymycobot-3.4.6/tests/
--rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.6/tests/test_api.py
--rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.6/tests/test_generator.py
--rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.6/tests/test_socket.py
--rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.6/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.391361 pymycobot-3.4.6b1/
+-rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    63944 2024-04-18 11:14:01.389362 pymycobot-3.4.6b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.6b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.349795 pymycobot-3.4.6b1/pymycobot/
+-rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     2171 2024-04-18 11:13:40.000000 pymycobot-3.4.6b1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    24930 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/common.py
+-rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.6b1/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    42593 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.6b1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.6b1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mecharmsocket.py
+-rw-rw-rw-   0        0        0     7695 2024-04-12 11:33:10.000000 pymycobot-3.4.6b1/pymycobot/mercury.py
+-rw-rw-rw-   0        0        0    16852 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mercury_api.py
+-rw-rw-rw-   0        0        0     6394 2024-03-01 10:10:12.000000 pymycobot-3.4.6b1/pymycobot/mercurychassis.py
+-rw-rw-rw-   0        0        0     2211 2024-03-21 08:57:25.000000 pymycobot-3.4.6b1/pymycobot/mercurychassisocket.py
+-rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.6b1/pymycobot/mercurysocket.py
+-rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.6b1/pymycobot/myagv.py
+-rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    16331 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarm_api.py
+-rw-rw-rw-   0        0        0      273 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarmc.py
+-rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarmm.py
+-rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/myarmsocket.py
+-rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0    85159 2024-04-18 01:28:43.000000 pymycobot-3.4.6b1/pymycobot/mycobotpro630.py
+-rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.6b1/pymycobot/public.py
+-rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.6b1/pymycobot/robot_limit.json
+-rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.388356 pymycobot-3.4.6b1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    63944 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1126 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.6b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:14:01.392361 pymycobot-3.4.6b1/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.6b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.386801 pymycobot-3.4.6b1/tests/
+-rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_api.py
+-rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_generator.py
+-rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_socket.py
+-rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_utils.py
```

### Comparing `pymycobot-3.4.6/LICENSE` & `pymycobot-3.4.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/PKG-INFO` & `pymycobot-3.4.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.6
+Version: 3.4.6b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.4.6/README.md` & `pymycobot-3.4.6b1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/Interface.py` & `pymycobot-3.4.6b1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/__init__.py` & `pymycobot-3.4.6b1/pymycobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.4.6"
+__version__ = "3.4.6b1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.4.6/pymycobot/bluet.py` & `pymycobot-3.4.6b1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/common.py` & `pymycobot-3.4.6b1/pymycobot/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         command_data = self._process_data_command(genre, self.__class__.__name__, args)
         if genre == 178:
             # 修改wifi端口
             command_data = self._encode_int16(command_data)
             
         elif genre in [76, 77]:
             command_data = [command_data[0]] + self._encode_int16(command_data[1]*10)
-        elif genre == 115 and self.__class__.__name__ not in  ["MyArmC", "MyArmM", "Mercury"]:
+        elif genre == 115 and self.__class__.__name__ not in  ["MyArmC", "MyArmM"]:
             command_data = [command_data[1],command_data[3]]
         LEN = len(command_data) + 2
         
         command = [
                 ProtocolCode.HEADER,
                 ProtocolCode.HEADER,
                 LEN,
```

### Comparing `pymycobot-3.4.6/pymycobot/elephantrobot.py` & `pymycobot-3.4.6b1/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/error.py` & `pymycobot-3.4.6b1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/generate.py` & `pymycobot-3.4.6b1/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/log.py` & `pymycobot-3.4.6b1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mecharmsocket.py` & `pymycobot-3.4.6b1/pymycobot/mecharmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mercury.py` & `pymycobot-3.4.6b1/pymycobot/mercury.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mercury_api.py` & `pymycobot-3.4.6b1/pymycobot/mercury_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,23 +187,23 @@
         Args:
             axis (_type_): _description_
             direction (_type_): _description_
             speed (_type_): _description_
         """
         return self._mesg(ProtocolCode.MERCURY_JOG_BASE_COORD, axis, direction, speed)
     
-    def drag_teach_save(self):
+    def drag_tech_save(self):
         """Start recording the dragging teaching point. In order to show the best sports effect, the recording time should not exceed 90 seconds."""
         return self._mesg(ProtocolCode.MERCURY_DRAG_TECH_SAVE)
     
-    def drag_teach_execute(self):
+    def drag_tech_execute(self):
         """Start dragging the teaching point and only execute it once."""
         return self._mesg(ProtocolCode.MERCURY_DRAG_TECH_EXECUTE)
     
-    def drag_teach_pause(self):
+    def drag_tech_pause(self):
         """Pause recording of dragging teaching point"""
         self._mesg(ProtocolCode.MERCURY_DRAG_TECH_PAUSE)
         
     def is_gripper_moving(self, mode=None):
         """Judge whether the gripper is moving or not
         
         Args:
```

### Comparing `pymycobot-3.4.6/pymycobot/mercurychassis.py` & `pymycobot-3.4.6b1/pymycobot/mercurychassis.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 import threading
 import struct
 
 class MercuryChassisError(Exception):
     pass
 
 class MercuryChassis:
-    """
-    Mercury X1 mobile chassis car socket class
-    """
     def __init__(self, ip=None):
         self.ifname = b"wlan0"
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         if ip is not None:
             self.host = ip
         else:
             import fcntl
```

### Comparing `pymycobot-3.4.6/pymycobot/mercurysocket.py` & `pymycobot-3.4.6b1/pymycobot/mercurysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/myagv.py` & `pymycobot-3.4.6b1/pymycobot/myagv.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/myarm.py` & `pymycobot-3.4.6b1/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/myarm_api.py` & `pymycobot-3.4.6b1/pymycobot/myarm_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/myarmm.py` & `pymycobot-3.4.6b1/pymycobot/myarmm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/myarmsocket.py` & `pymycobot-3.4.6b1/pymycobot/myarmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mybuddy.py` & `pymycobot-3.4.6b1/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mybuddybluetooth.py` & `pymycobot-3.4.6b1/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mybuddyemoticon.py` & `pymycobot-3.4.6b1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mybuddysocket.py` & `pymycobot-3.4.6b1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mycobot.py` & `pymycobot-3.4.6b1/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mycobotpro630.py` & `pymycobot-3.4.6b1/pymycobot/mycobotpro630.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mycobotsocket.py` & `pymycobot-3.4.6b1/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mypalletizer.py` & `pymycobot-3.4.6b1/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/mypalletizersocket.py` & `pymycobot-3.4.6b1/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/public.py` & `pymycobot-3.4.6b1/pymycobot/public.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/robot_limit.json` & `pymycobot-3.4.6b1/pymycobot/robot_limit.json`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/ultraArm.py` & `pymycobot-3.4.6b1/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot/utils.py` & `pymycobot-3.4.6b1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.4.6b1/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.6
+Version: 3.4.6b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.4.6/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.4.6b1/pymycobot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pymycobot/genre.py
 pymycobot/log.py
 pymycobot/mecharm.py
 pymycobot/mecharmsocket.py
 pymycobot/mercury.py
 pymycobot/mercury_api.py
 pymycobot/mercurychassis.py
+pymycobot/mercurychassisocket.py
 pymycobot/mercurysocket.py
 pymycobot/myagv.py
 pymycobot/myarm.py
 pymycobot/myarm_api.py
 pymycobot/myarmc.py
 pymycobot/myarmm.py
 pymycobot/myarmsocket.py
```

### Comparing `pymycobot-3.4.6/setup.py` & `pymycobot-3.4.6b1/setup.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/tests/test_api.py` & `pymycobot-3.4.6b1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/tests/test_generator.py` & `pymycobot-3.4.6b1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6/tests/test_socket.py` & `pymycobot-3.4.6b1/tests/test_socket.py`

 * *Files identical despite different names*

