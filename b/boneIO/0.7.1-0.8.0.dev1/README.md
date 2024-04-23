# Comparing `tmp/boneIO-0.7.1.tar.gz` & `tmp/boneIO-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.7.1.tar", last modified: Thu Sep 21 19:43:15 2023, max compression
+gzip compressed data, was "boneIO-0.8.0.dev1.tar", last modified: Tue Apr 23 17:44:54 2024, max compression
```

## Comparing `boneIO-0.7.1.tar` & `boneIO-0.8.0.dev1.tar`

### file list

```diff
@@ -1,87 +1,90 @@
--rw-r--r--   0        0        0    35149 2023-09-21 19:42:38.664071 boneIO-0.7.1/LICENSE
--rw-r--r--   0        0        0      474 2023-09-21 19:42:38.664071 boneIO-0.7.1/README.md
--rw-r--r--   0        0        0      147 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/__init__.py
--rw-r--r--   0        0        0     3435 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/bonecli.py
--rw-r--r--   0        0        0     3256 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/const.py
--rw-r--r--   0        0        0     8444 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/adc_v0_4.yaml
--rw-r--r--   0        0        0      286 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/binary_sensor.yaml
--rw-r--r--   0        0        0      369 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2692 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/event.yaml
--rw-r--r--   0        0        0     3392 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     1713 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/output24x16A_v0.3.yaml
--rw-r--r--   0        0        0     2403 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0       80 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/group/__init__.py
--rw-r--r--   0        0        0     2005 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/group/output.py
--rw-r--r--   0        0        0     2039 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/__init__.py
--rw-r--r--   0        0        0      993 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1184 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/click_timer.py
--rw-r--r--   0        0        0     2431 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/config.py
--rw-r--r--   0        0        0     8059 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/events.py
--rw-r--r--   0        0        0      717 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-09-21 19:42:38.664071 boneIO-0.7.1/boneio/helper/filter.py
--rw-r--r--   0        0        0     3557 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6437 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    17275 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/logger.py
--rw-r--r--   0        0        0      771 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0      311 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/pcf8575.py
--rw-r--r--   0        0        0     1066 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/queue.py
--rw-r--r--   0        0        0     2145 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5853 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0      200 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/input/__init__.py
--rw-r--r--   0        0        0     2709 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/input/gpio.py
--rw-r--r--   0        0        0     3228 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/input/gpio_new.py
--rw-r--r--   0        0        0    27237 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/modbus.py
--rw-r--r--   0        0        0     8551 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/oled.py
--rw-r--r--   0        0        0      231 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/relay/__init__.py
--rw-r--r--   0        0        0     3276 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2508 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4594 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/relay/pca.py
--rw-r--r--   0        0        0     2635 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/relay/pcf.py
--rw-r--r--   0        0        0     2789 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/runner.py
--rw-r--r--   0        0        0     1039 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/actions.yaml
--rw-r--r--   0        0        0       91 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0       96 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/id.yaml
--rw-r--r--   0        0        0    16625 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      566 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1328 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1296 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     1293 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/gpio_new.py
--rw-r--r--   0        0        0     8520 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1808 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       37 2023-09-21 19:42:38.668072 boneIO-0.7.1/boneio/version.py
--rw-r--r--   0        0        0     1878 2023-09-21 19:42:38.668072 boneIO-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      166 2023-09-21 19:42:38.668072 boneIO-0.7.1/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-09-21 19:42:38.668072 boneIO-0.7.1/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-09-21 19:42:38.668072 boneIO-0.7.1/tests/relay_32_5.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 boneIO-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/LICENSE
+-rw-r--r--   0        0        0      474 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/README.md
+-rw-r--r--   0        0        0      147 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/__init__.py
+-rw-r--r--   0        0        0     3491 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/bonecli.py
+-rw-r--r--   0        0        0     3293 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/const.py
+-rw-r--r--   0        0        0     8444 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/cover.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/adc.yaml
+-rw-r--r--   0        0        0      286 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/binary_sensor.yaml
+-rw-r--r--   0        0        0      397 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2692 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/event.yaml
+-rw-r--r--   0        0        0     2692 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/event_all.yaml
+-rw-r--r--   0        0        0     3392 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     1713 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/output24x16A_v0.3.yaml
+-rw-r--r--   0        0        0     2403 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0       80 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/group/__init__.py
+-rw-r--r--   0        0        0     1992 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/group/output.py
+-rw-r--r--   0        0        0     2118 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/__init__.py
+-rw-r--r--   0        0        0     1018 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1315 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     2431 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/config.py
+-rw-r--r--   0        0        0     8648 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/events.py
+-rw-r--r--   0        0        0      717 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/filter.py
+-rw-r--r--   0        0        0     4771 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     7107 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    17333 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/logger.py
+-rw-r--r--   0        0        0      859 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0      311 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/pcf8575.py
+-rw-r--r--   0        0        0     1066 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/queue.py
+-rw-r--r--   0        0        0     6170 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/sensor/ina_219_smbus.py
+-rw-r--r--   0        0        0     2633 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     6731 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      681 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/util.py
+-rw-r--r--   0        0        0    11334 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0      200 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2438 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/input/gpio.py
+-rw-r--r--   0        0        0     2822 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/input/gpio_new.py
+-rw-r--r--   0        0        0    28589 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/manager.py
+-rw-r--r--   0        0        0     3682 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/modbus.py
+-rw-r--r--   0        0        0     8665 2024-04-23 17:44:17.846643 boneIO-0.8.0.dev1/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5505 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/oled.py
+-rw-r--r--   0        0        0      231 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     4377 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2000 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     2951 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2288 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/relay/pcf.py
+-rw-r--r--   0        0        0     2855 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/runner.py
+-rw-r--r--   0        0        0     1039 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0       91 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0       96 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    18131 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      619 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1328 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1199 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     1223 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/gpio_new.py
+-rw-r--r--   0        0        0     3439 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/ina219.py
+-rw-r--r--   0        0        0     8573 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1808 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       41 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/boneio/version.py
+-rw-r--r--   0        0        0     1883 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      166 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2024-04-23 17:44:17.850643 boneIO-0.8.0.dev1/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.8.0.dev1/PKG-INFO
```

### Comparing `boneIO-0.7.1/LICENSE` & `boneIO-0.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/bonecli.py` & `boneIO-0.8.0.dev1/boneio/bonecli.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,13 +109,13 @@
     if args.action == "run":
         exit_code = run(
             config=args.config,
             mqttusername=args.mqttusername,
             mqttpassword=args.mqttpassword,
             debug=debug,
         )
-
+    _LOGGER.info("Exiting with exit code %s", exit_code)
     return exit_code
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `boneIO-0.7.1/boneio/const.py` & `boneIO-0.8.0.dev1/boneio/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "uart1": {ID: "/dev/ttyS1", TX: "P9.24", RX: "P9.26"},
     "uart2": {ID: "/dev/ttyS2", TX: "P9.21", RX: "P9.22"},
     "uart3": {ID: "/dev/ttyS3", TX: "P9.42", RX: None},
     "uart4": {ID: "/dev/ttyS4", TX: "P9.13", RX: "P9.11"},
     "uart5": {ID: "/dev/ttyS5", TX: "P8.37", RX: "P8.38"},
 }
 
-relay_actions = {ON: "turn_on", OFF: "turn_off", TOGGLE: "toggle"}
+relay_actions = {ON: "async_turn_on", OFF: "async_turn_off", TOGGLE: "async_toggle"}
 
 # HA CONSTS
 HOMEASSISTANT = "homeassistant"
 HA_DISCOVERY = "ha_discovery"
 OUTPUT_TYPE = "output_type"
 SHOW_HA = "show_in_ha"
 
@@ -154,7 +154,9 @@
     "OPEN": "open",
     "CLOSE": "close",
     "TOGGLE": "toggle",
     "STOP": "stop",
     "TOGGLE_OPEN": "toggle_open",
     "TOGGLE_CLOSE": "toggle_close",
 }
+
+INA219 = "ina219"
```

### Comparing `boneIO-0.7.1/boneio/cover.py` & `boneIO-0.8.0.dev1/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/example_config/event.yaml` & `boneIO-0.8.0.dev1/boneio/example_config/event.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/example_config/led32x4A.yaml` & `boneIO-0.8.0.dev1/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/example_config/output24x16A.yaml` & `boneIO-0.8.0.dev1/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/example_config/output24x16A_v0.3.yaml` & `boneIO-0.8.0.dev1/boneio/example_config/output24x16A_v0.3.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/example_config/output32x5A.yaml` & `boneIO-0.8.0.dev1/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/fonts/danube__.ttf` & `boneIO-0.8.0.dev1/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/group/output.py` & `boneIO-0.8.0.dev1/boneio/group/output.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-"""Cover module."""
+"""Group output module."""
 from __future__ import annotations
-import logging
 import asyncio
 from typing import List
-
 from boneio.const import COVER, SWITCH, ON, OFF
 from boneio.relay.basic import BasicRelay
 
-_LOGGER = logging.getLogger(__name__)
-
 
 class OutputGroup(BasicRelay):
     """Cover class of boneIO"""
 
     def __init__(
         self,
         members: List[BasicRelay],
@@ -37,28 +33,27 @@
             if x.state == ON:
                 state = ON
                 break
         if state != self._state or not relay_id:
             self._state = state
             self._loop.call_soon_threadsafe(self.send_state)
 
-    def turn_on(self) -> None:
+    async def async_turn_on(self) -> None:
         """Call turn on action."""
-        for x in self._group_members:
-            asyncio.create_task(x.async_turn_on())
+        await asyncio.gather(
+            *[self._loop.run_in_executor(self.executor, x.turn_on) for x in self._group_members]
+        )
 
-    def turn_off(self) -> None:
+    async def async_turn_off(self) -> None:
         """Call turn off action."""
-        for x in self._group_members:
-            asyncio.create_task(x.async_turn_off())
+        await asyncio.gather(
+            *[self._loop.run_in_executor(self.executor, x.turn_off) for x in self._group_members]
+        )
 
-    def toggle(self) -> None:
-        """Toggle group."""
-        _LOGGER.debug("Toggle relay.")
-        if self._state == ON:
-            self.turn_off()
-        else:
-            self.turn_on()
+    @property
+    def is_active(self) -> bool:
+        """Is relay active."""
+        return self._state == ON
 
     def send_state(self) -> None:
         """Send state to Mqtt on action."""
         self._send_message(topic=self._send_topic, payload=self.payload(), retain=True)
```

### Comparing `boneIO-0.7.1/boneio/helper/__init__.py` & `boneIO-0.8.0.dev1/boneio/helper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ha_button_availabilty_message,
     ha_event_availabilty_message,
     ha_light_availabilty_message,
     ha_sensor_availabilty_message,
     ha_sensor_temp_availabilty_message,
     ha_switch_availabilty_message,
     ha_led_availabilty_message,
+    ha_sensor_ina_availabilty_message
 )
 from boneio.helper.mqtt import BasicMqtt
 from boneio.helper.async_updater import AsyncUpdater
 from boneio.helper.oled import make_font
 from boneio.helper.queue import UniqueQueue
 from boneio.helper.state_manager import StateManager
 from boneio.helper.stats import HostData
@@ -50,14 +51,15 @@
     "ha_light_availabilty_message",
     "ha_switch_availabilty_message",
     "ha_sensor_availabilty_message",
     "ha_adc_sensor_availabilty_message",
     "ha_sensor_temp_availabilty_message",
     "ha_binary_sensor_availabilty_message",
     "ha_button_availabilty_message",
+    "ha_sensor_ina_availabilty_message",
     "ha_event_availabilty_message",
     "ha_led_availabilty_message",
     "GPIOInputException",
     "GPIOOutputException",
     "I2CError",
     "GpioBaseClass",
     "StateManager",
```

### Comparing `boneIO-0.7.1/boneio/helper/async_updater.py` & `boneIO-0.8.0.dev1/boneio/helper/async_updater.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import asyncio
-
+import time
 # Typing imports that create a circular dependency
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ..manager import Manager
 from boneio.helper.timeperiod import TimePeriod
 
