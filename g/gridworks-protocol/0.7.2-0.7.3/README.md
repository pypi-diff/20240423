# Comparing `tmp/gridworks_protocol-0.7.2.tar.gz` & `tmp/gridworks_protocol-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.7.2.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.7.3.tar", max compression
```

## Comparing `gridworks_protocol-0.7.2.tar` & `gridworks_protocol-0.7.3.tar`

### file list

```diff
@@ -1,110 +1,115 @@
--rw-r--r--   0        0        0     1070 2024-04-01 16:03:09.123299 gridworks_protocol-0.7.2/LICENSE
--rw-r--r--   0        0        0     3087 2024-04-01 16:03:09.123299 gridworks_protocol-0.7.2/README.md
--rw-r--r--   0        0        0     2291 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2030 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/__init__.py
--rw-r--r--   0        0        0     1340 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0      143 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/fibaro_smart_implant_cac.py
--rw-r--r--   0        0        0      132 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/hubitat_cac.py
--rw-r--r--   0        0        0      138 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/hubitat_poller_cac.py
--rw-r--r--   0        0        0      142 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/hubitat_tank_module_cac.py
--rw-r--r--   0        0        0     1489 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      996 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1113 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/relay_cac.py
--rw-r--r--   0        0        0     1119 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0      135 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/rest_poller_cac.py
--rw-r--r--   0        0        0     1581 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1095 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1660 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0      533 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/fibaro_smart_implant_component.py
--rw-r--r--   0        0        0      769 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_component.py
--rw-r--r--   0        0        0     3141 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_poller_component.py
--rw-r--r--   0        0        0     3701 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_tank_component.py
--rw-r--r--   0        0        0     1480 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1482 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1268 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/relay_component.py
--rw-r--r--   0        0        0     1466 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0      674 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/rest_poller_component.py
--rw-r--r--   0        0        0     1309 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    19818 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0      377 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/resolver.py
--rw-r--r--   0        0        0     2401 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    14860 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/decoders.py
--rw-r--r--   0        0        0     3498 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/default_decoders.py
--rw-r--r--   0        0        0     3167 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     8424 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     4686 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0    10910 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     8099 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     7060 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     4742 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0      336 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      460 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      442 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0    11428 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/topic.py
--rw-r--r--   0        0        0     1051 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/type_helpers/__init__.py
--rw-r--r--   0        0        0     8903 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     9990 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0    10683 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0     9168 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     7734 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     8183 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    13383 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    18082 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     2670 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_cac_gt.py
--rw-r--r--   0        0        0     2959 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_component_gt.py
--rw-r--r--   0        0        0    12880 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0    10676 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     9579 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     9646 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     9258 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    11997 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11090 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    15695 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    11589 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8430 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0    12904 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0     2281 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_cac_gt.py
--rw-r--r--   0        0        0     4802 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_component_gt.py
--rw-r--r--   0        0        0     2129 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_gt.py
--rw-r--r--   0        0        0     1328 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_cac_gt.py
--rw-r--r--   0        0        0     1573 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_component_gt.py
--rw-r--r--   0        0        0     1554 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_gt.py
--rw-r--r--   0        0        0     2469 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_cac_gt.py
--rw-r--r--   0        0        0     3017 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_component_gt.py
--rw-r--r--   0        0        0     8759 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_gt.py
--rw-r--r--   0        0        0    13945 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0    13879 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    10163 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0    12226 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     5915 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0     9932 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/relay_cac_gt.py
--rw-r--r--   0        0        0    11585 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/relay_component_gt.py
--rw-r--r--   0        0        0    11465 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0    11819 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0     2364 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_cac_gt.py
--rw-r--r--   0        0        0     3033 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_component_gt.py
--rw-r--r--   0        0        0     8900 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_gt.py
--rw-r--r--   0        0        0    12488 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0    11394 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     9456 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    14590 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    12356 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/ta_data_channels.py
--rw-r--r--   0        0        0    11281 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    11369 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2890 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/utils.py
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 gridworks_protocol-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-22 22:52:43.432922 gridworks_protocol-0.7.3/LICENSE
+-rw-r--r--   0        0        0     3087 2024-04-22 22:52:43.432922 gridworks_protocol-0.7.3/README.md
+-rw-r--r--   0        0        0     2291 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2030 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     1340 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0      143 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/fibaro_smart_implant_cac.py
+-rw-r--r--   0        0        0      132 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/hubitat_cac.py
+-rw-r--r--   0        0        0      138 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/hubitat_poller_cac.py
+-rw-r--r--   0        0        0      142 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/hubitat_tank_module_cac.py
+-rw-r--r--   0        0        0     1489 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      996 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1113 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1119 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0      135 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/rest_poller_cac.py
+-rw-r--r--   0        0        0     1581 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0      134 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/web_server_cac.py
+-rw-r--r--   0        0        0     1388 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1095 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1660 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0      533 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/fibaro_smart_implant_component.py
+-rw-r--r--   0        0        0      962 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_component.py
+-rw-r--r--   0        0        0     3575 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_poller_component.py
+-rw-r--r--   0        0        0     4189 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_tank_component.py
+-rw-r--r--   0        0        0     1480 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1482 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1268 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1466 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0      674 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/rest_poller_component.py
+-rw-r--r--   0        0        0     1309 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      687 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/web_server_component.py
+-rw-r--r--   0        0        0      165 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    21391 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0      377 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/resolver.py
+-rw-r--r--   0        0        0     2401 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    14860 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/decoders.py
+-rw-r--r--   0        0        0     3690 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/default_decoders.py
+-rw-r--r--   0        0        0     3167 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     8935 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     4686 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0    10910 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     8099 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     7274 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     4910 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0      336 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      442 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3237 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0    11428 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/topic.py
+-rw-r--r--   0        0        0     1051 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/type_helpers/__init__.py
+-rw-r--r--   0        0        0     8974 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     9990 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0    10683 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0     9168 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     7734 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     8183 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    13383 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    18082 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     2670 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_cac_gt.py
+-rw-r--r--   0        0        0     2959 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_component_gt.py
+-rw-r--r--   0        0        0    12880 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    10676 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     9579 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     9646 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     9258 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    11997 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11090 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    15695 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    11589 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8430 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0    12904 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0     2281 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_cac_gt.py
+-rw-r--r--   0        0        0     4772 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_component_gt.py
+-rw-r--r--   0        0        0     2555 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_gt.py
+-rw-r--r--   0        0        0     1328 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_cac_gt.py
+-rw-r--r--   0        0        0     1573 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_component_gt.py
+-rw-r--r--   0        0        0     1697 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_gt.py
+-rw-r--r--   0        0        0     2469 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_cac_gt.py
+-rw-r--r--   0        0        0     3017 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_component_gt.py
+-rw-r--r--   0        0        0     8831 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_gt.py
+-rw-r--r--   0        0        0    13945 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0    13879 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    10163 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0    12226 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     5915 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0     9932 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0    11585 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11465 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0    11819 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0     2364 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_cac_gt.py
+-rw-r--r--   0        0        0     3033 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_component_gt.py
+-rw-r--r--   0        0        0     8900 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_gt.py
+-rw-r--r--   0        0        0    12488 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0    11394 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     9456 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    14590 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    12356 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/ta_data_channels.py
+-rw-r--r--   0        0        0    11281 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    11369 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     1140 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/web_server_cac_gt.py
+-rw-r--r--   0        0        0     1463 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/web_server_component_gt.py
+-rw-r--r--   0        0        0      440 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/web_server_gt.py
+-rw-r--r--   0        0        0     2890 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/utils.py
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 gridworks_protocol-0.7.3/PKG-INFO
```

### Comparing `gridworks_protocol-0.7.2/LICENSE` & `gridworks_protocol-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/README.md` & `gridworks_protocol-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/pyproject.toml` & `gridworks_protocol-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.7.2"
+version = "0.7.3"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/__init__.py` & `gridworks_protocol-0.7.3/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/relay_cac.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/fibaro_smart_implant_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/fibaro_smart_implant_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_component.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 
 from gwproto.data_classes.component import Component
 from gwproto.types.hubitat_gt import HubitatGt
 
 
 class HubitatComponent(Component):
     hubitat_gt: HubitatGt
