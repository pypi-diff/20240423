# Comparing `tmp/xeberus_restful_api_server_library-1.6.6.tar.gz` & `tmp/xeberus_restful_api_server_library-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeberus_restful_api_server_library-1.6.6.tar", max compression
+gzip compressed data, was "xeberus_restful_api_server_library-1.6.7.tar", max compression
```

## Comparing `xeberus_restful_api_server_library-1.6.6.tar` & `xeberus_restful_api_server_library-1.6.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     3552 2023-12-17 15:49:13.116893 xeberus_restful_api_server_library-1.6.6/CHANGELOG.md
--rw-r--r--   0        0        0      752 2022-09-29 00:40:49.620301 xeberus_restful_api_server_library-1.6.6/LICENSE.md
--rw-r--r--   0        0        0       45 2020-11-12 14:25:27.510442 xeberus_restful_api_server_library-1.6.6/README.md
--rw-r--r--   0        0        0     1024 2023-12-17 15:49:13.122906 xeberus_restful_api_server_library-1.6.6/pyproject.toml
--rwxr-xr-x   0        0        0      854 2020-11-15 02:17:36.479492 xeberus_restful_api_server_library-1.6.6/src/majormode/__init__.py
--rwxr-xr-x   0        0        0      854 2022-09-29 00:40:49.626524 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/__init__.py
--rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626805 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/__init__.py
--rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626928 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/__init__.py
--rwxr-xr-x   0        0        0     4950 2022-09-29 00:40:49.627713 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/db/create_device_constraint.sql
--rwxr-xr-x   0        0        0     2361 2023-02-06 11:54:21.227279 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/db/create_device_index.sql
--rwxr-xr-x   0        0        0    32233 2023-01-02 01:33:24.762088 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/db/create_device_table.sql
--rw-r--r--   0        0        0   110291 2023-12-17 15:09:31.025035 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/device_service.py
--rw-r--r--   0        0        0    31591 2023-01-02 10:10:21.971072 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/device_service_http_handler.py
--rw-r--r--   0        0        0     1236 2020-11-12 14:25:27.518558 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst
--rw-r--r--   0        0        0     1662 2020-11-12 14:25:27.518702 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst
--rw-r--r--   0        0        0     4252 2020-11-12 14:25:27.518852 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst
--rw-r--r--   0        0        0     4611 2020-11-12 14:25:27.519028 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst
--rw-r--r--   0        0        0     3264 2020-11-12 14:25:27.519170 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst
--rw-r--r--   0        0        0     2360 2020-11-12 14:25:27.519330 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst
--rw-r--r--   0        0        0     9052 2020-11-12 14:25:27.519490 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst
--rw-r--r--   0        0        0     1729 2020-11-12 14:25:27.519661 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst
--rw-r--r--   0        0        0     5473 2020-11-12 14:25:27.519812 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst
--rw-r--r--   0        0        0     1524 2020-11-12 14:25:27.519949 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst
--rw-r--r--   0        0        0     6347 2020-11-12 14:25:27.520220 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst
--rw-r--r--   0        0        0     3266 2020-11-12 14:25:27.520355 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst
--rw-r--r--   0        0        0     2521 2020-11-12 14:25:27.520485 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst
--rw-r--r--   0        0        0     2592 2020-11-12 14:25:27.520618 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst
--rw-r--r--   0        0        0     1346 2020-11-12 14:25:27.520783 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst
--rw-r--r--   0        0        0     2152 2020-11-12 14:25:27.520927 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst
--rw-r--r--   0        0        0     3655 2020-11-12 14:25:27.521077 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst
--rw-r--r--   0        0        0     1967 2020-11-12 14:25:27.521209 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst
--rw-r--r--   0        0        0     3523 2020-11-12 14:25:27.521340 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst
--rw-r--r--   0        0        0     1414 2020-11-12 14:25:27.521474 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst
--rw-r--r--   0        0        0     3096 2020-11-12 14:25:27.521595 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst
--rw-r--r--   0        0        0     1447 2020-11-12 14:25:27.521730 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst
--rw-r--r--   0        0        0     2230 2020-11-12 14:25:27.521851 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst
--rw-r--r--   0        0        0     1694 2020-11-12 14:25:27.521975 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst
--rwxr-xr-x   0        0        0    19066 2020-11-12 14:25:27.522498 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst
--rw-r--r--   0        0        0     1115 2022-09-29 00:40:49.631529 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst
--rw-r--r--   0        0        0     7838 2022-09-29 00:40:49.632194 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/get_devices.rst
--rw-r--r--   0        0        0     3163 2023-02-08 01:48:44.050512 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/index.rst
--rw-r--r--   0        0        0     5403 2022-09-29 00:40:49.634374 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst
--rw-r--r--   0        0        0     1863 2022-09-29 00:40:49.635018 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst
--rw-r--r--   0        0        0     6229 2022-09-29 00:40:49.635560 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst
--rw-r--r--   0        0        0     6385 2022-09-29 00:40:49.636056 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst
--rw-r--r--   0        0        0     5451 2022-09-29 00:40:49.636533 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst
--rw-r--r--   0        0        0     7360 2022-09-29 00:40:49.637231 xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst
--rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.6/setup.py
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0     3655 2024-04-23 01:40:04.107960 xeberus_restful_api_server_library-1.6.7/CHANGELOG.md
+-rw-r--r--   0        0        0      752 2022-09-29 00:40:49.620301 xeberus_restful_api_server_library-1.6.7/LICENSE.md
+-rw-r--r--   0        0        0       45 2020-11-12 14:25:27.510442 xeberus_restful_api_server_library-1.6.7/README.md
+-rw-r--r--   0        0        0     1024 2024-04-23 01:41:22.853469 xeberus_restful_api_server_library-1.6.7/pyproject.toml
+-rwxr-xr-x   0        0        0      854 2020-11-15 02:17:36.479492 xeberus_restful_api_server_library-1.6.7/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0      854 2022-09-29 00:40:49.626524 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626805 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626928 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/__init__.py
+-rwxr-xr-x   0        0        0     4950 2022-09-29 00:40:49.627713 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_constraint.sql
+-rwxr-xr-x   0        0        0     2361 2023-02-06 11:54:21.227279 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_index.sql
+-rwxr-xr-x   0        0        0    32233 2023-01-02 01:33:24.762088 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_table.sql
+-rw-r--r--   0        0        0   109975 2024-04-23 01:39:01.759585 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service.py
+-rw-r--r--   0        0        0    31591 2023-01-02 10:10:21.971072 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service_http_handler.py
+-rw-r--r--   0        0        0     1236 2020-11-12 14:25:27.518558 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst
+-rw-r--r--   0        0        0     1662 2020-11-12 14:25:27.518702 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst
+-rw-r--r--   0        0        0     4252 2020-11-12 14:25:27.518852 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst
+-rw-r--r--   0        0        0     4611 2020-11-12 14:25:27.519028 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst
+-rw-r--r--   0        0        0     3264 2020-11-12 14:25:27.519170 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst
+-rw-r--r--   0        0        0     2360 2020-11-12 14:25:27.519330 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst
+-rw-r--r--   0        0        0     9052 2020-11-12 14:25:27.519490 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst
+-rw-r--r--   0        0        0     1729 2020-11-12 14:25:27.519661 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst
+-rw-r--r--   0        0        0     5473 2020-11-12 14:25:27.519812 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst
+-rw-r--r--   0        0        0     1524 2020-11-12 14:25:27.519949 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst
+-rw-r--r--   0        0        0     6347 2020-11-12 14:25:27.520220 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst
+-rw-r--r--   0        0        0     3266 2020-11-12 14:25:27.520355 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst
+-rw-r--r--   0        0        0     2521 2020-11-12 14:25:27.520485 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst
+-rw-r--r--   0        0        0     2592 2020-11-12 14:25:27.520618 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst
+-rw-r--r--   0        0        0     1346 2020-11-12 14:25:27.520783 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst
+-rw-r--r--   0        0        0     2152 2020-11-12 14:25:27.520927 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst
+-rw-r--r--   0        0        0     3655 2020-11-12 14:25:27.521077 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst
+-rw-r--r--   0        0        0     1967 2020-11-12 14:25:27.521209 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst
+-rw-r--r--   0        0        0     3523 2020-11-12 14:25:27.521340 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst
+-rw-r--r--   0        0        0     1414 2020-11-12 14:25:27.521474 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst
+-rw-r--r--   0        0        0     3096 2020-11-12 14:25:27.521595 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst
+-rw-r--r--   0        0        0     1447 2020-11-12 14:25:27.521730 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst
+-rw-r--r--   0        0        0     2230 2020-11-12 14:25:27.521851 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst
+-rw-r--r--   0        0        0     1694 2020-11-12 14:25:27.521975 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst
+-rwxr-xr-x   0        0        0    19066 2020-11-12 14:25:27.522498 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst
+-rw-r--r--   0        0        0     1115 2022-09-29 00:40:49.631529 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst
+-rw-r--r--   0        0        0     7838 2022-09-29 00:40:49.632194 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/get_devices.rst
+-rw-r--r--   0        0        0     3163 2023-02-08 01:48:44.050512 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/index.rst
+-rw-r--r--   0        0        0     5403 2022-09-29 00:40:49.634374 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst
+-rw-r--r--   0        0        0     1863 2022-09-29 00:40:49.635018 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst
+-rw-r--r--   0        0        0     6229 2022-09-29 00:40:49.635560 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst
+-rw-r--r--   0        0        0     6385 2022-09-29 00:40:49.636056 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst
+-rw-r--r--   0        0        0     5451 2022-09-29 00:40:49.636533 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst
+-rw-r--r--   0        0        0     7360 2022-09-29 00:40:49.637231 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst
+-rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.7/setup.py
+-rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.7/PKG-INFO
```

### Comparing `xeberus_restful_api_server_library-1.6.6/CHANGELOG.md` & `xeberus_restful_api_server_library-1.6.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.6.7] - 2024-04-23
+### Changed
+- Remove the patch consisting in associating the device to a user
+
 ## [1.6.6] - 2023-12-17
 ### Fixed
 - Fix the function `get_device_by_id` to return the missing attribute `device_id`
 
 ## [1.6.3] - 2023-01-03
 ### Changed
 - Make public the method `get_device_by_id`
