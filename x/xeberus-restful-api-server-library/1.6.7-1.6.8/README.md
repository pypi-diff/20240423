# Comparing `tmp/xeberus_restful_api_server_library-1.6.7.tar.gz` & `tmp/xeberus_restful_api_server_library-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeberus_restful_api_server_library-1.6.7.tar", max compression
+gzip compressed data, was "xeberus_restful_api_server_library-1.6.8.tar", max compression
```

## Comparing `xeberus_restful_api_server_library-1.6.7.tar` & `xeberus_restful_api_server_library-1.6.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     3655 2024-04-23 01:40:04.107960 xeberus_restful_api_server_library-1.6.7/CHANGELOG.md
--rw-r--r--   0        0        0      752 2022-09-29 00:40:49.620301 xeberus_restful_api_server_library-1.6.7/LICENSE.md
--rw-r--r--   0        0        0       45 2020-11-12 14:25:27.510442 xeberus_restful_api_server_library-1.6.7/README.md
--rw-r--r--   0        0        0     1024 2024-04-23 01:41:22.853469 xeberus_restful_api_server_library-1.6.7/pyproject.toml
--rwxr-xr-x   0        0        0      854 2020-11-15 02:17:36.479492 xeberus_restful_api_server_library-1.6.7/src/majormode/__init__.py
--rwxr-xr-x   0        0        0      854 2022-09-29 00:40:49.626524 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/__init__.py
--rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626805 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/__init__.py
--rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626928 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/__init__.py
--rwxr-xr-x   0        0        0     4950 2022-09-29 00:40:49.627713 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_constraint.sql
--rwxr-xr-x   0        0        0     2361 2023-02-06 11:54:21.227279 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_index.sql
--rwxr-xr-x   0        0        0    32233 2023-01-02 01:33:24.762088 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_table.sql
--rw-r--r--   0        0        0   109975 2024-04-23 01:39:01.759585 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service.py
--rw-r--r--   0        0        0    31591 2023-01-02 10:10:21.971072 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service_http_handler.py
--rw-r--r--   0        0        0     1236 2020-11-12 14:25:27.518558 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst
--rw-r--r--   0        0        0     1662 2020-11-12 14:25:27.518702 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst
--rw-r--r--   0        0        0     4252 2020-11-12 14:25:27.518852 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst
--rw-r--r--   0        0        0     4611 2020-11-12 14:25:27.519028 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst
--rw-r--r--   0        0        0     3264 2020-11-12 14:25:27.519170 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst
--rw-r--r--   0        0        0     2360 2020-11-12 14:25:27.519330 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst
--rw-r--r--   0        0        0     9052 2020-11-12 14:25:27.519490 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst
--rw-r--r--   0        0        0     1729 2020-11-12 14:25:27.519661 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst
--rw-r--r--   0        0        0     5473 2020-11-12 14:25:27.519812 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst
--rw-r--r--   0        0        0     1524 2020-11-12 14:25:27.519949 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst
--rw-r--r--   0        0        0     6347 2020-11-12 14:25:27.520220 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst
--rw-r--r--   0        0        0     3266 2020-11-12 14:25:27.520355 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst
--rw-r--r--   0        0        0     2521 2020-11-12 14:25:27.520485 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst
--rw-r--r--   0        0        0     2592 2020-11-12 14:25:27.520618 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst
--rw-r--r--   0        0        0     1346 2020-11-12 14:25:27.520783 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst
--rw-r--r--   0        0        0     2152 2020-11-12 14:25:27.520927 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst
--rw-r--r--   0        0        0     3655 2020-11-12 14:25:27.521077 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst
--rw-r--r--   0        0        0     1967 2020-11-12 14:25:27.521209 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst
--rw-r--r--   0        0        0     3523 2020-11-12 14:25:27.521340 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst
--rw-r--r--   0        0        0     1414 2020-11-12 14:25:27.521474 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst
--rw-r--r--   0        0        0     3096 2020-11-12 14:25:27.521595 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst
--rw-r--r--   0        0        0     1447 2020-11-12 14:25:27.521730 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst
--rw-r--r--   0        0        0     2230 2020-11-12 14:25:27.521851 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst
--rw-r--r--   0        0        0     1694 2020-11-12 14:25:27.521975 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst
--rwxr-xr-x   0        0        0    19066 2020-11-12 14:25:27.522498 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst
--rw-r--r--   0        0        0     1115 2022-09-29 00:40:49.631529 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst
--rw-r--r--   0        0        0     7838 2022-09-29 00:40:49.632194 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/get_devices.rst
--rw-r--r--   0        0        0     3163 2023-02-08 01:48:44.050512 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/index.rst
--rw-r--r--   0        0        0     5403 2022-09-29 00:40:49.634374 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst
--rw-r--r--   0        0        0     1863 2022-09-29 00:40:49.635018 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst
--rw-r--r--   0        0        0     6229 2022-09-29 00:40:49.635560 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst
--rw-r--r--   0        0        0     6385 2022-09-29 00:40:49.636056 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst
--rw-r--r--   0        0        0     5451 2022-09-29 00:40:49.636533 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst
--rw-r--r--   0        0        0     7360 2022-09-29 00:40:49.637231 xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst
--rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.7/setup.py
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0     3716 2024-04-23 06:33:18.528510 xeberus_restful_api_server_library-1.6.8/CHANGELOG.md
+-rw-r--r--   0        0        0      752 2022-09-29 00:40:49.620301 xeberus_restful_api_server_library-1.6.8/LICENSE.md
+-rw-r--r--   0        0        0       45 2020-11-12 14:25:27.510442 xeberus_restful_api_server_library-1.6.8/README.md
+-rw-r--r--   0        0        0     1029 2024-04-23 06:34:57.353350 xeberus_restful_api_server_library-1.6.8/pyproject.toml
+-rwxr-xr-x   0        0        0      854 2020-11-15 02:17:36.479492 xeberus_restful_api_server_library-1.6.8/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0      854 2022-09-29 00:40:49.626524 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626805 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-09-29 00:40:49.626928 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/__init__.py
+-rwxr-xr-x   0        0        0     4950 2022-09-29 00:40:49.627713 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/db/create_device_constraint.sql
+-rwxr-xr-x   0        0        0     2361 2023-02-06 11:54:21.227279 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/db/create_device_index.sql
+-rwxr-xr-x   0        0        0    32233 2023-01-02 01:33:24.762088 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/db/create_device_table.sql
+-rw-r--r--   0        0        0   111681 2024-04-23 06:32:46.992220 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/device_service.py
+-rw-r--r--   0        0        0    31591 2023-01-02 10:10:21.971072 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/device_service_http_handler.py
+-rw-r--r--   0        0        0     1236 2020-11-12 14:25:27.518558 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst
+-rw-r--r--   0        0        0     1662 2020-11-12 14:25:27.518702 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst
+-rw-r--r--   0        0        0     4252 2020-11-12 14:25:27.518852 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst
+-rw-r--r--   0        0        0     4611 2020-11-12 14:25:27.519028 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst
+-rw-r--r--   0        0        0     3264 2020-11-12 14:25:27.519170 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst
+-rw-r--r--   0        0        0     2360 2020-11-12 14:25:27.519330 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst
+-rw-r--r--   0        0        0     9052 2020-11-12 14:25:27.519490 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst
+-rw-r--r--   0        0        0     1729 2020-11-12 14:25:27.519661 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst
+-rw-r--r--   0        0        0     5473 2020-11-12 14:25:27.519812 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst
+-rw-r--r--   0        0        0     1524 2020-11-12 14:25:27.519949 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst
+-rw-r--r--   0        0        0     6347 2020-11-12 14:25:27.520220 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst
+-rw-r--r--   0        0        0     3266 2020-11-12 14:25:27.520355 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst
+-rw-r--r--   0        0        0     2521 2020-11-12 14:25:27.520485 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst
+-rw-r--r--   0        0        0     2592 2020-11-12 14:25:27.520618 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst
+-rw-r--r--   0        0        0     1346 2020-11-12 14:25:27.520783 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst
+-rw-r--r--   0        0        0     2152 2020-11-12 14:25:27.520927 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst
+-rw-r--r--   0        0        0     3655 2020-11-12 14:25:27.521077 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst
+-rw-r--r--   0        0        0     1967 2020-11-12 14:25:27.521209 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst
+-rw-r--r--   0        0        0     3523 2020-11-12 14:25:27.521340 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst
+-rw-r--r--   0        0        0     1414 2020-11-12 14:25:27.521474 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst
+-rw-r--r--   0        0        0     3096 2020-11-12 14:25:27.521595 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst
+-rw-r--r--   0        0        0     1447 2020-11-12 14:25:27.521730 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst
+-rw-r--r--   0        0        0     2230 2020-11-12 14:25:27.521851 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst
+-rw-r--r--   0        0        0     1694 2020-11-12 14:25:27.521975 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst
+-rwxr-xr-x   0        0        0    19066 2020-11-12 14:25:27.522498 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst
+-rw-r--r--   0        0        0     1115 2022-09-29 00:40:49.631529 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst
+-rw-r--r--   0        0        0     7838 2022-09-29 00:40:49.632194 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/get_devices.rst
+-rw-r--r--   0        0        0     3163 2023-02-08 01:48:44.050512 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/index.rst
+-rw-r--r--   0        0        0     5403 2022-09-29 00:40:49.634374 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst
+-rw-r--r--   0        0        0     1863 2022-09-29 00:40:49.635018 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst
+-rw-r--r--   0        0        0     6229 2022-09-29 00:40:49.635560 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst
+-rw-r--r--   0        0        0     6385 2022-09-29 00:40:49.636056 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst
+-rw-r--r--   0        0        0     5451 2022-09-29 00:40:49.636533 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst
+-rw-r--r--   0        0        0     7360 2022-09-29 00:40:49.637231 xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.8/setup.py
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 xeberus_restful_api_server_library-1.6.8/PKG-INFO
```

### Comparing `xeberus_restful_api_server_library-1.6.7/CHANGELOG.md` & `xeberus_restful_api_server_library-1.6.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.6.8] - 2024-04-23
+### Added
+- Link a device to a user
+
 ## [1.6.7] - 2024-04-23
 ### Changed
 - Remove the patch consisting in associating the device to a user
 
 ## [1.6.6] - 2023-12-17
 ### Fixed
 - Fix the function `get_device_by_id` to return the missing attribute `device_id`
