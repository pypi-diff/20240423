# Comparing `tmp/waylay-sdk-data-types-2.14.0rc1.tar.gz` & `tmp/waylay-sdk-data-types-2.14.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-data-types-2.14.0rc1.tar", last modified: Tue Mar 26 16:19:41 2024, max compression
+gzip compressed data, was "waylay-sdk-data-types-2.14.0rc2.tar", last modified: Wed Mar 27 14:43:22 2024, max compression
```

## Comparing `waylay-sdk-data-types-2.14.0rc1.tar` & `waylay-sdk-data-types-2.14.0rc2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.705638 waylay-sdk-data-types-2.14.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-26 16:19:41.705638 waylay-sdk-data-types-2.14.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:19:41.705638 waylay-sdk-data-types-2.14.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.693638 waylay-sdk-data-types-2.14.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.693638 waylay-sdk-data-types-2.14.0rc1/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.693638 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.693638 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.701638 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/delete_messages200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/delete_series_from_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/event_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_metric_series_from_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_series200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_series200_response_inner_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/grouping_any_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/latest_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_result_results_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_until.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_window.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/post_series_for_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/post_series_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_event_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_event_response_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_event_response_content_any_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_resource_event_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_resource_event_response_content.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/query_time_series200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/query_time_series_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/resource_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/scalar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_key_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_request_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_request_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_operator_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value_exact.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value_exact_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_json_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timestamped_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timestamped_resource_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/ttl_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.701638 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/messages_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/series_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-26 16:19:35.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/version_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:41.705638 waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-26 16:19:41.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-26 16:19:41.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:19:41.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-26 16:19:41.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 16:19:41.000000 waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.686021 waylay-sdk-data-types-2.14.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-27 14:43:22.686021 waylay-sdk-data-types-2.14.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:43:22.686021 waylay-sdk-data-types-2.14.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.670021 waylay-sdk-data-types-2.14.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.670021 waylay-sdk-data-types-2.14.0rc2/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.670021 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.670021 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.682021 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/delete_messages200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/delete_series_from_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/event_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_metric_series_from_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_series200_response_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_series200_response_inner_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/grouping_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/latest_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_result_results_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_until.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/post_series_for_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/post_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_event_response_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_event_response_content_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_resource_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_resource_event_response_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/query_time_series200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/query_time_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/resource_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/scalar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_key_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_request_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_request_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_operator_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value_exact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value_exact_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_json_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timestamped_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timestamped_resource_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/ttl_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.686021 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/messages_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-27 14:43:18.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:22.686021 waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-27 14:43:22.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-27 14:43:22.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:43:22.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 14:43:22.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 14:43:22.000000 waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/top_level.txt
```

### Comparing `waylay-sdk-data-types-2.14.0rc1/LICENSE.txt` & `waylay-sdk-data-types-2.14.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/PKG-INFO` & `waylay-sdk-data-types-2.14.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-data-types
-Version: 2.14.0rc1
+Version: 2.14.0rc2
 Summary: Waylay Broker Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -12,19 +12,22 @@
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Project-URL: Homepage, https://www.waylay.io/
+Project-URL: Documentation, https://docs.waylay.io/#/
+Project-URL: Repository, https://github.com/waylayio/waylay-sdk-data-py.git
 Keywords: Waylay Broker,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk~=0.0.4rc4
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay-sdk-data-types-2.14.0rc1/README.md` & `waylay-sdk-data-types-2.14.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/pyproject.toml` & `waylay-sdk-data-types-2.14.0rc2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-data-types"
-version = "2.14.0rc1"
+version = "2.14.0rc2"
 description = "Waylay Broker Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Broker" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk ~= 0.0.4rc4",
+    "waylay-sdk ~= 0.0.4rc5",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
+[project.urls]
+Homepage = "https://www.waylay.io/"
+Documentation = "https://docs.waylay.io/#/"
+Repository = "https://github.com/waylayio/waylay-sdk-data-py.git"
+
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
     "types-python-dateutil",
@@ -48,17 +53,18 @@
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
 # allow duplicate imports
 ignore=["F811"]
 # https://docs.astral.sh/ruff/rules
 select= [
-    "UP007", "FA102", "I001",  # convert Union to | (pep-604)
-    "F401", "E303",  # remove unused imports
+    "UP007", "FA102",  # convert Union to | (pep-604)
+    "I001", "F401",  # sort and remove unused imports
     "PIE790",  # remove unnecessary pass statements
+    "E303",  # too many blank lines
 ]
 
 [tool.ruff.lint.per-file-ignores]
 # do not touch imports here
 "__init__.py" = ["F401"]
 "conftest.py" = ["F401"]
```

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/__init__.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Data is ingested into the platform by the Waylay Broker.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "2.14.0rc1"
+__version__ = "2.14.0rc2"
 
 # import models into model package
 from .aggregate import Aggregate
 from .delete_messages200_response import DeleteMessages200Response
 from .delete_series_from_parameter import DeleteSeriesFromParameter
 from .error_response import ErrorResponse
 from .event import Event
```

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/aggregate.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/aggregate.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/delete_messages200_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/delete_messages200_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/delete_series_from_parameter.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/delete_series_from_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/error_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/error_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/event.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/event.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/event_timestamp.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/event_timestamp.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response_links.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_datapoints_for_metric_raw200_response_links.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_metric_series_from_parameter.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_metric_series_from_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_series200_response_inner.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_series200_response_inner.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/get_series200_response_inner_latest.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/get_series200_response_inner_latest.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/grouping.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/grouping.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/hal_link.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/latest_measurement.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/latest_measurement.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_from.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_from.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_result.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_result.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_result_results_inner.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_result_results_inner.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_until.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_until.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/message_query_window.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/message_query_window.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/post_series_for_resource_request.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/post_series_for_resource_request.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/post_series_request.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/post_series_request.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_event_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_event_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_event_response_content.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_event_response_content.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_event_response_content_any_of.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_event_response_content_any_of.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_resource_event_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_resource_event_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/publish_resource_event_response_content.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/publish_resource_event_response_content.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/query_time_series200_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/query_time_series200_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/query_time_series_request.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/query_time_series_request.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/resource_event.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/resource_event.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/scalar_data.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/scalar_data.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_key_value_inner.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_key_value_inner.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_request.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_request.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_request_from.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_request_from.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_request_window.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_request_window.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/series_query_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/series_query_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_operator.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_operator.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_operator_operator.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_operator_operator.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value_bounds.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value_bounds.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_filter_value_exact.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_filter_value_exact.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timeseries_json_result.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timeseries_json_result.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timestamped_event.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timestamped_event.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/timestamped_resource_event.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/timestamped_resource_event.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/ttl_duration.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/ttl_duration.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/models/version_response.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/models/version_response.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/events_api.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/events_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/messages_api.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/messages_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/series_api.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/series_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay/services/data/queries/version_api.py` & `waylay-sdk-data-types-2.14.0rc2/src/waylay/services/data/queries/version_api.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/PKG-INFO` & `waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-data-types
-Version: 2.14.0rc1
+Version: 2.14.0rc2
 Summary: Waylay Broker Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -12,19 +12,22 @@
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Project-URL: Homepage, https://www.waylay.io/
+Project-URL: Documentation, https://docs.waylay.io/#/
+Project-URL: Repository, https://github.com/waylayio/waylay-sdk-data-py.git
 Keywords: Waylay Broker,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk~=0.0.4rc4
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay-sdk-data-types-2.14.0rc1/src/waylay_sdk_data_types.egg-info/SOURCES.txt` & `waylay-sdk-data-types-2.14.0rc2/src/waylay_sdk_data_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