```

### Comparing `xeberus_restful_api_server_library-1.6.6/LICENSE.md` & `xeberus_restful_api_server_library-1.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/pyproject.toml` & `xeberus_restful_api_server_library-1.6.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 ]
 keywords = ["core", "library", "xeberus", "restful", "api"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "xeberus-restful-api-server-library"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/xeberus-restful-api-server-python-library"
-version = "1.6.6"
+version = "1.6.7"
 
 [tool.poetry.dependencies]
+fabric = "^2.7.0"
 perseus-core-library = "^1.19"
 perseus-restful-api-framework = "^1.26"
 python = "^3.9"
 xeberus-core-library = "*"
-Fabric = "^2.7.0"
 
 [tool.poetry.dev-dependencies]
-Sphinx = "^4.5.0"
+sphinx = "^4.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/__init__.py` & `xeberus_restful_api_server_library-1.6.7/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/__init__.py` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/__init__.py` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/__init__.py` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/db/create_device_constraint.sql` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_constraint.sql`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/db/create_device_index.sql` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_index.sql`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/db/create_device_table.sql` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_table.sql`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/device_service.py` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1634,15 +1634,14 @@
             app_version: Version,
             connection: RdbmsConnection = None):
         pass
 
     def __update_device_last_known_location(
             self,
             device_id: str,
-            account_id: uuid.UUID,  # @todo: Remove this patch used to allocate the device to an account
             events: list[LocationUpdate],
             connection: RdbmsConnection = None) -> None:
         """
         Update the last known location of a device.
 
 
         @todo: Replace the storage of the last known location of the device
@@ -1670,28 +1669,26 @@
 
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             connection.execute(
                 """
                 UPDATE
                     device
                   SET