```

### Comparing `xeberus_restful_api_server_library-1.6.7/LICENSE.md` & `xeberus_restful_api_server_library-1.6.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/pyproject.toml` & `xeberus_restful_api_server_library-1.6.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 ]
 keywords = ["core", "library", "xeberus", "restful", "api"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "xeberus-restful-api-server-library"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/xeberus-restful-api-server-python-library"
-version = "1.6.7"
+version = "1.6.8"
 
 [tool.poetry.dependencies]
 fabric = "^2.7.0"
-perseus-core-library = "^1.19"
-perseus-restful-api-framework = "^1.26"
-python = "^3.9"
+perseus-core-library = "^1.20.3"
+perseus-restful-api-framework = "^1.28.4"
+python = "^3.10"
 xeberus-core-library = "*"
 
 [tool.poetry.dev-dependencies]
-sphinx = "^4.5.0"
+sphinx = "^7.3.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/__init__.py` & `xeberus_restful_api_server_library-1.6.8/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/__init__.py` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/__init__.py` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/__init__.py` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/__init__.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_constraint.sql` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/db/create_device_constraint.sql`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_index.sql` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/db/create_device_index.sql`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/db/create_device_table.sql` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/db/create_device_table.sql`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service.py` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/device_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
 # PURPOSE, OR NON-INFRINGEMENT.  MAJORMODE SHALL NOT BE LIABLE FOR ANY
 # LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING
 # OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
 
 from __future__ import annotations
 
-from typing import Any
 import base64
 import datetime
 import hashlib
 import hmac
 import uuid
+from typing import Any
+from uuid import UUID
 
 from majormode.perseus.constant.obj import ObjectStatus
 from majormode.perseus.constant.team import MemberRole
 from majormode.perseus.constant.stage import EnvironmentStage
 from majormode.perseus.model.app import ClientApplication
 from majormode.perseus.model.date import ISO8601DateTime
 from majormode.perseus.model.geolocation import GeoPoint
@@ -112,26 +113,26 @@
             still reused to activate other device of the individual user or
             the organization, until this code expires.
 
 
         @param device_app: The client application to activate.  The object
             must contain the following attributes:
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the individual user who owns this mobile device, if any.  This
               information is required when the mobile device has been temporarily
               deactivated by its owner ({@link ObjectStatus.disabled}).
 
-            - `app_id: uuid.UUID` (required): The identification of the client
+            - `app_id: UUID` (required): The identification of the client
               application to be activated on the mobile device.
 
             - `device_id: str` (required): The identification of the device which
               the client application needs to be activated.
 
-            - `team_id: uuid.UUID` (optional): The identification of the
+            - `team_id: UUID` (optional): The identification of the
               organization that owns this mobile device, if any.  This information
               is required when the mobile device has been temporarily deactivated
               by the organization that manages it ({@link ObjectStatus.disabled}).
 
         @param activation_code: A code that has been generated by an
             individual user owning the mobile device or the organization
             managing the mobile device, and scanned by the mobile device.
@@ -314,18 +315,18 @@
         one more time these events.
 
 
         @param device_app: An object representing a client application
             installed on a mobile device.  This object must contain the
             following attributes
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the individual user that owns this device.
 
-            - `team_id: uuid.UUID` (optional): The identification of the
+            - `team_id: UUID` (optional): The identification of the
               organization that manages this device.
 
         @param events: A list of battery state update events.
 
         @param connection: An existing connection to the device database.
 
 
@@ -387,18 +388,18 @@
         one more time these events.
 
 
         @param device_app: An object representing a client application
             installed on a mobile device.  This object must contain the
             following attributes
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the individual user that owns this device.
 
-            - `team_id: uuid.UUID` (optional): The identification of the
+            - `team_id: UUID` (optional): The identification of the
               organization that manages this device.
 
         @param events: A list of location update events.
 
         @param connection: An existing connection to the device database.
 
 
@@ -440,19 +441,19 @@
                         if event.event_id not in duplicated_event_cids
                     ]
 
         return events
 
     def __generate_new_activation_code(
             self,
-            app_id: uuid.UUID,
-            account_id: uuid.UUID,
+            app_id: UUID,
+            account_id: UUID,
             activation_code_ttl: int,
             connection: RdbmsConnection = None,
-            team_id: uuid.UUID = None) -> Any:
+            team_id: UUID = None) -> Any:
         """
         Generate a new code to activate client applications running on one or
         more mobile devices.
 
         This activation code needs to be used before it expires.  A mobile
         device needs to scan this activation code (for instance, as a
         QR code) and to send it to the cloud service in order this device to
@@ -550,18 +551,18 @@
         secure the communication with the cloud service.
 
 
         @param device_app: An object representing a client application
             installed on a mobile device.  This object must contain the
             following attributes
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the individual user that owns this device.
 
-            - `team_id: uuid.UUID` (optional): The identification of the
+            - `team_id: UUID` (optional): The identification of the
               organization that manages this device.
 
 
         @return: A security key.
         """
         # Generated a random number.
         nonce = uuid.uuid4()
