# Comparing `tmp/aiovemmio-0.5.8.tar.gz` & `tmp/aiovemmio-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiovemmio-0.5.8.tar", max compression
+gzip compressed data, was "aiovemmio-0.5.9.tar", max compression
```

## Comparing `aiovemmio-0.5.8.tar` & `aiovemmio-0.5.9.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0        0 2023-12-27 22:19:21.515213 aiovemmio-0.5.8/README.md
--rw-r--r--   0        0        0     6676 2024-01-10 21:17:41.105861 aiovemmio-0.5.8/aiovemmio/__init__.py
--rw-r--r--   0        0        0      367 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/accelerometer.proto
--rw-r--r--   0        0        0     1695 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/accelerometer_pb2.py
--rw-r--r--   0        0        0     1062 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/accelerometer_pb2.pyi
--rw-r--r--   0        0        0      745 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/addon.proto
--rw-r--r--   0        0        0     2656 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/addon_pb2.py
--rw-r--r--   0        0        0     1887 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/addon_pb2.pyi
--rw-r--r--   0        0        0      566 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/admin.proto
--rw-r--r--   0        0        0     2072 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/admin_pb2.py
--rw-r--r--   0        0        0      953 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/admin_pb2.pyi
--rw-r--r--   0        0        0      461 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/battery.proto
--rw-r--r--   0        0        0     1900 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/battery_pb2.py
--rw-r--r--   0        0        0      940 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/battery_pb2.pyi
--rw-r--r--   0        0        0      417 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/ble.proto
--rw-r--r--   0        0        0     1657 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/ble_pb2.py
--rw-r--r--   0        0        0      384 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/ble_pb2.pyi
--rw-r--r--   0        0        0      507 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/bsensor.proto
--rw-r--r--   0        0        0     2068 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/bsensor_pb2.py
--rw-r--r--   0        0        0     1571 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/bsensor_pb2.pyi
--rw-r--r--   0        0        0      894 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/carbon_dioxide.proto
--rw-r--r--   0        0        0     2540 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/carbon_dioxide_pb2.py
--rw-r--r--   0        0        0     2604 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/carbon_dioxide_pb2.pyi
--rw-r--r--   0        0        0     1328 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/carbon_monoxide.proto
--rw-r--r--   0        0        0     3791 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/carbon_monoxide_pb2.py
--rw-r--r--   0        0        0     3710 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/carbon_monoxide_pb2.pyi
--rw-r--r--   0        0        0      779 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/color.proto
--rw-r--r--   0        0        0     2669 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/color_pb2.py
--rw-r--r--   0        0        0     2368 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/color_pb2.pyi
--rw-r--r--   0        0        0     2117 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/configuration.proto
--rw-r--r--   0        0        0     5208 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/configuration_pb2.py
--rw-r--r--   0        0        0     6299 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/configuration_pb2.pyi
--rw-r--r--   0        0        0       79 2023-12-27 22:19:12.403152 aiovemmio-0.5.8/aiovemmio/const.py
--rw-r--r--   0        0        0     3889 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/devices.proto
--rw-r--r--   0        0        0    11645 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/devices_pb2.py
--rw-r--r--   0        0        0    14569 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/devices_pb2.pyi
--rw-r--r--   0        0        0      327 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/door.proto
--rw-r--r--   0        0        0     1459 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/door_pb2.py
--rw-r--r--   0        0        0      826 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/door_pb2.pyi
--rw-r--r--   0        0        0      276 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/doorbell.proto
--rw-r--r--   0        0        0     1449 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/doorbell_pb2.py
--rw-r--r--   0        0        0      784 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/doorbell_pb2.pyi
--rw-r--r--   0        0        0      329 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/emergency.proto
--rw-r--r--   0        0        0     1495 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/emergency_pb2.py
--rw-r--r--   0        0        0      843 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/emergency_pb2.pyi
--rw-r--r--   0        0        0     1349 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/firmware.proto
--rw-r--r--   0        0        0     3950 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/firmware_pb2.py
--rw-r--r--   0        0        0     2974 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/firmware_pb2.pyi
--rw-r--r--   0        0        0      272 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/flood.proto
--rw-r--r--   0        0        0     1417 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/flood_pb2.py
--rw-r--r--   0        0        0      761 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/flood_pb2.pyi
--rw-r--r--   0        0        0      623 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/gate.proto
--rw-r--r--   0        0        0     2224 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/gate_pb2.py
--rw-r--r--   0        0        0     1271 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/gate_pb2.pyi
--rw-r--r--   0        0        0      617 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/gateway.proto
--rw-r--r--   0        0        0     2305 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/gateway_pb2.py
--rw-r--r--   0        0        0      869 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/gateway_pb2.pyi
--rw-r--r--   0        0        0      300 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/heartbeat.proto
--rw-r--r--   0        0        0     1389 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/heartbeat_pb2.py
--rw-r--r--   0        0        0      277 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      424 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/info.proto
--rw-r--r--   0        0        0     1654 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/info_pb2.py
--rw-r--r--   0        0        0      967 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/info_pb2.pyi
--rw-r--r--   0        0        0     1081 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/level.proto
--rw-r--r--   0        0        0     3184 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/level_pb2.py
--rw-r--r--   0        0        0     1995 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/level_pb2.pyi
--rw-r--r--   0        0        0      640 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/lock.proto
--rw-r--r--   0        0        0     2266 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/lock_pb2.py
--rw-r--r--   0        0        0     1652 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/lock_pb2.pyi
--rw-r--r--   0        0        0      405 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/messaging.proto
--rw-r--r--   0        0        0     1595 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/messaging_pb2.py
--rw-r--r--   0        0        0     1189 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/messaging_pb2.pyi
--rw-r--r--   0        0        0      678 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/metadata.proto
--rw-r--r--   0        0        0     2482 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/metadata_pb2.py
--rw-r--r--   0        0        0     2173 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/metadata_pb2.pyi
--rw-r--r--   0        0        0      691 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/meter.proto
--rw-r--r--   0        0        0     2556 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/meter_pb2.py
--rw-r--r--   0        0        0     1732 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/meter_pb2.pyi
--rw-r--r--   0        0        0      304 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/mqtt.proto
--rw-r--r--   0        0        0     1387 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/mqtt_pb2.py
--rw-r--r--   0        0        0      682 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/mqtt_pb2.pyi
--rw-r--r--   0        0        0      647 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/power_source.proto
--rw-r--r--   0        0        0     2044 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/power_source_pb2.py
--rw-r--r--   0        0        0     1963 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/power_source_pb2.pyi
--rw-r--r--   0        0        0    11088 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/pubsub.proto
--rw-r--r--   0        0        0    21022 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/pubsub_pb2.py
--rw-r--r--   0        0        0    38160 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/pubsub_pb2.pyi
--rw-r--r--   0        0        0      623 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/remote.proto
--rw-r--r--   0        0        0     2305 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/remote_pb2.py
--rw-r--r--   0        0        0     1634 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/remote_pb2.pyi
--rw-r--r--   0        0        0     3488 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/reports.proto
--rw-r--r--   0        0        0     9203 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/reports_pb2.py
--rw-r--r--   0        0        0    11518 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/reports_pb2.pyi
--rw-r--r--   0        0        0      725 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/roller_shutter.proto
--rw-r--r--   0        0        0     2425 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/roller_shutter_pb2.py
--rw-r--r--   0        0        0     1234 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/roller_shutter_pb2.pyi
--rw-r--r--   0        0        0      358 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/seismic.proto
--rw-r--r--   0        0        0     1631 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/seismic_pb2.py
--rw-r--r--   0        0        0      915 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/seismic_pb2.pyi
--rw-r--r--   0        0        0      411 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/sensor.proto
--rw-r--r--   0        0        0     1816 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/sensor_pb2.py
--rw-r--r--   0        0        0     1215 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/sensor_pb2.pyi
--rw-r--r--   0        0        0     2041 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/siren.proto
--rw-r--r--   0        0        0     6086 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/siren_pb2.py
--rw-r--r--   0        0        0     5405 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/siren_pb2.pyi
--rw-r--r--   0        0        0      827 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/smoke.proto
--rw-r--r--   0        0        0     2408 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/smoke_pb2.py
--rw-r--r--   0        0        0     2531 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/smoke_pb2.pyi
--rw-r--r--   0        0        0      510 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/status.proto
--rw-r--r--   0        0        0     2010 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/status_pb2.py
--rw-r--r--   0        0        0     1199 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/status_pb2.pyi
--rw-r--r--   0        0        0      574 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/structure.proto
--rw-r--r--   0        0        0     2117 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/structure_pb2.py
--rw-r--r--   0        0        0     1590 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/structure_pb2.pyi
--rw-r--r--   0        0        0      563 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/switch.proto
--rw-r--r--   0        0        0     2130 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/switch_pb2.py
--rw-r--r--   0        0        0     1232 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/switch_pb2.pyi
--rw-r--r--   0        0        0      327 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/tamper.proto
--rw-r--r--   0        0        0     1464 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/tamper_pb2.py
--rw-r--r--   0        0        0      834 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/tamper_pb2.pyi
--rw-r--r--   0        0        0      222 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/taptap.proto
--rw-r--r--   0        0        0     1208 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/taptap_pb2.py
--rw-r--r--   0        0        0      382 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/taptap_pb2.pyi
--rw-r--r--   0        0        0      577 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/temperature.proto
--rw-r--r--   0        0        0     2202 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/temperature_pb2.py
--rw-r--r--   0        0        0     1347 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/temperature_pb2.pyi
--rw-r--r--   0        0        0     2053 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/thermostat.proto
--rw-r--r--   0        0        0     5680 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/thermostat_pb2.py
--rw-r--r--   0        0        0     5768 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/thermostat_pb2.pyi
--rw-r--r--   0        0        0      564 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/ultraviolet.proto
--rw-r--r--   0        0        0     2181 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/ultraviolet_pb2.py
--rw-r--r--   0        0        0     1256 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/ultraviolet_pb2.pyi
--rw-r--r--   0        0        0     8927 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/units.proto
--rw-r--r--   0        0        0     1739 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/units_pb2.py
--rw-r--r--   0        0        0     1184 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/units_pb2.pyi
--rw-r--r--   0        0        0      392 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/websocket.proto
--rw-r--r--   0        0        0     1638 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/websocket_pb2.py
--rw-r--r--   0        0        0     1050 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/websocket_pb2.pyi
--rw-r--r--   0        0        0     1130 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/wifi.proto
--rw-r--r--   0        0        0     3440 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/wifi_pb2.py
--rw-r--r--   0        0        0     3224 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/wifi_pb2.pyi
--rw-r--r--   0        0        0      911 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/zigbee.proto
--rw-r--r--   0        0        0     2989 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/zigbee_pb2.py
--rw-r--r--   0        0        0     2166 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/zigbee_pb2.pyi
--rw-r--r--   0        0        0     6501 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/zwave.proto
--rw-r--r--   0        0        0    17516 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/zwave_pb2.py
--rw-r--r--   0        0        0    18957 2023-11-23 21:36:45.000000 aiovemmio-0.5.8/aiovemmio/zwave_pb2.pyi
--rw-r--r--   0        0        0      304 2024-01-10 21:18:20.461955 aiovemmio-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aiovemmio-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-27 22:19:21.515213 aiovemmio-0.5.9/README.md
+-rw-r--r--   0        0        0     6781 2024-01-10 21:22:31.350586 aiovemmio-0.5.9/aiovemmio/__init__.py
+-rw-r--r--   0        0        0      367 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/accelerometer.proto
+-rw-r--r--   0        0        0     1695 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/accelerometer_pb2.py
+-rw-r--r--   0        0        0     1062 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/accelerometer_pb2.pyi
+-rw-r--r--   0        0        0      745 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/addon.proto
+-rw-r--r--   0        0        0     2656 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/addon_pb2.py
+-rw-r--r--   0        0        0     1887 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/addon_pb2.pyi
+-rw-r--r--   0        0        0      566 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/admin.proto
+-rw-r--r--   0        0        0     2072 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/admin_pb2.py
+-rw-r--r--   0        0        0      953 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/admin_pb2.pyi
+-rw-r--r--   0        0        0      461 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/battery.proto
+-rw-r--r--   0        0        0     1900 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/battery_pb2.py
+-rw-r--r--   0        0        0      940 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/battery_pb2.pyi
+-rw-r--r--   0        0        0      417 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/ble.proto
+-rw-r--r--   0        0        0     1657 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/ble_pb2.py
+-rw-r--r--   0        0        0      384 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/ble_pb2.pyi
+-rw-r--r--   0        0        0      507 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/bsensor.proto
+-rw-r--r--   0        0        0     2068 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/bsensor_pb2.py
+-rw-r--r--   0        0        0     1571 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/bsensor_pb2.pyi
+-rw-r--r--   0        0        0      894 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/carbon_dioxide.proto
+-rw-r--r--   0        0        0     2540 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/carbon_dioxide_pb2.py
+-rw-r--r--   0        0        0     2604 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/carbon_dioxide_pb2.pyi
+-rw-r--r--   0        0        0     1328 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/carbon_monoxide.proto
+-rw-r--r--   0        0        0     3791 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/carbon_monoxide_pb2.py
+-rw-r--r--   0        0        0     3710 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/carbon_monoxide_pb2.pyi
+-rw-r--r--   0        0        0      779 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/color.proto
+-rw-r--r--   0        0        0     2669 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/color_pb2.py
+-rw-r--r--   0        0        0     2368 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/color_pb2.pyi
+-rw-r--r--   0        0        0     2117 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/configuration.proto
+-rw-r--r--   0        0        0     5208 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/configuration_pb2.py
+-rw-r--r--   0        0        0     6299 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/configuration_pb2.pyi
+-rw-r--r--   0        0        0       79 2023-12-27 22:19:12.403152 aiovemmio-0.5.9/aiovemmio/const.py
+-rw-r--r--   0        0        0     3889 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/devices.proto
+-rw-r--r--   0        0        0    11645 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/devices_pb2.py
+-rw-r--r--   0        0        0    14569 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/devices_pb2.pyi
+-rw-r--r--   0        0        0      327 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/door.proto
+-rw-r--r--   0        0        0     1459 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/door_pb2.py
+-rw-r--r--   0        0        0      826 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/door_pb2.pyi
+-rw-r--r--   0        0        0      276 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/doorbell.proto
+-rw-r--r--   0        0        0     1449 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/doorbell_pb2.py
+-rw-r--r--   0        0        0      784 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/doorbell_pb2.pyi
+-rw-r--r--   0        0        0      329 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/emergency.proto
+-rw-r--r--   0        0        0     1495 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/emergency_pb2.py
+-rw-r--r--   0        0        0      843 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/emergency_pb2.pyi
+-rw-r--r--   0        0        0     1349 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/firmware.proto
+-rw-r--r--   0        0        0     3950 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/firmware_pb2.py
+-rw-r--r--   0        0        0     2974 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/firmware_pb2.pyi
+-rw-r--r--   0        0        0      272 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/flood.proto
+-rw-r--r--   0        0        0     1417 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/flood_pb2.py
+-rw-r--r--   0        0        0      761 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/flood_pb2.pyi
+-rw-r--r--   0        0        0      623 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/gate.proto
+-rw-r--r--   0        0        0     2224 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/gate_pb2.py
+-rw-r--r--   0        0        0     1271 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/gate_pb2.pyi
+-rw-r--r--   0        0        0      617 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/gateway.proto
+-rw-r--r--   0        0        0     2305 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/gateway_pb2.py
+-rw-r--r--   0        0        0      869 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/gateway_pb2.pyi
+-rw-r--r--   0        0        0      300 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/heartbeat.proto
+-rw-r--r--   0        0        0     1389 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/heartbeat_pb2.py
+-rw-r--r--   0        0        0      277 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      424 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/info.proto
+-rw-r--r--   0        0        0     1654 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/info_pb2.py
+-rw-r--r--   0        0        0      967 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/info_pb2.pyi
+-rw-r--r--   0        0        0     1081 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/level.proto
+-rw-r--r--   0        0        0     3184 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/level_pb2.py
+-rw-r--r--   0        0        0     1995 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/level_pb2.pyi
+-rw-r--r--   0        0        0      640 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/lock.proto
+-rw-r--r--   0        0        0     2266 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/lock_pb2.py
+-rw-r--r--   0        0        0     1652 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/lock_pb2.pyi
+-rw-r--r--   0        0        0      405 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/messaging.proto
+-rw-r--r--   0        0        0     1595 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/messaging_pb2.py
+-rw-r--r--   0        0        0     1189 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/messaging_pb2.pyi
+-rw-r--r--   0        0        0      678 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/metadata.proto
+-rw-r--r--   0        0        0     2482 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/metadata_pb2.py
+-rw-r--r--   0        0        0     2173 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/metadata_pb2.pyi
+-rw-r--r--   0        0        0      691 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/meter.proto
+-rw-r--r--   0        0        0     2556 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/meter_pb2.py
+-rw-r--r--   0        0        0     1732 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/meter_pb2.pyi
+-rw-r--r--   0        0        0      304 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/mqtt.proto
+-rw-r--r--   0        0        0     1387 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/mqtt_pb2.py
+-rw-r--r--   0        0        0      682 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/mqtt_pb2.pyi
+-rw-r--r--   0        0        0      647 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/power_source.proto
+-rw-r--r--   0        0        0     2044 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/power_source_pb2.py
+-rw-r--r--   0        0        0     1963 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/power_source_pb2.pyi
+-rw-r--r--   0        0        0    11088 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/pubsub.proto
+-rw-r--r--   0        0        0    21022 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/pubsub_pb2.py
+-rw-r--r--   0        0        0    38160 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/pubsub_pb2.pyi
+-rw-r--r--   0        0        0      623 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/remote.proto
+-rw-r--r--   0        0        0     2305 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/remote_pb2.py
+-rw-r--r--   0        0        0     1634 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/remote_pb2.pyi
+-rw-r--r--   0        0        0     3488 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/reports.proto
+-rw-r--r--   0        0        0     9203 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/reports_pb2.py
+-rw-r--r--   0        0        0    11518 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/reports_pb2.pyi
+-rw-r--r--   0        0        0      725 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/roller_shutter.proto
+-rw-r--r--   0        0        0     2425 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/roller_shutter_pb2.py
+-rw-r--r--   0        0        0     1234 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/roller_shutter_pb2.pyi
+-rw-r--r--   0        0        0      358 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/seismic.proto
+-rw-r--r--   0        0        0     1631 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/seismic_pb2.py
+-rw-r--r--   0        0        0      915 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/seismic_pb2.pyi
+-rw-r--r--   0        0        0      411 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/sensor.proto
+-rw-r--r--   0        0        0     1816 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/sensor_pb2.py
+-rw-r--r--   0        0        0     1215 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/sensor_pb2.pyi
+-rw-r--r--   0        0        0     2041 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/siren.proto
+-rw-r--r--   0        0        0     6086 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/siren_pb2.py
+-rw-r--r--   0        0        0     5405 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/siren_pb2.pyi
+-rw-r--r--   0        0        0      827 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/smoke.proto
+-rw-r--r--   0        0        0     2408 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/smoke_pb2.py
+-rw-r--r--   0        0        0     2531 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/smoke_pb2.pyi
+-rw-r--r--   0        0        0      510 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/status.proto
+-rw-r--r--   0        0        0     2010 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/status_pb2.py
+-rw-r--r--   0        0        0     1199 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/status_pb2.pyi
+-rw-r--r--   0        0        0      574 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/structure.proto
+-rw-r--r--   0        0        0     2117 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/structure_pb2.py
+-rw-r--r--   0        0        0     1590 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/structure_pb2.pyi
+-rw-r--r--   0        0        0      563 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/switch.proto
+-rw-r--r--   0        0        0     2130 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/switch_pb2.py
+-rw-r--r--   0        0        0     1232 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/switch_pb2.pyi
+-rw-r--r--   0        0        0      327 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/tamper.proto
+-rw-r--r--   0        0        0     1464 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/tamper_pb2.py
+-rw-r--r--   0        0        0      834 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/tamper_pb2.pyi
+-rw-r--r--   0        0        0      222 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/taptap.proto
+-rw-r--r--   0        0        0     1208 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/taptap_pb2.py
+-rw-r--r--   0        0        0      382 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/taptap_pb2.pyi
+-rw-r--r--   0        0        0      577 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/temperature.proto
+-rw-r--r--   0        0        0     2202 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/temperature_pb2.py
+-rw-r--r--   0        0        0     1347 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/temperature_pb2.pyi
+-rw-r--r--   0        0        0     2053 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/thermostat.proto
+-rw-r--r--   0        0        0     5680 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/thermostat_pb2.py
+-rw-r--r--   0        0        0     5768 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/thermostat_pb2.pyi
+-rw-r--r--   0        0        0      564 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/ultraviolet.proto
+-rw-r--r--   0        0        0     2181 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/ultraviolet_pb2.py
+-rw-r--r--   0        0        0     1256 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/ultraviolet_pb2.pyi
+-rw-r--r--   0        0        0     8927 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/units.proto
+-rw-r--r--   0        0        0     1739 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/units_pb2.py
+-rw-r--r--   0        0        0     1184 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/units_pb2.pyi
+-rw-r--r--   0        0        0      392 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/websocket.proto
+-rw-r--r--   0        0        0     1638 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/websocket_pb2.py
+-rw-r--r--   0        0        0     1050 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/websocket_pb2.pyi
+-rw-r--r--   0        0        0     1130 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/wifi.proto
+-rw-r--r--   0        0        0     3440 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/wifi_pb2.py
+-rw-r--r--   0        0        0     3224 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/wifi_pb2.pyi
+-rw-r--r--   0        0        0      911 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/zigbee.proto
+-rw-r--r--   0        0        0     2989 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/zigbee_pb2.py
+-rw-r--r--   0        0        0     2166 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/zigbee_pb2.pyi
+-rw-r--r--   0        0        0     6501 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/zwave.proto
+-rw-r--r--   0        0        0    17516 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/zwave_pb2.py
+-rw-r--r--   0        0        0    18957 2023-11-23 21:36:45.000000 aiovemmio-0.5.9/aiovemmio/zwave_pb2.pyi
+-rw-r--r--   0        0        0      304 2024-01-10 21:23:16.426704 aiovemmio-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aiovemmio-0.5.9/PKG-INFO
```

### Comparing `aiovemmio-0.5.8/aiovemmio/__init__.py` & `aiovemmio-0.5.9/aiovemmio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import base64
 import pprint
 from collections.abc import Callable
