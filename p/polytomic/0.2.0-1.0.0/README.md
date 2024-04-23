# Comparing `tmp/polytomic-0.2.0.tar.gz` & `tmp/polytomic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytomic-0.2.0.tar", max compression
+gzip compressed data, was "polytomic-1.0.0.tar", max compression
```

## Comparing `polytomic-0.2.0.tar` & `polytomic-1.0.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
--rw-r--r--   0        0        0     1066 2024-04-16 17:49:36.865207 polytomic-0.2.0/LICENSE
--rw-r--r--   0        0        0     1764 2024-04-16 17:49:36.865207 polytomic-0.2.0/README.md
--rw-r--r--   0        0        0      596 2024-04-16 17:49:36.869207 polytomic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7452 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/__init__.py
--rw-r--r--   0        0        0     7179 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/client.py
--rw-r--r--   0        0        0      790 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/api_error.py
--rw-r--r--   0        0        0     1936 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/request_options.py
--rw-r--r--   0        0        0      152 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/environment.py
--rw-r--r--   0        0        0      534 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/__init__.py
--rw-r--r--   0        0        0      348 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/bad_request_error.py
--rw-r--r--   0        0        0      347 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/forbidden_error.py
--rw-r--r--   0        0        0      352 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/internal_server_error.py
--rw-r--r--   0        0        0      346 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/not_found_error.py
--rw-r--r--   0        0        0      286 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/unauthorized_error.py
--rw-r--r--   0        0        0      357 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/py.typed
--rw-r--r--   0        0        0      460 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/__init__.py
--rw-r--r--   0        0        0      145 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/__init__.py
--rw-r--r--   0        0        0    75561 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/client.py
--rw-r--r--   0        0        0      136 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/executions/__init__.py
--rw-r--r--   0        0        0    11087 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/executions/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/schemas/__init__.py
--rw-r--r--   0        0        0    26486 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/connections/__init__.py
--rw-r--r--   0        0        0    54184 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/connections/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/events/__init__.py
--rw-r--r--   0        0        0    13121 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/events/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/identity/__init__.py
--rw-r--r--   0        0        0     5538 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/identity/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/jobs/__init__.py
--rw-r--r--   0        0        0     6731 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/jobs/client.py
--rw-r--r--   0        0        0      125 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/__init__.py
--rw-r--r--   0        0        0    92987 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/client.py
--rw-r--r--   0        0        0      116 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/resources/executions/__init__.py
--rw-r--r--   0        0        0    23586 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/resources/executions/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/models/__init__.py
--rw-r--r--   0        0        0    38479 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/models/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/organization/__init__.py
--rw-r--r--   0        0        0    33551 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/organization/client.py
--rw-r--r--   0        0        0      137 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/__init__.py
--rw-r--r--   0        0        0      849 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/client.py
--rw-r--r--   0        0        0      128 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/policies/__init__.py
--rw-r--r--   0        0        0    32163 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/policies/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/roles/__init__.py
--rw-r--r--   0        0        0    29695 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/roles/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/schemas/__init__.py
--rw-r--r--   0        0        0    24085 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/schemas/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/users/__init__.py
--rw-r--r--   0        0        0    38734 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/users/client.py
--rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/webhooks/__init__.py
--rw-r--r--   0        0        0    30810 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/webhooks/client.py
--rw-r--r--   0        0        0    10365 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/__init__.py
--rw-r--r--   0        0        0      998 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/activate_sync_envelope.py
--rw-r--r--   0        0        0      906 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/activate_sync_input.py
--rw-r--r--   0        0        0      967 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/activate_sync_output.py
--rw-r--r--   0        0        0     1010 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/api_error.py
--rw-r--r--   0        0        0      925 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/api_key_response.py
--rw-r--r--   0        0        0      988 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/api_key_response_envelope.py
--rw-r--r--   0        0        0      851 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_discover.py
--rw-r--r--   0        0        0     1756 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_execution_status.py
--rw-r--r--   0        0        0     1004 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_field.py
--rw-r--r--   0        0        0     1134 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_itemized_schedule.py
--rw-r--r--   0        0        0     1152 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_multi_schedule_configuration.py
--rw-r--r--   0        0        0     1407 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schedule.py
--rw-r--r--   0        0        0     1145 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schema.py
--rw-r--r--   0        0        0      971 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schema_envelope.py
--rw-r--r--   0        0        0     1337 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schema_execution_status.py
--rw-r--r--   0        0        0      763 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_selective_mode.py
--rw-r--r--   0        0        0     1060 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_dest.py
--rw-r--r--   0        0        0      980 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_dest_envelope.py
--rw-r--r--   0        0        0     1456 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_execution.py
--rw-r--r--   0        0        0     1000 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_execution_envelope.py
--rw-r--r--   0        0        0     1005 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_list_envelope.py
--rw-r--r--   0        0        0     1555 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_response.py
--rw-r--r--   0        0        0      996 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_response_envelope.py
--rw-r--r--   0        0        0     1429 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_schema_execution.py
--rw-r--r--   0        0        0     1024 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source.py
--rw-r--r--   0        0        0      988 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_envelope.py
--rw-r--r--   0        0        0      968 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_schema_envelope.py
--rw-r--r--   0        0        0     1063 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status.py
--rw-r--r--   0        0        0     1013 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status_envelope.py
--rw-r--r--   0        0        0     1013 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_status_envelope.py
--rw-r--r--   0        0        0     1133 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_status_response.py
--rw-r--r--   0        0        0      987 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/configuration_value.py
--rw-r--r--   0        0        0      976 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connect_card_response.py
--rw-r--r--   0        0        0     1008 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connect_card_response_envelope.py
--rw-r--r--   0        0        0     1039 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_list_response_envelope.py
--rw-r--r--   0        0        0     1051 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_meta.py
--rw-r--r--   0        0        0     1217 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_meta_response.py
--rw-r--r--   0        0        0      981 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_parameter_value.py
--rw-r--r--   0        0        0     1090 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_parameter_values_resp.py
--rw-r--r--   0        0        0     1088 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_parameter_values_response_envelope.py
--rw-r--r--   0        0        0     1022 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_response_envelope.py
--rw-r--r--   0        0        0     1344 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_response_schema.py
--rw-r--r--   0        0        0     1194 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_type.py
--rw-r--r--   0        0        0     1008 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_type_response_envelope.py
--rw-r--r--   0        0        0     1023 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_type_schema.py
--rw-r--r--   0        0        0     1047 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/create_connection_response_envelope.py
--rw-r--r--   0        0        0     1639 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/create_connection_response_schema.py
--rw-r--r--   0        0        0     1098 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/event.py
--rw-r--r--   0        0        0      941 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/event_types_envelope.py
--rw-r--r--   0        0        0      964 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/events_envelope.py
--rw-r--r--   0        0        0     1045 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_counts.py
--rw-r--r--   0        0        0      992 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_log_response.py
--rw-r--r--   0        0        0     1013 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_logs_response_envelope.py
--rw-r--r--   0        0        0     1867 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_status.py
--rw-r--r--   0        0        0     1019 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/filter.py
--rw-r--r--   0        0        0     1015 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_connection_meta_envelope.py
--rw-r--r--   0        0        0     1031 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_execution_response_envelope.py
--rw-r--r--   0        0        0     1379 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_execution_response_schema.py
--rw-r--r--   0        0        0     1027 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_identity_response_envelope.py
--rw-r--r--   0        0        0     1291 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_identity_response_schema.py
--rw-r--r--   0        0        0     1037 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_model_sync_source_meta_envelope.py
--rw-r--r--   0        0        0     1058 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/identity.py
--rw-r--r--   0        0        0      963 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/identity_function.py
--rw-r--r--   0        0        0     1143 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/job_response.py
--rw-r--r--   0        0        0      975 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/job_response_envelope.py
--rw-r--r--   0        0        0      118 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/jsonschema_form.py
--rw-r--r--   0        0        0      114 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/label_label.py
--rw-r--r--   0        0        0      980 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/list_bulk_schema.py
--rw-r--r--   0        0        0     1018 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/list_bulk_sync_executions_envelope.py
--rw-r--r--   0        0        0     1045 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/list_execution_response_envelope.py
--rw-r--r--   0        0        0     1017 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/list_model_sync_response_envelope.py
--rw-r--r--   0        0        0     1006 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/list_policies_response_envelope.py
--rw-r--r--   0        0        0      964 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/list_users_envelope.py
--rw-r--r--   0        0        0     1167 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/mode.py
--rw-r--r--   0        0        0     1221 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_field.py
--rw-r--r--   0        0        0      984 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_field_response.py
--rw-r--r--   0        0        0     1000 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_list_response_envelope.py
--rw-r--r--   0        0        0      978 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_model_field_request.py
--rw-r--r--   0        0        0     1135 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_relation.py
--rw-r--r--   0        0        0      968 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_relation_to.py
--rw-r--r--   0        0        0     1652 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_response.py
--rw-r--r--   0        0        0     1066 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_response_envelope.py
--rw-r--r--   0        0        0     1077 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_field.py
--rw-r--r--   0        0        0     1827 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_response.py
--rw-r--r--   0        0        0     1000 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_response_envelope.py
--rw-r--r--   0        0        0     1210 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_source_meta_response.py
--rw-r--r--   0        0        0     1086 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/organization.py
--rw-r--r--   0        0        0      978 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/organization_envelope.py
--rw-r--r--   0        0        0      992 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/organizations_envelope.py
--rw-r--r--   0        0        0     1059 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/override.py
--rw-r--r--   0        0        0      959 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/pick_value.py
--rw-r--r--   0        0        0      955 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/policy_action.py
--rw-r--r--   0        0        0     1160 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/policy_response.py
--rw-r--r--   0        0        0      987 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/policy_response_envelope.py
--rw-r--r--   0        0        0     1114 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/relation.py
--rw-r--r--   0        0        0      963 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/relation_to.py
--rw-r--r--   0        0        0     1331 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/rest_err_response.py
--rw-r--r--   0        0        0      996 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/role_list_response_envelope.py
--rw-r--r--   0        0        0     1048 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/role_response.py
--rw-r--r--   0        0        0      979 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/role_response_envelope.py
--rw-r--r--   0        0        0      995 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/run_after.py
--rw-r--r--   0        0        0     1298 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule.py
--rw-r--r--   0        0        0     1669 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_frequency.py
--rw-r--r--   0        0        0     1037 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_option_response.py
--rw-r--r--   0        0        0     1020 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_option_response_envelope.py
--rw-r--r--   0        0        0     1187 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_schedule_option.py
--rw-r--r--   0        0        0     1051 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema.py
--rw-r--r--   0        0        0     1072 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema_association.py
--rw-r--r--   0        0        0     1242 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema_field.py
--rw-r--r--   0        0        0      977 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema_records_response_envelope.py
--rw-r--r--   0        0        0      911 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/source.py
--rw-r--r--   0        0        0     1047 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/source_meta.py
--rw-r--r--   0        0        0     1040 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/start_model_sync_response_envelope.py
--rw-r--r--   0        0        0     1086 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/start_model_sync_response_schema.py
--rw-r--r--   0        0        0     1220 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/supported_mode.py
--rw-r--r--   0        0        0     1476 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/sync_destination_properties.py
--rw-r--r--   0        0        0      996 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/sync_status_envelope.py
--rw-r--r--   0        0        0     1166 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/sync_status_response.py
--rw-r--r--   0        0        0     1149 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target.py
--rw-r--r--   0        0        0     1487 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target_field.py
--rw-r--r--   0        0        0     1322 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target_response.py
--rw-r--r--   0        0        0      987 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target_response_envelope.py
--rw-r--r--   0        0        0     1038 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/user.py
--rw-r--r--   0        0        0      946 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/user_envelope.py
--rw-r--r--   0        0        0     1098 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/webhook.py
--rw-r--r--   0        0        0      958 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/webhook_envelope.py
--rw-r--r--   0        0        0      975 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/webhook_list_envelope.py
--rw-r--r--   0        0        0      623 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/work_task_status.py
--rw-r--r--   0        0        0       77 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/version.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 polytomic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-23 18:27:46.113371 polytomic-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1764 2024-04-23 18:27:46.113371 polytomic-1.0.0/README.md
+-rw-r--r--   0        0        0      596 2024-04-23 18:27:46.113371 polytomic-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7452 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/__init__.py
+-rw-r--r--   0        0        0     7179 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/client.py
+-rw-r--r--   0        0        0      790 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/api_error.py
+-rw-r--r--   0        0        0     1936 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/core/request_options.py
+-rw-r--r--   0        0        0      152 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/environment.py
+-rw-r--r--   0        0        0      534 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/bad_request_error.py
+-rw-r--r--   0        0        0      347 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/forbidden_error.py
+-rw-r--r--   0        0        0      352 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/internal_server_error.py
+-rw-r--r--   0        0        0      346 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/not_found_error.py
+-rw-r--r--   0        0        0      286 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      357 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/py.typed
+-rw-r--r--   0        0        0      460 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/__init__.py
+-rw-r--r--   0        0        0    74737 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/client.py
+-rw-r--r--   0        0        0      136 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/executions/__init__.py
+-rw-r--r--   0        0        0    11087 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/executions/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/schemas/__init__.py
+-rw-r--r--   0        0        0    26364 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/connections/__init__.py
+-rw-r--r--   0        0        0    53644 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/connections/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/events/__init__.py
+-rw-r--r--   0        0        0    13121 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/events/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/identity/__init__.py
+-rw-r--r--   0        0        0     5538 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/identity/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     6731 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/jobs/client.py
+-rw-r--r--   0        0        0      125 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/model_sync/__init__.py
+-rw-r--r--   0        0        0    90843 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/model_sync/client.py
+-rw-r--r--   0        0        0      116 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/model_sync/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/model_sync/resources/executions/__init__.py
+-rw-r--r--   0        0        0    23586 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/model_sync/resources/executions/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/models/__init__.py
+-rw-r--r--   0        0        0    38363 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/models/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/organization/__init__.py
+-rw-r--r--   0        0        0    32917 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/organization/client.py
+-rw-r--r--   0        0        0      137 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/client.py
+-rw-r--r--   0        0        0      128 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/resources/policies/__init__.py
+-rw-r--r--   0        0        0    31199 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/resources/policies/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/resources/roles/__init__.py
+-rw-r--r--   0        0        0    29695 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/permissions/resources/roles/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/schemas/__init__.py
+-rw-r--r--   0        0        0    24085 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/schemas/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/users/__init__.py
+-rw-r--r--   0        0        0    38786 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/users/client.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0    30882 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/resources/webhooks/client.py
+-rw-r--r--   0        0        0    10365 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/__init__.py
+-rw-r--r--   0        0        0      998 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/activate_sync_envelope.py
+-rw-r--r--   0        0        0      906 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/activate_sync_input.py
+-rw-r--r--   0        0        0      967 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/activate_sync_output.py
+-rw-r--r--   0        0        0     1010 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/api_error.py
+-rw-r--r--   0        0        0      925 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/api_key_response.py
+-rw-r--r--   0        0        0      988 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/api_key_response_envelope.py
+-rw-r--r--   0        0        0      851 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_discover.py
+-rw-r--r--   0        0        0     1756 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_execution_status.py
+-rw-r--r--   0        0        0     1004 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_field.py
+-rw-r--r--   0        0        0     1134 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_itemized_schedule.py
+-rw-r--r--   0        0        0     1152 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_multi_schedule_configuration.py
+-rw-r--r--   0        0        0     1407 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_schedule.py
+-rw-r--r--   0        0        0     1145 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_schema.py
+-rw-r--r--   0        0        0      971 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_schema_envelope.py
+-rw-r--r--   0        0        0     1337 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_schema_execution_status.py
+-rw-r--r--   0        0        0      763 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_selective_mode.py
+-rw-r--r--   0        0        0     1060 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_dest.py
+-rw-r--r--   0        0        0      980 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_dest_envelope.py
+-rw-r--r--   0        0        0     1456 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_execution.py
+-rw-r--r--   0        0        0     1000 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_execution_envelope.py
+-rw-r--r--   0        0        0     1005 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_list_envelope.py
+-rw-r--r--   0        0        0     1555 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_response.py
+-rw-r--r--   0        0        0      996 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_response_envelope.py
+-rw-r--r--   0        0        0     1429 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_schema_execution.py
+-rw-r--r--   0        0        0     1024 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_source.py
+-rw-r--r--   0        0        0      988 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_source_envelope.py
+-rw-r--r--   0        0        0      968 2024-04-23 18:27:46.113371 polytomic-1.0.0/src/polytomic/types/bulk_sync_source_schema_envelope.py
+-rw-r--r--   0        0        0     1063 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/bulk_sync_source_status.py
+-rw-r--r--   0        0        0     1013 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/bulk_sync_source_status_envelope.py
+-rw-r--r--   0        0        0     1013 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/bulk_sync_status_envelope.py
+-rw-r--r--   0        0        0     1133 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/bulk_sync_status_response.py
+-rw-r--r--   0        0        0      987 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/configuration_value.py
+-rw-r--r--   0        0        0      976 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connect_card_response.py
+-rw-r--r--   0        0        0     1008 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connect_card_response_envelope.py
+-rw-r--r--   0        0        0     1039 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_list_response_envelope.py
+-rw-r--r--   0        0        0     1051 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_meta.py
+-rw-r--r--   0        0        0     1217 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_meta_response.py
+-rw-r--r--   0        0        0      981 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_parameter_value.py
+-rw-r--r--   0        0        0     1090 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_parameter_values_resp.py
+-rw-r--r--   0        0        0     1088 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_parameter_values_response_envelope.py
+-rw-r--r--   0        0        0     1022 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_response_envelope.py
+-rw-r--r--   0        0        0     1344 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_response_schema.py
+-rw-r--r--   0        0        0     1194 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_type.py
+-rw-r--r--   0        0        0     1008 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_type_response_envelope.py
+-rw-r--r--   0        0        0     1023 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/connection_type_schema.py
+-rw-r--r--   0        0        0     1047 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/create_connection_response_envelope.py
+-rw-r--r--   0        0        0     1639 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/create_connection_response_schema.py
+-rw-r--r--   0        0        0     1098 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/event.py
+-rw-r--r--   0        0        0      941 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/event_types_envelope.py
+-rw-r--r--   0        0        0      964 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/events_envelope.py
+-rw-r--r--   0        0        0     1045 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/execution_counts.py
+-rw-r--r--   0        0        0      992 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/execution_log_response.py
+-rw-r--r--   0        0        0     1013 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/execution_logs_response_envelope.py
+-rw-r--r--   0        0        0     1867 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/execution_status.py
+-rw-r--r--   0        0        0     1019 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/filter.py
+-rw-r--r--   0        0        0     1015 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/get_connection_meta_envelope.py
+-rw-r--r--   0        0        0     1031 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/get_execution_response_envelope.py
+-rw-r--r--   0        0        0     1379 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/get_execution_response_schema.py
+-rw-r--r--   0        0        0     1027 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/get_identity_response_envelope.py
+-rw-r--r--   0        0        0     1291 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/get_identity_response_schema.py
+-rw-r--r--   0        0        0     1037 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/get_model_sync_source_meta_envelope.py
+-rw-r--r--   0        0        0     1058 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/identity.py
+-rw-r--r--   0        0        0      963 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/identity_function.py
+-rw-r--r--   0        0        0     1143 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/job_response.py
+-rw-r--r--   0        0        0      975 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/job_response_envelope.py
+-rw-r--r--   0        0        0      118 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/jsonschema_form.py
+-rw-r--r--   0        0        0      114 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/label_label.py
+-rw-r--r--   0        0        0      980 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/list_bulk_schema.py
+-rw-r--r--   0        0        0     1018 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/list_bulk_sync_executions_envelope.py
+-rw-r--r--   0        0        0     1045 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/list_execution_response_envelope.py
+-rw-r--r--   0        0        0     1017 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/list_model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1006 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/list_policies_response_envelope.py
+-rw-r--r--   0        0        0      964 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/list_users_envelope.py
+-rw-r--r--   0        0        0     1167 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/mode.py
+-rw-r--r--   0        0        0     1221 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_field.py
+-rw-r--r--   0        0        0      984 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_field_response.py
+-rw-r--r--   0        0        0     1000 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_list_response_envelope.py
+-rw-r--r--   0        0        0      978 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_model_field_request.py
+-rw-r--r--   0        0        0     1135 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_relation.py
+-rw-r--r--   0        0        0      968 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_relation_to.py
+-rw-r--r--   0        0        0     1652 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_response.py
+-rw-r--r--   0        0        0     1066 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_response_envelope.py
+-rw-r--r--   0        0        0     1077 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_sync_field.py
+-rw-r--r--   0        0        0     1827 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_sync_response.py
+-rw-r--r--   0        0        0     1000 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1210 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/model_sync_source_meta_response.py
+-rw-r--r--   0        0        0     1086 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/organization.py
+-rw-r--r--   0        0        0      978 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/organization_envelope.py
+-rw-r--r--   0        0        0      992 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/organizations_envelope.py
+-rw-r--r--   0        0        0     1059 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/override.py
+-rw-r--r--   0        0        0      959 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/pick_value.py
+-rw-r--r--   0        0        0      955 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/policy_action.py
+-rw-r--r--   0        0        0     1160 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/policy_response.py
+-rw-r--r--   0        0        0      987 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/policy_response_envelope.py
+-rw-r--r--   0        0        0     1114 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/relation.py
+-rw-r--r--   0        0        0      963 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/relation_to.py
+-rw-r--r--   0        0        0     1331 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/rest_err_response.py
+-rw-r--r--   0        0        0      996 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/role_list_response_envelope.py
+-rw-r--r--   0        0        0     1048 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/role_response.py
+-rw-r--r--   0        0        0      979 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/role_response_envelope.py
+-rw-r--r--   0        0        0      995 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/run_after.py
+-rw-r--r--   0        0        0     1298 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schedule.py
+-rw-r--r--   0        0        0     1669 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schedule_frequency.py
+-rw-r--r--   0        0        0     1037 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schedule_option_response.py
+-rw-r--r--   0        0        0     1020 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schedule_option_response_envelope.py
+-rw-r--r--   0        0        0     1187 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schedule_schedule_option.py
+-rw-r--r--   0        0        0     1051 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schema.py
+-rw-r--r--   0        0        0     1072 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schema_association.py
+-rw-r--r--   0        0        0     1242 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schema_field.py
+-rw-r--r--   0        0        0      977 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/schema_records_response_envelope.py
+-rw-r--r--   0        0        0      911 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/source.py
+-rw-r--r--   0        0        0     1047 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/source_meta.py
+-rw-r--r--   0        0        0     1040 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/start_model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1086 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/start_model_sync_response_schema.py
+-rw-r--r--   0        0        0     1220 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/supported_mode.py
+-rw-r--r--   0        0        0     1476 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/sync_destination_properties.py
+-rw-r--r--   0        0        0      996 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/sync_status_envelope.py
+-rw-r--r--   0        0        0     1166 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/sync_status_response.py
+-rw-r--r--   0        0        0     1149 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/target.py
+-rw-r--r--   0        0        0     1487 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/target_field.py
+-rw-r--r--   0        0        0     1322 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/target_response.py
+-rw-r--r--   0        0        0      987 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/target_response_envelope.py
+-rw-r--r--   0        0        0     1038 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/user.py
+-rw-r--r--   0        0        0      946 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/user_envelope.py
+-rw-r--r--   0        0        0     1098 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/webhook.py
+-rw-r--r--   0        0        0      958 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/webhook_envelope.py
+-rw-r--r--   0        0        0      975 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/webhook_list_envelope.py
+-rw-r--r--   0        0        0      623 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/types/work_task_status.py
+-rw-r--r--   0        0        0       77 2024-04-23 18:27:46.117371 polytomic-1.0.0/src/polytomic/version.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 polytomic-1.0.0/PKG-INFO
```

### Comparing `polytomic-0.2.0/LICENSE` & `polytomic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/README.md` & `polytomic-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/pyproject.toml` & `polytomic-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polytomic"
-version = "0.2.0"
+version = "1.0.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "polytomic", from = "src"}
 ]