@@ -580,15 +581,15 @@
             .hexdigest()
 
         return security_key
 
     def __get_device_app(
             self,
             device_id: str,
-            app_id: uuid.UUID,
+            app_id: UUID,
             check_status: bool = False,
             connection: RdbmsConnection = None,
             include_security_info: bool = False) -> Any:
         """
         Return information about a client application installed on a mobile
         device.
 
@@ -610,42 +611,42 @@
 
 
         @return: An object containing the following attributes:
 
             - `activation_time: ISO8601DateTime` (optional): The time when the
                client application has been activated on the mobile device.
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the individual user, that owns this mobile device, if any.
 
-            - `app_id: uuid.UUID` (required): The identification of the
+            - `app_id: UUID` (required): The identification of the
               client application.
 
             - `app_version: Version` (required): The version of the client
               application installed on the mobile device.
 
             - `device_id: str` (required): The identification of the device which
               which the client application is installed on.
 
-            - `mac_address: uuid.UUID` (optional): The Media Access Control (MAC)
+            - `mac_address: UUID` (optional): The Media Access Control (MAC)
               address of the mobile device.  This attribute is returned only if the
               argument `include_security_info` equals `True`.
 
 
             - `object_status: ObjectStatus` (required): The current status of the
               client application.
 
             - `security_key: str` (optional): The security key generated by the
               cloud service and shared with the client application installed on
               the device to secure the communication.  This information is only
               available when the client application has been activated on the device.
               This attribute is returned only if the argument `include_security_info`
               equals `True`.
 
-            - `team_id: uuid.UUID` (optional): The identification of the
+            - `team_id: UUID` (optional): The identification of the
               organization that owns this mobile device, if any.
 
             - `update_time: ISO8601DateTime` (required): The time of the most
               recent modification of one or more attribute of the client
               application.
 
 
@@ -728,26 +729,26 @@
         @param device_id: The identification of a mobile device.
 
         @param connection: An existing connection to the device database.
 
 
         @return: A list of objects containing the following attributes:
 
-            - `app_id: uuid.UUID`: The identification of the application.
+            - `app_id: UUID`: The identification of the application.
 
             - `app_version: Version`: The version of the application installed in
               the mobile device.
 
             - `creation_time: ISO8601DateTime`: The time when the application has
               been registered as installed on the mobile device.
 
             - `object_status: ObjectStatus`: The current status of the application
               installed in this mobile device.
 
-            - `picture_id: uuid.UUID`: The identification of the application's logo.
+            - `picture_id: UUID`: The identification of the application's logo.
 
             - `picture_url: str`: The Uniform Resource Locator (URL) of the
               application's logo.
 
             - `update_time: ISO8601DateTime`: The time of the most recent
               modification of an attribute of the application installed in the
               mobile device (version, status, and/or logo).
@@ -812,32 +813,32 @@
             this activation request.
 
         @param connection: An existing connection to the device database.
 
 
         @return: An object containing the following attributes:
 
-            - `account_id: uuid.UUID` (required): The identification of the
+            - `account_id: UUID` (required): The identification of the
               account of the administrator of the organization who requested the
               generation of this activation code.
 
-            - `app_id: uuid.UUID` (required): The identification of the
+            - `app_id: UUID` (required): The identification of the
               administration application that requests to generate this code for
               activating a client application running on a mobile device.
 
             - `creation_time: ISO8601DateTime` (required): The time when this
               activation code has been generated.
 
             - `expiration_time: ISO8601DateTime` (required): The time when the
               activation code expires.
 
             - `object_status: ObjectStatus` (required): The current status of this
               activation code.
 
-            - `team_id: uuid.UUID` (required): The identification of the
+            - `team_id: UUID` (required): The identification of the
               organization on behalf of which this activation code has been
               generated.
 
             - `update_time: ISO8601DateTime` (required): The time of the most
               recent modification of one or more attributes of this activation
               request.
 
@@ -910,15 +911,15 @@
 
         @param connection: An existing connection to the device database for
             read-only access.
 
 
         @return: An object containing the following attributes:
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the user who has activated the device.  This is either an
               individual user (the owner of the device), either an administrator of
               the organization that manages this device.
 
             - `device_id: str` (required): The identification of the device.
 
             - `object_status: ObjectStatus` (required): The current status of the
@@ -932,15 +933,15 @@
                 the organization that manages this device.
 
               - {@link ObjectStatus.enabled}: The device is activated and is expected
                 to operate properly.
 
               - {@link ObjectStatus.pending}: The device has not been activated yet.
 
-            - `team_id: uuid.UUID` (optional): The organization on behalf of which
+            - `team_id: UUID` (optional): The organization on behalf of which
               an administrator has activated the device.
 
             - `update_time: ISO8601DateTime` (required): The time of the most
               recent modification of one or more attributes of the device.
 
 
         @raise DeletedObjectException: If the team that is managing the device
@@ -1005,15 +1006,15 @@
                     include_contacts=False)
 
             return device
 
     def __get_last_keepalive_event(
             self,
             device_id: str,
-            app_id: uuid.UUID,
+            app_id: UUID,
             connection: RdbmsConnection = None) -> Any | None:
         """
         Return the last keep-alive event sent by a client application
         installed on a mobile device.
 
 
         @todo Retrieve the last keep-alive event of the client application