@@ -15,15 +15,15 @@
         self._update_interval = update_interval or TimePeriod(seconds=60)
         self.manager.append_task(coro=self._refresh, name=self.id)
 
     async def _refresh(self) -> None:
         while True:
             if hasattr(self, "async_update"):
                 update_interval = (
-                    await self.async_update(time=None)
+                    await self.async_update(time=time.time())
                     or self._update_interval.total_in_seconds
                 )
             else:
                 update_interval = (
-                    self.update(time=None) or self._update_interval.total_in_seconds
+                    self.update(time=time.time()) or self._update_interval.total_in_seconds
                 )
             await asyncio.sleep(update_interval)
```

### Comparing `boneIO-0.7.1/boneio/helper/click_timer.py` & `boneIO-0.8.0.dev1/boneio/helper/click_timer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from __future__ import annotations
+import logging
 import asyncio
 from boneio.helper.timeperiod import TimePeriod
 import time
 
+_LOGGER = logging.getLogger(__name__)
+
+
 class ClickTimer:
     """Represent async call later function with variable to check if timing is ON."""
 
     def __init__(self, delay: TimePeriod, action) -> None:
         """Initialize Click timer."""
         self._loop = asyncio.get_running_loop()
         self._remove_listener = None
         self._delay: float = delay.total_in_seconds
         self._action = action
 
     def is_waiting(self) -> bool:
         """If variable is set then timer is ON, if None is Off."""
         return self._remove_listener is not None
+    
+    @property
+    def delay(self) -> float:
+        return self._delay
 
     def reset(self) -> None:
         """Uninitialize variable remove_listener."""
         if self._remove_listener:
             self._remove_listener.cancel()
             self._remove_listener = None
```

### Comparing `boneIO-0.7.1/boneio/helper/config.py` & `boneIO-0.8.0.dev1/boneio/helper/config.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/events.py` & `boneIO-0.8.0.dev1/boneio/helper/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import datetime as dt
 import logging
 import signal
 import time
 from datetime import datetime
-from typing import Callable, Optional
+from typing import Any, Coroutine, List, Optional, Callable, Optional
+
 
 from boneio.helper.util import callback
 
 _LOGGER = logging.getLogger(__name__)
 UTC = dt.timezone.utc
 EVENT_TIME_CHANGED = "event_time_changed"
 CALLBACK_TYPE = Callable[[], None]
@@ -257,7 +258,26 @@
 ) -> CALLBACK_TYPE:
     """Add a listener that fires once after a specific point in UTC time."""
     # Ensure point_in_time is UTC
     expected_fire_timestamp = time.time() + (delay / 1000)
     return async_track_point_in_timestamp(
         loop=loop, action=action, timestamp=expected_fire_timestamp
     )
+
+
+def create_unawaited_task_threadsafe(
+    loop: asyncio.AbstractEventLoop,
+    transient_tasks: List["asyncio.Task[Any]"],
+    coro: Coroutine[Any, Any, None],
+    task_future: Optional["asyncio.Future[asyncio.Task[Any]]"] = None,
+) -> None:
+    """
+    Schedule a coroutine on the loop and add the Task to transient_tasks.
+    """
+
+    def callback() -> None:
+        task = loop.create_task(coro)
+        transient_tasks.append(task)
+        if task_future is not None:
+            task_future.set_result(task)
+
+    loop.call_soon_threadsafe(callback)
```

### Comparing `boneIO-0.7.1/boneio/helper/exceptions.py` & `boneIO-0.8.0.dev1/boneio/helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/filter.py` & `boneIO-0.8.0.dev1/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/gpio.py` & `boneIO-0.8.0.dev1/boneio/helper/gpio.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import asyncio
 import logging
-
+from datetime import datetime
 try:
     from Adafruit_BBIO import GPIO
 except ModuleNotFoundError:
 
     class GPIO:
         PUD_OFF = "poff"
         PUD_UP = "poff"
@@ -13,21 +13,22 @@
 
         def __init__(self):
             pass
 
     pass
 
 import subprocess
-from typing import Callable
+from typing import Callable, Awaitable, List
 
 from boneio.const import CONFIG_PIN, FALLING
 from boneio.const import GPIO as GPIO_STR
-from boneio.const import GPIO_MODE, LOW, ClickTypes, Gpio_Edges, Gpio_States
+from boneio.const import GPIO_MODE, LOW, ClickTypes, Gpio_Edges, Gpio_States, InputTypes
 from boneio.helper.exceptions import GPIOInputException
 from boneio.helper.timeperiod import TimePeriod
+from concurrent.futures import ThreadPoolExecutor
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def configure_pin(pin: str, mode: str = GPIO_STR) -> None:
     pin = f"{pin[0:3]}0{pin[3]}" if len(pin) == 4 else pin
     _LOGGER.debug(f"Configuring pin {pin} for mode {mode}.")
@@ -77,53 +78,88 @@
     pin: str, callback: Callable, bounce: int = 0, edge: Gpio_Edges = FALLING
 ) -> None:
     """Add detection for RISING and FALLING events."""
     try:
         GPIO.add_event_detect(gpio=pin, edge=edge, callback=callback, bouncetime=bounce)
     except RuntimeError as err:
         raise GPIOInputException(err)
-    
-def add_event_detect(
-    pin: str, edge: Gpio_Edges = FALLING
-) -> None:
+
+
+def add_event_detect(pin: str, edge: Gpio_Edges = FALLING) -> None:
     """Add detection for RISING and FALLING events."""
     try:
         GPIO.add_event_detect(gpio=pin, edge=edge)
     except RuntimeError as err:
         raise GPIOInputException(err)
-    
-def add_event_callback(
-    pin: str, callback: Callable
-) -> None:
+
+
+def add_event_callback(pin: str, callback: Callable) -> None:
     """Add detection for RISING and FALLING events."""
     try:
-        GPIO.add_event_callback(gpio=pin,callback=callback)
+        GPIO.add_event_callback(gpio=pin, callback=callback)
     except RuntimeError as err:
         raise GPIOInputException(err)
 
 
 class GpioBaseClass:
     """Base class for initialize GPIO"""
 
     def __init__(
-        self, pin: str, press_callback: Callable[[ClickTypes, str, bool | None], None], **kwargs
+        self,
+        pin: str,
+        press_callback: Callable[
+            [ClickTypes, str, List, InputTypes, bool, float | None], Awaitable[None]
+        ],
+        name: str,
+        actions: dict,
+        input_type,
+        empty_message_after: bool,
+        **kwargs,
     ) -> None:
         """Setup GPIO Input Button"""
         self._pin = pin
         gpio_mode = kwargs.get(GPIO_MODE, GPIO_STR)
-        self._bounce_time = kwargs.get("bounce_time", TimePeriod(milliseconds=50))
+        bounce_time: TimePeriod = kwargs.get("bounce_time", TimePeriod(milliseconds=50))
+        self._bounce_time = bounce_time.total_in_seconds
         self._loop = asyncio.get_running_loop()
         self._press_callback = press_callback
+        self._name = name
         setup_input(pin=self._pin, pull_mode=gpio_mode)
+        self.executor = ThreadPoolExecutor()
+        self._actions = actions
+        self._input_type = input_type
+        self._empty_message_after = empty_message_after
+
+    def press_callback(self, click_type: ClickTypes, duration: float | None = None) -> None:
+        actions = self._actions.get(click_type, [])
+        self._loop.create_task(self.async_press_callback(click_type, duration, actions))
 
-    def set_press_callback(self, press_callback: Callable[[ClickTypes, str, bool | None], None]) -> None:
-        self._press_callback = press_callback
+    async def async_press_callback(
+        self, click_type: ClickTypes, duration: float | None = None, actions: List = []
+    ) -> None:
+        _LOGGER.warn("press callback %s", datetime.now())
+        await self._press_callback(
+            click_type,
+            self._pin,
+            actions,
+            self._input_type,
+            self._empty_message_after,
+            duration,
+        )
+
+    def set_actions(self, actions: dict) -> None:
+        self._actions = actions
 
     @property
     def is_pressed(self) -> bool:
         """Is button pressed."""
         return read_input(self._pin)
-    
+
+    @property
+    def name(self) -> str:
+        """Name of the GPIO visible in HA/MQTT."""
+        return self._name
+
     @property
     def pin(self) -> str:
         """Return configured pin."""
         return self._pin
```

### Comparing `boneIO-0.7.1/boneio/helper/ha_discovery.py` & `boneIO-0.8.0.dev1/boneio/helper/ha_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,36 @@
         "payload_off": "released",
         "name": name,
         "state_topic": f"{topic}/{INPUT_SENSOR}/{id}",
         "unique_id": f"{topic}{INPUT_SENSOR}{id}",
     }
 
 