+    web_listener_nodes: set[str]
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
         hubitat_gt: HubitatGt,
         display_name: Optional[str] = None,
         hw_uid: Optional[str] = None,
     ):
         self.hubitat_gt = hubitat_gt
+        self.web_listener_nodes = set()
         super().__init__(
             component_id=component_id,
             component_attribute_class_id=component_attribute_class_id,
             display_name=display_name,
             hw_uid=hw_uid,
         )
 
     def urls(self) -> dict[str, Optional[yarl.URL]]:
         return self.hubitat_gt.urls()
+
+    def add_web_listener(self, web_listener_node: str) -> None:
+        self.web_listener_nodes.add(web_listener_node)
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_poller_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_poller_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,39 +40,49 @@
             raise ValueError(
                 f"ERROR. resolve_rest() has not yet been called for {self}."
             )
         return self._rest
 
     def resolve(
         self,
-        tank_node_name: str,
+        node_name: str,
         nodes: dict[str, ShNode],
         components: dict[str, Component],
     ):
         if self._rest is not None:
             raise ValueError(
                 f"resolve() must be called exactly once. "
                 f"Rest settings already exist for {self}."
             )
 
         # replace proxy hubitat component, which only had component id.
         # with the actual hubitat component containing data.
-        self.hubitat_gt = HubitatComponentGt.from_component_id(
+        hubitat_component = HubitatComponentGt.from_component_id(
             self.hubitat_gt.ComponentId,
             components,
         )
+        self.hubitat_gt = HubitatComponentGt.from_data_class(hubitat_component)
 
         # Constuct url config on top of maker api url url config
         self._rest = RESTPollerSettings(
             request=RequestArgs(
                 url=self.hubitat_gt.refresh_url_config(self.poller_gt.device_id)
             ),
             poll_period_seconds=self.poller_gt.poll_period_seconds,
         )
 
+        # register attributes which accept web posts
+        if (
+            self.poller_gt.web_listen_enabled
+            and hubitat_component.hubitat_gt.WebListenEnabled
+        ):
+            for attribute in self.poller_gt.attributes:
+                if attribute.web_listen_enabled:
+                    hubitat_component.add_web_listener(node_name)
+
     def urls(self) -> dict[str, Optional[yarl.URL]]:
         urls = self.hubitat_gt.urls()
         for attribute in self.poller_gt.attributes:
             urls[attribute.node_name] = self.rest.url
         return urls
 
     @property
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_tank_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_tank_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class HubitatTankComponent(Component, ComponentResolver):
     hubitat: HubitatComponentGt
     sensor_supply_voltage: float
     default_poll_period_seconds: Optional[float] = None
     devices_gt: list[FibaroTempSensorSettingsGt]
     devices: list[FibaroTempSensorSettings] = []
+    web_listen_enabled: bool
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
         tank_gt: HubitatTankSettingsGt,
         display_name: Optional[str] = None,
@@ -32,30 +33,32 @@
         # of the hubitat; the actual component data will be resolved
         # when resolve() is called; Here in the constructor we cannot
         # rely on the actual HubitatComponentGt existing yet.
         self.hubitat = HubitatComponentGt.make_stub(tank_gt.hubitat_component_id)
         self.sensor_supply_voltage = tank_gt.sensor_supply_voltage
         self.default_poll_period_seconds = tank_gt.default_poll_period_seconds
         self.devices_gt = list(tank_gt.devices)
+        self.web_listen_enabled = tank_gt.web_listen_enabled
         super().__init__(
             display_name=display_name,
             component_id=component_id,
             hw_uid=hw_uid,
             component_attribute_class_id=component_attribute_class_id,
         )
 
     def resolve(
         self,
         tank_node_name: str,
         nodes: dict[str, ShNode],
         components: dict[str, Component],
     ):
-        hubitat_component_gt = HubitatComponentGt.from_component_id(
+        hubitat_component = HubitatComponentGt.from_component_id(
             self.hubitat.ComponentId, components
         )
+        hubitat_component_gt = HubitatComponentGt.from_data_class(hubitat_component)
         hubitat_settings = HubitatRESTResolutionSettings(hubitat_component_gt)
         devices = [
             FibaroTempSensorSettings.create(
                 tank_name=tank_node_name,
                 settings_gt=device_gt,
                 hubitat=hubitat_settings,
                 default_poll_period_seconds=self.default_poll_period_seconds,
@@ -69,14 +72,20 @@
                     f"ERROR. Node not found for tank temp sensor <{device.node_name}>"
                 )
         # replace proxy hubitat component, which only had component id.
         # with the actual hubitat component containing data.
         self.hubitat = hubitat_component_gt
         self.devices = devices
 
+        # register voltage attribute for fibaros which accept web posts
+        if self.web_listen_enabled and hubitat_component.hubitat_gt.WebListenEnabled:
+            for device in self.devices:
+                if device.web_listen_enabled:
+                    hubitat_component.add_web_listener(tank_node_name)
+
     def urls(self) -> dict[str, Optional[yarl.URL]]:
         urls = self.hubitat.urls()
         for device in self.devices:
             urls[device.node_name] = device.url
         return urls
 
     @property
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/relay_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/relay_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/rest_poller_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/rest_poller_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/hardware_layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 away with).
 """
 
 import copy
 import json
 import re
 import typing
+from collections import defaultdict
 from dataclasses import dataclass
 from functools import cached_property
 from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
+from typing import Type
+from typing import TypeVar
 
 from gwproto.data_classes.cacs.electric_meter_cac import ElectricMeterCac
 from gwproto.data_classes.component import Component
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.data_classes.components.electric_meter_component import (
     ElectricMeterComponent,
 )
@@ -46,14 +49,16 @@
 from gwproto.types import SpaceheatNodeGt_Maker
 from gwproto.types.electric_meter_component_gt import ElectricMeterComponentGt_Maker
 from gwproto.types.multipurpose_sensor_component_gt import (
     MultipurposeSensorComponentGt_Maker,
 )
 
 
+T = TypeVar("T")
+
 snake_add_underscore_to_camel_pattern = re.compile(r"(?<!^)(?=[A-Z])")
 
 
 def camel_to_snake(name: str) -> str:
     return snake_add_underscore_to_camel_pattern.sub("_", name).lower()
 
 
@@ -206,15 +211,17 @@
             errors.append(LoadError("ShNode", d, e))
 
 
 class HardwareLayout:
     layout: dict[Any, Any]
     cacs: dict[str, ComponentAttributeClass]
     components: dict[str, Component]
+    components_by_type: dict[Type, list[Component]]
     nodes: dict[str, ShNode]
+    nodes_by_component: dict[str, str]
 
     def __init__(
         self,
         layout: dict[Any, Any],
         cacs: Optional[dict[str, ComponentAttributeClass]] = None,
         components: Optional[dict[str, Component]] = None,
         nodes: Optional[dict[str, ShNode]] = None,
@@ -222,17 +229,23 @@
         self.layout = copy.deepcopy(layout)
         if cacs is None:
             cacs = ComponentAttributeClass.by_id
         self.cacs = dict(cacs)
         if components is None:
             components = Component.by_id
         self.components = dict(components)
+        self.components_by_type = defaultdict(list)
+        for component in components.values():
+            self.components_by_type[type(component)].append(component)
         if nodes is None:
             nodes = ShNode.by_id
         self.nodes = dict(nodes)
+        self.nodes_by_component = {
+            node.component_id: node.alias for node in self.nodes.values()
+        }
 
     def clear_property_cache(self) -> None:
         for cached_prop_name in [
             prop_name
             for prop_name in type(self).__dict__
             if isinstance(type(self).__dict__[prop_name], cached_property)
         ]:
@@ -298,19 +311,41 @@
             errors=errors,
         )
         return HardwareLayout(layout, **load_args)
 
     def node(self, alias: str, default: Any = None) -> ShNode:
         return self.nodes.get(alias, default)
 
-    def component(self, alias: str) -> Optional[Component]:
-        return self.component_from_node(self.node(alias, None))
+    def component(self, node_alias: str) -> Optional[Component]:
+        return self.component_from_node(self.node(node_alias, None))
+
+    def cac(self, node_alias: str) -> Optional[ComponentAttributeClass]:
+        return self.cac_from_component(self.component(node_alias))
+
+    def get_component_as_type(self, component_id: str, type_: Type[T]) -> Optional[T]:
+        component = self.components.get(component_id, None)
+        if component is not None and not isinstance(component, type_):
+            raise ValueError(
+                f"ERROR. Component <{component_id}> has type {type(component)} not {type_}"
+            )
+        return component
+
+    def get_components_by_type(self, type_: Type[T]) -> list[T]:
+        entries = self.components_by_type.get(type_, [])
+        for i, entry in enumerate(entries):
+            if not isinstance(entry, type_):
+                raise ValueError(
+                    f"ERROR. Entry {i+1} in "
+                    f"HardwareLayout.components_by_typ[{type_}] "
+                    f"has the wrong type {type(entry)}"
+                )
+        return entries
 
-    def cac(self, alias: str) -> Optional[ComponentAttributeClass]:
-        return self.cac_from_component(self.component(alias))
+    def node_from_component(self, component_id: str) -> Optional[ShNode]:
+        return self.nodes.get(self.nodes_by_component.get(component_id, ""), None)
 
     def component_from_node(self, node: Optional[ShNode]) -> Optional[Component]:
         return (
             self.components.get(
                 node.component_id if node.component_id is not None else "", None
             )
             if node is not None
@@ -493,14 +528,15 @@
         multi_nodes = list(
             filter(
                 lambda x: (
                     (
                         x.actor_class == ActorClass.MultipurposeSensor
                         or x.actor_class == ActorClass.HubitatTankModule
                         or x.actor_class == ActorClass.HubitatPoller
+                        or x.actor_class == ActorClass.HoneywellThermostat
                     )
                     and hasattr(x.component, "config_list")
                 ),
                 self.nodes.values(),
             )
         )
         telemetry_tuples = []
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.7.3/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/decoders.py` & `gridworks_protocol-0.7.3/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/default_decoders.py` & `gridworks_protocol-0.7.3/src/gwproto/default_decoders.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import gwproto.types.hubitat_component_gt  # noqa
 import gwproto.types.hubitat_poller_cac_gt  # noqa
 import gwproto.types.hubitat_poller_component_gt  # noqa
 import gwproto.types.hubitat_tank_cac_gt  # noqa
 import gwproto.types.hubitat_tank_component_gt  # noqa
 import gwproto.types.rest_poller_cac_gt  # noqa
 import gwproto.types.rest_poller_component_gt  # noqa
+import gwproto.types.web_server_cac_gt  # noqa
+import gwproto.types.web_server_component_gt  # noqa
 from gwproto.data_classes.component import Component
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.decoders import PydanticTypeNameDecoder
 
 
 T = TypeVar("T")
 
@@ -82,20 +84,22 @@
     model_name="DefaultCacDecoder",
     module_names=[
         "gwproto.types.fibaro_smart_implant_cac_gt",
         "gwproto.types.hubitat_cac_gt",
         "gwproto.types.hubitat_poller_cac_gt",
         "gwproto.types.hubitat_tank_cac_gt",
         "gwproto.types.rest_poller_cac_gt",
+        "gwproto.types.web_server_cac_gt",
     ],
 )
 
 default_component_decoder = ComponentDecoder(
     model_name="DefaultComponentDecoder",
     module_names=[
         "gwproto.types.fibaro_smart_implant_component_gt",
         "gwproto.types.hubitat_component_gt",
         "gwproto.types.hubitat_poller_component_gt",
         "gwproto.types.hubitat_tank_component_gt",
         "gwproto.types.rest_poller_component_gt",
+        "gwproto.types.web_server_component_gt",
     ],
 )
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/__init__.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/actor_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,28 +49,34 @@
         Home Automation Hub LAN API. [More Info](https://drive.google.com/drive/u/0/folders/1AqAU_lC2phzuI9XRYvogiIYA7GXNtlr6).
       - HubitatTankModule (e2877329): The actor for running a GridWorks TankModule, comprised of
         two Z-Wave Fibaro temp sensors built together inside a small container that has 4 thermistors
         attached. These are designed to be installed from top (1) to bottom (4) on a stratified
         thermal storage tank. [More Info](https://drive.google.com/drive/u/0/folders/1GSxDd8Naf1GKK_fSOgQU933M1UcJ4r8q).
       - HubitatPoller (00000100): An actor for representing a somewhat generic ShNode (like a thermostat)
         that can be polled through the Hubitat.
+      - Hubitat: (0000101): An actor for representing a Hubitat for receiving Hubitat events over HTTP.
+      - HoneywellThermostat: (0000102): An actor for representing a Honeywell Hubitat thermostat which
+        can load thermostat heating state change messages into status reports.
+
     """
 
     NoActor = auto()
     Scada = auto()
     HomeAlone = auto()
     BooleanActuator = auto()
     PowerMeter = auto()
     Atn = auto()
     SimpleSensor = auto()
     MultipurposeSensor = auto()
     Thermostat = auto()
     HubitatTelemetryReader = auto()
     HubitatTankModule = auto()
     HubitatPoller = auto()
+    Hubitat = auto()
+    HoneywellThermostat = auto()
 
     @classmethod
     def default(cls) -> "ActorClass":
         """
         Returns default value (in this case NoActor)
         """
         return cls.NoActor
@@ -168,14 +174,16 @@
             "b103058f",
             "dae4b2f0",
             "7c483ad0",
             "4a9c1785",
             "0401b27e",
             "e2877329",
             "00000100",
+            "00000101",
+            "00000102",
         ]
 
 
 symbol_to_value = {
     "00000000": "NoActor",
     "6d37aa41": "Scada",
     "32d3d19f": "HomeAlone",
@@ -184,14 +192,16 @@
     "b103058f": "Atn",
     "dae4b2f0": "SimpleSensor",
     "7c483ad0": "MultipurposeSensor",
     "4a9c1785": "Thermostat",
     "0401b27e": "HubitatTelemetryReader",
     "e2877329": "HubitatTankModule",
     "00000100": "HubitatPoller",
+    "00000101": "Hubitat",
+    "00000102": "HoneywellThermostat",
 }
 
 value_to_symbol = {value: key for key, value in symbol_to_value.items()}
 
 value_to_version = {
     "NoActor": "000",
     "Scada": "000",
@@ -201,8 +211,10 @@
     "Atn": "000",
     "SimpleSensor": "000",
     "MultipurposeSensor": "000",
     "Thermostat": "000",
     "HubitatTelemetryReader": "001",
     "HubitatTankModule": "001",
     "HubitatPoller": "001",
+    "Hubitat": "001",
+    "HoneywellThermostat": "001",
 }
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/role.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/telemetry_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
       - VoltageRmsMilliVolts (bb6fdd59): Voltage in Root Mean Square MilliVolts.
       - MilliWattHours (e0bb014b): Energy in MilliWattHours.
       - FrequencyMicroHz (337b8659): Frequency in MicroHz. Example: 59,965,332 means 59.965332 Hz.
       - AirTempCTimes1000 (0f627faa): Air temperature, in Degrees Celsius multiplied by 1000. Example:
         6234 means 6.234 deg Celcius.
       - AirTempFTimes1000 (4c3f8c78): Air temperature, in Degrees F multiplied by 1000. Example:
         69329 means 69.329 deg Fahrenheit.
+      - ThermostatState (00002000): An enum representing the state of the thermostat heat call.
     """
 
     Unknown = auto()
     PowerW = auto()
     RelayState = auto()
     WaterTempCTimes1000 = auto()
     WaterTempFTimes1000 = auto()
@@ -52,14 +53,15 @@
     CurrentRmsMicroAmps = auto()
     GallonsTimes100 = auto()
     VoltageRmsMilliVolts = auto()
     MilliWattHours = auto()
     FrequencyMicroHz = auto()
     AirTempCTimes1000 = auto()
     AirTempFTimes1000 = auto()
+    ThermostatState = auto()
 
     @classmethod
     def default(cls) -> "TelemetryName":
         """
         Returns default value (in this case Unknown)
         """
         return cls.Unknown
@@ -158,14 +160,15 @@
             "ad19e79c",
             "329a68c0",
             "bb6fdd59",
             "e0bb014b",
             "337b8659",
             "0f627faa",
             "4c3f8c78",
+            "00002000",
         ]
 
 
 symbol_to_value = {
     "00000000": "Unknown",
     "af39eec9": "PowerW",
     "5a71d4b3": "RelayState",
@@ -175,14 +178,15 @@
     "ad19e79c": "CurrentRmsMicroAmps",
     "329a68c0": "GallonsTimes100",
     "bb6fdd59": "VoltageRmsMilliVolts",
     "e0bb014b": "MilliWattHours",
     "337b8659": "FrequencyMicroHz",
     "0f627faa": "AirTempCTimes1000",
     "4c3f8c78": "AirTempFTimes1000",
+    "00002000": "ThermostatState",
 }
 
 value_to_symbol = {value: key for key, value in symbol_to_value.items()}
 
 value_to_version = {
     "Unknown": "000",
     "PowerW": "000",
@@ -193,8 +197,9 @@
     "CurrentRmsMicroAmps": "000",
     "GallonsTimes100": "000",
     "VoltageRmsMilliVolts": "001",
     "MilliWattHours": "001",
     "FrequencyMicroHz": "001",
     "AirTempCTimes1000": "001",
     "AirTempFTimes1000": "001",
+    "ThermostatState": "001",
 }
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/enums/unit.py` & `gridworks_protocol-0.7.3/src/gwproto/enums/unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,28 @@
       - Celcius (ec14bd47)
       - Fahrenheit (7d8832f8)
       - Gpm (b4580361)
       - WattHours (d66f1622)
       - AmpsRms (a969ac7c)
       - VoltsRms (e5d7555c)
       - Gallons (8e123a26)
+      - ThermostatStateEnum (00003000)
     """
 
     Unknown = auto()
     Unitless = auto()
     W = auto()
     Celcius = auto()
     Fahrenheit = auto()
     Gpm = auto()
     WattHours = auto()
     AmpsRms = auto()
     VoltsRms = auto()
     Gallons = auto()
+    ThermostatStateEnum = auto()
 
     @classmethod
     def default(cls) -> "Unit":
         """
         Returns default value (in this case Unknown)
         """
         return cls.Unknown
@@ -137,28 +139,30 @@
             "ec14bd47",
             "7d8832f8",
             "b4580361",
             "d66f1622",
             "a969ac7c",
             "e5d7555c",
             "8e123a26",
+            "00003000",
         ]
 
 
 symbol_to_value = {
     "00000000": "Unknown",
     "ec972387": "Unitless",
     "f459a9c3": "W",
     "ec14bd47": "Celcius",
     "7d8832f8": "Fahrenheit",
     "b4580361": "Gpm",
     "d66f1622": "WattHours",
     "a969ac7c": "AmpsRms",
     "e5d7555c": "VoltsRms",
     "8e123a26": "Gallons",
+    "00003000": "ThermostatStateEnum",
 }
 
 value_to_symbol = {value: key for key, value in symbol_to_value.items()}
 
 value_to_version = {
     "Unknown": "000",
     "Unitless": "000",
@@ -166,8 +170,9 @@
     "Celcius": "000",
     "Fahrenheit": "000",
     "Gpm": "000",
     "WattHours": "000",
     "AmpsRms": "000",
     "VoltsRms": "000",
     "Gallons": "000",
+    "ThermostatStateEnum": "000"
 }
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/message.py` & `gridworks_protocol-0.7.3/src/gwproto/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,17 +49,18 @@
 
 
 class Message(GenericModel, Generic[PayloadT]):
     Header: Header
     Payload: PayloadT
     TypeName: str = Field(GRIDWORKS_ENVELOPE_TYPE, const=True)
 