@@ -1065,25 +1066,25 @@
 
             return last_keepalive_event
 
     def __insert_battery_events(
             self,
             device_app: Any,
             events: list[BatteryStateChangeEvent],
-            account_id: uuid.UUID,
+            account_id: UUID,
             connection: RdbmsConnection = None) -> None:
         """
         Store a list of battery state change events reported by a client
         application running on a mobile device.
 
 
         @param device_app: An object representing the client application that
             sent these events:
 
-            - `app_id: uuid.UUID` (required): The identification of the client
+            - `app_id: UUID` (required): The identification of the client
               application.
 
             - `device_id: str` (required): The identification of the device.
 
         @param events: A list of battery state changes.
 
         @param account_id: The identification of the account of the user who
@@ -1226,15 +1227,15 @@
             })
 
             return device
 
     def __insert_device_app(
             self,
             device_id: str,
-            app_id: uuid.UUID,
+            app_id: UUID,
             agent_application: ClientApplication,
             connection: RdbmsConnection = None):
         """
         Insert into the device database the information about a client
         application installed on a mobile device.
 
 
@@ -1273,26 +1274,26 @@
                 }
             )
 
     def __insert_keepalive_event(
             self,
             device_app: Any,
             event_time: ISO8601DateTime,
-            account_id: uuid.UUID = None,
+            account_id: UUID = None,
             connection: RdbmsConnection = None,
             location: GeoPoint = None,
             network_type: str = None) -> Any:
         """
         Store a keep-alive event sent by a mobile device.
 
 
         @param device_app: An object representing the client application that
             sent this keep-alive event:
 
-            - `app_id: uuid.UUID` (required): The identification of the client
+            - `app_id: UUID` (required): The identification of the client
               application.
 
             - `device_id: str` (required): The identification of the device.
 
         @param event_time: The time when the client application sent this
             keep-alive event.
 
@@ -1322,15 +1323,15 @@
               Network of type `wifi` has no subtype.  Network of type `mobile` can
               have a subtype such as `egde`, `gprs`, `hsdpa`, `hspa`, `hspa+`,
               `umts`, etc.
 
 
         @return: An object containing the following attributes:
 
-            - `event_id: uuid.UUID` (required): The identification of the keep-
+            - `event_id: UUID` (required): The identification of the keep-
               alive event.
 
             - `creation_time: ISO8601DateTime (required): The time when this keep-
               alive event has been stored.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             cursor = connection.execute(
@@ -1393,25 +1394,25 @@
 
             return keepalive_event
 
     def __insert_location_events(
             self,
             device_app: Any,
             events: list[LocationUpdate],
-            account_id: uuid.UUID,
+            account_id: UUID,
             connection: RdbmsConnection = None) -> None:
         """
         Store a list of location update events reported by a client
         application running on a mobile device.
 
 
         @param device_app: An object representing the client application that
             sent these events:
 
