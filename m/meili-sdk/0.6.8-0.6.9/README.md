# Comparing `tmp/meili-sdk-0.6.8.tar.gz` & `tmp/meili-sdk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili-sdk-0.6.8.tar", last modified: Thu Apr 18 10:46:49 2024, max compression
+gzip compressed data, was "meili-sdk-0.6.9.tar", last modified: Tue Apr 23 18:04:07 2024, max compression
```

## Comparing `meili-sdk-0.6.8.tar` & `meili-sdk-0.6.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.180484 meili-sdk-0.6.8/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5025 2024-04-18 10:46:49.180484 meili-sdk-0.6.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4735 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.169485 meili-sdk-0.6.8/meili_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.171485 meili-sdk-0.6.8/meili_sdk/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/apitoken_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/base.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/persistent_token_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/clients/sdk_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.171485 meili-sdk-0.6.8/meili_sdk/config/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/config/type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/config/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.173485 meili-sdk-0.6.8/meili_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/form.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/organization.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/ros_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/team.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.174485 meili-sdk-0.6.8/meili_sdk/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/action_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8530 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.174485 meili-sdk-0.6.8/meili_sdk/mqtt/models/
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/action.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/order.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/models/state.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/mqtt/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.176484 meili-sdk-0.6.8/meili_sdk/resources/
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/maps.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/ros.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/teams.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/users.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/resources/vehicles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.177485 meili-sdk-0.6.8/meili_sdk/schedules/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/schedules/models.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/site.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/token.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.177485 meili-sdk-0.6.8/meili_sdk/websockets/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19393 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.180484 meili-sdk-0.6.8/meili_sdk/websockets/models/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/action_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/cancel_task_message.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/docking_routine_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7135 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/move_message.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/path.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/preset.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/station.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/task_v2.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/topic.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/traffic_control_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/update_map_message.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/meili_sdk/websockets/models/vehicle_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:46:49.170485 meili-sdk-0.6.8/meili_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5025 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2285 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-18 10:46:49.000000 meili-sdk-0.6.8/meili_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-18 10:46:49.181484 meili-sdk-0.6.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-18 10:46:39.000000 meili-sdk-0.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.329956 meili-sdk-0.6.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-04-23 18:04:07.329956 meili-sdk-0.6.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.319956 meili-sdk-0.6.9/meili_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.321956 meili-sdk-0.6.9/meili_sdk/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/apitoken_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/persistent_token_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/sdk_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.321956 meili-sdk-0.6.9/meili_sdk/config/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/config/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/config/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.322956 meili-sdk-0.6.9/meili_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/ros_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/team.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.323957 meili-sdk-0.6.9/meili_sdk/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/action_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.324957 meili-sdk-0.6.9/meili_sdk/mqtt/models/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.325956 meili-sdk-0.6.9/meili_sdk/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/ros.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/teams.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/vehicles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.326957 meili-sdk-0.6.9/meili_sdk/schedules/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/token.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.326957 meili-sdk-0.6.9/meili_sdk/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18613 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.329956 meili-sdk-0.6.9/meili_sdk/websockets/models/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/action_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/cancel_task_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/docking_routine_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/move_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/preset.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/station.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/task_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/traffic_control_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/update_map_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/vehicle_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.320957 meili-sdk-0.6.9/meili_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-23 18:04:07.330957 meili-sdk-0.6.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/setup.py
```

### Comparing `meili-sdk-0.6.8/LICENSE.txt` & `meili-sdk-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/PKG-INFO` & `meili-sdk-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.8
+Version: 0.6.9
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.8/README.md` & `meili-sdk-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/clients/__init__.py` & `meili-sdk-0.6.9/meili_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/clients/apitoken_client.py` & `meili-sdk-0.6.9/meili_sdk/clients/apitoken_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/clients/base.py` & `meili-sdk-0.6.9/meili_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/clients/sdk_client.py` & `meili-sdk-0.6.9/meili_sdk/clients/sdk_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/exceptions.py` & `meili-sdk-0.6.9/meili_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/models/base.py` & `meili-sdk-0.6.9/meili_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/models/form.py` & `meili-sdk-0.6.9/meili_sdk/models/form.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/models/task.py` & `meili-sdk-0.6.9/meili_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/models/team.py` & `meili-sdk-0.6.9/meili_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/models/trigger.py` & `meili-sdk-0.6.9/meili_sdk/models/trigger.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/models/vehicle.py` & `meili-sdk-0.6.9/meili_sdk/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/mqtt/action_client.py` & `meili-sdk-0.6.9/meili_sdk/mqtt/action_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/mqtt/client.py` & `meili-sdk-0.6.9/meili_sdk/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/mqtt/models/action.py` & `meili-sdk-0.6.9/meili_sdk/mqtt/models/action.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/mqtt/models/order.py` & `meili-sdk-0.6.9/meili_sdk/mqtt/models/order.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/mqtt/models/state.py` & `meili-sdk-0.6.9/meili_sdk/mqtt/models/state.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/mqtt/site.py` & `meili-sdk-0.6.9/meili_sdk/mqtt/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/base.py` & `meili-sdk-0.6.9/meili_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/forms.py` & `meili-sdk-0.6.9/meili_sdk/resources/forms.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/organizations.py` & `meili-sdk-0.6.9/meili_sdk/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/tasks.py` & `meili-sdk-0.6.9/meili_sdk/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/teams.py` & `meili-sdk-0.6.9/meili_sdk/resources/teams.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/triggers.py` & `meili-sdk-0.6.9/meili_sdk/resources/triggers.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/resources/vehicles.py` & `meili-sdk-0.6.9/meili_sdk/resources/vehicles.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/schedules/loader.py` & `meili-sdk-0.6.9/meili_sdk/schedules/loader.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/schedules/models.py` & `meili-sdk-0.6.9/meili_sdk/schedules/models.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/site.py` & `meili-sdk-0.6.9/meili_sdk/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/client.py` & `meili-sdk-0.6.9/meili_sdk/websockets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from meili_sdk.resources.base import BaseResource
 from meili_sdk.site import get_host
 from meili_sdk.version import VERSION
 from meili_sdk.websockets import constants
 from meili_sdk.websockets.models import CancelTaskMessage, DockingRoutineMessage
 from meili_sdk.websockets.models.message import Message
 from meili_sdk.websockets.models.move_message import MoveMessage