+from enum import Enum
 from typing import Any, Self, Iterable
 
 import aiohttp
 import async_timeout
 from aiohttp import WSMsgType
 
 from .const import LOGGER
@@ -56,16 +57,21 @@
         )
 
 
 class DeviceConnectionError(Exception):
     pass
 
 
+class Event(Enum):
+    CONN_CLOSED = 1
+
+
 class Client:
     message_handler: Callable[[GatewayReport], None]
+    event_handler: Callable[[Event], None]
 
     def __init__(self, host: str, port: int, session: aiohttp.ClientSession):
         self.host = host
         self.port = port
         self.session = session
         self._calls: dict[int, Call] = {}
         self._call_id = 0
@@ -107,15 +113,15 @@
         LOGGER.debug("Trying to connect to device at %s", self.host)
         self._client = await self.session.ws_connect(
             f"http://{self.host}:{self.port}/rpc", autoping=False
         )
         self._rx_task = asyncio.create_task(self._rx_msgs())
         LOGGER.debug("Connected to %s", self.host)
 
-    async def _rx_msgs(self, disconnected: Callable) -> None:
+    async def _rx_msgs(self) -> None:
         while not self._client.closed:
             msg = await self._client.receive()
             LOGGER.debug("Received msg (%s): %s", self.host, msg)
             LOGGER.debug("MSG type %s : %s", msg.type, msg.type == WSMsgType.CLOSED)
             if msg.type == WSMsgType.CLOSED:
                 LOGGER.debug("MSG TYPE CLOSED")
                 break