-            - `app_id: uuid.UUID` (required): The identification of the client
+            - `app_id: UUID` (required): The identification of the client
               application.
 
             - `device_id: str` (required): The identification of the device.
 
         @param events: A list of location updates.
 
         @param account_id: The identification of the account of the user who
@@ -1464,15 +1465,15 @@
                     ]
                 }
             )
 
     def __register_device(
             self,
             device_id: str,
-            app_id: uuid.UUID,
+            app_id: UUID,
             agent_application: ClientApplication,
             ip_address: str,
             connection: RdbmsConnection = None,
             location: GeoPoint = None,
             mac_address: str = None,
             serial_number: str = None):
         """
@@ -1535,19 +1536,19 @@
                 agent_application,
                 connection=connection)
 
             return device
 
     def __reuse_previous_activation_code(
             self,
-            app_id: uuid.UUID,
-            account_id: uuid.UUID,
+            app_id: UUID,
+            account_id: UUID,
             minimum_remaining_ttl_for_reuse: int,
             connection: RdbmsConnection = None,
-            team_id: uuid.UUID = None) -> Any:
+            team_id: UUID = None) -> Any:
         """
         Reuse a previous activation code that is not yet expired.
 
         A previously generated activation code can be reused for the same
         individual user or the same organization that has requested the
         generation of this activation code, as long as this activation code
         has not expired yet.