-from meili_sdk.websockets.models.task import process_task_message
 from meili_sdk.websockets.models.task_v2 import process_task_v2_message
 from meili_sdk.websockets.models.topic import RosTopic
 from meili_sdk.websockets.models.traffic_control_action_message import (
     PathReroutingMessage,
     SlowDownMessage,
     process_clearance_data,
 )
@@ -42,15 +41,14 @@
     token (str) - authentication token with the WS
     fleet (bool) - use fleet websocket if set to true (default: true)
     open_handler() (callable) - a callable object that will be called with no parameters when websocket is opened
     close_handler() (callable) - a callable objects that will be called with no parameters when websocket is closed
     error_handler(err) (callable) - a callable with a single parameter that will receive the exception as a parameter
     docking_routine_request_handler(message: DockingRoutineMessage, vehicle: str) (callable) - a callable with a single parameter that will receive the message as a parameter
     docking_routine_finalize_handler(message: DockingRoutineMessage, vehicle: str) (callable) - a callable with a single parameter that will receive the message as a parameter
-    task_handler(task: Task, data: dict, vehicle: str) - a callable that will be called when a new task is received
     move_action_handler(message: MoveMessage, data: dict, vehicle: str) - a callable for moving vehicle according to FMS
     slow_down_handler(message: SlowDownMessage, data: dict, vehicle: str) - a callable for altering movement of robots
     path_rerouting_handler(message: path_rerouting_handler, data: dict, vehicle: str) - a callable for altering path of robots
     collision_clearance_handler(message: collision_clearance_handler, data: dict, vehicle: str) - a callable for clearing the collision messages
     topic_list_handler(data: dict, vehicle: str) - a callable for handling topic list request
     topic_list_initializer_handler(topics: List[RosTopic], data: dict, vehicle: str) - a callable to initialize topics
     """
@@ -65,15 +63,14 @@
             override_host: t.Optional[str] = None,
             fleet: t.Optional[bool] = True,
             open_handler: t.Optional[t.Callable] = None,
             close_handler: t.Optional[t.Callable] = None,
             error_handler: t.Optional[t.Callable] = None,
             docking_routine_request_handler: t.Optional[t.Callable] = None,
             docking_routine_finalize_handler: t.Optional[t.Callable] = None,
-            task_handler: t.Optional[t.Callable] = None,
             task_v2_handler: t.Optional[t.Callable] = None,
             task_cancellation_handler: t.Optional[t.Callable] = None,
             move_action_handler: t.Optional[t.Callable] = None,
             slow_down_handler: t.Optional[t.Callable] = None,
             path_rerouting_handler: t.Optional[t.Callable] = None,
             collision_clearance_handler: t.Optional[t.Callable] = None,
             topic_list_handler: t.Optional[t.Callable] = None,
@@ -98,15 +95,14 @@
 
         self.__open_handler = open_handler
         self.__close_handler = close_handler
         self.__error_handler = error_handler
 
         self.__docking_routine_request_handler = docking_routine_request_handler
         self.__docking_routine_finalize_handler = docking_routine_finalize_handler
-        self.__task_handler = task_handler
         self.__task_v2_handler = task_v2_handler
         self.__task_cancellation_handler = task_cancellation_handler
         self.__move_handler = move_action_handler
         self.__slow_down_handler = slow_down_handler
         self.__path_rerouting_handler = path_rerouting_handler
         self.__collision_clearance_handler = collision_clearance_handler
         self.__topic_list_handler = topic_list_handler
@@ -231,15 +227,14 @@
 
     def process_message(
         self, action: str, message: dict, vehicle: t.Optional[str] = None
     ):
         processors = {
             constants.ACTION_DOCKING_ROUTINE_REQUEST: self.process_docking_routine_request,
             constants.ACTION_DOCKING_ROUTINE_FINALIZE: self.process_docking_routine_finalize,
-            constants.ACTION_TASK: self.process_task,
             constants.ACTION_TASK_V2: self.process_task_v2,
             constants.ACTION_TASK_CANCELLATION: self.process_task_cancellation,
             constants.ACTION_MOVE: self.process_move,
             constants.ACTION_MOVE_TO_CHARGING_POINT: self.process_move,
             constants.ACTION_SLOW_DOWN: self.process_slow_down,
             constants.ACTION_PATH_REROUTING: self.process_path_rerouting,
             constants.ACTION_COLLISION_CLEARANCE: self.process_collision_clearance,
@@ -308,25 +303,14 @@
     ):
         dock_message = DockingRoutineMessage(**message["data"])
         if self.__docking_routine_finalize_handler and callable(
             self.__docking_routine_finalize_handler
         ):
             self.__docking_routine_finalize_handler(dock_message, vehicle)
 
-    def process_task(self, message: dict, vehicle: t.Optional[str] = None):
-        """
-        Load task to a Python object and pass it to task handler provided in the __init__
-        method by implementers if applicable
-        """
-        task_data = message["data"]
-        task = process_task_message(task_data)
-
-        if self.__task_handler and callable(self.__task_handler):
-            self.__task_handler(task, task_data, vehicle)
-
     def process_task_v2(self, message: dict, vehicle: t.Optional[str] = None):
         """
         Load task to a Python object and pass it to task handler provided in the __init__
         method by implementers if applicable
         """
         task_data = message["data"]
         task = process_task_v2_message(task_data)
```

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/constants.py` & `meili-sdk-0.6.9/meili_sdk/websockets/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     EVENT_STATUS,
     EVENT_MAP_UPDATE,
 )
 
 # Incoming actions
 ACTION_DOCKING_ROUTINE_REQUEST = "docking_routine_request"
 ACTION_DOCKING_ROUTINE_FINALIZE = "docking_routine_finalize_request"
-ACTION_TASK = "task"
 ACTION_TASK_V2 = "taskv2"
 ACTION_TASK_CANCELLATION = "cancelOrder"
 ACTION_MOVE = "move"
 ACTION_MOVE_TO_CHARGING_POINT = "move_charge"
 ACTION_SLOW_DOWN = "slow_down"
 ACTION_TOPIC_LIST = "request_topics"
 ACTION_TOPIC_INITIALIZATION = "topic_init"
@@ -44,15 +43,14 @@
 ACTION_UPDATE_VEHICLE_SETTINGS = "vehicle_settings"
 ACTION_PAUSE_TASK = "startPause"
 ACTION_RESUME_TASK = "stopPause"
 
 ALL_ACTIONS = (
     ACTION_DOCKING_ROUTINE_REQUEST,
     ACTION_DOCKING_ROUTINE_FINALIZE,
-    ACTION_TASK,
     ACTION_TASK_V2,
     ACTION_MOVE,
     ACTION_MOVE_TO_CHARGING_POINT,
     ACTION_SLOW_DOWN,
     ACTION_PATH_REROUTING,
     ACTION_TOPIC_LIST,
     ACTION_TOPIC_INITIALIZATION,
```

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/models/__init__.py` & `meili-sdk-0.6.9/meili_sdk/websockets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/models/message.py` & `meili-sdk-0.6.9/meili_sdk/websockets/models/message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/models/task.py` & `meili-sdk-0.6.9/meili_sdk/websockets/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/models/task_v2.py` & `meili-sdk-0.6.9/meili_sdk/websockets/models/task_v2.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/models/traffic_control_action_message.py` & `meili-sdk-0.6.9/meili_sdk/websockets/models/traffic_control_action_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk/websockets/models/update_map_message.py` & `meili-sdk-0.6.9/meili_sdk/websockets/models/update_map_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/meili_sdk.egg-info/PKG-INFO` & `meili-sdk-0.6.9/meili_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.8
+Version: 0.6.9
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.8/meili_sdk.egg-info/SOURCES.txt` & `meili-sdk-0.6.9/meili_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.8/setup.cfg` & `meili-sdk-0.6.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = meili-sdk
 description = Meili FMS SDK
-version = 0.6.8
+version = 0.6.9
 license = MIT
 license_files = LICENSE.txt
 description_file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Meili Robots
 author_email = info@meilirobots.com
```