-    def __init__(self, **kwargs: Any):
-        kwargs["Header"] = self._header_from_kwargs(kwargs)
-        super().__init__(**kwargs)
+    def __init__(self, header: Optional[Header] = None, **kwargs: Any):
+        if header is None:
+            header = self._header_from_kwargs(kwargs)
+        super().__init__(Header=header, **kwargs)
 
     def message_type(self) -> str:
         return self.Header.MessageType
 
     def src(self) -> str:
         return self.Header.Src
 
@@ -87,15 +88,15 @@
                     for payload_field in payload_fields:
                         if hasattr(payload, payload_field):
                             val = getattr(payload, payload_field)
                         elif isinstance(payload, Mapping) and payload_field in payload:
                             val = payload[payload_field]
                 if val is not None:
                     header_kwargs[header_field] = val
-        header: Optional[Union[Header, dict[str, Any]]] = kwargs.get("Header", None)
+        header: Optional[Union[Header, dict[str, Any]]] = kwargs.pop("Header", None)
         if isinstance(header, Header):
             header = header.copy(update=header_kwargs, deep=True)
         else:
             if header is not None:
                 header_kwargs = dict(header, **header_kwargs)
             header = Header(**header_kwargs)
         return header
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.7.3/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/messages/event.py` & `gridworks_protocol-0.7.3/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/messages/misc.py` & `gridworks_protocol-0.7.3/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/property_format.py` & `gridworks_protocol-0.7.3/src/gwproto/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/topic.py` & `gridworks_protocol-0.7.3/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/type_helpers/__init__.py` & `gridworks_protocol-0.7.3/src/gwproto/type_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/__init__.py` & `gridworks_protocol-0.7.3/src/gwproto/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 from gwproto.types.spaceheat_node_gt import SpaceheatNodeGt_Maker
 from gwproto.types.ta_data_channels import TaDataChannels
 from gwproto.types.ta_data_channels import TaDataChannels_Maker
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig_Maker
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat_Maker
+from gwproto.types.web_server_gt import WebServerGt
 
 
 __all__ = [
     "ComponentAttributeClassGt",
     "ComponentAttributeClassGt_Maker",
     "ComponentGt",
     "ComponentGt_Maker",
@@ -187,8 +188,9 @@
     "SpaceheatNodeGt_Maker",
     "TaDataChannels",
     "TaDataChannels_Maker",
     "TelemetryReportingConfig",
     "TelemetryReportingConfig_Maker",
     "TelemetrySnapshotSpaceheat",
     "TelemetrySnapshotSpaceheat_Maker",
+    "WebServerGt",
 ]
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/component_attribute_class_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.7.3/src/gwproto/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.7.3/src/gwproto/types/egauge_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.7.3/src/gwproto/types/egauge_register_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.7.3/src/gwproto/types/gt_telemetry.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.7.3/src/gwproto/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_component_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class HubitatComponentGt(ComponentGt):
     Hubitat: HubitatGt
     TypeName: Literal["hubitat.component.gt"] = "hubitat.component.gt"
     Version: Literal["000"] = "000"
 
     def __hash__(self):