+def ha_sensor_ina_availabilty_message(
+    id: str, name: str, topic: str = "boneIO", **kwargs
+):
+    """Create availability topic for HA."""
+    return {
+        "availability": [{"topic": f"{topic}/{STATE}"}],
+        "device": {
+            "identifiers": [topic],
+            "manufacturer": "boneIO",
+            "model": "boneIO Relay Board",
+            "name": f"boneIO {topic}",
+            "sw_version": __version__,
+        },
+        "name": name,
+        "state_topic": f"{topic}/{SENSOR}/{id}",
+        "unique_id": f"{topic}{SENSOR}{id}",
+        "state_class": "measurement",
+        "value_template": "{{ value_json.state }}",
+        **kwargs,
+    }
+
+
 def ha_sensor_temp_availabilty_message(
     id: str, name: str, topic: str = "boneIO", **kwargs
 ):
     """Create availability topic for HA."""
     return {
         "availability": [{"topic": f"{topic}/{STATE}"}],
         "device": {
```

### Comparing `boneIO-0.7.1/boneio/helper/loader.py` & `boneIO-0.8.0.dev1/boneio/helper/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-
 import logging
 import time
 from collections import namedtuple
 from typing import TYPE_CHECKING, Any, Callable, Dict, Union
 
 from adafruit_mcp230xx.mcp23017 import MCP23017
 from adafruit_pca9685 import PCA9685
@@ -50,14 +49,15 @@
     GPIOOutputException,
     I2CError,
     StateManager,
     ha_adc_sensor_availabilty_message,
     ha_binary_sensor_availabilty_message,
     ha_event_availabilty_message,
     ha_sensor_temp_availabilty_message,
+    ha_sensor_ina_availabilty_message,
 )
 from boneio.helper.onewire import (
     DS2482,
     DS2482_ADDRESS,
     OneWireBus,
     AsyncBoneIOW1ThermSensor,
     OneWireAddress,
@@ -232,46 +232,38 @@
         return OutputEntry(PCFRelay, PCF, expander_id)
     else:
         raise GPIOOutputException(f"""Output type {output_kind} dont exists""")
 
 
 def configure_output_group(
     manager: Manager,
-    state_manager: StateManager,
     topic_prefix: str,
-    relay_id: str,
     config: dict,
     **kwargs,
 ) -> Any:
     """Configure kind of relay. Most common MCP."""
-    restore_state = config.pop(RESTORE_STATE, False)
     _id = config.pop(ID)
-    restored_state = (
-        state_manager.get(attr_type=RELAY, attr=relay_id, default_value=False)
-        if restore_state
-        else False
-    )
 
     output = OutputGroup(
         send_message=manager.send_message,
         topic_prefix=topic_prefix,
         id=_id,
-        restored_state=restored_state,
         callback=lambda: None,
         **config,
         **kwargs,
     )
     return output
 
 
 def configure_relay(
     manager: Manager,
     state_manager: StateManager,
     topic_prefix: str,
     relay_id: str,
+    name: str,
     relay_callback: Callable,
     config: dict,
     **kwargs,
 ) -> Any:
     """Configure kind of relay. Most common MCP."""
     restore_state = config.pop(RESTORE_STATE, False)
     output_type = config.pop(OUTPUT_TYPE)
@@ -330,16 +322,17 @@
             "Output kind: %s is not configured", getattr(output, "output_kind")
         )
         return
 
     relay = getattr(output, "OutputClass")(
         send_message=manager.send_message,
         topic_prefix=topic_prefix,
-        id=config.pop(ID),
+        id=relay_id,
         restored_state=restored_state,
+        name=name,
         **config,
         **kwargs,
         **extra_args,
         callback=lambda: relay_callback(
             expander_id=getattr(output, "expander_id"),
             relay_id=relay_id,
             restore_state=False if output_type == NONE else restore_state,
@@ -350,56 +343,45 @@
 
 
 def configure_event_sensor(
     gpio: dict,
     pin: str,
     press_callback: Callable,
     send_ha_autodiscovery: Callable,
-    input: GpioEventButtonOld | GpioEventButtonNew | None = None,
+    input: GpioEventButtonOld | GpioEventButtonNew | None = None
 ) -> GpioEventButtonOld | GpioEventButtonNew | None:
     """Configure input sensor or button."""
     try:
         GpioEventButtonClass = (
             GpioEventButtonNew
             if gpio.get("detection_type", "new") == "new"
             else GpioEventButtonOld
         )
+        name = gpio.pop(ID, pin)
         if input:
             if not isinstance(input, GpioEventButtonClass):
                 _LOGGER.warn(
                     "You preconfigured type of input. It's forbidden. Please restart boneIO."
                 )
                 return input
-            input.set_press_callback(
-                press_callback=lambda x, i, z: press_callback(
-                    x=x,
-                    inpin=i,
-                    actions=gpio.get(ACTIONS, {}).get(x, []),
-                    input_type=INPUT,
-                    empty_message_after=gpio.get("clear_message", False),
-                    duration=z,
-                )
-            )
+            input.set_actions(actions=gpio.get(ACTIONS, {}))
         else:
             input = GpioEventButtonClass(
                 pin=pin,
-                press_callback=lambda x, i, z: press_callback(
-                    x=x,
-                    inpin=i,
-                    actions=gpio.get(ACTIONS, {}).get(x, []),
-                    input_type=INPUT,
-                    empty_message_after=gpio.get("clear_message", False),
-                    duration=z,
-                ),
+                name=name,
+                input_type=INPUT,
+                empty_message_after=gpio.pop("clear_message", False),
+                actions=gpio.pop(ACTIONS, {}),
+                press_callback=press_callback,
                 **gpio,
             )
         if gpio.get(SHOW_HA, True):
             send_ha_autodiscovery(
                 id=pin,
-                name=gpio.get(ID, pin),
+                name=name,
                 ha_type=EVENT_ENTITY,
                 device_class=gpio.get(DEVICE_CLASS, None),
                 availability_msg_func=ha_event_availabilty_message,
             )
         return input
     except GPIOInputException as err:
         _LOGGER.error("This PIN %s can't be configured. %s", pin, err)
@@ -416,46 +398,36 @@
     """Configure input sensor or button."""
     try:
         GpioInputBinarySensorClass = (
             GpioInputBinarySensorNew
             if gpio.get("detection_type", "new") == "new"
             else GpioInputBinarySensorOld
         )
+        name = gpio.pop(ID, pin)
         if input:
             if not isinstance(input, GpioInputBinarySensorClass):
                 _LOGGER.warn(
                     "You preconfigured type of input. It's forbidden. Please restart boneIO."
                 )
                 return input
-            input.set_press_callback(
-                press_callback=lambda x, i, z: press_callback(
-                    x=x,
-                    inpin=i,
-                    actions=gpio.get(ACTIONS, {}).get(x, []),
-                    input_type=INPUT,
-                    empty_message_after=gpio.get("clear_message", False),
-                    duration=z,
-                )
-            )
+            input.set_actions(actions=gpio.get(ACTIONS, {}))
         else:
             input = GpioInputBinarySensorClass(
                 pin=pin,
-                press_callback=lambda x, i: press_callback(
-                    x=x,
-                    inpin=i,
-                    actions=gpio.get(ACTIONS, {}).get(x, []),
-                    input_type=INPUT_SENSOR,
-                    empty_message_after=gpio.get("clear_message", False),
-                ),
+                name=name,
+                actions=gpio.pop(ACTIONS, {}),
+                input_type=INPUT_SENSOR,
+                empty_message_after=gpio.pop("clear_message", False),
+                press_callback=press_callback,
                 **gpio,
             )
         if gpio.get(SHOW_HA, True):
             send_ha_autodiscovery(
                 id=pin,
-                name=gpio.get(ID, pin),
+                name=name,
                 ha_type=BINARY_SENSOR,
                 device_class=gpio.get(DEVICE_CLASS, None),
                 availability_msg_func=ha_binary_sensor_availabilty_message,
             )
         return input
     except GPIOInputException as err:
         _LOGGER.error("This PIN %s can't be configured. %s", pin, err)
@@ -553,7 +525,42 @@
             id=sensor.id,
             name=sensor.name,
             ha_type=SENSOR,
             availability_msg_func=ha_sensor_temp_availabilty_message,
             unit_of_measurement=config.get("unit_of_measurement", "°C"),
         )
     return sensor
+
+
+def create_ina219_sensor(
+    manager: Manager,
+    topic_prefix: str,
+    config: dict = {},
+):
+    """Create INA219 sensor in manager."""
+    from boneio.sensor import INA219
+
+    address = config[ADDRESS]
+    id = config.get(ID, str(address)).replace(" ", "")
+    try:
+        ina219 = INA219(
+            id=id,
+            address=address,
+            sensors=config.get("sensors", []),
+            manager=manager,
+            send_message=manager.send_message,
+            topic_prefix=topic_prefix,
+            update_interval=config.get(UPDATE_INTERVAL, TimePeriod(seconds=60)),
+        )
+        for sensor in ina219.sensors.values():
+            manager.send_ha_autodiscovery(
+                id=sensor.id,
+                name=sensor.name,
+                ha_type=SENSOR,
+                availability_msg_func=ha_sensor_ina_availabilty_message,
+                unit_of_measurement=sensor.unit_of_measurement,
+                device_class=sensor.device_class,
+            )
+        return ina219
+    except I2CError as err:
+        _LOGGER.error("Can't configure Temp sensor. %s", err)
+        pass
```

### Comparing `boneIO-0.7.1/boneio/helper/logger.py` & `boneIO-0.8.0.dev1/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/mqtt.py` & `boneIO-0.8.0.dev1/boneio/helper/mqtt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Class to help initialize classes which uses mqtt send."""
 from typing import Callable, Union
+from boneio.helper.util import strip_accents
 
 
 class BasicMqtt:
     """Basic MQTT class."""
 
     def __init__(
         self,
@@ -14,15 +15,16 @@
         topic_type: str,
         **kwargs,
     ):
         """Initialize module."""
         self._id = id.replace(" ", "")
         self._name = name
         self._send_message = send_message
-        self._send_topic = f"{topic_prefix}/{topic_type}/{self.id}"
+        topic_id = strip_accents(self.id)
+        self._send_topic = f"{topic_prefix}/{topic_type}/{topic_id}"
 
     @property
     def id(self) -> str:
         """Id of the module."""
         return self._id
 
     @property
```

### Comparing `boneIO-0.7.1/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.8.0.dev1/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/onewire/ds2482.py` & `boneIO-0.8.0.dev1/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/onewire/onewire.py` & `boneIO-0.8.0.dev1/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/queue.py` & `boneIO-0.8.0.dev1/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/state_manager.py` & `boneIO-0.8.0.dev1/boneio/helper/state_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """State files manager."""
 from __future__ import annotations
 import asyncio
 import logging
 import json
 from typing import Any
+from concurrent.futures import ThreadPoolExecutor
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class StateManager:
     """StateManager to load and save states to file."""
 
@@ -15,14 +16,16 @@
         """Initialize disk StateManager."""
         self._loop = asyncio.get_event_loop()
         self._lock = asyncio.Lock()
         self._file = state_file
         self._state = self.load_states()
         _LOGGER.info("Loaded state file from %s", self._file)
         self._file_uptodate = False
+        self._save_attributes_callback = None
+        self.executor = ThreadPoolExecutor()
 
     def load_states(self) -> dict:
         """Load state file."""
         try:
             with open(self._file, "r") as state_file:
                 datastore = json.load(state_file)
                 return datastore
@@ -36,29 +39,36 @@
             del self._state[attr_type][attribute]
 
     def save_attribute(self, attr_type: str, attribute: str, value: str) -> None:
         """Save single attribute to file."""
         if attr_type not in self._state:
             self._state[attr_type] = {}
         self._state[attr_type][attribute] = value
-        asyncio.run_coroutine_threadsafe(self.save_state(), self._loop)
+        if self._save_attributes_callback is not None:
+            print(self._save_attributes_callback)
+            self._save_attributes_callback.cancel()
+            self._save_attributes_callback = None
+        self._save_attributes_callback = self._loop.call_later(1, lambda: self._loop.create_task(self.save_state()))
 
     def get(self, attr_type: str, attr: str, default_value: Any = None) -> Any:
         """Retrieve attribute from json."""
         attrs = self._state.get(attr_type)
         if attrs:
             return attrs.get(attr, default_value)
         return default_value
 
     @property
     def state(self) -> dict:
         """Retrieve all states."""
         return self._state
+    
+    def _save_state(self) -> None:
+        with open(self._file, "w+", encoding="utf-8") as f:
+            json.dump(self._state, f, indent=2)
 
     async def save_state(self) -> None:
         """Async save state."""
         if self._lock.locked():
             # Let's not save state if something happens same time.
             return
         async with self._lock:
-            with open(self._file, "w+", encoding="utf-8") as f:
-                json.dump(self._state, f, indent=2)
+            self._loop.run_in_executor(None, self._save_state)
```

### Comparing `boneIO-0.7.1/boneio/helper/stats.py` & `boneIO-0.8.0.dev1/boneio/helper/stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import psutil
 
 from boneio.const import (
     CPU,
     DISK,
     GIGABYTE,
+    INA219,
     IP,
     MAC,
     MASK,
     MEGABYTE,
     MEMORY,
     NETWORK,
     NONE,
@@ -29,15 +30,15 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from boneio.manager import Manager
 
 from boneio.helper.async_updater import AsyncUpdater
 from boneio.helper.timeperiod import TimePeriod
-from boneio.sensor import LM75Sensor, MCP9808Sensor
+from boneio.sensor import LM75Sensor, MCP9808Sensor, INA219 as INA219Class
 from boneio.version import __version__
 
 intervals = (("d", 86400), ("h", 3600), ("m", 60))
 
 
 def display_time(seconds):
     """Strf time."""
@@ -118,15 +119,15 @@
 class HostSensor(AsyncUpdater):
     """Host sensor."""
 
     def __init__(
         self,
         update_function: Callable,
         manager_callback: Callable,
-        static_data: dict,
+        static_data: dict | None,
         id: str,
         type: str,
         **kwargs,
     ) -> None:
         self._update_function = update_function
         self._static_data = static_data
         self._state = {}
@@ -146,46 +147,64 @@
             return {**self._static_data, **self._state}
         return self._state
 
 
 class HostData:
     """Helper class to store host data."""
 
-    data = {UPTIME: {}, NETWORK: {}, CPU: {}, DISK: {}, MEMORY: {}, SWAP: {}}
-
     def __init__(
         self,
         output: dict,
         callback: Callable,
         temp_sensor: Callable[[LM75Sensor, MCP9808Sensor], None],
+        ina219: INA219Class | None,
         manager: Manager,
         enabled_screens: List[str],
     ) -> None:
         """Initialize HostData."""
         self._hostname = socket.gethostname()
         self._temp_sensor = temp_sensor
         host_stats = {
             NETWORK: {"f": get_network_info, "update_interval": TimePeriod(seconds=60)},
             CPU: {"f": get_cpu_info, "update_interval": TimePeriod(seconds=5)},
             DISK: {"f": get_disk_info, "update_interval": TimePeriod(seconds=60)},
             MEMORY: {"f": get_memory_info, "update_interval": TimePeriod(seconds=10)},
             SWAP: {"f": get_swap_info, "update_interval": TimePeriod(seconds=60)},
             UPTIME: {
                 "f": lambda: {
-                    "uptime": get_uptime(),
-                    "temp": f"{self._temp_sensor.state} C"
-                } if self._temp_sensor else {"uptime": get_uptime() },
-                "static": {HOST: self._hostname, "version": __version__},
+                    "uptime": {"data": get_uptime(), "fontSize": "small", "row": 2, "col": 3},
+                    "MQTT": {"data": "CONN" if manager.mqtt_state else "DOWN", "fontSize": "small", "row": 3, "col": 60},
+                    "T": {
+                        "data": f"{self._temp_sensor.state} C",
+                        "fontSize": "small",
+                        "row": 3,
+                        "col": 3
+                    },
+                }
+                if self._temp_sensor
+                else {"uptime": {"data": get_uptime(), "fontSize": "small", "row": 2, "col": 3}},
+                "static": {
+                    HOST: {"data": self._hostname, "fontSize": "small", "row": 0, "col": 3},
+                    "ver": {"data": __version__, "fontSize": "small", "row": 1, "col": 3},
+                },
                 "update_interval": TimePeriod(seconds=30),
             },
         }
+        if ina219 is not None:
+            host_stats[INA219] = {
+                "f": lambda: {
+                    *{sensor.device_class: sensor.state for sensor in ina219.sensors}
+                },
+                "update_interval": TimePeriod(seconds=60)
+            }
+        self._data = {}
         for k, _v in host_stats.items():
             if k not in enabled_screens:
                 continue
-            self.data[k] = HostSensor(
+            self._data[k] = HostSensor(
                 update_function=_v["f"],
                 static_data=_v.get("static"),
                 manager=manager,
                 manager_callback=callback,
                 id=f"{k}_hoststats",
                 type=k,
                 update_interval=_v["update_interval"],
@@ -194,15 +213,15 @@
         self._callback = callback
         self._loop = asyncio.get_running_loop()
 
     def get(self, type: str) -> dict:
         """Get saved stats."""
         if type in self._output:
             return self._get_output(type)
-        return self.data[type].state
+        return self._data[type].state
 
     def _get_output(self, type: str) -> dict:
         """Get stats for output."""
         out = {}
         for output in self._output[type].values():
             out[output.id] = output.state
         return out
```

### Comparing `boneIO-0.7.1/boneio/helper/timeperiod.py` & `boneIO-0.8.0.dev1/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/helper/yaml_util.py` & `boneIO-0.8.0.dev1/boneio/helper/yaml_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,26 +281,26 @@
             "ms": "milliseconds",
             "milliseconds": "milliseconds",
             "s": "seconds",
             "sec": "seconds",
             "secs": "seconds",
             "seconds": "seconds",
             "min": "minutes",
+            "mins": "minutes",
             "minutes": "minutes",
             "h": "hours",
             "hours": "hours",
             "d": "days",
             "days": "days",
         }
 
         match = re.match(r"^([-+]?[0-9]*\.?[0-9]*)\s*(\w*)$", value)
         if match is None:
             raise ConfigurationException(f"Expected time period with unit, got {value}")
         kwarg = unit_to_kwarg[one_of(*unit_to_kwarg)(match.group(2))]
-
         return TimePeriod(**{kwarg: float(match.group(1))})
 
     def _normalize_coerce_check_action_def(self, value):
         parent = self.root_document[self.document_path[0]][self.document_path[1]]
         _schema = self.schema["actions"]
         keys = value.keys()
         out = {}
```

### Comparing `boneIO-0.7.1/boneio/input/gpio.py` & `boneIO-0.8.0.dev1/boneio/input/gpio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """GpioEventButton to receive signals."""
 from __future__ import annotations
 import logging
 import asyncio
-from functools import partial
-from boneio.const import DOUBLE, LONG, SINGLE, ClickTypes
+from boneio.const import DOUBLE, LONG, SINGLE
 from boneio.helper import GpioBaseClass, ClickTimer, TimePeriod
 
 
 # TIMINGS FOR BUTTONS
 
 DOUBLE_CLICK_DURATION_MS = 350
 LONG_PRESS_DURATION_MS = 600
@@ -32,28 +31,23 @@
             action=lambda x: self.press_callback(click_type=LONG, duration=x),
         )
         self._double_click_ran = False
         self._is_waiting_for_second_click = False
         self._long_press_ran = False
         asyncio.create_task(self._run())
 
-    def press_callback(self, click_type: ClickTypes, duration: float | None = None):
-        self._loop.call_soon_threadsafe(
-            partial(self._press_callback, click_type, self._pin, duration)
-        )
-
     def double_click_press_callback(self):
         self._is_waiting_for_second_click = False
         if not self._state and not self._timer_long.is_waiting():
             self.press_callback(click_type=SINGLE, duration=None)
 
     async def _run(self) -> None:
         while True:
             self.check_state(state=self.is_pressed)
-            await asyncio.sleep(self._bounce_time.total_in_seconds)
+            await asyncio.sleep(self._bounce_time)
 
     def check_state(self, state: bool) -> None:
         if state == self._state:
             return
         self._state = state
         if state: #is pressed?
             self._timer_long.start_timer()
```

### Comparing `boneIO-0.7.1/boneio/input/gpio_new.py` & `boneIO-0.8.0.dev1/boneio/input/gpio_new.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,74 @@
 """GpioEventButtonNew to receive signals."""
 from __future__ import annotations
 import time
 import logging
-from functools import partial
-from boneio.const import DOUBLE, LONG, SINGLE, ClickTypes, BOTH
+from boneio.const import DOUBLE, LONG, SINGLE, BOTH
 from boneio.helper import GpioBaseClass, ClickTimer
-from boneio.helper.gpio import add_event_callback, add_event_detect
+from boneio.helper.gpio import edge_detect
 from boneio.helper.timeperiod import TimePeriod
-# TIMINGS FOR BUTTONS
-
-
-DOUBLE_CLICK_TIME = 0.35  # Maximum time between two clicks for a double-click
-LONG_CLICK_TIME = 0.6  # Minimum time for a long click
-DEBOUNCE_TIME = 0.05
 _LOGGER = logging.getLogger(__name__)
 
-
-DOUBLE_CLICK_DURATION_MS = 300
+# TIMINGS FOR BUTTONS
+DOUBLE_CLICK_DURATION_MS = 180
 LONG_PRESS_DURATION_MS = 600
 
 
 class GpioEventButtonNew(GpioBaseClass):
     """Represent Gpio input switch."""
 
     def __init__(self, **kwargs) -> None:
         """Setup GPIO Input Button"""
         super().__init__(**kwargs)
         self._state = self.is_pressed
         self.button_pressed_time = 0.0
-        self.click_count = 0
         self.last_click_time = 0.0
         self._double_test = None
         self._long_test = None
 
         self._timer_double = ClickTimer(
             delay=TimePeriod(milliseconds=DOUBLE_CLICK_DURATION_MS),
-            action=lambda x: self.double_click_press_callback(),
+            action=lambda x: self.single_click_callback(),
         )
         self._timer_long = ClickTimer(
             delay=TimePeriod(milliseconds=LONG_PRESS_DURATION_MS),
-            action=lambda x: self.press_callback(click_type=LONG, duration=x),
+            action=lambda x: self.long_click_callback(x),
         )
         self._double_click_ran = False
-        self._is_waiting_for_second_click = False
         self._long_press_ran = False
-
-        add_event_detect(pin=self._pin, edge=BOTH)
-        add_event_callback(pin=self._pin, callback=self.check_state)
+        edge_detect(pin=self._pin, callback=self.check_state, bounce=0, edge=BOTH)
         _LOGGER.debug("Configured NEW listening for input pin %s", self._pin)
 
-    def double_click_press_callback(self):
-        self._is_waiting_for_second_click = False
+    def single_click_callback(self):
+        """This is invoked by double timer if time is up for double timer."""
         if not self._state and not self._timer_long.is_waiting():
             self.press_callback(click_type=SINGLE, duration=None)
 
-    def check_state(self, channel) -> None:
+    def double_click_callback(self):
+        """This is double click callback."""
+        self.press_callback(click_type=DOUBLE, duration=None)
+
+    def long_click_callback(self, duration: float):
+        """This is long click callback."""
+        self.press_callback(click_type=LONG, duration=duration)
+
+    def check_state(self, _) -> None:
         time_now = time.time()
         self._state = self.is_pressed
         if self._state:
-            if time_now - self.button_pressed_time >= DEBOUNCE_TIME:
+            if time_now - self.button_pressed_time >= self._bounce_time:
                 self.button_pressed_time = time_now
-                self.click_count += 1
                 self._timer_long.start_timer()
                 if self._timer_double.is_waiting():
                     self._timer_double.reset()
                     self._double_click_ran = True
-                    self.press_callback(click_type=DOUBLE, duration=None)
+                    self.double_click_callback()
                     return
                 self._timer_double.start_timer()
-                self._is_waiting_for_second_click = True
 
         else:
-            if not self._is_waiting_for_second_click and not self._double_click_ran:
+            if not self._timer_double.is_waiting() and not self._double_click_ran:
                 if self._timer_long.is_waiting():
                     self.press_callback(click_type=SINGLE, duration=None)
             self._timer_long.reset()
             self._double_click_ran = False
 
-    def press_callback(self, click_type: ClickTypes, duration: float | None = None):
-        self.click_count = 0
-        self._loop.call_soon_threadsafe(
-            partial(self._press_callback, click_type, self._pin, duration)
-        )
```

### Comparing `boneIO-0.7.1/boneio/manager.py` & `boneIO-0.8.0.dev1/boneio/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from __future__ import annotations
 import asyncio
 import logging
 from collections import deque
+import datetime
 from typing import Callable, Coroutine, List, Optional, Set, Union, Awaitable
 from board import SCL, SDA
 from busio import I2C
+from concurrent.futures import ThreadPoolExecutor
+
 
 from boneio.const import (
     ACTION,
     ADDRESS,
     BINARY_SENSOR,
     BUTTON,
     CLOSE,
     COVER,
     DALLAS,
     EVENT_ENTITY,
     ID,
+    INA219,
     INPUT,
     LM75,
     MCP_TEMP_9808,
     MODBUS,
     MQTT,
     NONE,
     ONEWIRE,
@@ -51,14 +55,15 @@
     I2CError,
     StateManager,
     ha_button_availabilty_message,
     ha_light_availabilty_message,
     ha_switch_availabilty_message,
     ha_led_availabilty_message,
 )
+from boneio.helper.util import strip_accents
 from boneio.helper.config import ConfigHelper
 from boneio.helper.events import EventBus
 from boneio.helper.exceptions import ModbusUartException
 from boneio.helper.loader import (
     configure_cover,
     configure_event_sensor,
     configure_binary_sensor,
@@ -85,14 +90,15 @@
 class Manager:
     """Manager to communicate MQTT with GPIO inputs and outputs."""
 
     def __init__(
         self,
         send_message: Callable[[str, Union[str, dict], bool], None],
         stop_client: Callable[[], Awaitable[None]],
+        mqtt_state: Callable[[], bool],
         state_manager: StateManager,
         config_helper: ConfigHelper,
         config_file_path: str,
         relay_pins: List = [],
         event_pins: List = [],
         binary_pins: List = [],
         output_group: List = [],
@@ -116,34 +122,37 @@
         self._host_data = None
         self._config_file_path = config_file_path
         self._state_manager = state_manager
         self._event_bus = EventBus(loop=self._loop)
 
         self.send_message = send_message
         self.stop_client = stop_client
+        self._mqtt_state = mqtt_state
         self._event_pins = event_pins
         self._inputs = {}
         self._binary_pins = binary_pins
         self._i2cbusio = I2C(SCL, SDA)
         self._mcp = {}
         self._pcf = {}
         self._pca = {}
         self._output = {}
         self._configured_output_groups = {}
         self._oled = None
         self._tasks: List[asyncio.Task] = []
         self._covers = {}
         self._temp_sensors = []
+        self._ina219_sensors = []
         self._modbus = None
 
         self._configure_modbus(modbus=modbus)
 
         self._configure_temp_sensors(sensors=sensors)
 
         self._configure_modbus_sensors(sensors=sensors)
+        self._configure_ina219_sensors(sensors=sensors)
         self._configure_sensors(
             dallas=dallas, ds2482=ds2482, sensors=sensors.get(ONEWIRE)
         )
 
         self.grouped_outputs = create_expander(
             expander_dict=self._mcp,
             expander_config=mcp23017,
@@ -166,19 +175,21 @@
                 i2cbusio=self._i2cbusio,
             )
         )
 
         self._configure_adc(adc_list=adc)
 
         for _config in relay_pins:
-            _id = _config[ID].replace(" ", "")
+            _name = _config.pop(ID)
+            _id = strip_accents(_name)
             out = configure_relay(
                 manager=self,
                 state_manager=self._state_manager,
                 topic_prefix=self._config_helper.topic_prefix,
+                name=_name,
                 relay_id=_id,
                 relay_callback=self._relay_callback,
                 config=_config,
                 event_bus=self._event_bus,
             )
             if not out:
                 continue
@@ -195,15 +206,15 @@
             self._loop.call_soon_threadsafe(
                 self._loop.call_later,
                 0.5,
                 out.send_state,
             )
 
         for _config in cover:
-            _id = _config[ID].replace(" ", "")
+            _id = strip_accents(_config[ID])
             open_relay = self._output.get(_config.get("open_relay"))
             close_relay = self._output.get(_config.get("close_relay"))
             if not open_relay:
                 _LOGGER.error(
                     "Can't configure cover %s. This relay doesn't exist.",
                     _config.get("open_relay"),
                 )
@@ -233,46 +244,54 @@
                 event_bus=self._event_bus,
                 send_ha_autodiscovery=self.send_ha_autodiscovery,
                 topic_prefix=self._config_helper.topic_prefix,
             )
 
         self._output_group = output_group
         self._configure_output_group()
+        self.executor = ThreadPoolExecutor()
 
         _LOGGER.info("Initializing inputs. This will take a while.")
         self.configure_inputs(reload_config=False)
 
         if oled.get("enabled", False):
             from boneio.oled import Oled
 
             screens = oled.get("screens", [])
 
             self._host_data = HostData(
                 manager=self,
                 enabled_screens=screens,
                 output=self.grouped_outputs,
                 temp_sensor=self._temp_sensors[0] if self._temp_sensors else None,
+                ina219=self._ina219_sensors[0] if self._ina219_sensors else None,
                 callback=self._host_data_callback,
             )
             try:
                 self._oled = Oled(
                     host_data=self._host_data,
                     screen_order=screens,
                     output_groups=list(self.grouped_outputs),
                     sleep_timeout=oled.get("screensaver_timeout", 60),
                 )
             except (GPIOInputException, I2CError) as err:
                 _LOGGER.error("Can't configure OLED display. %s", err)
         self.prepare_ha_buttons()
+
         _LOGGER.info("BoneIO manager is ready.")
 
+    @property
+    def mqtt_state(self) -> bool:
+        return self._mqtt_state()
+
     def _configure_output_group(self):
         def get_outputs(output_list):
             outputs = []
             for x in output_list:
+                x = strip_accents(x)
                 if x in self._output:
                     output = self._output[x]
                     if output.output_type == COVER:
                         _LOGGER.warn("You can't add cover output to group.")
                     else:
                         outputs.append(output)
             return outputs
@@ -281,14 +300,15 @@
             members = get_outputs(group.pop("outputs"))
             if not members:
                 _LOGGER.warn(
                     "This group %s doesn't have any valid members. Not adding it.",
                     group[ID],
                 )
                 continue
+            _LOGGER.debug("Configuring output group %s with members: %s", group[ID], [x.name for x in members])
             configured_group = configure_output_group(
                 config=group,
                 manager=self,
                 state_manager=self._state_manager,
                 topic_prefix=self._config_helper.topic_prefix,
                 relay_id=group[ID].replace(" ", ""),
                 event_bus=self._event_bus,
@@ -472,14 +492,27 @@
                         sensor_type=sensor_type,
                         config=temp_def,
                         i2cbusio=self._i2cbusio,
                     )
                     if temp_sensor:
                         self._temp_sensors.append(temp_sensor)
 
+    def _configure_ina219_sensors(self, sensors: dict) -> None:
+        if sensors.get(INA219):
+            from boneio.helper.loader import create_ina219_sensor
+
+            for sensor_config in sensors[INA219]:
+                ina219 = create_ina219_sensor(
+                    topic_prefix=self._config_helper.topic_prefix,
+                    manager=self,
+                    config=sensor_config,
+                )
+                if ina219:
+                    self._ina219_sensors.append(ina219)
+
     def _configure_modbus_sensors(self, sensors: dict) -> None:
         if sensors.get(MODBUS) and self._modbus:
             from boneio.helper.loader import create_modbus_sensors
 
             create_modbus_sensors(
                 manager=self,
                 event_bus=self._event_bus,
@@ -563,15 +596,15 @@
         return self._pca
 
     @property
     def pcf(self):
         """Get PCF by it's id."""
         return self._pcf
 
-    def press_callback(
+    async def press_callback(
         self,
         x: ClickTypes,
         inpin: str,
         actions: List,
         input_type: InputTypes = INPUT,
         empty_message_after: bool = False,
         duration: float | None = None,
@@ -587,48 +620,48 @@
                 return {"event_type": x}
             return x
 
         def get_output_and_action(device_id, action, action_output, action_cover):
             if action == OUTPUT:
                 return (
                     self._output.get(
-                        device_id, self._configured_output_groups.get(device_id)
+                        strip_accents(device_id), self._configured_output_groups.get(device_id)
                     ),
                     relay_actions.get(action_output),
                 )
             else:
-                return (self._covers.get(device_id), cover_actions.get(action_cover))
-
-        self.send_message(topic=topic, payload=generate_payload(), retain=False)
+                return (self._covers.get(strip_accents(device_id)), cover_actions.get(action_cover))
         for action_definition in actions:
             _LOGGER.debug("Executing action %s", action_definition)
             if action_definition[ACTION] in (OUTPUT, COVER):
                 device = action_definition.get(PIN)
                 if not device:
                     continue
                 (output, action) = get_output_and_action(
                     device_id=device.replace(" ", ""),
                     action=action_definition[ACTION],
                     action_output=action_definition.get("action_output"),
                     action_cover=action_definition.get("action_cover"),
                 )
                 if output and action:
-                    getattr(output, action)()
+                    _f = getattr(output, action)
+                    asyncio.create_task(_f())
                 else:
                     if not action:
                         _LOGGER.warn("Action doesn't exists %s. Check spelling", action)
                     if not output:
                         _LOGGER.warn("Device %s for action not found", device)
             elif action_definition[ACTION] == MQTT:
                 action_topic = action_definition.get(TOPIC)
                 action_payload = action_definition.get("action_mqtt_msg")
                 if action_topic and action_payload:
                     self.send_message(
                         topic=action_topic, payload=action_payload, retain=False
                     )
+        self._loop.run_in_executor(self.executor, lambda: self.send_message(topic=topic, payload=generate_payload(), retain=False))
         # This is similar how Z2M is clearing click sensor.
         if empty_message_after:
             self._loop.call_soon_threadsafe(
                 self._loop.call_later, 0.2, self.send_message, topic, ""
             )
 
     def send_ha_autodiscovery(
@@ -682,26 +715,23 @@
             return
         if msg_type == RELAY and command == "set":
             target_device = self._output.get(device_id)
 
             if target_device and target_device.output_type != NONE:
                 action_from_msg = relay_actions.get(message.upper())
                 if action_from_msg:
-                    getattr(target_device, action_from_msg)()
+                    _f = getattr(target_device, action_from_msg)
+                    asyncio.create_task(_f())
                 else:
                     _LOGGER.debug("Action not exist %s.", message.upper())
             else:
                 _LOGGER.debug("Target device not found %s.", device_id)
         elif msg_type == RELAY and command == SET_BRIGHTNESS:
             target_device = self._output.get(device_id)
-            if (
-                target_device
-                and target_device.output_type != NONE
-                and message != ""
-            ):
+            if target_device and target_device.output_type != NONE and message != "":
                 target_device.set_brightness(int(message))
             else:
                 _LOGGER.debug("Target device not found %s.", device_id)
         elif msg_type == COVER:
             cover = self._covers.get(device_id)
             if not cover:
                 return
@@ -724,15 +754,15 @@
                         "Positon cannot be set. Not number between 0-100. %s", message
                     )
         elif msg_type == "group" and command == "set":
             target_device = self._configured_output_groups.get(device_id)
             if target_device and target_device.output_type != NONE:
                 action_from_msg = relay_actions.get(message.upper())
                 if action_from_msg:
-                    getattr(target_device, action_from_msg)()
+                    asyncio.create_task(getattr(target_device, action_from_msg)())
                 else:
                     _LOGGER.debug("Action not exist %s.", message.upper())
             else:
                 _LOGGER.debug("Target device not found %s.", device_id)
         elif msg_type == BUTTON and command == "set":
             if device_id == "logger" and message == "reload":
                 _LOGGER.info("Reloading logger configuration.")
```

### Comparing `boneIO-0.7.1/boneio/modbus.py` & `boneIO-0.8.0.dev1/boneio/modbus.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,41 +67,18 @@
         """Connect client."""
         try:
             return self._client.connect()  # type: ignore[union-attr]
         except ModbusException as exception_error:
             _LOGGER.error(exception_error)
             return False
 
-    async def read_single_register(
-        self, unit: int, address: int, count: int = 2, method: str = "input"
-    ) -> float | None:
-        """Call sync. pymodbus."""
-        async with self._lock:
-            if not self._pymodbus_connect():
-                _LOGGER.error("Can't connect to Modbus address %s.", address)
-                return None
-            kwargs = {"unit": unit, "count": count} if unit else {}
-            try:
-                result: ReadInputRegistersResponse = self._read_methods[method](
-                    address, **kwargs
-                )
-            except ModbusException as exception_error:
-                _LOGGER.error(exception_error)
-                return None
-            if not hasattr(result, REGISTERS):
-                _LOGGER.error(str(result))
-                return None
-            return BinaryPayloadDecoder.fromRegisters(
-                result.registers, byteorder=Endian.Big, wordorder=Endian.Big
-            ).decode_32bit_float()
-
     async def read_multiple_registers(
         self, unit: int, address: int, count: int = 2, method: str = "input"
     ) -> ModbusResponse:
-        """Call sync. pymodbus."""
+        """Read single or multiple register(s)."""
         async with self._lock:
             if not self._pymodbus_connect():
                 _LOGGER.error("Can't connect to Modbus.")
                 return None
             kwargs = {"unit": unit, "count": count} if unit else {}
             try:
                 result: ReadInputRegistersResponse = self._read_methods[method](
@@ -110,7 +87,18 @@
             except ModbusException as exception_error:
                 _LOGGER.error(exception_error)
                 return None
             if not hasattr(result, REGISTERS):
                 _LOGGER.error(str(result))
                 return None
             return result
+
+    async def read_single_register(
+        self, unit: int, address: int, count: int = 2, method: str = "input"
+    ) -> float | None:
+        """Call sync. pymodbus."""
+        result = await self.read_multiple_registers(
+            unit=unit, address=address, count=count, method=method
+        )
+        return None if not result else BinaryPayloadDecoder.fromRegisters(
+            result.registers, byteorder=Endian.Big, wordorder=Endian.Big
+        ).decode_32bit_float()
```

### Comparing `boneIO-0.7.1/boneio/mqtt_client.py` & `boneIO-0.8.0.dev1/boneio/mqtt_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,18 @@
 
     async def stop_client(self) -> None:
         await self.unsubscribe(
             topics=self._topics
         )
         raise RestartRequestException("Restart requested.")
     
+    def state(self) -> bool:
+        """State of MQTT Client."""
+        return self._connection_established
+    
     async def _subscribe_manager(self, manager: Manager) -> None:
         """Connect and subscribe to manager topics + host stats."""
         async with AsyncExitStack() as stack:
             tasks: Set[asyncio.Task] = set()
 
             # Connect to the MQTT broker.
             await stack.enter_async_context(self.asyncio_client)
```

### Comparing `boneIO-0.7.1/boneio/oled.py` & `boneIO-0.8.0.dev1/boneio/oled.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,28 +18,36 @@
     make_font,
     setup_input,
 )
 from boneio.helper.events import async_track_point_in_time, utcnow
 
 _LOGGER = logging.getLogger(__name__)
 
+fonts = {
+    "big": make_font("DejaVuSans.ttf", 12),
+    "small": make_font("DejaVuSans.ttf", 9),
+    "extraSmall": make_font("DejaVuSans.ttf", 7),
+    "danube": make_font("danube__.ttf", 15, local=True)
 
-fontBig = make_font("DejaVuSans.ttf", 12)
-fontSmall = make_font("DejaVuSans.ttf", 9)
-fontExtraSmall = make_font("DejaVuSans.ttf", 7)
-danube = make_font("danube__.ttf", 15, local=True)
+}
 
 # screen_order = [UPTIME, NETWORK, CPU, DISK, MEMORY, SWAP]
 
 STANDARD_ROWS = [17, 32, 47]
 UPTIME_ROWS = list(range(22, 60, 10))
 OUTPUT_ROWS = list(range(14, 60, 6))
 OUTPUT_COLS = range(0, 113, 56)
 
 
+def shorten_name(name: str) -> str:
+    if len(name) > 6:
+        return f"{name[:4]}{name[-2:]}"
+    return name
+
+
 class Oled:
     """Oled display class."""
 
     def __init__(
         self,
         host_data: HostData,
         output_groups: List[str],
@@ -49,15 +57,15 @@
         """Initialize OLED screen."""
         self._loop = asyncio.get_running_loop()
         self._output_groups = None
         try:
             _ind_screen = screen_order.index("outputs")
             if not output_groups:
                 _LOGGER.debug("No outputs configured. Omitting in screen.")
-                screen_order.pop(_ind_screen)
+            screen_order.pop(_ind_screen)
             screen_order[_ind_screen:_ind_screen] = output_groups
             self._output_groups = output_groups
         except ValueError:
             pass
         self._screen_order = cycle(screen_order)
         self._current_screen = next(self._screen_order)
         self._host_data = host_data
@@ -71,56 +79,56 @@
             self._device = sh1106(serial)
         except DeviceNotFoundError as err:
             raise I2CError(err)
         _LOGGER.debug("Configuring OLED screen.")
 
     def _draw_standard(self, data: dict, draw: ImageDraw) -> None:
         """Draw standard information about host screen."""
-        draw.text((1, 1), self._current_screen, font=fontBig, fill=WHITE)
+        draw.text((1, 1), self._current_screen, font=fonts["big"], fill=WHITE)
         i = 0
         for k in data:
             draw.text(
                 (3, STANDARD_ROWS[i]),
                 f"{k} {data[k]}",
-                font=fontSmall,
+                font=fonts["small"],
                 fill=WHITE,
             )
             i += 1
 
     def _sleeptime(self):
         with canvas(self._device) as draw:
             draw.rectangle(self._device.bounding_box, outline="black", fill="black")
         self._sleep = True
 
     def _draw_uptime(self, data: dict, draw: ImageDraw) -> None:
         """Draw uptime screen with boneIO logo."""
-        draw.text((3, 3), "bone", font=danube, fill=WHITE)
-        draw.text((53, 3), "iO", font=danube, fill=WHITE)
-        i = 0
+        draw.text((3, 3), "bone", font=fonts["danube"], fill=WHITE)
+        draw.text((53, 3), "iO", font=fonts["danube"], fill=WHITE)
         for k in data:
+            text = data[k]["data"]
+            fontSize = fonts[data[k]["fontSize"]]
             draw.text(
-                (3, UPTIME_ROWS[i]),
-                f"{k}: {data[k]}",
-                font=fontSmall,
+                (data[k]["col"], UPTIME_ROWS[data[k]["row"]]),
+                f"{k}: {text}",
+                font=fontSize,
                 fill=WHITE,
             )
-            i += 1
 
     def _draw_output(self, data: dict, draw: ImageDraw) -> None:
         "Draw outputs of GPIO/MCP relays."
         cols = cycle(OUTPUT_COLS)
-        draw.text((1, 1), f"Relay {self._current_screen}", font=fontSmall, fill=WHITE)
+        draw.text((1, 1), f"Relay {self._current_screen}", font=fonts["small"], fill=WHITE)
         i = 0
         j = next(cols)
         for k in data:
             if len(OUTPUT_ROWS) == i:
                 j = next(cols)
                 i = 0
             draw.text(
-                (j, OUTPUT_ROWS[i]), f"{k} {data[k]}", font=fontExtraSmall, fill=WHITE
+                (j, OUTPUT_ROWS[i]), f"{shorten_name(k)} {data[k]}", font=fonts["extraSmall"], fill=WHITE
             )
             i += 1
 
     def render_display(self) -> None:
         """Render display."""
         data = self._host_data.get(self._current_screen)
         if data:
```

### Comparing `boneIO-0.7.1/boneio/relay/basic.py` & `boneIO-0.8.0.dev1/boneio/relay/basic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """Basic Relay module."""
-
+from __future__ import annotations
 import asyncio
+from concurrent.futures import ThreadPoolExecutor
 import logging
 from typing import Callable
 from boneio.helper.util import callback
 from boneio.const import COVER, LIGHT, NONE, OFF, ON, RELAY, STATE, SWITCH
 from boneio.helper import BasicMqtt
-from boneio.helper.events import EventBus
+from boneio.helper.events import EventBus, async_track_point_in_time, utcnow
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class BasicRelay(BasicMqtt):
     """Basic relay class."""
 
     def __init__(
         self,
         callback: Callable,
         id: str,
         event_bus: EventBus,
+        name: str | None = None,
         output_type=SWITCH,
         restored_state: bool = False,
         topic_type: str = RELAY,
         **kwargs,
     ) -> None:
         """Initialize Basic relay."""
         self._momentary_turn_on = kwargs.pop("momentary_turn_on", None)
         self._momentary_turn_off = kwargs.pop("momentary_turn_off", None)
-        super().__init__(id=id, name=id, topic_type=topic_type, **kwargs)
+        super().__init__(id=id, name=name or id, topic_type=topic_type, **kwargs)
         self._output_type = output_type
         self._event_bus = event_bus
         if output_type == COVER:
             self._momentary_turn_on = None
             self._momentary_turn_off = None
         self._state = ON if restored_state else OFF
         self._callback = callback
+        self._momentary_action = None
         self._loop = asyncio.get_running_loop()
+        self.executor = ThreadPoolExecutor()
 
     @property
     def is_mcp_type(self) -> bool:
         """Check if relay is mcp type."""
         return False
 
     @property
@@ -63,53 +67,73 @@
         """Not trimmed id."""
         return self._name or self._pin
 
     @property
     def state(self) -> str:
         """Is relay active."""
         return self._state
-    
+
     def payload(self) -> dict:
         return {STATE: self.state}
 
-    def send_state(self) -> None:
+    def send_state(self, optimized_value: bool | None = None) -> None:
         """Send state to Mqtt on action."""
-        state = ON if self.is_active else OFF
+        if optimized_value:
+            state = optimized_value
+        else:
+            state = ON if self.is_active else OFF
         self._state = state
         if self.output_type not in (NONE, COVER):
             self._send_message(
                 topic=self._send_topic, payload=self.payload(), retain=True
             )
         self._event_bus.trigger_output_event(self.id)
         self._loop.call_soon_threadsafe(self._callback)
 
-    def toggle(self) -> None:
-        """Toggle relay."""
-        _LOGGER.debug("Toggle relay.")
-        if self.is_active:
-            self.turn_off()
-        else:
-            self.turn_on()
-
     @callback
     def _momentary_callback(self, time, action):
         _LOGGER.info("Momentary callback at %s", time)
         action()
 
     @property
     def is_active(self) -> bool:
         """Is active check."""
         raise NotImplementedError
-    
+
     async def async_turn_on(self) -> None:
-        self._loop.call_soon(self.turn_on)
+        self.turn_on()
 
     async def async_turn_off(self) -> None:
-        self._loop.call_soon(self.turn_off)
+        self.turn_off()
+
+    async def async_toggle(self) -> None:
+        """Toggle relay."""
+        _LOGGER.debug("Toggle relay %s.", self.name)
+        if self.is_active:
+            await self.async_turn_off()
+        else:
+            await self.async_turn_on()
 
     def turn_on(self) -> None:
         """Call turn on action."""
         raise NotImplementedError
-
+    
     def turn_off(self) -> None:
         """Call turn off action."""
         raise NotImplementedError
+
+    def _execute_momentary_turn(self, momentary_type: str) -> None:
+        """Execute momentary action."""
+        if self._momentary_action:
+            self._momentary_action()
+        (action, time) = (
+            (self.turn_on, self._momentary_turn_on)
+            if momentary_type == ON
+            else (self.turn_off, self._momentary_turn_off)
+        )
+        if time:
+            _LOGGER.debug("Applying momentary action for %s in %s", self.name, time.as_timedelta)
+            self._momentary_action = async_track_point_in_time(
+                loop=self._loop,
+                action=lambda x: self._momentary_callback(time=x, action=action),
+                point_in_time=utcnow() + time.as_timedelta,
+            )
```

### Comparing `boneIO-0.7.1/boneio/relay/gpio.py` & `boneIO-0.8.0.dev1/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/relay/mcp.py` & `boneIO-0.8.0.dev1/boneio/relay/pcf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,78 @@
-"""MCP23017 Relay module."""
+"""PCF8575 Relay module."""
 
 import logging
 
-from adafruit_mcp230xx.mcp23017 import MCP23017, DigitalInOut
+from adafruit_pcf8575 import DigitalInOut
 
-from boneio.const import SWITCH, MCP, COVER
+from boneio.const import NONE, SWITCH, PCF, ON, OFF
 from boneio.helper.events import async_track_point_in_time, utcnow
+from boneio.helper.pcf8575 import PCF8575
 from boneio.relay.basic import BasicRelay
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class MCPRelay(BasicRelay):
-    """Represents MCP Relay output"""
+class PCFRelay(BasicRelay):
+    """Represents PCF Relay output"""
 
     def __init__(
         self,
         pin: int,
-        mcp: MCP23017,
-        mcp_id: str,
+        expander: PCF8575,
+        expander_id: str,
         output_type: str = SWITCH,
         restored_state: bool = False,
-        **kwargs
+        **kwargs,
     ) -> None:
         """Initialize MCP relay."""
-        self._pin: DigitalInOut = mcp.get_pin(pin)
-        if output_type == COVER:
+        self._pin: DigitalInOut = expander.get_pin(pin)
+        if output_type == NONE:
             """Just in case to not restore state of covers etc."""
             restored_state = False
         self._pin.switch_to_output(value=restored_state)
         super().__init__(
             **kwargs, output_type=output_type, restored_state=restored_state
         )
         self._pin_id = pin
-        self._expander_id = mcp_id
-        _LOGGER.debug("Setup MCP with pin %s", self._pin_id)
+        self._expander_id = expander_id
+        self._active_state = False
+        _LOGGER.debug("Setup PCF with pin %s", self._pin_id)
 
     @property
     def expander_type(self) -> str:
         """Check expander type."""
-        return MCP
+        return PCF
 
     @property
     def pin_id(self) -> int:
         """Return PIN id."""
         return self._pin_id
 
     @property
     def expander_id(self) -> str:
         """Retrieve parent MCP ID."""
         return self._expander_id
 
     @property
     def is_active(self) -> bool:
         """Is relay active."""
-        return self.pin.value
+        return self.pin.value == self._active_state
 
     @property
     def pin(self) -> str:
         """PIN of the relay"""
         return self._pin
 
     def turn_on(self) -> None:
         """Call turn on action."""
-        self.pin.value = True
-        if self._momentary_turn_on:
-            async_track_point_in_time(
-                loop=self._loop,
-                action=lambda x: self._momentary_callback(time=x, action=self.turn_off),
-                point_in_time=utcnow() + self._momentary_turn_on.as_timedelta,
-            )
+        self.pin.value = self._active_state
+        self._execute_momentary_turn(momentary_type=ON)
         self._loop.call_soon_threadsafe(self.send_state)
+        self._loop.call_soon_threadsafe(self._callback)
 
     def turn_off(self) -> None:
         """Call turn off action."""
-        self.pin.value = False
-        if self._momentary_turn_off:
-            async_track_point_in_time(
-                loop=self._loop,
-                action=lambda x: self._momentary_callback(time=x, action=self.turn_on),
-                point_in_time=utcnow() + self._momentary_turn_off.as_timedelta,
-            )
+        self.pin.value = not self._active_state
+        self._execute_momentary_turn(momentary_type=OFF)
         self._loop.call_soon_threadsafe(self.send_state)
+        self._loop.call_soon_threadsafe(self._callback)
```

### Comparing `boneIO-0.7.1/boneio/relay/pca.py` & `boneIO-0.8.0.dev1/boneio/relay/pca.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,98 +1,53 @@
 """PCA9685 PWM module."""
 
 from __future__ import annotations
-import asyncio
 import logging
-from typing import Callable
 from adafruit_pca9685 import PCA9685, PCAChannels
 
-from boneio.helper.events import async_track_point_in_time, utcnow
-from boneio.helper.util import callback
-
-from boneio.const import LED, NONE, OFF, ON, STATE, SWITCH, BRIGHTNESS, RELAY, PCA
-from boneio.helper import BasicMqtt
+from boneio.const import LED, OFF, ON, STATE, SWITCH, BRIGHTNESS, PCA
+from boneio.relay.basic import BasicRelay
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class PWMPCA(BasicMqtt):
+class PWMPCA(BasicRelay):
     """Initialize PWMPCA."""
 
     def __init__(
         self,
         pin: int,
         pca: PCA9685,
         percentage_default_brightness: int,
-        callback: Callable,
-        id: str | None = None,
         output_type=SWITCH,
         restored_state: bool = False,
         restored_brightness: int = 0,
         **kwargs,
     ) -> None:
         """Initialize PWMPCA."""
         self._pin: PCAChannels = pca.channels[pin]
-
-        self._momentary_turn_on = kwargs.pop("momentary_turn_on", None)
-        self._momentary_turn_off = kwargs.pop("momentary_turn_off", None)
-        super().__init__(id=id, name=id, topic_type=RELAY, **kwargs)
-
-        self._output_type = output_type
+        super().__init__(
+            **kwargs, output_type=output_type, restored_state=restored_state
+        )
         self._percentage_default_brightness = percentage_default_brightness
-
-        if output_type == NONE:
-            self._momentary_turn_on = None
-            self._momentary_turn_off = None
-
-        if restored_state:
-            self._state = ON
-            self._brightness = restored_brightness
-        else:
-            self._state = OFF
-            self._brightness = 0
-
-        self._callback = callback
-        self._loop = asyncio.get_running_loop()
-
+        self._brightness = restored_brightness if restored_state else 0
         self._pin_id = pin
         _LOGGER.debug("Setup PCA with pin %s", self._pin_id)
 
     @property
     def expander_type(self) -> str:
         """Check expander type."""
         return PCA
 
     @property
-    def output_type(self) -> str:
-        """HA type."""
-        return self._output_type
-
-    @property
     def is_led(self) -> bool:
         """Check if HA type is light"""
         return self._output_type == LED
 
     @property
-    def id(self) -> str:
-        """Id of the relay.
-        Has to be trimmed out of spaces because of MQTT handling in HA."""
-        return self._id
-
-    @property
-    def name(self) -> str:
-        """Not trimmed name."""
-        return self._name
-
-    @property
-    def state(self) -> str:
-        """Is relay active."""
-        return self._state
-
-    @property
     def brightness(self) -> int:
         """Get brightness in 0-65535 scale. PCA can force over 65535 value after restart, so we treat that as a 0"""
         try:
             if self._pin.duty_cycle > 65535:
                 return 0
             return self._pin.duty_cycle
         except:
@@ -113,35 +68,21 @@
         return self.brightness > 1
 
     def turn_on(self) -> None:
         """Call turn on action. When brightness is 0, and turn on by switch, default set value to 1%"""
         _LOGGER.debug("Turn on relay.")
         if self.brightness == 0:
             self.set_brightness(int(65535 / 100 * self._percentage_default_brightness))
-
-        if self._momentary_turn_on:
-            async_track_point_in_time(
-                loop=self._loop,
-                action=lambda x: self._momentary_callback(time=x, action=self.turn_off),
-                point_in_time=utcnow() + self._momentary_turn_on.as_timedelta,
-            )
+        self._execute_momentary_turn(momentary_type=ON)
         self._loop.call_soon_threadsafe(self.send_state)
+        self._loop.call_soon_threadsafe(self._callback)
 
     def turn_off(self) -> None:
         """Call turn off action."""
         _LOGGER.debug("Turn off relay.")
         self._pin.duty_cycle = 0
-        if self._momentary_turn_off:
-            async_track_point_in_time(
-                loop=self._loop,
-                action=lambda x: self._momentary_callback(time=x, action=self.turn_on),
-                point_in_time=utcnow() + self._momentary_turn_off.as_timedelta,
-            )
+        self._execute_momentary_turn(momentary_type=OFF)
         self._loop.call_soon_threadsafe(self.send_state)
-
-    @callback
-    def _momentary_callback(self, time, action):
-        _LOGGER.info("Momentary callback at %s", time)
-        action()
+        self._loop.call_soon_threadsafe(self._callback)
 
     def payload(self) -> dict:
         return {BRIGHTNESS: self.brightness, STATE: self.state}
```

### Comparing `boneIO-0.7.1/boneio/runner.py` & `boneIO-0.8.0.dev1/boneio/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     COVER,
     DALLAS,
     DS2482,
     ENABLED,
     EVENT_ENTITY,
     HA_DISCOVERY,
     HOST,
+    INA219,
     LM75,
     MCP23017,
     MCP_TEMP_9808,
     MODBUS,
     MQTT,
     OLED,
     ONEWIRE,
@@ -75,31 +76,34 @@
         config_helper=_config_helper,
     )
     manager_kwargs = {
         item["name"]: config.get(item["name"], item["default"])
         for item in config_modules
     }
 
+
     manager = Manager(
         send_message=client.send_message,
         stop_client=client.stop_client,
+        mqtt_state=client.state,
         relay_pins=config.get(OUTPUT, []),
         event_pins=config.get(EVENT_ENTITY, []),
         binary_pins=config.get(BINARY_SENSOR, []),
         config_file_path=config_file,
         state_manager=StateManager(
             state_file=f"{os.path.split(config_file)[0]}state.json"
         ),
         config_helper=_config_helper,
         sensors={
             LM75: config.get(LM75, []),
+            INA219: config.get(INA219, []),
             MCP_TEMP_9808: config.get(MCP_TEMP_9808, []),
             MODBUS: config.get("modbus_sensors"),
             ONEWIRE: config.get(SENSOR, []),
         },
         **manager_kwargs,
     )
     tasks = set()
     tasks.update(manager.get_tasks())
     _LOGGER.info("Connecting to MQTT.")
     tasks.add(client.start_client(manager))
-    return await asyncio.gather(*tasks, return_exceptions=True)
+    return await asyncio.gather(*tasks)
```

### Comparing `boneIO-0.7.1/boneio/schema/actions.yaml` & `boneIO-0.8.0.dev1/boneio/schema/actions.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/schema/schema.yaml` & `boneIO-0.8.0.dev1/boneio/schema/schema.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -51,41 +51,50 @@
 logger:
   type: dict
   required: False
   schema:
     default:
       type: string
       required: False
-      allowed: ["critical", "error", "warning", "info", "debug"]
+      allowed: ['critical', 'error', 'warning', 'info', 'debug']
       meta:
         label: Module which you want logger to set. Default for app logger.
     logs:
       type: dict
       meta:
         label: List of dict module\:level.
 
-
-
 oled:
   type: dict
   default: {}
   required: True
   schema:
     enabled:
       type: boolean
       default: False
       meta:
         label: Disable builtin screen.
     screens:
       type: list
       required: True
-      allowed: ["uptime", "network", "cpu", "disk", "memory", "swap", "outputs"]
+      allowed:
+        [
+          'uptime',
+          'network',
+          'ina219',
+          'cpu',
+          'disk',
+          'memory',
+          'swap',
+          'outputs',
+        ]
       default:
         - uptime
         - network
+        - ina219
         - cpu
         - disk
         - memory
         - swap
         - outputs
     screensaver_timeout:
       type:
@@ -101,15 +110,15 @@
 modbus:
   type: dict
   required: False
   schema:
     uart:
       type: string
       required: True
-      allowed: ["uart1", "uart2", "uart3", "uart4", "uart5"]
+      allowed: ['uart1', 'uart2', 'uart3', 'uart4', 'uart5']
       meta:
         label: Uart ID to use
 
 modbus_sensors:
   type: list
   required: False
   meta:
@@ -128,15 +137,15 @@
           - integer
         required: True
         meta:
           label: Address of Modbus sensor to use.
       model:
         type: string
         required: True
-        allowed: ["sdm630", "sdm120", "sofar"]
+        allowed: ['sdm630', 'sdm120', 'sofar']
         meta:
           label: Model to load from database.
       update_interval:
         type:
           - string
           - timeperiod
         coerce:
@@ -164,14 +173,52 @@
         default: 0x48
         meta:
           label: Address of I2C
       update_interval: !include update_interval.yaml
       filters: !include filters.yaml
       unit_of_measurement: !include temp_unit.yaml
 
+ina219:
+  type: list
+  required: False
+  meta:
+    label: INA219 Sensor list.
+  schema:
+    type: dict
+    required: False
+    schema:
+      id: !include id.yaml
+      address:
+        type:
+          - string
+          - integer
+        required: True
+        default: 0x40
+        meta:
+          label: Address of I2C
+      sensors:
+        type: list
+        required: True
+        schema:
+          type: dict
+          required: False
+          schema:
+            id: !include id.yaml
+            device_class:
+              type: string
+              allowed: ['current', 'power', 'voltage']
+            filters: !include filters.yaml
+        default:
+          - id: INA219 Current
+            device_class: current
+          - id: INA219 Power
+            device_class: power
+          - id: INA219 Voltage
+            device_class: voltage
+      update_interval: !include update_interval.yaml
 
 mcp9808:
   type: list
   required: False
   meta:
     label: MCP9808 Sensor list.
   schema:
@@ -186,15 +233,14 @@
         required: True
         default: 0x18
         meta:
           label: Address of I2C device
       update_interval: !include update_interval.yaml
       filters: !include filters.yaml
       unit_of_measurement: !include temp_unit.yaml
-      
 
 mcp23017:
   type: list
   required: False
   meta:
     label: mcp23017 Pin config
   schema:
@@ -214,15 +260,14 @@
           - str
           - positive_time_period
         required: True
         default: 0s
         meta:
           label: How long to sleep for MCP to initialize.
 
-
 pcf8575:
   type: list
   required: False
   meta:
     label: pcf8575 Pin config
   schema:
     type: dict
@@ -283,15 +328,15 @@
         type: string
         required: False
         coerce: str
         meta:
           label: Id to send to use in HA and in GPIO Input. Default to `kind_pin`
       kind:
         type: string
-        allowed: ["gpio", "mcp", "pca", "pcf"]
+        allowed: ['gpio', 'mcp', 'pca', 'pcf']
         meta:
           label: Either GPIO or i2c.
       mcp_id:
         type: string
         required: False
         meta:
           label: MCP ID to connect
@@ -343,21 +388,20 @@
         required: False
         default: 1
         meta:
           label: When the brightness is not set in ha, and we switch led to turn this value will be used
       output_type:
         type: string
         required: True
-        allowed: ["switch", "light", "cover", "none"]
-        default: "switch"
+        allowed: ['switch', 'light', 'cover', 'none']
+        default: 'switch'
         coerce: lower
         meta:
           label: If HA discovery is used device if relay is light or switch. Cover if this output will be used for cover. If None is declared then any state is not published to MQTT (used for cover).
 
-
 output_group:
   type: list
   meta:
     label: List of groupes outputs
   check_with: output_id_uniqueness
   schema:
     type: dict
@@ -372,21 +416,20 @@
         type: list
         required: True
         meta:
           label: List of outputs.
       output_type:
         type: string
         required: True
-        allowed: ["switch", "light"]
-        default: "switch"
+        allowed: ['switch', 'light']
+        default: 'switch'
         coerce: lower
         meta:
           label: If HA discovery is used device if relay is light or switch.
 
-
 binary_sensor:
   type: list
   meta:
     label: GPIO inputs section
   schema:
     type: dict
     schema:
@@ -399,23 +442,23 @@
         type: string
         required: True
         meta:
           label: PIN to use.
       gpio_mode:
         type: string
         required: True
-        default: "gpio"
-        allowed: ["gpio", "gpio_pu", "gpio_pd", "gpio_input"]
+        default: 'gpio'
+        allowed: ['gpio', 'gpio_pu', 'gpio_pd', 'gpio_input']
         meta:
           label: What mode to use in config PIN.
       detection_type:
         type: string
         required: True
-        default: "new"
-        allowed: ["new", "old"]
+        default: 'new'
+        allowed: ['new', 'old']
         meta:
           label: There are 2 detector algorithms. Old consumes more CPU but it is tested by many users. New is more optimized, but needed extra time for testing.
       clear_message:
         type: boolean
         default: False
         meta:
           label: Decide if after press/release callback send empty message to mqtt. Same as Zigbee2Mqtt is doing in button actions.
@@ -423,15 +466,15 @@
         type:
           - string
           - timeperiod
         coerce:
           - str
           - positive_time_period
         required: True
-        default: "120ms"
+        default: '120ms'
         meta:
           label: Bounce time for GPIO in miliseconds. Only for advanced usage.
       show_in_ha:
         type: boolean
         required: True
         default: True
         meta:
@@ -441,26 +484,54 @@
         default: False
         required: True
         meta:
           label: Check if sensor type is inverted. Only aplicable for sensor kind.
       device_class:
         type: string
         required: False
-        allowed: ["battery", "battery_charging", "carbon_monoxide", "cold", "connectivity", "door", "garage_door", "gas", "heat", "light", "lock", "moisture", "motion", "moving", "occupancy", "opening", "plug", "power", "presence", "problem", "running", "safety", "smoke", "sound", "tamper", "vibration", "window"]
+        allowed:
+          [
+            'battery',
+            'battery_charging',
+            'carbon_monoxide',
+            'cold',
+            'connectivity',
+            'door',
+            'garage_door',
+            'gas',
+            'heat',
+            'light',
+            'lock',
+            'moisture',
+            'motion',
+            'moving',
+            'occupancy',
+            'opening',
+            'plug',
+            'power',
+            'presence',
+            'problem',
+            'running',
+            'safety',
+            'smoke',
+            'sound',
+            'tamper',
+            'vibration',
+            'window',
+          ]
         meta:
           label: Device class to use in HA
       actions:
         required: False
         type: dict
         coerce: check_actions
         schema:
           pressed: !include actions_sensor.yaml
           released: !include actions_sensor.yaml
 
-
 event:
   type: list
   meta:
     label: GPIO inputs section
   schema:
     type: dict
     schema:
@@ -473,23 +544,23 @@
         type: string
         required: True
         meta:
           label: PIN to use.
       gpio_mode:
         type: string
         required: True
-        default: "gpio"
-        allowed: ["gpio", "gpio_pu", "gpio_pd", "gpio_input"]
+        default: 'gpio'
+        allowed: ['gpio', 'gpio_pu', 'gpio_pd', 'gpio_input']
         meta:
           label: What mode to use in config PIN.
       detection_type:
         type: string
         required: True
-        default: "new"
-        allowed: ["new", "old"]
+        default: 'new'
+        allowed: ['new', 'old']
         meta:
           label: There are 2 detector algorithms. Old consumes more CPU but it is tested by many users. New is more optimized, but needed extra time for testing.
       clear_message:
         type: boolean
         default: False
         meta:
           label: Decide if after press/release callback send empty message to mqtt. Same as Zigbee2Mqtt is doing in button actions.
@@ -497,15 +568,15 @@
         type:
           - string
           - timeperiod
         coerce:
           - str
           - positive_time_period
         required: True
-        default: "120ms"
+        default: '30ms'
         meta:
           label: Bounce time for GPIO in miliseconds. Only for advanced usage.
       show_in_ha:
         type: boolean
         required: True
         default: True
         meta:
@@ -515,16 +586,16 @@
         default: False
         required: True
         meta:
           label: Check if sensor type is inverted. Only aplicable for sensor kind.
       device_class:
         type: string
         required: False
-        default: "button"
-        allowed: ["button", "doorbell", "motion"]
+        default: 'button'
+        allowed: ['button', 'doorbell', 'motion']
         meta:
           label: Device class to use in HA
       actions:
         required: False
         type: dict
         coerce: check_actions
         schema:
@@ -542,15 +613,15 @@
         type: string
         required: False
         meta:
           label: Id to use in HA if needed. Default to pin number.
       pin:
         type: string
         required: True
-        allowed: ["P9_33", "P9_35", "P9_36", "P9_37", "P9_38", "P9_39", "P9_40"]
+        allowed: ['P9_33', 'P9_35', 'P9_36', 'P9_37', 'P9_38', 'P9_39', 'P9_40']
         meta:
           label: PIN to use.
       update_interval: !include update_interval.yaml
       show_in_ha:
         type: boolean
         required: True
         default: True
@@ -605,15 +676,27 @@
           - positive_time_period
         required: True
         meta:
           label: Time to close cover. Example 30s. Minimum is 1s.
       device_class:
         type: string
         required: False
-        allowed: ["awning", "blind", "curtain", "damper", "door", "garage", "gate", "shade", "shutter", "window"]
+        allowed:
+          [
+            'awning',
+            'blind',
+            'curtain',
+            'damper',
+            'door',
+            'garage',
+            'gate',
+            'shade',
+            'shutter',
+            'window',
+          ]
         meta:
           label: Device class to use in HA
       show_in_ha:
         type: boolean
         required: True
         default: True
         meta:
@@ -659,15 +742,15 @@
         required: False
         meta:
           label: Id to use in HA if needed. Default to address.
       platform:
         type: string
         required: True
         default: dallas
-        allowed: ["dallas"]
+        allowed: ['dallas']
         meta:
           label: Platform of sensor to use. Currently only Dallas platform is supported.
       address:
         type: integer
         required: True
         meta:
           label: Address of Dallas device
```

### Comparing `boneIO-0.7.1/boneio/sensor/adc.py` & `boneIO-0.8.0.dev1/boneio/sensor/adc.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/gpio.py` & `boneIO-0.8.0.dev1/boneio/sensor/gpio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """GpioInputBinarySensor to receive signals."""
 import logging
-from functools import partial
 import asyncio
 from boneio.const import PRESSED, RELEASED
 from boneio.helper import GpioBaseClass
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -22,18 +21,16 @@
         )
         _LOGGER.debug("Configured sensor pin %s", self._pin)
         asyncio.create_task(self._run())
 
     async def _run(self) -> None:
         while True:
             self.check_state(state=self.is_pressed)
-            await asyncio.sleep(self._bounce_time.total_in_seconds)
+            await asyncio.sleep(self._bounce_time)
 
     def check_state(self, state: bool) -> None:
         if state == self._state:
             return
         self._state = state
         click_type = self._click_type[0] if state else self._click_type[1]
         _LOGGER.debug("%s event on pin %s", click_type, self._pin)
-        self._loop.call_soon_threadsafe(
-            partial(self._press_callback, click_type, self._pin)
-        )
+        self.press_callback(click_type=click_type, duration=None)
```

### Comparing `boneIO-0.7.1/boneio/sensor/gpio_new.py` & `boneIO-0.8.0.dev1/boneio/sensor/gpio_new.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """GpioInputBinarySensorNew to receive signals."""
 import logging
-from functools import partial
 from boneio.const import PRESSED, RELEASED, BOTH
 from boneio.helper import GpioBaseClass
 from boneio.helper.gpio import add_event_callback, add_event_detect
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -20,17 +19,15 @@
             if kwargs.get("inverted", False)
             else (PRESSED, RELEASED)
         )
         _LOGGER.debug("Configured sensor pin %s", self._pin)
         add_event_detect(pin=self._pin, edge=BOTH)
         add_event_callback(pin=self._pin, callback=self.check_state)
 
-    def check_state(self, channel) -> None:
+    def check_state(self, _) -> None:
         state = self.is_pressed
         if state == self._state:
             return
         self._state = state
         click_type = self._click_type[0] if state else self._click_type[1]
-        _LOGGER.debug("%s event on pin %s", click_type, self._pin)
-        self._loop.call_soon_threadsafe(
-            partial(self._press_callback, click_type, self._pin)
-        )
+        _LOGGER.debug("%s event on pin %s - %s", click_type, self._pin, self.name)
+        self.press_callback(click_type=click_type, duration=None)
```

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/__init__.py` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,18 @@
                 )
                 if register is not None:
                     self._discovery_sent = self._send_discovery_for_all_registers(
                         register
                     )
                     await asyncio.sleep(2)
                     break
-            _LOGGER.error(
-                "Discovery for %s not sent. First register not available.", self._id
-            )
+            if not self._discovery_sent:
+                _LOGGER.error(
+                    "Discovery for %s not sent. First register not available.", self._id
+                )
 
     async def async_update(self, time: datetime) -> None:
         """Fetch state periodically and send to MQTT."""
         update_interval = self._update_interval.total_in_seconds
         await self.check_availability()
         for data in self._db[REGISTERS_BASE]:
             values = await self._modbus.read_multiple_registers(
```

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/pt100.json` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/sdm120.json` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/sdm630.json` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/modbus/sofar.json` & `boneIO-0.8.0.dev1/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/temp/__init__.py` & `boneIO-0.8.0.dev1/boneio/sensor/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/boneio/sensor/temp/dallas.py` & `boneIO-0.8.0.dev1/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/pyproject.toml` & `boneIO-0.8.0.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "psutil>=5.9.5",
     "adafruit-circuitpython-onewire>=2.0.5",
     "w1thermsensor[async]>=2.0.0",
     "adafruit-circuitpython-pca9685>=3.4.10",
     "adafruit-circuitpython-pcf8575>=1.0.2",
 ]
 requires-python = ">=3.7"
-version = "0.7.1"
+version = "0.8.0.dev1"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
```

### Comparing `boneIO-0.7.1/tests/relay_32_5.py` & `boneIO-0.8.0.dev1/tests/relay_32_5.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.1/PKG-INFO` & `boneIO-0.8.0.dev1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boneIO
-Version: 0.7.1
+Version: 0.8.0.dev1
 Summary: Python App for BoneIO
 License: GNU General Public License v3.0
 Author-email: Paweł Szafer <pszafer@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Changelog, https://github.com/boneIO-eu/app_bbb/releases
 Project-URL: Documentation, https://boneio.eu/docs/intro/
 Project-URL: Homepage, https://boneio.eu
```

