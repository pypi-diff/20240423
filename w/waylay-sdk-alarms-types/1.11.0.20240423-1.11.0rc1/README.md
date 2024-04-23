# Comparing `tmp/waylay_sdk_alarms_types-1.11.0.20240423.tar.gz` & `tmp/waylay-sdk-alarms-types-1.11.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_alarms_types-1.11.0.20240423.tar", last modified: Tue Apr 23 16:04:56 2024, max compression
+gzip compressed data, was "waylay-sdk-alarms-types-1.11.0rc1.tar", last modified: Wed Mar 27 16:12:59 2024, max compression
```

## Comparing `waylay_sdk_alarms_types-1.11.0.20240423.tar` & `waylay-sdk-alarms-types-1.11.0rc1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.411536 waylay_sdk_alarms_types-1.11.0.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-23 16:04:56.411536 waylay_sdk_alarms_types-1.11.0.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:04:56.411536 waylay_sdk_alarms_types-1.11.0.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.395536 waylay_sdk_alarms_types-1.11.0.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.395536 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.395536 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.395536 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.407536 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/a_batch_alarms_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_audit_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_changes_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_type_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_type_one_of1.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_type_one_of2.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_severity_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_source_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_status_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_timeline_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_type_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarms_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarms_timeline_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_alarm_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_delete_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_delete_alarm_all_of_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_enqueued.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_operation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_update_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_update_alarm_all_of_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/bulk_query_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/bulk_query_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/cloud_alarm_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/cloud_alarm_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/create_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/error_response_with_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/failure_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/id_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/list_order_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/list_sort_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/nd_json_response_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/operation_result_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/operation_result_object_results.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/queued_operation_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/queued_operation_summary_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/ss_event_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/success_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.407536 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/alarm_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/alarms_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/alarms_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:51.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:56.411536 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-23 16:04:56.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-23 16:04:56.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:04:56.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 16:04:56.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:04:56.000000 waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.785406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.797406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/a_batch_alarms_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_audit_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_severity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_source_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_status_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_timeline_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_type_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_timeline_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_alarm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm_all_of_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_operation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_update_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_update_alarm_all_of_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/create_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/failure_operation_result_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/id_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_order_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_sort_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/nd_json_response_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/queued_operation_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/queued_operation_summary_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/ss_event_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/success_operation_result_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.797406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarm_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-27 16:12:53.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.801406 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 16:12:59.000000 waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/LICENSE.txt` & `waylay-sdk-alarms-types-1.11.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/PKG-INFO` & `waylay-sdk-alarms-types-1.11.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms-types
-Version: 1.11.0.20240423
+Version: 1.11.0rc1
 Summary: Waylay Alarms Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-alarms==1.11.0.20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,50 +44,54 @@
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
 It is considered an extension of the waylay-sdk-alarms package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-alarms`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from ..models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from ..models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/README.md` & `waylay-sdk-alarms-types-1.11.0rc1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
 It is considered an extension of the waylay-sdk-alarms package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-alarms`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from ..models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from ..models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/pyproject.toml` & `waylay-sdk-alarms-types-1.11.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-alarms-types"
-version = "1.11.0.20240423"
+version = "1.11.0rc1"
 description = "Waylay Alarms Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Alarms" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