-        return hash((type(self),) + tuple(self.__dict__.values()))
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
     def url_config(self) -> URLConfig:
         return self.Hubitat.url_config()
 
     def maker_api_url_config(self) -> URLConfig:
         return self.Hubitat.maker_api_url_config()
 
@@ -70,29 +70,29 @@
                 MacAddress="000000000000",
             ),
         )
 
     @classmethod
     def from_component_id(
         cls, component_id: str, components: dict[str, Component]
-    ) -> "HubitatComponentGt":
+    ) -> "HubitatComponent":
         hubitat_component = components.get(component_id, None)
         if hubitat_component is None:
             raise ValueError(
                 "ERROR. No component found for "
                 f"HubitatTankComponent.hubitat.CompnentId {component_id}"
             )
         if not isinstance(hubitat_component, HubitatComponent):
             raise ValueError(
                 "ERROR. Referenced hubitat component has type "
                 f"{type(hubitat_component)}; "
                 "must be instance of HubitatComponent. "
                 f"Hubitat component id: {component_id}"
             )
-        return HubitatComponentGt.from_data_class(hubitat_component)
+        return hubitat_component
 
 
 class HubitatRESTResolutionSettings:
     component_gt: HubitatComponentGt
     maker_api_url_config: URLConfig
 
     def __init__(self, component_gt: HubitatComponentGt):
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_gt.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 class MakerAPIAttributeGt(BaseModel):
     attribute_name: str
     node_name: str
     telemetry_name_gt_enum_symbol: str = "c89d0ba1"
     unit_gt_enum_symbol: str = "ec14bd47"
     exponent: int = 3