@@ -1626,15 +1627,15 @@
             })
 
             return activation_request
 
     def __update_device_app(
             self,
             device_id: str,
-            app_id: uuid.UUID,
+            app_id: UUID,
             app_version: Version,
             connection: RdbmsConnection = None):
         pass
 
     def __update_device_last_known_location(
             self,
             device_id: str,
@@ -1695,15 +1696,15 @@
                     'provider': most_recent_location.provider,
                     'speed': most_recent_location.speed
                 }
             )
 
     def activate_device_app(
             self,
-            app_id: uuid.UUID,
+            app_id: UUID,
             device_id: str,
             activation_code: str,
             connection: RdbmsConnection = None) -> Any:
         """
         Activate a client application running on a mobile device.
 
         The client application must have sent a handshake to the server
@@ -1728,15 +1729,15 @@
 
             - `account: any` (optional): The information about the individual user
               who owns this mobile device (cf. {@link AccountService.get_account}).
 
             - `activation_time: ISO8601DateTime` (required): The time when the client
               application has been activated on the mobile device.
 
-            - `app_id: uuid.UUID` (required): The identification of the client
+            - `app_id: UUID` (required): The identification of the client
               application that has been activated.
 
             - `app_version: Version` (required): The current version of the client
               application installed on the mobile device.
 
             - `device_id: str` (required): The identification of the device.
 
@@ -1820,20 +1821,20 @@
             del device_app.account_id
             del device_app.team_id
 
             return device_app
 
     def generate_activation_code(
             self,
-            app_id: uuid.UUID,
-            account_id: uuid.UUID,
+            app_id: UUID,
+            account_id: UUID,
             activation_code_ttl: int = None,
             connection: RdbmsConnection = None,
             minimum_remaining_ttl_for_reuse: int = None,
-            team_id: uuid.UUID = None) -> Any:
+            team_id: UUID = None) -> Any:
         """
         Request a code to activate a client application installed on a mobile
         device.
 
         The function tries to reuse a previously generated activation code for
         the same individual user or organization.  This allows reusing a same
         code for activating multiple mobile devices without having to generate