-    "waylay-sdk-alarms == 1.11.0.20240423",
+    "waylay-sdk ~= 0.0.4rc5",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-alarms-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/alarms.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/__init__.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "1.11.0.20240423"
+__version__ = "1.11.0rc1"
 
 # import models into model package
 from .a_batch_alarms_specification import ABatchAlarmsSpecification
 from .alarm_audit_record import AlarmAuditRecord
 from .alarm_entity import AlarmEntity
 from .alarm_event import AlarmEvent
 from .alarm_event_alarm import AlarmEventAlarm
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/a_batch_alarms_specification.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/a_batch_alarms_specification.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_audit_record.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_audit_record.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 
     id: StrictStr
     type: AlarmEventType
     text: StrictStr = Field(description="Text describing the change")
     timestamp: Any
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_entity.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,9 +54,12 @@
     additional_properties: Dict[str, Any] | None = Field(
         default=None,
         description="Additional properties that were present in the creation payload",
         alias="additionalProperties",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,9 +33,12 @@
     alarm: AlarmEventAlarm
     changes: List[AlarmEventChangesInner] | None = Field(
         default=None,
         description="Describes the changes that where done  Will only be there if `eventtype` is `io.waylay.alarm.AlarmUpdated`",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_alarm.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,9 +39,12 @@
     timestamp: datetime
     source: IdObject
     severity: AlarmSeverity
     status: AlarmStatus
     count: Annotated[int, Field(strict=True, ge=1)]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_changes_inner.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 
     attribute: StrictStr | None = None
     type: AlarmEventChangesInnerType | None = None
     old_value: StrictStr | None = Field(default=None, alias="oldValue")
     new_value: StrictStr | None = Field(default=None, alias="newValue")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_changes_inner_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_type.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_event_type_one_of1.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_event_type_one_of1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_severity_filter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_severity_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_status_filter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_status_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_timeline_info.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_timeline_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,9 +37,12 @@
     severity: AlarmSeverity
     status: AlarmStatus
     assignee: StrictStr | None = Field(
         default=None, description="String field to indicate an assignee for the alarm."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarm_update.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarm_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """At least one field must be specified.."""
 
     severity: AlarmSeverity | None = None
     status: AlarmStatus | None = None
     assignee: Any | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarms_query_result.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_query_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,9 +38,12 @@
     )
     prev: StrictStr | None = Field(
         default=None,
         description="Link to the previous page of result (if previous page is available)",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/alarms_timeline_item.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/alarms_timeline_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """AlarmsTimelineItem."""
 
     timestamp: StrictInt = Field(description="Timestamp of the event")
     type: AlarmEventType
     alarm: AlarmTimelineInfo
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_alarm.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """BatchAlarm."""
 
     entity: BatchAlarmEntity | None = None
     action: StrictStr | None = None
     query: Dict[str, Any] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_delete_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """BatchDeleteAlarm."""
 
     entity: BatchAlarmEntity
     action: BatchDeleteAlarmAllOfAction
     query: BatchDeleteAlarmAllOfQuery
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_delete_alarm_all_of_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 
     id: StrictStr
     user: StrictStr = Field(description="User id of the user who started the operation")
     operation: BatchOperationOperation
     queue_time: datetime = Field(alias="queueTime")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_enqueued.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     status_code: StrictInt = Field(alias="statusCode")
     uri: StrictStr = Field(
         description="URI where the batch operation status can be followed"
     )
     entity: BatchOperationEnqueuedEntity
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_enqueued_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     """BatchOperationEnqueuedEntity."""
 
     id: StrictStr
     queue_time: datetime = Field(alias="queueTime")
     operation: QueuedOperationSummary
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_operation.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """Summary of the batch operation."""
 
     entity: BatchAlarmEntity
     action: BatchOperationOperationAction
     description: StrictStr = Field(description="Description of the operation")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_result.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     user: StrictStr = Field(description="User id of the user who started the operation")
     operation: BatchOperationOperation
     queue_time: datetime = Field(alias="queueTime")
     finished_time: datetime = Field(alias="finishedTime")
     results: OperationResultObjectResults
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_operation_results.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_operation_results.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/batch_update_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/batch_update_alarm.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 
     entity: BatchAlarmEntity
     action: BatchUpdateAlarmAllOfAction
     query: BulkQueryIds
     action_parameters: AlarmUpdate = Field(alias="actionParameters")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/bulk_query_filter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,9 +42,12 @@
     creation_time_to: Any | None = Field(default=None, alias="creationTimeTo")
     last_updated_from: Any | None = Field(default=None, alias="lastUpdatedFrom")
     last_updated_to: Any | None = Field(default=None, alias="lastUpdatedTo")
     last_triggered_from: Any | None = Field(default=None, alias="lastTriggeredFrom")
     last_triggered_to: Any | None = Field(default=None, alias="lastTriggeredTo")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/bulk_query_ids.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/bulk_query_ids.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 
 class BulkQueryIds(WaylayBaseModel):
     """BulkQueryIds."""
 
     ids: Annotated[List[StrictStr], Field(min_length=1)]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/cloud_alarm_event.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     source: Dict[str, Any] | None = None
     subject: StrictStr
     type: CloudAlarmEventDataType | None = None
     data: AlarmEvent | None = None
     time: datetime
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/cloud_alarm_event_data.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     source: Any | None = None
     subject: StrictStr | None = None
     type: CloudAlarmEventDataType | None = None
     data: AlarmEvent | None = None
     time: datetime | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/cloud_alarm_event_data_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/create_alarm.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/create_alarm.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,9 +34,12 @@
     status: AlarmStatus | None = None
     timestamp: SO8601TimestampOrMillis | None = None
     assignee: StrictStr | None = Field(
         default=None, description="String field to indicate an assignee for the alarm."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/error_response.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/error_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 class ErrorResponse(WaylayBaseModel):
     """ErrorResponse."""
 
     status_code: StrictInt = Field(alias="statusCode")
     error: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/error_response_with_details.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/version_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,31 +7,26 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictInt,
     StrictStr,
 )
-from typing_extensions import (
-    Annotated,  # >=3.11
-)
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class ErrorResponseWithDetails(WaylayBaseModel):
-    """ErrorResponseWithDetails."""
+class VersionResponse(WaylayBaseModel):
+    """VersionResponse."""
 
-    status_code: StrictInt = Field(alias="statusCode")
-    error: StrictStr
-    details: Annotated[List[StrictStr], Field(min_length=1)] | None = None
+    version: StrictStr
+    name: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/failure_operation_result_value.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/success_operation_result_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
     StrictInt,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class FailureOperationResultValue(WaylayBaseModel):
+class SuccessOperationResultValue(WaylayBaseModel):
     """The keys will be alarm ids.."""
 
     status_code: StrictInt = Field(
         description="The statusCode of the operation", alias="statusCode"
     )
-    error: StrictStr = Field(description="Error description of what went wrong.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/get_eventstream_event_format_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/id_object.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/id_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,9 +20,12 @@
 
 class IdObject(WaylayBaseModel):
     """A JSON object with an id field indicating the resource.."""
 
     id: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_additional_query_params_parameter_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/list_sort_parameter.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/list_sort_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/nd_json_response_stream.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/nd_json_response_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/operation_result_object.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class OperationResultObject(WaylayBaseModel):
     """Finished Batch Operation results."""
 
     finished_time: datetime = Field(alias="finishedTime")
     results: OperationResultObjectResults
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/operation_result_object_results.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/operation_result_object_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,9 +30,12 @@
         description="Object containing the successful operation results.  The keys will be alarm ids."
     )
     failure: Dict[str, FailureOperationResultValue] = Field(
         description="Object containing the unsuccessful operation results.  The keys will be alarm ids."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/queued_operation_summary.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/queued_operation_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 class QueuedOperationSummary(WaylayBaseModel):
     """QueuedOperationSummary."""
 
     entity: BatchAlarmEntity
     action: QueuedOperationSummaryAction
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/so8601_timestamp_or_millis.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/ss_event_stream.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/models/ss_event_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/models/success_operation_result_value.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/version_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # coding: utf-8
-"""Waylay Alarms models.
+"""Waylay Alarms query parameters.
 
 This code was generated from the OpenAPI documentation of 'Waylay Alarms'
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
-
 """
 
-from __future__ import annotations
+from __future__ import annotations  # for Python 3.7–3.9
 
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class SuccessOperationResultValue(WaylayBaseModel):
-    """The keys will be alarm ids.."""
+def _get_query_alias_for(field_name: str) -> str:
+    return field_name
 
-    status_code: StrictInt = Field(
-        description="The statusCode of the operation", alias="statusCode"
-    )
+
+class GetQuery(WaylayBaseModel):
+    """Model for `get` query parameters."""
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_get_query_alias_for,
+        populate_by_name=True,
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/about_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_batch_operations_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,12 +20,29 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
+
+
+def _start_query_alias_for(field_name: str) -> str:
+    return field_name
+
+
+class StartQuery(WaylayBaseModel):
+    """Model for `start` query parameters."""
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_start_query_alias_for,
+        populate_by_name=True,
+    )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/alarm_events_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarm_events_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,12 +37,13 @@
         GetEventstreamEventFormatParameter | None,
         Field(
             description="The format of events in the stream.   If specified this must be `application/cloudevents+json` (make sure to correctly URL encode the `+` as `%2B`)"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay/services/alarms/queries/alarms_api.py` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay/services/alarms/queries/alarms_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -51,14 +52,15 @@
     return field_name
 
 
 class DeleteQuery(WaylayBaseModel):
     """Model for `delete` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -66,14 +68,15 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -211,14 +214,15 @@
         Dict[str, ListAdditionalQueryParamsParameterValue] | None,
         Field(
             description="To query the alarms based on the value of an additional property of the alarm,  you can add the key of the additional property as query parameter  with value the value you expect the alarm to have."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -226,12 +230,13 @@
     return field_name
 
 
 class UpdateQuery(WaylayBaseModel):
     """Model for `update` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/PKG-INFO` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms-types
-Version: 1.11.0.20240423
+Version: 1.11.0rc1
 Summary: Waylay Alarms Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-alarms==1.11.0.20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,50 +44,54 @@
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
 It is considered an extension of the waylay-sdk-alarms package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-alarms`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from ..models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from ..models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms_types-1.11.0.20240423/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt` & `waylay-sdk-alarms-types-1.11.0rc1/src/waylay_sdk_alarms_types.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 src/waylay/services/alarms/models/queued_operation_summary.py
 src/waylay/services/alarms/models/queued_operation_summary_action.py
 src/waylay/services/alarms/models/so8601_timestamp_or_millis.py
 src/waylay/services/alarms/models/ss_event_stream.py
 src/waylay/services/alarms/models/success_operation_result_value.py
 src/waylay/services/alarms/models/version_response.py
 src/waylay/services/alarms/queries/__init__.py
-src/waylay/services/alarms/queries/about_api.py
 src/waylay/services/alarms/queries/alarm_events_api.py
 src/waylay/services/alarms/queries/alarms_api.py
 src/waylay/services/alarms/queries/alarms_batch_operations_api.py
 src/waylay/services/alarms/queries/py.typed
+src/waylay/services/alarms/queries/version_api.py
 src/waylay_sdk_alarms_types.egg-info/PKG-INFO
 src/waylay_sdk_alarms_types.egg-info/SOURCES.txt
 src/waylay_sdk_alarms_types.egg-info/dependency_links.txt
 src/waylay_sdk_alarms_types.egg-info/requires.txt
 src/waylay_sdk_alarms_types.egg-info/top_level.txt
```