```

### Comparing `polytomic-0.2.0/src/polytomic/__init__.py` & `polytomic-1.0.0/src/polytomic/__init__.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/client.py` & `polytomic-1.0.0/src/polytomic/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/core/__init__.py` & `polytomic-1.0.0/src/polytomic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/core/client_wrapper.py` & `polytomic-1.0.0/src/polytomic/core/client_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "polytomic",
-            "X-Fern-SDK-Version": "0.2.0",
+            "X-Fern-SDK-Version": "1.0.0",
         }
         headers["Authorization"] = f"Bearer {self._get_token()}"
         headers["X-Polytomic-Version"] = "2024-02-08"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
```

### Comparing `polytomic-0.2.0/src/polytomic/core/datetime_utils.py` & `polytomic-1.0.0/src/polytomic/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/core/file.py` & `polytomic-1.0.0/src/polytomic/core/file.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/core/http_client.py` & `polytomic-1.0.0/src/polytomic/core/http_client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/core/jsonable_encoder.py` & `polytomic-1.0.0/src/polytomic/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/core/request_options.py` & `polytomic-1.0.0/src/polytomic/core/request_options.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/errors/__init__.py` & `polytomic-1.0.0/src/polytomic/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/bulk_sync/client.py` & `polytomic-1.0.0/src/polytomic/resources/bulk_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,23 +146,17 @@
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.bulk_sync.create(
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="replicate",
             name="My Bulk Sync",
             schedule=BulkSchedule(
-                day_of_month="1",
-                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
-                hour="0",
-                minute="0",
-                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -319,15 +313,15 @@
         source_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         source_connection_id: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> BulkSyncResponseEnvelope:
         """
         > 📘 Updating schemas
         >
-        > Schema updates can be performed using the [Update Bulk Sync Schemas](https://docs.polytomic.com/reference/apiv3updatebulksyncschemas) endpoint.
+        > Schema updates can be performed using the [Update Bulk Sync Schemas](https://apidocs.polytomic.com/api-reference/bulk-sync/schemas/patch) endpoint.
 
         Parameters:
             - id: str.
 
             - active: typing.Optional[bool].
 
             - automatically_add_new_fields: typing.Optional[BulkDiscover].
@@ -365,23 +359,17 @@
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.bulk_sync.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="replicate",
             name="My Bulk Sync",
             schedule=BulkSchedule(
-                day_of_month="1",
-                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
-                hour="0",
-                minute="0",
-                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -616,16 +604,14 @@
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.bulk_sync.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            resync=False,
-            test=False,
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if resync is not OMIT:
             _request["resync"] = resync
         if schemas is not OMIT:
             _request["schemas"] = schemas
@@ -960,23 +946,17 @@
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.create(
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="replicate",
             name="My Bulk Sync",
             schedule=BulkSchedule(
-                day_of_month="1",
-                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
-                hour="0",
-                minute="0",
-                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -1133,15 +1113,15 @@
         source_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         source_connection_id: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> BulkSyncResponseEnvelope:
         """
         > 📘 Updating schemas
         >
-        > Schema updates can be performed using the [Update Bulk Sync Schemas](https://docs.polytomic.com/reference/apiv3updatebulksyncschemas) endpoint.
+        > Schema updates can be performed using the [Update Bulk Sync Schemas](https://apidocs.polytomic.com/api-reference/bulk-sync/schemas/patch) endpoint.
 
         Parameters:
             - id: str.
 
             - active: typing.Optional[bool].
 
             - automatically_add_new_fields: typing.Optional[BulkDiscover].
@@ -1179,23 +1159,17 @@
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="replicate",
             name="My Bulk Sync",
             schedule=BulkSchedule(
-                day_of_month="1",
-                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
-                hour="0",
-                minute="0",
-                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -1430,16 +1404,14 @@
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            resync=False,
-            test=False,
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if resync is not OMIT:
             _request["resync"] = resync
         if schemas is not OMIT:
             _request["schemas"] = schemas
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/executions/client.py` & `polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/executions/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py` & `polytomic-1.0.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,16 +255,14 @@
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.bulk_sync.schemas.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             schema_id="contact",
-            enabled=True,
-            partition_key="email",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if enabled is not OMIT:
             _request["enabled"] = enabled
         if fields is not OMIT:
             _request["fields"] = fields
@@ -542,16 +540,14 @@
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.schemas.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             schema_id="contact",
-            enabled=True,
-            partition_key="email",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if enabled is not OMIT:
             _request["enabled"] = enabled
         if fields is not OMIT:
             _request["fields"] = fields
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/connections/client.py` & `polytomic-1.0.0/src/polytomic/resources/connections/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,15 @@
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.connections.create(
             name="My Postgres Connection",
-            redirect_url="https://example.com/oauth_redirect",
             type="postgresql",
-            validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
@@ -253,32 +251,30 @@
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.connections.connect(
-            connection="248df4b7-aa70-47b8-a036-33ac447e668d",
             name="Salesforce Connection",
             redirect_url="redirect_url",
-            type="salesforce",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "redirect_url": redirect_url}
         if connection is not OMIT:
             _request["connection"] = connection
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if type is not OMIT:
             _request["type"] = type
         if whitelist is not OMIT:
             _request["whitelist"] = whitelist
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect/"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -403,17 +399,14 @@
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.connections.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             name="My Postgres Connection",
-            reconnect=False,
-            type="postgresql",
-            validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
@@ -725,17 +718,15 @@
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.connections.create(
             name="My Postgres Connection",
-            redirect_url="https://example.com/oauth_redirect",
             type="postgresql",
-            validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
@@ -820,32 +811,30 @@
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.connections.connect(
-            connection="248df4b7-aa70-47b8-a036-33ac447e668d",
             name="Salesforce Connection",
             redirect_url="redirect_url",
-            type="salesforce",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "redirect_url": redirect_url}
         if connection is not OMIT:
             _request["connection"] = connection
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if type is not OMIT:
             _request["type"] = type
         if whitelist is not OMIT:
             _request["whitelist"] = whitelist
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect/"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -972,17 +961,14 @@
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.connections.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             name="My Postgres Connection",
-            reconnect=False,
-            type="postgresql",
-            validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/events/client.py` & `polytomic-1.0.0/src/polytomic/resources/events/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/identity/client.py` & `polytomic-1.0.0/src/polytomic/resources/identity/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/jobs/client.py` & `polytomic-1.0.0/src/polytomic/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/model_sync/client.py` & `polytomic-1.0.0/src/polytomic/resources/model_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,46 +430,24 @@
 
             - sync_all_records: typing.Optional[bool].
 
             - target: Target.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import Identity, ModelSyncField, Schedule, Source, Target
+        from polytomic import Schedule, Target
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.model_sync.create(
-            fields=[
-                ModelSyncField(
-                    source=Source(
-                        field="id",
-                        model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                    ),
-                    target="name",
-                )
-            ],
-            filter_logic="A and B or C",
-            identity=Identity(
-                function="Equality",
-                source=Source(
-                    field="id",
-                    model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                ),
-                target="name",
-            ),
             mode="create",
             name="Users Sync",
-            schedule=Schedule(
-                connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                frequency="daily",
-            ),
-            sync_all_records=False,
+            schedule=Schedule(),
             target=Target(
                 connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
                 object="Users",
             ),
         )
         """
         _request: typing.Dict[str, typing.Any] = {"mode": mode, "name": name, "schedule": schedule, "target": target}
@@ -685,47 +663,25 @@
 
             - sync_all_records: typing.Optional[bool].
 
             - target: Target.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import Identity, ModelSyncField, Schedule, Source, Target
+        from polytomic import Schedule, Target
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.model_sync.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            fields=[
-                ModelSyncField(
-                    source=Source(
-                        field="id",
-                        model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                    ),
-                    target="name",
-                )
-            ],
-            filter_logic="A and B or C",
-            identity=Identity(
-                function="Equality",
-                source=Source(
-                    field="id",
-                    model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                ),
-                target="name",
-            ),
             mode="create",
             name="Users Sync",
-            schedule=Schedule(
-                connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                frequency="daily",
-            ),
-            sync_all_records=False,
+            schedule=Schedule(),
             target=Target(
                 connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
                 object="Users",
             ),
         )
         """
         _request: typing.Dict[str, typing.Any] = {"mode": mode, "name": name, "schedule": schedule, "target": target}
@@ -918,36 +874,45 @@
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def start(
         self,
         id: str,
         *,
         identities: typing.Optional[typing.Sequence[str]] = OMIT,
+        resync: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> StartModelSyncResponseEnvelope:
         """
+        > 🚧 Force full resync
+        >
+        > Use caution when setting the `resync` parameter to `true`. This will force a full resync of the data from the source system. This can be a time-consuming operation and may impact the performance of the source system. It is recommended to only use this option when necessary.
+
         Parameters:
             - id: str.
 
             - identities: typing.Optional[typing.Sequence[str]].
 
+            - resync: typing.Optional[bool].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.model_sync.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if identities is not OMIT:
             _request["identities"] = identities
+        if resync is not OMIT:
+            _request["resync"] = resync
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{jsonable_encoder(id)}/executions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -1426,46 +1391,24 @@
 
             - sync_all_records: typing.Optional[bool].
 
             - target: Target.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import Identity, ModelSyncField, Schedule, Source, Target
+        from polytomic import Schedule, Target
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.model_sync.create(
-            fields=[
-                ModelSyncField(
-                    source=Source(
-                        field="id",
-                        model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                    ),
-                    target="name",
-                )
-            ],
-            filter_logic="A and B or C",
-            identity=Identity(
-                function="Equality",
-                source=Source(
-                    field="id",
-                    model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                ),
-                target="name",
-            ),
             mode="create",
             name="Users Sync",
-            schedule=Schedule(
-                connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                frequency="daily",
-            ),
-            sync_all_records=False,
+            schedule=Schedule(),
             target=Target(
                 connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
                 object="Users",
             ),
         )
         """
         _request: typing.Dict[str, typing.Any] = {"mode": mode, "name": name, "schedule": schedule, "target": target}
@@ -1683,47 +1626,25 @@
 
             - sync_all_records: typing.Optional[bool].
 
             - target: Target.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import Identity, ModelSyncField, Schedule, Source, Target
+        from polytomic import Schedule, Target
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.model_sync.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            fields=[
-                ModelSyncField(
-                    source=Source(
-                        field="id",
-                        model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                    ),
-                    target="name",
-                )
-            ],
-            filter_logic="A and B or C",
-            identity=Identity(
-                function="Equality",
-                source=Source(
-                    field="id",
-                    model_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                ),
-                target="name",
-            ),
             mode="create",
             name="Users Sync",
-            schedule=Schedule(
-                connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-                frequency="daily",
-            ),
-            sync_all_records=False,
+            schedule=Schedule(),
             target=Target(
                 connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
                 object="Users",
             ),
         )
         """
         _request: typing.Dict[str, typing.Any] = {"mode": mode, "name": name, "schedule": schedule, "target": target}
@@ -1916,36 +1837,45 @@
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def start(
         self,
         id: str,
         *,
         identities: typing.Optional[typing.Sequence[str]] = OMIT,
+        resync: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> StartModelSyncResponseEnvelope:
         """
+        > 🚧 Force full resync
+        >
+        > Use caution when setting the `resync` parameter to `true`. This will force a full resync of the data from the source system. This can be a time-consuming operation and may impact the performance of the source system. It is recommended to only use this option when necessary.
+
         Parameters:
             - id: str.
 
             - identities: typing.Optional[typing.Sequence[str]].
 
+            - resync: typing.Optional[bool].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.model_sync.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if identities is not OMIT:
             _request["identities"] = identities
+        if resync is not OMIT:
+            _request["resync"] = resync
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{jsonable_encoder(id)}/executions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/model_sync/resources/executions/client.py` & `polytomic-1.0.0/src/polytomic/resources/model_sync/resources/executions/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/models/client.py` & `polytomic-1.0.0/src/polytomic/resources/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,14 @@
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.models.create(
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            identifier="id",
             name="Users",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
         if additional_fields is not OMIT:
             _request["additional_fields"] = additional_fields
         if configuration is not OMIT:
@@ -307,15 +306,14 @@
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.models.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             async_=False,
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            identifier="id",
             name="Users",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
         if additional_fields is not OMIT:
             _request["additional_fields"] = additional_fields
         if configuration is not OMIT:
@@ -534,15 +532,14 @@
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.models.create(
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            identifier="id",
             name="Users",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
         if additional_fields is not OMIT:
             _request["additional_fields"] = additional_fields
         if configuration is not OMIT:
@@ -715,15 +712,14 @@
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.models.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             async_=False,
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            identifier="id",
             name="Users",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
         if additional_fields is not OMIT:
             _request["additional_fields"] = additional_fields
         if configuration is not OMIT:
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/organization/client.py` & `polytomic-1.0.0/src/polytomic/resources/organization/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationsEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
@@ -89,15 +89,15 @@
         sso_domain: typing.Optional[str] = OMIT,
         sso_org_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - client_id: typing.Optional[str].
 
             - client_secret: typing.Optional[str].
 
             - issuer: typing.Optional[str].
@@ -112,20 +112,15 @@
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.organization.create(
-            client_id="client_id",
-            client_secret="client_secret",
-            issuer="https://example.com",
             name="My Organization",
-            sso_domain="example.com",
-            sso_org_id="123456",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if client_id is not OMIT:
             _request["client_id"] = client_id
         if client_secret is not OMIT:
             _request["client_secret"] = client_secret
@@ -177,15 +172,15 @@
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
@@ -242,15 +237,15 @@
         sso_domain: typing.Optional[str] = OMIT,
         sso_org_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - client_id: typing.Optional[str].
 
             - client_secret: typing.Optional[str].
@@ -268,20 +263,15 @@
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.organization.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            client_id="client_id",
-            client_secret="client_secret",
-            issuer="https://example.com",
             name="My Organization",
-            sso_domain="example.com",
-            sso_org_id="123456",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if client_id is not OMIT:
             _request["client_id"] = client_id
         if client_secret is not OMIT:
             _request["client_secret"] = client_secret
@@ -335,15 +325,15 @@
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
@@ -396,15 +386,15 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationsEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
@@ -454,15 +444,15 @@
         sso_domain: typing.Optional[str] = OMIT,
         sso_org_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - client_id: typing.Optional[str].
 
             - client_secret: typing.Optional[str].
 
             - issuer: typing.Optional[str].
@@ -477,20 +467,15 @@
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.organization.create(
-            client_id="client_id",
-            client_secret="client_secret",
-            issuer="https://example.com",
             name="My Organization",
-            sso_domain="example.com",
-            sso_org_id="123456",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if client_id is not OMIT:
             _request["client_id"] = client_id
         if client_secret is not OMIT:
             _request["client_secret"] = client_secret
@@ -542,15 +527,15 @@
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
@@ -607,15 +592,15 @@
         sso_domain: typing.Optional[str] = OMIT,
         sso_org_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - client_id: typing.Optional[str].
 
             - client_secret: typing.Optional[str].
@@ -633,20 +618,15 @@
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.organization.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            client_id="client_id",
-            client_secret="client_secret",
-            issuer="https://example.com",
             name="My Organization",
-            sso_domain="example.com",
-            sso_org_id="123456",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if client_id is not OMIT:
             _request["client_id"] = client_id
         if client_secret is not OMIT:
             _request["client_secret"] = client_secret
@@ -700,15 +680,15 @@
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         > 🚧 Requires partner key
         >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > Organization endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/permissions/client.py` & `polytomic-1.0.0/src/polytomic/resources/permissions/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/permissions/resources/policies/client.py` & `polytomic-1.0.0/src/polytomic/resources/permissions/resources/policies/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,28 +91,21 @@
 
             - organization_id: typing.Optional[str].
 
             - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.permissions.policies.create(
             name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policy_actions is not OMIT:
             _request["policy_actions"] = policy_actions
@@ -229,29 +222,22 @@
 
             - organization_id: typing.Optional[str].
 
             - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.permissions.policies.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policy_actions is not OMIT:
             _request["policy_actions"] = policy_actions
@@ -418,28 +404,21 @@
 
             - organization_id: typing.Optional[str].
 
             - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.permissions.policies.create(
             name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policy_actions is not OMIT:
             _request["policy_actions"] = policy_actions
@@ -556,29 +535,22 @@
 
             - organization_id: typing.Optional[str].
 
             - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.permissions.policies.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policy_actions is not OMIT:
             _request["policy_actions"] = policy_actions
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/permissions/resources/roles/client.py` & `polytomic-1.0.0/src/polytomic/resources/permissions/resources/roles/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/schemas/client.py` & `polytomic-1.0.0/src/polytomic/resources/schemas/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/resources/users/client.py` & `polytomic-1.0.0/src/polytomic/resources/users/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
@@ -93,15 +93,15 @@
         email: str,
         role: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - org_id: str.
 
             - email: str.
 
             - role: typing.Optional[str].
@@ -112,15 +112,14 @@
 
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.users.create(
             org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             email="mail@example.com",
-            role="admin",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"email": email}
         if role is not OMIT:
             _request["role"] = role
         _response = self._client_wrapper.httpx_client.request(
             "POST",
@@ -166,15 +165,15 @@
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -234,15 +233,15 @@
         email: str,
         role: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - org_id: str.
 
             - email: str.
@@ -256,15 +255,14 @@
         client = Polytomic(
             token="YOUR_TOKEN",
         )
         client.users.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             email="mail@example.com",
-            role="admin",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"email": email}
         if role is not OMIT:
             _request["role"] = role
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
@@ -311,15 +309,15 @@
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def remove(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -378,15 +376,15 @@
         *,
         force: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ApiKeyResponseEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - org_id: str.
 
             - id: str.
 
             - force: typing.Optional[bool].
@@ -458,15 +456,15 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
@@ -519,15 +517,15 @@
         email: str,
         role: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - org_id: str.
 
             - email: str.
 
             - role: typing.Optional[str].
@@ -538,15 +536,14 @@
 
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.users.create(
             org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             email="mail@example.com",
-            role="admin",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"email": email}
         if role is not OMIT:
             _request["role"] = role
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
@@ -594,15 +591,15 @@
 
     async def get(
         self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -662,15 +659,15 @@
         email: str,
         role: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - org_id: str.
 
             - email: str.
@@ -684,15 +681,14 @@
         client = AsyncPolytomic(
             token="YOUR_TOKEN",
         )
         await client.users.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             email="mail@example.com",
-            role="admin",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"email": email}
         if role is not OMIT:
             _request["role"] = role
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
@@ -741,15 +737,15 @@
 
     async def remove(
         self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - id: str.
 
             - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
@@ -808,15 +804,15 @@
         *,
         force: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ApiKeyResponseEnvelope:
         """
         > 🚧 Requires partner key
         >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+        > User endpoints are only accessible using [partner keys](https://apidocs.polytomic.com/getting-started/obtaining-api-keys#partner-keys)
 
         Parameters:
             - org_id: str.
 
             - id: str.
 
             - force: typing.Optional[bool].
```

### Comparing `polytomic-0.2.0/src/polytomic/resources/webhooks/client.py` & `polytomic-1.0.0/src/polytomic/resources/webhooks/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookListEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
@@ -90,15 +90,15 @@
         request_options: typing.Optional[RequestOptions] = None,
     ) -> WebhookEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - endpoint: str.
 
             - organization_id: typing.Optional[str].
 
             - secret: str.
@@ -162,15 +162,15 @@
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
@@ -224,15 +224,15 @@
         request_options: typing.Optional[RequestOptions] = None,
     ) -> WebhookEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - id: str.
 
             - endpoint: str.
 
             - organization_id: typing.Optional[str].
@@ -354,15 +354,15 @@
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookListEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
@@ -411,15 +411,15 @@
         request_options: typing.Optional[RequestOptions] = None,
     ) -> WebhookEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - endpoint: str.
 
             - organization_id: typing.Optional[str].
 
             - secret: str.
@@ -483,15 +483,15 @@
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
@@ -545,15 +545,15 @@
         request_options: typing.Optional[RequestOptions] = None,
     ) -> WebhookEnvelope:
         """
         Webooks can be set up using the webhook API endpoints. Currently, only one
         webhook may be created per organization. The webhook will be called for events
         in that organization.
 
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+        Consult the [Events documentation](https://apidocs.polytomic.com/getting-started/events) for more information.
 
         Parameters:
             - id: str.
 
             - endpoint: str.
 
             - organization_id: typing.Optional[str].
```

### Comparing `polytomic-0.2.0/src/polytomic/types/__init__.py` & `polytomic-1.0.0/src/polytomic/types/__init__.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/activate_sync_envelope.py` & `polytomic-1.0.0/src/polytomic/types/activate_sync_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/activate_sync_input.py` & `polytomic-1.0.0/src/polytomic/types/activate_sync_input.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/activate_sync_output.py` & `polytomic-1.0.0/src/polytomic/types/activate_sync_output.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/api_error.py` & `polytomic-1.0.0/src/polytomic/types/api_error.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/api_key_response.py` & `polytomic-1.0.0/src/polytomic/types/api_key_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/api_key_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/api_key_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_discover.py` & `polytomic-1.0.0/src/polytomic/types/bulk_discover.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_execution_status.py` & `polytomic-1.0.0/src/polytomic/types/bulk_execution_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_field.py` & `polytomic-1.0.0/src/polytomic/types/bulk_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_itemized_schedule.py` & `polytomic-1.0.0/src/polytomic/types/bulk_itemized_schedule.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_multi_schedule_configuration.py` & `polytomic-1.0.0/src/polytomic/types/bulk_multi_schedule_configuration.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_schedule.py` & `polytomic-1.0.0/src/polytomic/types/bulk_schedule.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_schema.py` & `polytomic-1.0.0/src/polytomic/types/bulk_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_schema_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_schema_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_schema_execution_status.py` & `polytomic-1.0.0/src/polytomic/types/bulk_schema_execution_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_selective_mode.py` & `polytomic-1.0.0/src/polytomic/types/bulk_selective_mode.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_dest.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_dest.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_dest_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_dest_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_execution.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_execution.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_execution_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_execution_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_list_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_list_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_response.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_schema_execution.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_schema_execution.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_source.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_source.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_source_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_schema_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_source_schema_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_source_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_source_status_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_status_envelope.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_status_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/bulk_sync_status_response.py` & `polytomic-1.0.0/src/polytomic/types/bulk_sync_status_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/configuration_value.py` & `polytomic-1.0.0/src/polytomic/types/configuration_value.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connect_card_response.py` & `polytomic-1.0.0/src/polytomic/types/connect_card_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connect_card_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/connect_card_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_list_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/connection_list_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_meta.py` & `polytomic-1.0.0/src/polytomic/types/connection_meta.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_meta_response.py` & `polytomic-1.0.0/src/polytomic/types/connection_meta_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_parameter_value.py` & `polytomic-1.0.0/src/polytomic/types/connection_parameter_value.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_parameter_values_resp.py` & `polytomic-1.0.0/src/polytomic/types/connection_parameter_values_resp.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_parameter_values_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/connection_parameter_values_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/connection_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_response_schema.py` & `polytomic-1.0.0/src/polytomic/types/connection_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_type.py` & `polytomic-1.0.0/src/polytomic/types/connection_type.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_type_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/connection_type_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/connection_type_schema.py` & `polytomic-1.0.0/src/polytomic/types/connection_type_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/create_connection_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/create_connection_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/create_connection_response_schema.py` & `polytomic-1.0.0/src/polytomic/types/create_connection_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/event.py` & `polytomic-1.0.0/src/polytomic/types/event.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/event_types_envelope.py` & `polytomic-1.0.0/src/polytomic/types/event_types_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/events_envelope.py` & `polytomic-1.0.0/src/polytomic/types/events_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/execution_counts.py` & `polytomic-1.0.0/src/polytomic/types/execution_counts.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/execution_log_response.py` & `polytomic-1.0.0/src/polytomic/types/execution_log_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/execution_logs_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/execution_logs_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/execution_status.py` & `polytomic-1.0.0/src/polytomic/types/execution_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/filter.py` & `polytomic-1.0.0/src/polytomic/types/filter.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/get_connection_meta_envelope.py` & `polytomic-1.0.0/src/polytomic/types/get_connection_meta_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/get_execution_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/get_execution_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/get_execution_response_schema.py` & `polytomic-1.0.0/src/polytomic/types/get_execution_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/get_identity_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/get_identity_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/get_identity_response_schema.py` & `polytomic-1.0.0/src/polytomic/types/get_identity_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/get_model_sync_source_meta_envelope.py` & `polytomic-1.0.0/src/polytomic/types/get_model_sync_source_meta_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/identity.py` & `polytomic-1.0.0/src/polytomic/types/identity.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/identity_function.py` & `polytomic-1.0.0/src/polytomic/types/identity_function.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/job_response.py` & `polytomic-1.0.0/src/polytomic/types/job_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/job_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/job_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/list_bulk_schema.py` & `polytomic-1.0.0/src/polytomic/types/list_bulk_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/list_bulk_sync_executions_envelope.py` & `polytomic-1.0.0/src/polytomic/types/list_bulk_sync_executions_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/list_execution_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/list_execution_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/list_model_sync_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/list_model_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/list_policies_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/list_policies_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/list_users_envelope.py` & `polytomic-1.0.0/src/polytomic/types/list_users_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/mode.py` & `polytomic-1.0.0/src/polytomic/types/mode.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_field.py` & `polytomic-1.0.0/src/polytomic/types/model_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_field_response.py` & `polytomic-1.0.0/src/polytomic/types/model_field_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_list_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/model_list_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_model_field_request.py` & `polytomic-1.0.0/src/polytomic/types/model_model_field_request.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_relation.py` & `polytomic-1.0.0/src/polytomic/types/model_relation.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_relation_to.py` & `polytomic-1.0.0/src/polytomic/types/model_relation_to.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_response.py` & `polytomic-1.0.0/src/polytomic/types/model_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/model_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_sync_field.py` & `polytomic-1.0.0/src/polytomic/types/model_sync_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_sync_response.py` & `polytomic-1.0.0/src/polytomic/types/model_sync_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_sync_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/model_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/model_sync_source_meta_response.py` & `polytomic-1.0.0/src/polytomic/types/model_sync_source_meta_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/organization.py` & `polytomic-1.0.0/src/polytomic/types/organization.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/organization_envelope.py` & `polytomic-1.0.0/src/polytomic/types/organization_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/organizations_envelope.py` & `polytomic-1.0.0/src/polytomic/types/organizations_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/override.py` & `polytomic-1.0.0/src/polytomic/types/override.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/pick_value.py` & `polytomic-1.0.0/src/polytomic/types/pick_value.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/policy_action.py` & `polytomic-1.0.0/src/polytomic/types/policy_action.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/policy_response.py` & `polytomic-1.0.0/src/polytomic/types/policy_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/policy_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/policy_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/relation.py` & `polytomic-1.0.0/src/polytomic/types/relation.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/relation_to.py` & `polytomic-1.0.0/src/polytomic/types/relation_to.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/rest_err_response.py` & `polytomic-1.0.0/src/polytomic/types/rest_err_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/role_list_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/role_list_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/role_response.py` & `polytomic-1.0.0/src/polytomic/types/role_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/role_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/role_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/run_after.py` & `polytomic-1.0.0/src/polytomic/types/run_after.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schedule.py` & `polytomic-1.0.0/src/polytomic/types/schedule.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schedule_frequency.py` & `polytomic-1.0.0/src/polytomic/types/schedule_frequency.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schedule_option_response.py` & `polytomic-1.0.0/src/polytomic/types/schedule_option_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schedule_option_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/schedule_option_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schedule_schedule_option.py` & `polytomic-1.0.0/src/polytomic/types/schedule_schedule_option.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schema.py` & `polytomic-1.0.0/src/polytomic/types/schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schema_association.py` & `polytomic-1.0.0/src/polytomic/types/schema_association.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schema_field.py` & `polytomic-1.0.0/src/polytomic/types/schema_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/schema_records_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/schema_records_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/source.py` & `polytomic-1.0.0/src/polytomic/types/source.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/source_meta.py` & `polytomic-1.0.0/src/polytomic/types/source_meta.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/start_model_sync_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/start_model_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/start_model_sync_response_schema.py` & `polytomic-1.0.0/src/polytomic/types/start_model_sync_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/supported_mode.py` & `polytomic-1.0.0/src/polytomic/types/supported_mode.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/sync_destination_properties.py` & `polytomic-1.0.0/src/polytomic/types/sync_destination_properties.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/sync_status_envelope.py` & `polytomic-1.0.0/src/polytomic/types/sync_status_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/sync_status_response.py` & `polytomic-1.0.0/src/polytomic/types/sync_status_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/target.py` & `polytomic-1.0.0/src/polytomic/types/target.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/target_field.py` & `polytomic-1.0.0/src/polytomic/types/target_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/target_response.py` & `polytomic-1.0.0/src/polytomic/types/target_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/target_response_envelope.py` & `polytomic-1.0.0/src/polytomic/types/target_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/user.py` & `polytomic-1.0.0/src/polytomic/types/user.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/user_envelope.py` & `polytomic-1.0.0/src/polytomic/types/user_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/webhook.py` & `polytomic-1.0.0/src/polytomic/types/webhook.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/webhook_envelope.py` & `polytomic-1.0.0/src/polytomic/types/webhook_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/webhook_list_envelope.py` & `polytomic-1.0.0/src/polytomic/types/webhook_list_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/src/polytomic/types/work_task_status.py` & `polytomic-1.0.0/src/polytomic/types/work_task_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.2.0/PKG-INFO` & `polytomic-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytomic
-Version: 0.2.0
+Version: 1.0.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