@@ -145,15 +151,15 @@
                 call_item.resolve.set_exception(Exception())
         self._calls.clear()
 
         if not self._client.closed:
             await self._client.close()
 
         self._client = None
-        disconnected()
+        self.event_handler(Event.CONN_CLOSED)
 
     async def close(self):
         if self._rx_task:
             self._rx_task.cancel()
         if self._client:
             await self._client.close()
```

### Comparing `aiovemmio-0.5.8/aiovemmio/accelerometer_pb2.py` & `aiovemmio-0.5.9/aiovemmio/accelerometer_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/accelerometer_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/accelerometer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/addon.proto` & `aiovemmio-0.5.9/aiovemmio/addon.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/addon_pb2.py` & `aiovemmio-0.5.9/aiovemmio/addon_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/addon_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/addon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/admin.proto` & `aiovemmio-0.5.9/aiovemmio/admin.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/admin_pb2.py` & `aiovemmio-0.5.9/aiovemmio/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/admin_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/battery_pb2.py` & `aiovemmio-0.5.9/aiovemmio/battery_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/battery_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/battery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/ble_pb2.py` & `aiovemmio-0.5.9/aiovemmio/ble_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/bsensor_pb2.py` & `aiovemmio-0.5.9/aiovemmio/bsensor_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/bsensor_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/bsensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/carbon_dioxide.proto` & `aiovemmio-0.5.9/aiovemmio/carbon_dioxide.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/carbon_dioxide_pb2.py` & `aiovemmio-0.5.9/aiovemmio/carbon_dioxide_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/carbon_dioxide_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/carbon_dioxide_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/carbon_monoxide.proto` & `aiovemmio-0.5.9/aiovemmio/carbon_monoxide.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/carbon_monoxide_pb2.py` & `aiovemmio-0.5.9/aiovemmio/carbon_monoxide_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/carbon_monoxide_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/carbon_monoxide_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/color.proto` & `aiovemmio-0.5.9/aiovemmio/color.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/color_pb2.py` & `aiovemmio-0.5.9/aiovemmio/color_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/color_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/color_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/configuration.proto` & `aiovemmio-0.5.9/aiovemmio/configuration.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/configuration_pb2.py` & `aiovemmio-0.5.9/aiovemmio/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/configuration_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/devices.proto` & `aiovemmio-0.5.9/aiovemmio/devices.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/devices_pb2.py` & `aiovemmio-0.5.9/aiovemmio/devices_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/devices_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/devices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/door_pb2.py` & `aiovemmio-0.5.9/aiovemmio/door_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/door_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/door_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/doorbell_pb2.py` & `aiovemmio-0.5.9/aiovemmio/doorbell_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/doorbell_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/doorbell_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/emergency_pb2.py` & `aiovemmio-0.5.9/aiovemmio/emergency_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/emergency_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/emergency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/firmware.proto` & `aiovemmio-0.5.9/aiovemmio/firmware.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/firmware_pb2.py` & `aiovemmio-0.5.9/aiovemmio/firmware_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/firmware_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/firmware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/flood_pb2.py` & `aiovemmio-0.5.9/aiovemmio/flood_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/flood_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/flood_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/gate.proto` & `aiovemmio-0.5.9/aiovemmio/gate.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/gate_pb2.py` & `aiovemmio-0.5.9/aiovemmio/gate_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/gate_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/gate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/gateway.proto` & `aiovemmio-0.5.9/aiovemmio/gateway.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/gateway_pb2.py` & `aiovemmio-0.5.9/aiovemmio/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/gateway_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/gateway_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/heartbeat_pb2.py` & `aiovemmio-0.5.9/aiovemmio/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/info_pb2.py` & `aiovemmio-0.5.9/aiovemmio/info_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/info_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/level.proto` & `aiovemmio-0.5.9/aiovemmio/level.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/level_pb2.py` & `aiovemmio-0.5.9/aiovemmio/level_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/level_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/level_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/lock.proto` & `aiovemmio-0.5.9/aiovemmio/lock.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/lock_pb2.py` & `aiovemmio-0.5.9/aiovemmio/lock_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/lock_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/lock_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/messaging_pb2.py` & `aiovemmio-0.5.9/aiovemmio/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/messaging_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/metadata.proto` & `aiovemmio-0.5.9/aiovemmio/metadata.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/metadata_pb2.py` & `aiovemmio-0.5.9/aiovemmio/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/metadata_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/meter.proto` & `aiovemmio-0.5.9/aiovemmio/meter.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/meter_pb2.py` & `aiovemmio-0.5.9/aiovemmio/meter_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/meter_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/meter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/mqtt_pb2.py` & `aiovemmio-0.5.9/aiovemmio/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/mqtt_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/mqtt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/power_source.proto` & `aiovemmio-0.5.9/aiovemmio/power_source.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/power_source_pb2.py` & `aiovemmio-0.5.9/aiovemmio/power_source_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/power_source_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/power_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/pubsub.proto` & `aiovemmio-0.5.9/aiovemmio/pubsub.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/pubsub_pb2.py` & `aiovemmio-0.5.9/aiovemmio/pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/pubsub_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/pubsub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/remote.proto` & `aiovemmio-0.5.9/aiovemmio/remote.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/remote_pb2.py` & `aiovemmio-0.5.9/aiovemmio/remote_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/remote_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/remote_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/reports.proto` & `aiovemmio-0.5.9/aiovemmio/reports.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/reports_pb2.py` & `aiovemmio-0.5.9/aiovemmio/reports_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/reports_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/reports_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/roller_shutter.proto` & `aiovemmio-0.5.9/aiovemmio/roller_shutter.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/roller_shutter_pb2.py` & `aiovemmio-0.5.9/aiovemmio/roller_shutter_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/roller_shutter_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/roller_shutter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/seismic_pb2.py` & `aiovemmio-0.5.9/aiovemmio/seismic_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/seismic_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/seismic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/sensor_pb2.py` & `aiovemmio-0.5.9/aiovemmio/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/sensor_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/sensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/siren.proto` & `aiovemmio-0.5.9/aiovemmio/siren.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/siren_pb2.py` & `aiovemmio-0.5.9/aiovemmio/siren_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/siren_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/siren_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/smoke.proto` & `aiovemmio-0.5.9/aiovemmio/smoke.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/smoke_pb2.py` & `aiovemmio-0.5.9/aiovemmio/smoke_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/smoke_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/smoke_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/status_pb2.py` & `aiovemmio-0.5.9/aiovemmio/status_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/status_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/structure.proto` & `aiovemmio-0.5.9/aiovemmio/structure.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/structure_pb2.py` & `aiovemmio-0.5.9/aiovemmio/structure_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/structure_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/structure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/switch.proto` & `aiovemmio-0.5.9/aiovemmio/switch.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/switch_pb2.py` & `aiovemmio-0.5.9/aiovemmio/switch_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/switch_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/switch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/tamper_pb2.py` & `aiovemmio-0.5.9/aiovemmio/tamper_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/tamper_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/tamper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/taptap_pb2.py` & `aiovemmio-0.5.9/aiovemmio/taptap_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/temperature.proto` & `aiovemmio-0.5.9/aiovemmio/temperature.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/temperature_pb2.py` & `aiovemmio-0.5.9/aiovemmio/temperature_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/temperature_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/temperature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/thermostat.proto` & `aiovemmio-0.5.9/aiovemmio/thermostat.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/thermostat_pb2.py` & `aiovemmio-0.5.9/aiovemmio/thermostat_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/thermostat_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/thermostat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/ultraviolet.proto` & `aiovemmio-0.5.9/aiovemmio/ultraviolet.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/ultraviolet_pb2.py` & `aiovemmio-0.5.9/aiovemmio/ultraviolet_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/ultraviolet_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/ultraviolet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/units.proto` & `aiovemmio-0.5.9/aiovemmio/units.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/units_pb2.py` & `aiovemmio-0.5.9/aiovemmio/units_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/units_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/units_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/websocket_pb2.py` & `aiovemmio-0.5.9/aiovemmio/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/websocket_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/websocket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/wifi.proto` & `aiovemmio-0.5.9/aiovemmio/wifi.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/wifi_pb2.py` & `aiovemmio-0.5.9/aiovemmio/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/wifi_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/wifi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/zigbee.proto` & `aiovemmio-0.5.9/aiovemmio/zigbee.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/zigbee_pb2.py` & `aiovemmio-0.5.9/aiovemmio/zigbee_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/zigbee_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/zigbee_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/zwave.proto` & `aiovemmio-0.5.9/aiovemmio/zwave.proto`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/zwave_pb2.py` & `aiovemmio-0.5.9/aiovemmio/zwave_pb2.py`

 * *Files identical despite different names*

### Comparing `aiovemmio-0.5.8/aiovemmio/zwave_pb2.pyi` & `aiovemmio-0.5.9/aiovemmio/zwave_pb2.pyi`

 * *Files identical despite different names*