@@ -1928,22 +1929,22 @@
                     team_id=team_id)
 
             return activation_request
 
     def get_device_by_id(
             self,
             device_id: str,
-            account_id: uuid.UUID = None,
+            account_id: UUID = None,
             check_access: bool = False,
             check_status: bool = False,
             connection: RdbmsConnection = None,
             include_app_list: bool = False,
             include_system_info: bool = False,
             strict_status: bool = True,
-            team_id: uuid.UUID = None) -> Any:
+            team_id: UUID = None) -> Any:
         """
         Return the information about a mobile device.
 
 
         @param device_id: The identification of a mobile device.
 
         @param account_id: The identification of the user on behalf of whom
@@ -1974,15 +1975,15 @@
 
         @param team_id: The identification of the organization that the user
             (on behalf of whom the function is called) belongs to.
 
 
         @return: An object containing the following attributes:
 
-            - `account_id: uuid.UUID` (optional): The identification of the
+            - `account_id: UUID` (optional): The identification of the
               individual user who owns this device, or the identification of the
               member of the organization on behalf of which the device has been
               activated.
 
             - `activation_time: ISO8601DateTime (required)': The time when the
               device has been activated.
 
@@ -2018,25 +2019,25 @@
             - `os_name: str` (optional): The Name of the operating system of the
               mobile device.  This information is immutable.
 
             - `os_version: Version` (optional): The version of the operating system
               of the mobile device.  This information may be updated from time to
               time when the operating system of the device is upgraded.
 
-            - `picture_id: uuid.UUID` (optional): The identification of the mobile
+            - `picture_id: UUID` (optional): The identification of the mobile
               device's picture.
 
             - `picture_url: str` (optional): The Uniform Resource Locator (URL) of
               the mobile device's picture.
 
             - `serial_number: str`: The hardware serial number of the mobile device.
               It corresponds to a unique number assigned by the manufacturer to help
               identify an individual device.
 
-            - `team_id: uuid.UUID`: The identification of the organization that
+            - `team_id: UUID`: The identification of the organization that
              manages this device.
 
             - `update_time: ISO8601DateTime`: The time of the most recent
               modification of one or more attributes of this device.
         """
         with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
             cursor = connection.execute(
@@ -2095,21 +2096,72 @@
                 del device.mac_address
                 del device.os_name
                 del device.os_version
                 del device.serial_number
 
             return device
 
+    def link_device_to_account(
+            self,
+            device_id: str,
+            account_id: UUID,
+            connection: RdbmsConnection = None,
+            location: GeoPoint = None
+    ) -> None:
+        """
+        Link a device to a specified user's account.
+
+
+        :param device_id: The identifier of a device.
+
+        :param account_id: The identifier of a user who is currently using the
+            device.
+
+        :param connection: A connection to the device database.
+
+        :param location: The current location of the device.
+        """
+        with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
+            connection.execute(
+                '''
+                UPDATE
+                    device
+                  SET
+                    account_id = %(account_id)s,
+                    accuracy = %(accuracy)s,
+                    bearing = %(bearing)s,
+                    fix_time = %(fix_time)s,
+                    location = ST_SetSRID(ST_MakePoint(%(longitude)s, %(latitude)s, %(altitude)s), 4326),
+                    provider = %(provider)s,
+                    speed = %(speed)s,
+                    update_time = current_timestamp
+                  WHERE
+                    device_id = %(device_id)s
+                ''',
+                {
+                    'account_id': account_id,
+                    'accuracy': location and location.accuracy,
+                    'altitude': location and location.altitude,
+                    'bearing': location and location.bearing,
+                    'device_id': device_id,
+                    'fix_time': location and location.fix_time,
+                    'latitude': location and location.latitude,
+                    'longitude': location and location.longitude,
+                    'provider': location and location.provider,
+                    'speed': location and location.speed,
+                }
+            )
+
     def report_battery_events(
             self,
-            app_id: uuid.UUID,
+            app_id: UUID,
             device_id: str,
             token: str,
             events: list[BatteryStateChangeEvent],
-            account_id: uuid.UUID = None,
+            account_id: UUID = None,
             connection: RdbmsConnection = None) -> None:
         """
         Report one or more battery state changes of a device:
 
         - the device is connected to or disconnected from a power source (such
           as the battery of the vehicle this device is mounted on);
 
@@ -2195,19 +2247,19 @@
                 account_id=account_id,
                 connection=connection)
 
             # @todo: Update the memory cache with the last battery level and state.
 
     def report_keepalive_event(
             self,
-            app_id: uuid.UUID,
+            app_id: UUID,
             device_id: str,
             token: str,
             event_time: ISO8601DateTime,
-            account_id: uuid.UUID = None,
+            account_id: UUID = None,
             connection: RdbmsConnection = None,
             location: GeoPoint = None,
             network_type: str = None) -> None:
         """
         Report a keep-alive (KA) event from a client application running on
         a mobile device.
 
@@ -2331,19 +2383,19 @@
 
             # @todo: We may want to send a notification to a message bus to inform
             #     other software components about this event, providing the
             #     identification of this event and the time when it occurs.
 
     def report_location_events(
             self,
-            app_id: uuid.UUID,
+            app_id: UUID,
             device_id: str,
             token: str,
             events: list[LocationUpdate],
-            account_id: uuid.UUID = None,
+            account_id: UUID = None,
             connection: RdbmsConnection = None) -> None:
         """
         Report one or more location updates of a mobile device.
 
 
         @param app_id: The identification of the client application running on
             the mobile device.
@@ -2387,15 +2439,16 @@
             # Check whether the client application has been activated on this mobile
             # device.
             device_app = self.__get_device_app(
                 device_id,
                 app_id,
                 check_status=True,
                 connection=connection,
-                include_security_info=True)  # MAC address & security key
+                include_security_info=True
+            )  # MAC address & security key
 
             # Verify that the token has been encrypted with the security key shared
             # with the client application.
             self.verify_token(device_app, token)
 
             # Remove the battery state update events that have not been already
             # stored.
@@ -2417,15 +2470,15 @@
                     events,
                     connection=connection
                 )
 
     def shake_hands(
             self,
             device_id: str,
-            app_id: uuid.UUID,
+            app_id: UUID,
             agent_application: ClientApplication,
             ip_address: str,
             location: GeoPoint = None,
             mac_address: str = None,
             serial_number: str = None,
             connection: RdbmsConnection = None) -> Any:
         """
@@ -2484,15 +2537,15 @@
 
         @param connection: An existing connection to the device database, with
             auto-commit option enabled.
 
 
         @return: An object containing the following attributes:
 
-            - `account_id: uuid.UUID` (optional): The identification of the account
+            - `account_id: UUID` (optional): The identification of the account
               of the user who has activated the device.  This is either an
               individual user (the owner of the device), either an administrator of
               the organization that manages this device.
 
             - `device_id: str` (required): The identification of the device.
 
             - `object_status: ObjectStatus` (required): The current status of the
@@ -2569,15 +2622,15 @@
           platform and the application, and converted to a BASE64 string.
 
 
         @param device_app: An object representing a client application
             installed on a mobile device.  This object must contain the
             following attributes:
 
-            - `app_id: uuid.UUID`: The identification of the client application
+            - `app_id: UUID`: The identification of the client application
               that has generated and encrypted the token.
 
             - `device_id: str`: The identification of the device that sends the
               token.
 
             - `mac_address: str`: The Media Access Control (MAC) address of the
               device.
@@ -2652,8 +2705,9 @@
 #                             package=XeberusService.XEBERUS_MOBILE_APPLICATION_PACKAGE,
 #                             payload={
 #                                 "battery_level": battery_level,
 #                                 "device_id": device_id,
 #                                 "event_time": date_util.ISO8601DateTime.now(),
 #                                 "event_type": BatteryStateChange.BatteryStateEventType.battery_level_changed,
 #                                 "is_battery_plugged": is_battery_plugged })
-#
+#
+
```

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/device_service_http_handler.py` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/device_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_delete_playback.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_delete_venue.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_device_activation_requests.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_devices_locations.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_incident.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_vehicle_models.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_get_venues.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_activation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_alert_message.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_allocation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_signal.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_device_stopovers.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_cash.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_payment_transfer.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_playback.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_prospect_vehicle_model_registration.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_route.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_sim_plan.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_topup_card.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_post_wifi_configurations.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_put_device.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_put_device_mileage.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_put_device_picture.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/_route_monitoring.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/notifications.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/backup/tracker_installation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/get_devices.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/get_devices.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/index.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_activation_code.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_activation_code_generation.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_battery_event.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_handshake.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_keepalive_event.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst` & `xeberus_restful_api_server_library-1.6.8/src/majormode/xeberus/service/device/doc/api/post_device_location_event.rst`

 * *Files identical despite different names*

### Comparing `xeberus_restful_api_server_library-1.6.7/setup.py` & `xeberus_restful_api_server_library-1.6.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,30 +22,30 @@
                                       'db/create_device_table.sql',
                                       'db/create_device_table.sql',
                                       'doc/api/*',
                                       'doc/api/backup/*']}
 
 install_requires = \
 ['fabric>=2.7.0,<3.0.0',
- 'perseus-core-library>=1.19,<2.0',
- 'perseus-restful-api-framework>=1.26,<2.0',
+ 'perseus-core-library>=1.20.3,<2.0.0',
+ 'perseus-restful-api-framework>=1.28.4,<2.0.0',
  'xeberus-core-library']
 
 setup_kwargs = {
     'name': 'xeberus-restful-api-server-library',
-    'version': '1.6.7',
+    'version': '1.6.8',
     'description': 'Xeberus RESTful API Server Python Library',
     'long_description': '# Xeberus RESTful API Server Python Library\n\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/xeberus-restful-api-server-python-library',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `xeberus_restful_api_server_library-1.6.7/PKG-INFO` & `xeberus_restful_api_server_library-1.6.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: xeberus-restful-api-server-library
-Version: 1.6.7
+Version: 1.6.8
 Summary: Xeberus RESTful API Server Python Library
 Home-page: https://github.com/majormode/xeberus-restful-api-server-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library,xeberus,restful,api
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: fabric (>=2.7.0,<3.0.0)
-Requires-Dist: perseus-core-library (>=1.19,<2.0)
-Requires-Dist: perseus-restful-api-framework (>=1.26,<2.0)
+Requires-Dist: perseus-core-library (>=1.20.3,<2.0.0)
+Requires-Dist: perseus-restful-api-framework (>=1.28.4,<2.0.0)
 Requires-Dist: xeberus-core-library
 Project-URL: Repository, https://github.com/majormode/xeberus-restful-api-server-python-library
 Description-Content-Type: text/markdown
 
 # Xeberus RESTful API Server Python Library
```