+    interpret_as_number: bool = True
     enabled: bool = True
+    web_poll_enabled: bool = True
+    web_listen_enabled: bool = True
     report_missing: bool = True
     report_parse_error: bool = True
 
     @property
     def telemetry_name(self) -> TelemetryName:
         value = TelemetryName.symbol_to_value(
             self.telemetry_name_gt_enum_symbol,
@@ -44,13 +47,14 @@
 
 
 class HubitatPollerGt(BaseModel):
     hubitat_component_id: str
     device_id: int
     attributes: list[MakerAPIAttributeGt] = []
     enabled: bool = True
+    web_listen_enabled: bool = True
     poll_period_seconds: float = 60
 
     class Config:
         extra = Extra.allow
         alias_generator = snake_to_camel
         allow_population_by_field_name = True
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     fibaro_component_id: str
     analog_input_id: conint(ge=1, le=2)
     tank_label: str = ""
     exponent: int = 1
     telemetry_name_gt_enum_symbol: str = "c89d0ba1"
     temp_unit_gt_enum_symbol: str = "ec14bd47"
     enabled: bool = True
+    web_listen_enabled: bool = True
     poll_period_seconds: Optional[float] = None
     """The actual poll_seconds_used will be the first of:
     1. Any value specified in an explicit 'rest' member, if 'rest' member is not None.
     2. The value from this object, if that value is not None.
     3. The value of HubitatTanksSettingsGt.default_poll_period_seconds if it is not None.
     4. The default value.
     """
@@ -232,12 +233,13 @@
 
 
 class HubitatTankSettingsGt(BaseModel):
     hubitat_component_id: str
     sensor_supply_voltage: float = DEFAULT_TANK_MODULE_VOLTAGE
     default_poll_period_seconds: Optional[float] = None
     devices: list[FibaroTempSensorSettingsGt] = []
+    web_listen_enabled: bool = True
 
     class Config:
         extra = Extra.allow
         alias_generator = snake_to_camel
         allow_population_by_field_name = True
```

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.7.3/src/gwproto/types/power_watts.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/relay_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/relay_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/relay_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/relay_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.7.3/src/gwproto/types/snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.7.3/src/gwproto/types/spaceheat_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/ta_data_channels.py` & `gridworks_protocol-0.7.3/src/gwproto/types/ta_data_channels.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.7.3/src/gwproto/types/telemetry_reporting_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.7.3/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/src/gwproto/utils.py` & `gridworks_protocol-0.7.3/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.2/PKG-INFO` & `gridworks_protocol-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.7.2
+Version: 0.7.3
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