-                    account_id = %(account_id)s,  -- @todo: Remove this ugly patch!
                     accuracy = %(accuracy)s,
                     bearing = %(bearing)s,
                     fix_time = %(fix_time)s,
                     location = ST_SetSRID(ST_MakePoint(%(longitude)s, %(latitude)s, %(altitude)s), 4326),
                     provider = %(provider)s,
                     speed = %(speed)s,
                     update_time = current_timestamp
                   WHERE 
                     device_id = %(device_id)s
                     AND (fix_time IS NULL OR fix_time < %(fix_time)s)
                 """,
                 {
-                    'account_id': account_id,
                     'accuracy': most_recent_location.accuracy,
                     'altitude': most_recent_location.altitude,
                     'bearing': most_recent_location.bearing,
                     'device_id': device_id,
                     'fix_time': most_recent_location.fix_time,
                     'latitude': most_recent_location.latitude,
                     'longitude': most_recent_location.longitude,
@@ -2413,17 +2410,17 @@
                     device_app,
                     events,
                     account_id=account_id,
                     connection=connection)
 
                 self.__update_device_last_known_location(
                     device_id,
-                    account_id,  # @todo: Remove this patch used to allocate the device to a user
                     events,
-                    connection=connection)
+                    connection=connection
+                )
 
     def shake_hands(
             self,
             device_id: str,
             app_id: uuid.UUID,
             agent_application: ClientApplication,
             ip_address: str,
```

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/device_service_http_handler.py` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/get_devices.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/get_devices.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/index.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst` & `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.6/setup.py` & `xeberus_restful_api_server_library-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
                                       'db/create_device_table.sql',
                                       'db/create_device_table.sql',
                                       'db/create_device_table.sql',
                                       'doc/api/*',
                                       'doc/api/backup/*']}
 
 install_requires = \
-['Fabric>=2.7.0,<3.0.0',
+['fabric>=2.7.0,<3.0.0',
  'perseus-core-library>=1.19,<2.0',
  'perseus-restful-api-framework>=1.26,<2.0',
  'xeberus-core-library']
 
 setup_kwargs = {
     'name': 'xeberus-restful-api-server-library',
-    'version': '1.6.6',
+    'version': '1.6.7',
     'description': 'Xeberus RESTful API Server Python Library',
     'long_description': '# Xeberus RESTful API Server Python Library\n\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/xeberus-restful-api-server-python-library',
```

### Comparing `xeberus_restful_api_server_library-1.6.6/PKG-INFO` & `xeberus_restful_api_server_library-1.6.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeberus-restful-api-server-library
-Version: 1.6.6
+Version: 1.6.7
 Summary: Xeberus RESTful API Server Python Library
 Home-page: https://github.com/majormode/xeberus-restful-api-server-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library,xeberus,restful,api
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: Fabric (>=2.7.0,<3.0.0)
+Requires-Dist: fabric (>=2.7.0,<3.0.0)
 Requires-Dist: perseus-core-library (>=1.19,<2.0)
 Requires-Dist: perseus-restful-api-framework (>=1.26,<2.0)
 Requires-Dist: xeberus-core-library
 Project-URL: Repository, https://github.com/majormode/xeberus-restful-api-server-python-library
 Description-Content-Type: text/markdown
 
 # Xeberus RESTful API Server Python Library
```

