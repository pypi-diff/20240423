# Comparing `tmp/meili_ros_lib-0.3.7.tar.gz` & `tmp/meili_ros_lib-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili_ros_lib-0.3.7.tar", last modified: Thu Mar  7 10:46:28 2024, max compression
+gzip compressed data, was "meili_ros_lib-0.3.8.tar", last modified: Tue Apr 23 16:41:31 2024, max compression
```

## Comparing `meili_ros_lib-0.3.7.tar` & `meili_ros_lib-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 10:46:28.126726 meili_ros_lib-0.3.7/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      297 2024-03-07 10:46:28.126726 meili_ros_lib-0.3.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 10:46:28.125726 meili_ros_lib-0.3.7/meili_ros_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25836 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2679 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/agent_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4412 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/config_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/docking.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/maths.py
--rw-rw-rw-   0 root         (0) root         (0)    11990 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/offline.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/parse_data.py
--rw-rw-rw-   0 root         (0) root         (0)    13751 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/sdk_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/meili_ros_lib/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 10:46:28.126726 meili_ros_lib-0.3.7/meili_ros_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      297 2024-03-07 10:46:28.000000 meili_ros_lib-0.3.7/meili_ros_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2024-03-07 10:46:28.000000 meili_ros_lib-0.3.7/meili_ros_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 10:46:28.000000 meili_ros_lib-0.3.7/meili_ros_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-07 10:46:28.000000 meili_ros_lib-0.3.7/meili_ros_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-03-07 10:46:28.126726 meili_ros_lib-0.3.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-07 10:46:18.000000 meili_ros_lib-0.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:41:31.863186 meili_ros_lib-0.3.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-23 16:41:31.863186 meili_ros_lib-0.3.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:41:31.862186 meili_ros_lib-0.3.8/meili_ros_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25836 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/agent_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4412 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/config_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/docking.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/maths.py
+-rw-rw-rw-   0 root         (0) root         (0)    11990 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/offline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13982 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/sdk_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/meili_ros_lib/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:41:31.862186 meili_ros_lib-0.3.8/meili_ros_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-23 16:41:31.000000 meili_ros_lib-0.3.8/meili_ros_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 16:41:31.000000 meili_ros_lib-0.3.8/meili_ros_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 16:41:31.000000 meili_ros_lib-0.3.8/meili_ros_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-23 16:41:31.000000 meili_ros_lib-0.3.8/meili_ros_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-04-23 16:41:31.863186 meili_ros_lib-0.3.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-23 16:41:20.000000 meili_ros_lib-0.3.8/setup.py
```

### Comparing `meili_ros_lib-0.3.7/LICENSE.txt` & `meili_ros_lib-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/agent.py` & `meili_ros_lib-0.3.8/meili_ros_lib/agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/agent_setup.py` & `meili_ros_lib-0.3.8/meili_ros_lib/agent_setup.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/config_agent.py` & `meili_ros_lib-0.3.8/meili_ros_lib/config_agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/connection.py` & `meili_ros_lib-0.3.8/meili_ros_lib/connection.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/docking.py` & `meili_ros_lib-0.3.8/meili_ros_lib/docking.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/maths.py` & `meili_ros_lib-0.3.8/meili_ros_lib/maths.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/offline.py` & `meili_ros_lib-0.3.8/meili_ros_lib/offline.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/parse_data.py` & `meili_ros_lib-0.3.8/meili_ros_lib/parse_data.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/sdk_handlers.py` & `meili_ros_lib-0.3.8/meili_ros_lib/sdk_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
                 path_rerouting_handler=self.path_rerouting_handler,
                 docking_routine_request_handler=self.docking_routine_request_handler,
                 docking_routine_finalize_handler=self.docking_routine_finalize_handler,
                 collision_clearance_handler=self.collision_clearance_handler,
                 update_map_handler=self.update_map_handler,
                 update_vehicle_settings=self.update_vehicle_settings, 
                 pause_task_handler=self.pause_task_handler, 
-                resume_task_handler=self.resume_task_handler
+                resume_task_handler=self.resume_task_handler,
+                remove_vehicle_from_fleet_handler=self.remove_vehicle_from_fleet_handler
             )
         except KeyError as error:
             self.agent.log_info(f"[ROSHandler] No handler named {error}")
             capture_exception(error)
         return self.agent.client
 
     def check_fleet_get_vehicle_position(self, vehicle):
@@ -314,8 +315,11 @@
         # Method should be written in the particular ROS Handler
         pass
     def pause_task_handler(self, pause_task_msg, vehicle: str):
         # Method should be written in the particular ROS Handler
         pass
     def resume_task_handler(self, pause_task_msg, vehicle: str):
         # Method should be written in the particular ROS Handler
+        pass
+    def remove_vehicle_from_fleet_handler(self, vehicle: str):
+        # Method should be written in the particular ROS Handler
         pass
```

### Comparing `meili_ros_lib-0.3.7/meili_ros_lib/sentry.py` & `meili_ros_lib-0.3.8/meili_ros_lib/sentry.py`

 * *Files identical despite different names*

