# Comparing `tmp/waylay_sdk_resources_types-8.1.0.20240423.tar.gz` & `tmp/waylay_sdk_resources_types-8.1.0a20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_resources_types-8.1.0.20240423.tar", last modified: Tue Apr 23 16:13:02 2024, max compression
+gzip compressed data, was "waylay_sdk_resources_types-8.1.0a20240415.tar", last modified: Mon Apr 15 08:05:31 2024, max compression
```

## Comparing `waylay_sdk_resources_types-8.1.0.20240423.tar` & `waylay_sdk_resources_types-8.1.0a20240415.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.665265 waylay_sdk_resources_types-8.1.0.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-23 16:13:02.665265 waylay_sdk_resources_types-8.1.0.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:13:02.665265 waylay_sdk_resources_types-8.1.0.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.645265 waylay_sdk_resources_types-8.1.0.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.641265 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.645265 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.645265 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.661265 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/array_must_contain_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/array_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/array_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/attribute_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_operation_enqueued.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_operation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_operation_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_running_resource_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_running_resource_operation_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/boolean_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/boolean_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/changed_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/changed_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint_status_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/create_delete_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/create_delete_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/discovered_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/discovered_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/failure_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/generic_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/get_stream_event_format_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_page_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_type_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links_links_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links_links_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/halid_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/list_constraints200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_entity_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_entity_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/nd_json_response_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/numeric_enum_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/numeric_enum_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/numeric_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/numeric_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/object_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/object_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/operation_result_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/operation_result_object_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links_next.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links_prev.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/paging_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/patch_resource_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/patch_resource_type_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_change_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_changes_paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_constraint_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_constraint_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_constraint_with_id_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metadata_event_all_of_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of1.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of2.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_ref_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_ref_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_sensor_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_with_id_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_types_changes_paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_with_id_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resourcetype_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resourcetype_metadata_event_all_of_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/schema_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/ss_event_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/string_enum_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/string_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/string_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/success_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/task_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/task_configuration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/validation_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/with_id_required.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.665265 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/metadata_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/resource_constraint_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-23 16:12:58.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/resource_type_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:02.665265 waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-23 16:13:02.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-23 16:13:02.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:13:02.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-23 16:13:02.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:13:02.000000 waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/top_level.txt
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.260614 waylay_sdk_resources_types-8.1.0a20240415/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      745 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/LICENSE.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     5024 2024-04-15 08:05:31.260093 waylay_sdk_resources_types-8.1.0a20240415/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2744 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/README.md
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1824 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/pyproject.toml
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-15 08:05:31.260688 waylay_sdk_resources_types-8.1.0a20240415/setup.cfg
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.155325 waylay_sdk_resources_types-8.1.0a20240415/src/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.154690 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.154822 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.155134 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.243506 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    11903 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      484 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_must_contain_inner.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1718 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      448 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      963 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/attribute_item.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      943 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_enqueued.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1754 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_result.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      668 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_status_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      977 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      458 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_action.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      494 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      907 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      605 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1590 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      977 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      528 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      761 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/boolean_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      456 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/boolean_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      903 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/changed_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      434 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/changed_event_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1062 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1112 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      590 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_source.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1330 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1144 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      989 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_error.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1636 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_status.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      498 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_status_status.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      716 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/create_delete_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      466 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/create_delete_event_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      880 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/discovered_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      448 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/discovered_event_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      794 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/error_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      884 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/failure_operation_result_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      763 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/generic_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      515 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/get_stream_event_format_parameter.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      680 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_link.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      729 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_page_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     3036 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      813 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1210 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      736 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      810 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      822 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1337 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2378 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_type_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      716 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      708 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_self.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      788 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      762 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/halid_link.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1140 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/list_constraints200_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1815 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      906 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_location.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      536 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      628 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      596 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/nd_json_response_stream.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1124 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_enum_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      458 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_enum_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1094 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      456 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      154 2024-04-15 07:53:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      948 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      452 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      845 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1199 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object_results.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      951 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      704 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_next.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      704 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_prev.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      704 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_self.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      735 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_count.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      937 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_result.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1341 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1416 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_type_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:52:48.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/py.typed
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1666 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_change.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      492 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_change_change.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1093 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_changes_paged_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      881 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_creation_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1843 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1775 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_with_id_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      861 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_creation_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2701 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      564 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_id.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1135 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_listing.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1377 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      478 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metadata_event_all_of_object_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2349 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1145 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      483 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      492 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of1.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      458 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of2.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      587 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      564 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      607 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_parent.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1520 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_ref_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      472 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_ref_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1201 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_reference.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      862 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1455 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor_sensor.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      610 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1765 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_change.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_creation_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2277 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      581 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_id.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1112 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_listing.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2627 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_constraints.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2781 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_id_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1116 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_types_changes_paged_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2679 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_with_id_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1271 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resourcetype_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      494 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resourcetype_metadata_event_all_of_object_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      985 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/schema_validation_error.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      576 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/ss_event_stream.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1089 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_enum_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1158 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      452 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      787 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/success_operation_result_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      900 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      526 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1025 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/validation_failure.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      655 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/version_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      628 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/with_id_required.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.248467 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      645 2024-04-15 07:52:48.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      758 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/about_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1124 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/batch_operations_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1296 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/metadata_events_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:52:48.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/py.typed
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    10002 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2862 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_constraint_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     6976 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_type_api.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.258751 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     5024 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     8840 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/SOURCES.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/dependency_links.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      326 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/requires.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/LICENSE.txt` & `waylay_sdk_resources_types-8.1.0a20240415/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/PKG-INFO` & `waylay_sdk_resources_types-8.1.0a20240415/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources-types
-Version: 8.1.0.20240423
+Version: 8.1.0a20240415
 Summary: Waylay Resources Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -20,16 +20,16 @@
 Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-resources==8.1.0.20240423
+Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk-resources==8.1.0a20240415
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/README.md` & `waylay_sdk_resources_types-8.1.0a20240415/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/pyproject.toml` & `waylay_sdk_resources_types-8.1.0a20240415/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-resources-types"
-version = "8.1.0.20240423"
+version = "8.1.0a20240415"
 description = "Waylay Resources Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Resources" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
-    "waylay-sdk-resources == 8.1.0.20240423",
+    "waylay-sdk-core ~= 0.2.0",
+    "waylay-sdk-resources == 8.1.0a20240415",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/__init__.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This service manages  [Waylay Resources](/#/features/resources/?id=resource) and related entities.  A _Waylay Resource_ models a real-world device or abstract entity of your IoT solution, and provides a context when processing data in the Rule Engine.  You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model,  a process that's also called _resource provisioning_.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "8.1.0.20240423"
+__version__ = "8.1.0a20240415"
 
 # import models into model package
 from .array_must_contain_inner import ArrayMustContainInner
 from .array_value_constraint import ArrayValueConstraint
 from .array_value_constraint_type import ArrayValueConstraintType
 from .attribute_item import AttributeItem
 from .batch_operation_enqueued import BatchOperationEnqueued
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/array_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_value_constraint.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,9 +46,12 @@
     )
     contains: List[ArrayMustContainInner] | None = Field(
         default=None,
         description="Only supported if the `elementType` is `boolean`, `numeric` or `string`. Specifies values the array attribute must contain.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/attribute_item.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/halid_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
-from waylay.sdk.api._models import Model as GenericModel
 
 
-class AttributeItem(WaylayBaseModel):
-    """Constraint on the presence and value of a single named _Resource_ attribute.."""
+class HALIdLink(WaylayBaseModel):
+    """HALIdLink."""
 
-    name: StrictStr = Field(description="name of the attribute")
-    required: StrictBool = Field(
-        description="Indicates if the attribute must be present or is optional"
-    )
-    type: GenericModel
+    href: StrictStr = Field(description="(Relative) URL of the entity.")
+    id: StrictStr = Field(description="Unique identifier of the linked item")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_operation_enqueued.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_value.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,27 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictInt,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.batch_running_resource_operation import BatchRunningResourceOperation
 
+class HALSelfLinksLinksValue(WaylayBaseModel):
+    """HALSelfLinksLinksValue."""
 
-class BatchOperationEnqueued(WaylayBaseModel):
-    """BatchOperationEnqueued."""
-
-    status_code: StrictInt = Field(alias="statusCode")
-    uri: StrictStr = Field(
-        description="URI where the batch operation status can be followed"
-    )
-    entity: BatchRunningResourceOperation
+    href: StrictStr = Field(description="(Relative) URL of the entity.")
+    id: StrictStr = Field(description="Unique identifier of the linked item")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_operation_result.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,37 +24,37 @@
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.batch_running_resource_operation_operation import (
     BatchRunningResourceOperationOperation,
 )
-from ..models.operation_result_object_results import OperationResultObjectResults
 
 
-class BatchOperationResult(WaylayBaseModel):
-    """BatchOperationResult."""
+class BatchRunningResourceOperation(WaylayBaseModel):
+    """BatchRunningResourceOperation."""
 
     id: StrictStr
     user: Annotated[str, Field(strict=True)] = Field(
         description="User subject id in the Waylay Accounts database"
     )
     queue_time: datetime = Field(alias="queueTime")
     operation: BatchRunningResourceOperationOperation
-    finished_time: datetime = Field(alias="finishedTime")
-    results: OperationResultObjectResults
 
     @field_validator("user")
     @classmethod
     def user_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(
             r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value
         ):
             raise ValueError(
                 r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_operation_status_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_status_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """BatchResourceOperation."""
 
     entity: BatchResourceOperationEntity
     action: BatchResourceOperationAction
     query: BatchResourceOperationQuery
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation_query.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,9 +29,12 @@
 
 class BatchResourceOperationQuery(WaylayBaseModel):
     """BatchResourceOperationQuery."""
 
     ids: Annotated[List[BatchResourceOperationQueryIdsInner], Field(min_length=1)]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_running_resource_operation.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_change.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,45 +13,48 @@
 
 import re
 from datetime import datetime
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.batch_running_resource_operation_operation import (
-    BatchRunningResourceOperationOperation,
-)
-
+from ..models.resource_change_change import ResourceChangeChange
+from ..models.resource_id import ResourceId
+from ..models.resource_with_id_entity import ResourceWithIdEntity
 
-class BatchRunningResourceOperation(WaylayBaseModel):
-    """BatchRunningResourceOperation."""
 
-    id: StrictStr
-    user: Annotated[str, Field(strict=True)] = Field(
-        description="User subject id in the Waylay Accounts database"
+class ResourceChange(WaylayBaseModel):
+    """ResourceChange."""
+
+    time: datetime
+    resource_id: ResourceId = Field(alias="resourceId")
+    user_id: Annotated[str, Field(strict=True)] = Field(
+        description="User subject id in the Waylay Accounts database", alias="userId"
     )
-    queue_time: datetime = Field(alias="queueTime")
-    operation: BatchRunningResourceOperationOperation
+    change: ResourceChangeChange
+    resource: ResourceWithIdEntity | None = None
 
-    @field_validator("user")
+    @field_validator("user_id")
     @classmethod
-    def user_validate_regular_expression(cls, value):
+    def user_id_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(
             r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value
         ):
             raise ValueError(
                 r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_running_resource_operation_operation.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     """Queued operation summary."""
 
     entity: BatchRunningResourceOperationOperationEntity
     action: BatchResourceOperationAction
     description: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/boolean_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/boolean_value_constraint.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class BooleanValueConstraint(WaylayBaseModel):
     """Specifies that the value must be a boolean."""
 
     type: BooleanValueConstraintType | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/changed_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/changed_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     old_values: Dict[str, Any] | None = Field(
         default=None,
         description="old values of all attributes that have changed",
         alias="oldValues",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     source: CloudMetadataEventDataSource
     subject: Dict[str, Any]
     type: CloudMetadataEventDataType
     data: MetadataEvent | None = None
     time: datetime
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event_data.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     source: CloudMetadataEventDataSource | None = None
     subject: Any | None = None
     type: CloudMetadataEventDataType | None = None
     data: MetadataEvent | None = None
     time: datetime | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event_data_source.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_source.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/cloud_metadata_event_data_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,9 +36,12 @@
         default=None, description="A description for the _Resource Constraint_"
     )
     attributes: List[AttributeItem] = Field(
         description="List of attribute descriptions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint_error.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     error: StrictStr = Field(description="User error message")
     error_path: StrictStr = Field(description="Attribute path", alias="errorPath")
     resources: List[ResourceId] = Field(
         description="Ids of the _Resources_ that fail the constraint"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/constraint_status.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,9 +47,12 @@
         ):
             raise ValueError(
                 r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/create_delete_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/create_delete_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class CreateDeleteEvent(WaylayBaseModel):
     """CreateDeleteEvent."""
 
     type: CreateDeleteEventType | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/discovered_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/discovered_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,9 +27,12 @@
 
     type: DiscoveredEventType | None = None
     message: Dict[str, Any] | None = Field(
         default=None, description="The broker message that triggered the discovery"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/error_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/error_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,9 +24,12 @@
     """ErrorResponse."""
 
     status_code: StrictInt = Field(alias="statusCode")
     error: StrictStr
     code: StrictStr | None = Field(default=None, description="Optional error code")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/failure_operation_result_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_next.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictInt,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class FailureOperationResultValue(WaylayBaseModel):
-    """The keys will be resource ids or resource type ids.."""
+class PaginationLinksNext(WaylayBaseModel):
+    """PaginationLinksNext."""
 
-    status_code: StrictInt = Field(
-        description="The statusCode of the operation", alias="statusCode"
-    )
-    error: StrictStr = Field(description="Error description of what went wrong.")
+    href: StrictStr = Field(description="(Relative) URL of the entity.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/generic_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/generic_metadata_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """GenericMetadataEvent."""
 
     type: StrictStr
     object_type: StrictStr = Field(alias="objectType")
     timestamp: datetime
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/get_stream_event_format_parameter.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/get_stream_event_format_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_link.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_link.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class HALLink(WaylayBaseModel):
     """HALLink."""
 
     href: StrictStr = Field(description="(Relative) URL of the entity.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_page_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_prev.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.pagination_links import PaginationLinks
 
+class PaginationLinksPrev(WaylayBaseModel):
+    """PaginationLinksPrev."""
 
-class HALPageLinks(WaylayBaseModel):
-    """HALPageLinks."""
-
-    links: PaginationLinks | None = Field(default=None, alias="_links")
+    href: StrictStr = Field(description="(Relative) URL of the entity.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,12 @@
         description="Set of sensors that are applicable for a given _Resource_. Please note that there is no explicit action taken by the Waylay platform on this meta key. The idea behind this abstraction is to assist integrations where an architect of the digital twin can specify which sensors from waylay library are applicable for a given _Resource_ (or _Resource Type_).",
     )
     embedded: HALResourceEntityAllOfEmbedded | None = Field(
         default=None, alias="_embedded"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,9 +24,12 @@
     """HALResourceEntityAllOfEmbedded."""
 
     resource_type: HALResourceTypeEntity | None = Field(
         default=None, alias="resourceType"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,9 +34,12 @@
     parent: HALResourceEntityAllOfLinksParent | None = None
     children: HALResourceEntityAllOfLinksChildren | None = None
     resource_type: HALResourceEntityAllOfLinksResourceType | None = Field(
         default=None, alias="resourceType"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.hal_self_links_links import HALSelfLinksLinks
 
-class HALResourceEntityAllOfLinksChildren(WaylayBaseModel):
-    """HALResourceEntityAllOfLinksChildren."""
 
-    href: StrictStr = Field(description="(Relative) URL of the entity.")
+class HALSelfLinks(WaylayBaseModel):
+    """HALSelfLinks."""
+
+    links: HALSelfLinksLinks = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 class HALResourceEntityAllOfLinksParent(WaylayBaseModel):
     """HALResourceEntityAllOfLinksParent."""
 
     href: StrictStr = Field(description="(Relative) URL of the entity.")
     id: StrictStr = Field(description="Unique identifier of the linked item")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class HALResourceEntityAllOfLinksResourceType(WaylayBaseModel):
-    """HALResourceEntityAllOfLinksResourceType."""
+class HALResourceEntityAllOfLinksChildren(WaylayBaseModel):
+    """HALResourceEntityAllOfLinksChildren."""
 
     href: StrictStr = Field(description="(Relative) URL of the entity.")
-    id: StrictStr = Field(description="Unique identifier of the linked item")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_listing.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,9 +35,12 @@
         description="Total number of items matching the query of which this is one page of results."
     )
     count: StrictInt = Field(description="The number of items in this result page.")
     links: PaginationLinks = Field(alias="_links")
     embedded: HALResourceListingAllOfEmbedded = Field(alias="_embedded")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """HALResourceListingAllOfEmbedded."""
 
     values: List[HALResourceEntity] = Field(
         description="_Resource_ entities in HAL format"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_resource_type_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_type_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,9 +51,12 @@
     )
     sensors: List[ResourceSensor] | None = Field(
         default=None,
         description="Set of sensors that are applicable for a given _Resource_. Please note that there is no explicit action taken by the Waylay platform on this meta key. The idea behind this abstraction is to assist integrations where an architect of the digital twin can specify which sensors from waylay library are applicable for a given _Resource_ (or _Resource Type_).",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_parent.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_self_links_links import HALSelfLinksLinks
 
-
-class HALSelfLinks(WaylayBaseModel):
-    """HALSelfLinks."""
-
-    links: HALSelfLinksLinks = Field(alias="_links")
+class ResourceParent(WaylayBaseModel):
+    """Id of the parent _Resource_."""
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_self_links_links_self import HALSelfLinksLinksSelf
+from ..models.task_configuration_type import TaskConfigurationType
 
 
-class HALSelfLinksLinks(WaylayBaseModel):
-    """Links to related objects."""
+class TaskConfiguration(WaylayBaseModel):
+    """Specification of a template and task creation attributes for the task that gets instantiate when a _Resource_ created.."""
 
-    var_self: HALSelfLinksLinksSelf = Field(alias="self")
+    template_name: StrictStr = Field(alias="templateName")
+    type: TaskConfigurationType | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links_links_self.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_self.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class HALSelfLinksLinksSelf(WaylayBaseModel):
     """HALSelfLinksLinksSelf."""
 
     href: StrictStr = Field(description="(Relative) URL of the entity.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/hal_self_links_links_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_page_links.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.pagination_links import PaginationLinks
 
-class HALSelfLinksLinksValue(WaylayBaseModel):
-    """HALSelfLinksLinksValue."""
 
-    href: StrictStr = Field(description="(Relative) URL of the entity.")
-    id: StrictStr = Field(description="Unique identifier of the linked item")
+class HALPageLinks(WaylayBaseModel):
+    """HALPageLinks."""
+
+    links: PaginationLinks | None = Field(default=None, alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/halid_link.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/success_operation_result_value.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
+    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class HALIdLink(WaylayBaseModel):
-    """HALIdLink."""
+class SuccessOperationResultValue(WaylayBaseModel):
+    """The keys will be resource ids or resource type ids.."""
 
-    href: StrictStr = Field(description="(Relative) URL of the entity.")
-    id: StrictStr = Field(description="Unique identifier of the linked item")
+    status_code: StrictInt = Field(
+        description="The statusCode of the operation", alias="statusCode"
+    )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/list_constraints200_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/list_constraints200_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     limit: StrictInt = Field(description="Size of one page of results.")
     total: StrictInt = Field(
         description="Total number of items matching the query of which this is one page of results."
     )
     values: List[ResourceConstraintWithIdEntity] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,9 +39,12 @@
     )
     sensors: List[ResourceSensor] | None = Field(
         default=None,
         description="Set of sensors that are applicable for a given _Resource_. Please note that there is no explicit action taken by the Waylay platform on this meta key. The idea behind this abstraction is to assist integrations where an architect of the digital twin can specify which sensors from waylay library are applicable for a given _Resource_ (or _Resource Type_).",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_entity_location.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_location.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,12 @@
         description="The latitude degrees of a location."
     )
     lon: StrictFloat | StrictInt = Field(
         description="The longitudinal degrees of a location."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_entity_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/nd_json_response_stream.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/nd_json_response_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/numeric_enum_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_enum_value_constraint.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictFloat,
-    StrictInt,
+    StrictStr,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.numeric_enum_value_constraint_type import NumericEnumValueConstraintType
-from ..models.numeric_value_constraint_type import NumericValueConstraintType
+from ..models.string_value_constraint_type import StringValueConstraintType
 
 
-class NumericEnumValueConstraint(WaylayBaseModel):
-    """Specifies that a value must be one of the given numbers.."""
+class StringEnumValueConstraint(WaylayBaseModel):
+    """Specifies that a value must be one of the given strings.."""
 
     type: NumericEnumValueConstraintType
-    enum_type: NumericValueConstraintType = Field(alias="enumType")
-    items: Annotated[List[StrictFloat | StrictInt], Field(min_length=1)]
+    enum_type: StringValueConstraintType = Field(alias="enumType")
+    items: Annotated[List[StrictStr], Field(min_length=1)]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/numeric_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_value_constraint.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,9 +30,12 @@
         default=None, description="Specifies the minimum value the attribute can have"
     )
     maximum: StrictFloat | StrictInt | None = Field(
         default=None, description="Specifies the maximum value the attribute can have"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/object_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object_value_constraint.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 class ObjectValueConstraint(WaylayBaseModel):
     """Specifies that a value must be an object and which attributes it needs to have."""
 
     type: ObjectValueConstraintType
     attributes: List[AttributeItem] = Field(description="Attributes descriptions")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/operation_result_object.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,27 +7,22 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from datetime import datetime
-
 from pydantic import (
     ConfigDict,
-    Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.operation_result_object_results import OperationResultObjectResults
-
-
-class OperationResultObject(WaylayBaseModel):
-    """Finished Batch Operation results."""
 
-    finished_time: datetime = Field(alias="finishedTime")
-    results: OperationResultObjectResults
+class ResourceType(WaylayBaseModel):
+    """Id of the linked _Resource Type_."""
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/operation_result_object_results.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,9 +30,12 @@
         description="Object containing the successful operation results.  The keys will be resource ids or resource type ids."
     )
     failure: Dict[str, FailureOperationResultValue] = Field(
         description="Object containing the unsuccessful operation results.  The keys will be resource ids or resource type ids."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """HAL links for pagination."""
 
     var_self: PaginationLinksSelf = Field(alias="self")
     next: PaginationLinksNext | None = None
     prev: PaginationLinksPrev | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links_next.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_self.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class PaginationLinksNext(WaylayBaseModel):
-    """PaginationLinksNext."""
+class PaginationLinksSelf(WaylayBaseModel):
+    """PaginationLinksSelf."""
 
     href: StrictStr = Field(description="(Relative) URL of the entity.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links_prev.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/version_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class PaginationLinksPrev(WaylayBaseModel):
-    """PaginationLinksPrev."""
+class VersionResponse(WaylayBaseModel):
+    """VersionResponse."""
 
-    href: StrictStr = Field(description="(Relative) URL of the entity.")
+    name: StrictStr
+    version: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/pagination_links_self.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.hal_self_links_links_self import HALSelfLinksLinksSelf
 
-class PaginationLinksSelf(WaylayBaseModel):
-    """PaginationLinksSelf."""
 
-    href: StrictStr = Field(description="(Relative) URL of the entity.")
+class HALSelfLinksLinks(WaylayBaseModel):
+    """Links to related objects."""
+
+    var_self: HALSelfLinksLinksSelf = Field(alias="self")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/paging_count.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_count.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,9 +23,12 @@
     """PagingCount."""
 
     count: StrictInt | None = Field(
         default=None, description="The number of items in this result page."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/paging_result.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     )
     limit: StrictInt = Field(description="Size of one page of results.")
     total: StrictInt = Field(
         description="Total number of items matching the query of which this is one page of results."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/patch_resource_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,9 +40,12 @@
     customer: Any | None = None
     firmware: Any | None = None
     location: Any | None = None
     metrics: Any | None = None
     sensors: Any | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/patch_resource_type_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_type_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,9 +41,12 @@
     constraints: List[Annotated[str, Field(strict=True)]] | None = Field(
         default=None,
         description="Validation constraint to be applied to each _Resource_ that has its `resourceTypeId` attribute set to the `id` of this _Resource Type_.",
         alias="$constraints",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_change.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_change.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,37 +21,42 @@
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.resource_change_change import ResourceChangeChange
-from ..models.resource_id import ResourceId
-from ..models.resource_with_id_entity import ResourceWithIdEntity
+from ..models.resource_type_id import ResourceTypeId
+from ..models.resource_type_with_id_entity import ResourceTypeWithIdEntity
 
 
-class ResourceChange(WaylayBaseModel):
-    """ResourceChange."""
+class ResourceTypeChange(WaylayBaseModel):
+    """ResourceTypeChange."""
 
     time: datetime
-    resource_id: ResourceId = Field(alias="resourceId")
+    resource_type_id: ResourceTypeId = Field(alias="resourceTypeId")
     user_id: Annotated[str, Field(strict=True)] = Field(
         description="User subject id in the Waylay Accounts database", alias="userId"
     )
     change: ResourceChangeChange
-    resource: ResourceWithIdEntity | None = None
+    resource_type: ResourceTypeWithIdEntity | None = Field(
+        default=None, alias="resourceType"
+    )
 
     @field_validator("user_id")
     @classmethod
     def user_id_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(
             r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value
         ):
             raise ValueError(
                 r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_changes_paged_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_changes_paged_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     limit: StrictInt = Field(description="Size of one page of results.")
     total: StrictInt = Field(
         description="Total number of items matching the query of which this is one page of results."
     )
     values: List[ResourceChange] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_constraint_creation_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_creation_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """ResourceConstraintCreationResponse."""
 
     status_code: StrictInt = Field(alias="statusCode")
     uri: StrictStr
     entity: ResourceConstraintWithIdEntity
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_constraint_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,9 +56,12 @@
         ):
             raise ValueError(
                 r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_constraint_with_id_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_with_id_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,9 +53,12 @@
         ):
             raise ValueError(
                 r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_creation_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/with_id_required.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,23 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictFloat,
-    StrictInt,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.resource_with_id_entity import ResourceWithIdEntity
 
+class WithIdRequired(WaylayBaseModel):
+    """WithIdRequired."""
 
-class ResourceCreationResponse(WaylayBaseModel):
-    """ResourceCreationResponse."""
-
-    status_code: StrictFloat | StrictInt = Field(alias="statusCode")
-    uri: StrictStr
-    entity: ResourceWithIdEntity
+    id: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,9 +57,12 @@
     )
     owner: StrictStr | None = Field(default=None, description="Owner of the _Resource_")
     tags: List[StrictStr] | None = Field(
         default=None, description="Custom classifiers for this _Resource_."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_id.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_listing.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_listing.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     limit: StrictInt = Field(description="Size of one page of results.")
     total: StrictInt = Field(
         description="Total number of items matching the query of which this is one page of results."
     )
     values: List[ResourceWithIdEntity] = Field(description="_Resource_ entities")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metadata_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,9 +40,12 @@
         alias="oldValues",
     )
     message: Dict[str, Any] | None = Field(
         default=None, description="The broker message that triggered the discovery"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,9 +50,12 @@
         default=None, description="Expected maximum value for this metric."
     )
     minimum: StrictFloat | StrictInt | None = Field(
         default=None, description="Expected minimum value for this metric."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_ref_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_ref_value_constraint.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,9 +40,12 @@
     )
     exists: StrictBool | None = Field(
         default=False,
         description="Flag to indicate if the referenced _Resource_ must exist",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_reference.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_reference.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,9 +37,12 @@
     def ref_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^\/resources\/.*", value):
             raise ValueError(r"must validate the regular expression /^\/resources\/.*/")
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_sensor.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 
     name: StrictStr = Field(
         description="An alias name for the sensor in the context of this _Resource_."
     )
     sensor: ResourceSensorSensor
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_sensor_sensor.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor_sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,9 +44,12 @@
         if value is None:
             return value
         if not re.match(r"\d+\.\d+\.\d+", value):
             raise ValueError(r"must validate the regular expression /\d+\.\d+\.\d+/")
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_creation_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/attribute_item.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictFloat,
-    StrictInt,
+    StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
+from waylay.sdk.api._models import Model as GenericModel
 
-from ..models.resource_type_with_id_entity import ResourceTypeWithIdEntity
 
+class AttributeItem(WaylayBaseModel):
+    """Constraint on the presence and value of a single named _Resource_ attribute.."""
 
-class ResourceTypeCreationResponse(WaylayBaseModel):
-    """ResourceTypeCreationResponse."""
-
-    status_code: StrictFloat | StrictInt = Field(alias="statusCode")
-    uri: StrictStr
-    entity: ResourceTypeWithIdEntity
+    name: StrictStr = Field(description="name of the attribute")
+    required: StrictBool = Field(
+        description="Indicates if the attribute must be present or is optional"
+    )
+    type: GenericModel
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,9 +49,12 @@
     )
     templates: List[TaskConfiguration] | None = Field(
         default=None,
         description="Templates for task that is automatically created whenever a new  _Resource_ of this _Resource Type_ is created.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_id.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_id.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_listing.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_listing.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     limit: StrictInt = Field(description="Size of one page of results.")
     total: StrictInt = Field(
         description="Total number of items matching the query of which this is one page of results."
     )
     values: List[ResourceTypeWithIdEntity]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_with_constraints.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_constraints.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,9 +57,12 @@
     constraints: List[Annotated[str, Field(strict=True)]] | None = Field(
         default=None,
         description="Validation constraint to be applied to each _Resource_ that has its `resourceTypeId` attribute set to the `id` of this _Resource Type_.",
         alias="$constraints",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_type_with_id_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_id_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,9 +60,12 @@
     constraints: List[ConstraintStatus] | None = Field(
         default=None,
         description="Validation constraint as applied to each _Resource_ that has its `resourceTypeId` attribute set to the `id` of this _Resource Type_.",
         alias="$constraints",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_types_changes_paged_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/validation_failure.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 
 from typing import List
 
 from pydantic import (
     ConfigDict,
     Field,
     StrictInt,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.resource_type_change import ResourceTypeChange
+from ..models.schema_validation_error import SchemaValidationError
 
 
-class ResourceTypesChangesPagedResponse(WaylayBaseModel):
-    """ResourceTypesChangesPagedResponse."""
+class ValidationFailure(WaylayBaseModel):
+    """ValidationFailure."""
 
-    skip: StrictInt = Field(
-        description="Number of items skipped before this page of results."
+    status_code: StrictInt = Field(alias="statusCode")
+    error: StrictStr
+    code: StrictStr | None = Field(default=None, description="Optional error code")
+    details: List[SchemaValidationError] | None = Field(
+        default=None, description="List of SchemaValidationErrors"
     )
-    limit: StrictInt = Field(description="Size of one page of results.")
-    total: StrictInt = Field(
-        description="Total number of items matching the query of which this is one page of results."
-    )
-    values: List[ResourceTypeChange] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resource_with_id_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_with_id_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,9 +57,12 @@
     )
     sensors: List[ResourceSensor] | None = Field(
         default=None,
         description="Set of sensors that are applicable for a given _Resource_. Please note that there is no explicit action taken by the Waylay platform on this meta key. The idea behind this abstraction is to assist integrations where an architect of the digital twin can specify which sensors from waylay library are applicable for a given _Resource_ (or _Resource Type_).",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/resourcetype_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resourcetype_metadata_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,12 @@
         default=None,
         description="old values of all attributes that have changed",
         alias="oldValues",
     )
     resourcetype: ResourceTypeEntity
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/schema_validation_error.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/schema_validation_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     errors: Dict[str, Any] | None = None
     keyword: StrictStr | None = None
     msgs: List[StrictStr] | None = None
     value: Dict[str, Any] | None = None
     instance_path: StrictStr | None = Field(default=None, alias="instancePath")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/ss_event_stream.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/ss_event_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/string_enum_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_enum_value_constraint.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
+    StrictFloat,
+    StrictInt,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.numeric_enum_value_constraint_type import NumericEnumValueConstraintType
-from ..models.string_value_constraint_type import StringValueConstraintType
+from ..models.numeric_value_constraint_type import NumericValueConstraintType
 
 
-class StringEnumValueConstraint(WaylayBaseModel):
-    """Specifies that a value must be one of the given strings.."""
+class NumericEnumValueConstraint(WaylayBaseModel):
+    """Specifies that a value must be one of the given numbers.."""
 
     type: NumericEnumValueConstraintType
-    enum_type: StringValueConstraintType = Field(alias="enumType")
-    items: Annotated[List[StrictStr], Field(min_length=1)]
+    enum_type: NumericValueConstraintType = Field(alias="enumType")
+    items: Annotated[List[StrictFloat | StrictInt], Field(min_length=1)]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/string_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_value_constraint.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,9 +31,12 @@
         default=None, description="Minimum length a value must have", alias="minLength"
     )
     max_length: Annotated[int, Field(strict=True, ge=0)] | None = Field(
         default=None, description="Maximum length a value can have", alias="maxLength"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/success_operation_result_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_enqueued.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,21 +11,29 @@
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
     StrictInt,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.batch_running_resource_operation import BatchRunningResourceOperation
 
-class SuccessOperationResultValue(WaylayBaseModel):
-    """The keys will be resource ids or resource type ids.."""
 
-    status_code: StrictInt = Field(
-        description="The statusCode of the operation", alias="statusCode"
+class BatchOperationEnqueued(WaylayBaseModel):
+    """BatchOperationEnqueued."""
+
+    status_code: StrictInt = Field(alias="statusCode")
+    uri: StrictStr = Field(
+        description="URI where the batch operation status can be followed"
     )
+    entity: BatchRunningResourceOperation
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/task_configuration.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.task_configuration_type import TaskConfigurationType
 
+class HALResourceEntityAllOfLinksResourceType(WaylayBaseModel):
+    """HALResourceEntityAllOfLinksResourceType."""
 
-class TaskConfiguration(WaylayBaseModel):
-    """Specification of a template and task creation attributes for the task that gets instantiate when a _Resource_ created.."""
-
-    template_name: StrictStr = Field(alias="templateName")
-    type: TaskConfigurationType | None = None
+    href: StrictStr = Field(description="(Relative) URL of the entity.")
+    id: StrictStr = Field(description="Unique identifier of the linked item")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/models/task_configuration_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/__init__.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/about_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/about_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,13 @@
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
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/batch_operations_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/batch_operations_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
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
 
 
@@ -35,12 +36,13 @@
     return field_name
 
 
 class StartQuery(WaylayBaseModel):
     """Model for `start` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_start_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/metadata_events_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/metadata_events_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,12 +35,13 @@
         GetStreamEventFormatParameter | None,
         Field(
             description="The format of events in the stream.   If specified this must be `application/cloudevents+json` (make sure to correctly URL encode the `+` as `%2B`)"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_stream_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/resource_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
 
 
@@ -47,14 +48,15 @@
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
 
 
@@ -87,14 +89,15 @@
         List[StrictStr] | None,
         Field(
             description="Select which attributes to render for each matching _Resource_ (comma-separated)."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -113,14 +116,15 @@
         StrictInt | None, Field(description="(Paging) items to skip in the listing")
     ] = None
     limit: Annotated[
         StrictInt | None, Field(description="(Paging) maximal number of items returned")
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_changes_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -163,14 +167,15 @@
         StrictInt | None, Field(description="(Paging) items to skip in the listing")
     ] = None
     limit: Annotated[
         StrictInt | None, Field(description="(Paging) maximal number of items returned")
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_children_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -205,14 +210,15 @@
         StrictInt | None, Field(description="(Paging) items to skip in the listing")
     ] = None
     limit: Annotated[
         StrictInt | None, Field(description="(Paging) maximal number of items returned")
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_referrers_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -290,14 +296,15 @@
     distance: StrictStr | None = None
     toplevel_only: Annotated[
         StrictBool | None,
         Field(description="If true, search only for _Resources_ without parent."),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -305,14 +312,15 @@
     return field_name
 
 
 class PatchQuery(WaylayBaseModel):
     """Model for `patch` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_patch_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -320,12 +328,13 @@
     return field_name
 
 
 class ReplaceQuery(WaylayBaseModel):
     """Model for `replace` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_replace_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/resource_constraint_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_constraint_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,15 @@
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
 
 
@@ -41,14 +42,15 @@
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
 
 
@@ -56,14 +58,15 @@
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
 
 
@@ -87,14 +90,15 @@
         StrictInt | None, Field(description="(Paging) maximal number of items returned")
     ] = None
     filter: Annotated[
         StrictStr | None, Field(description="(Filter) fuzzy search on multiple fields.")
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -102,12 +106,13 @@
     return field_name
 
 
 class ReplaceQuery(WaylayBaseModel):
     """Model for `replace` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_replace_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay/services/resources/queries/resource_type_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_type_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
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
 
 
@@ -45,14 +46,15 @@
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
 
 
@@ -77,14 +79,15 @@
         List[StrictStr] | None,
         Field(
             description="Select which attributes to render for each matching _Resource_ (comma-separated)."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -103,14 +106,15 @@
         StrictInt | None, Field(description="(Paging) items to skip in the listing")
     ] = None
     limit: Annotated[
         StrictInt | None, Field(description="(Paging) maximal number of items returned")
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_changes_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -118,14 +122,15 @@
     return field_name
 
 
 class ListConstraintsQuery(WaylayBaseModel):
     """Model for `list_constraints` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_constraints_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -184,14 +189,15 @@
         StrictStr | None,
         Field(
             description="Return _Resource Types_ that are associated with the template."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -199,14 +205,15 @@
     return field_name
 
 
 class PatchQuery(WaylayBaseModel):
     """Model for `patch` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_patch_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -214,14 +221,15 @@
     return field_name
 
 
 class ReplaceQuery(WaylayBaseModel):
     """Model for `replace` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_replace_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -229,12 +237,13 @@
     return field_name
 
 
 class RevalidateQuery(WaylayBaseModel):
     """Model for `revalidate` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_revalidate_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/PKG-INFO` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources-types
-Version: 8.1.0.20240423
+Version: 8.1.0a20240415
 Summary: Waylay Resources Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -20,16 +20,16 @@
 Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-resources==8.1.0.20240423
+Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk-resources==8.1.0a20240415
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240423/src/waylay_sdk_resources_types.egg-info/SOURCES.txt` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

