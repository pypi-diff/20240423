# Comparing `tmp/truvity_sdk-0.0.7rc1.tar.gz` & `tmp/truvity_sdk-0.0.7rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truvity_sdk-0.0.7rc1.tar", max compression
+gzip compressed data, was "truvity_sdk-0.0.7rc2.tar", max compression
```

## Comparing `truvity_sdk-0.0.7rc1.tar` & `truvity_sdk-0.0.7rc2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0        0 2024-03-28 17:52:31.275000 truvity_sdk-0.0.7rc1/README.md
--rw-r--r--   0        0        0      434 2024-03-28 17:52:31.265000 truvity_sdk-0.0.7rc1/pyproject.toml
--rw-r--r--   0        0        0     7208 2024-03-28 17:52:31.197000 truvity_sdk-0.0.7rc1/src/truvity_sdk/__init__.py
--rw-r--r--   0        0        0     4087 2024-03-28 17:52:29.381000 truvity_sdk-0.0.7rc1/src/truvity_sdk/client.py
--rw-r--r--   0        0        0      790 2024-03-28 17:52:31.218000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-28 17:52:30.937000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/api_error.py
--rw-r--r--   0        0        0     1192 2024-03-28 17:52:29.258000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-28 17:52:30.923000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-03-28 17:52:31.045000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/file.py
--rw-r--r--   0        0        0     4882 2024-03-28 17:52:31.081000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-03-28 17:52:30.996000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-28 17:52:31.010000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-03-28 17:52:31.027000 truvity_sdk-0.0.7rc1/src/truvity_sdk/core/request_options.py
--rw-r--r--   0        0        0      163 2024-03-28 17:52:29.162000 truvity_sdk-0.0.7rc1/src/truvity_sdk/environment.py
--rw-r--r--   0        0        0      414 2024-03-28 17:52:31.255000 truvity_sdk-0.0.7rc1/src/truvity_sdk/errors/__init__.py
--rw-r--r--   0        0        0      305 2024-03-28 17:52:30.588000 truvity_sdk-0.0.7rc1/src/truvity_sdk/errors/bad_request_error.py
--rw-r--r--   0        0        0      293 2024-03-28 17:52:30.746000 truvity_sdk-0.0.7rc1/src/truvity_sdk/errors/forbidden_error.py
--rw-r--r--   0        0        0      330 2024-03-28 17:52:30.904000 truvity_sdk-0.0.7rc1/src/truvity_sdk/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-03-28 17:52:30.829000 truvity_sdk-0.0.7rc1/src/truvity_sdk/errors/not_found_error.py
--rw-r--r--   0        0        0      305 2024-03-28 17:52:30.667000 truvity_sdk-0.0.7rc1/src/truvity_sdk/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2024-03-28 17:52:31.270000 truvity_sdk-0.0.7rc1/src/truvity_sdk/py.typed
--rw-r--r--   0        0        0      118 2024-03-28 17:52:31.241000 truvity_sdk-0.0.7rc1/src/truvity_sdk/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-03-28 17:52:31.229000 truvity_sdk-0.0.7rc1/src/truvity_sdk/resources/credentials/__init__.py
--rw-r--r--   0        0        0   102754 2024-03-28 17:52:30.509000 truvity_sdk-0.0.7rc1/src/truvity_sdk/resources/credentials/client.py
--rw-r--r--   0        0        0     9255 2024-03-28 17:52:31.148000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/__init__.py
--rw-r--r--   0        0        0       87 2024-03-28 17:52:21.369000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/annotation_value.py
--rw-r--r--   0        0        0      175 2024-03-28 17:52:21.458000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/annotations.py
--rw-r--r--   0        0        0     1203 2024-03-28 17:52:29.083000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/bad_request_error_body.py
--rw-r--r--   0        0        0       78 2024-03-28 17:52:21.529000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/blob_id.py
--rw-r--r--   0        0        0       83 2024-03-28 17:52:21.597000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/content_type.py
--rw-r--r--   0        0        0     1862 2024-03-28 17:52:21.701000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential.py
--rw-r--r--   0        0        0     1803 2024-03-28 17:52:21.800000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_11.py
--rw-r--r--   0        0        0     1789 2024-03-28 17:52:21.899000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_20.py
--rw-r--r--   0        0        0     2161 2024-03-28 17:52:22.000000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_field.py
--rw-r--r--   0        0        0     1883 2024-03-28 17:52:22.286000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_filter.py
--rw-r--r--   0        0        0     1301 2024-03-28 17:52:22.098000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_filter_data.py
--rw-r--r--   0        0        0      987 2024-03-28 17:52:22.183000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_filter_kind.py
--rw-r--r--   0        0        0       84 2024-03-28 17:52:22.362000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_id.py
--rw-r--r--   0        0        0     1463 2024-03-28 17:52:22.452000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_input.py
--rw-r--r--   0        0        0       88 2024-03-28 17:52:22.526000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_issuer.py
--rw-r--r--   0        0        0     1046 2024-03-28 17:52:22.616000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_list.py
--rw-r--r--   0        0        0     1502 2024-03-28 17:52:22.714000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_resource.py
--rw-r--r--   0        0        0     1103 2024-03-28 17:52:22.804000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_sort.py
--rw-r--r--   0        0        0      151 2024-03-28 17:52:22.876000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_subject.py
--rw-r--r--   0        0        0      114 2024-03-28 17:52:22.947000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_type.py
--rw-r--r--   0        0        0      122 2024-03-28 17:52:23.019000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_valid_from.py
--rw-r--r--   0        0        0      123 2024-03-28 17:52:23.091000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_valid_until.py
--rw-r--r--   0        0        0       87 2024-03-28 17:52:23.161000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credentil_holder.py
--rw-r--r--   0        0        0      687 2024-03-28 17:52:23.245000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/data_model_credential.py
--rw-r--r--   0        0        0       80 2024-03-28 17:52:23.315000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/download.py
--rw-r--r--   0        0        0       76 2024-03-28 17:52:23.384000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/e_tag.py
--rw-r--r--   0        0        0     1146 2024-03-28 17:52:23.480000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id.py
--rw-r--r--   0        0        0     1034 2024-03-28 17:52:23.565000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_equal.py
--rw-r--r--   0        0        0     1043 2024-03-28 17:52:23.651000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_in.py
--rw-r--r--   0        0        0     1045 2024-03-28 17:52:23.804000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_not_equal.py
--rw-r--r--   0        0        0     1050 2024-03-28 17:52:23.890000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_not_in.py
--rw-r--r--   0        0        0     2343 2024-03-28 17:52:23.996000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer.py
--rw-r--r--   0        0        0     1142 2024-03-28 17:52:24.084000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_between.py
--rw-r--r--   0        0        0     1049 2024-03-28 17:52:24.171000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_equal.py
--rw-r--r--   0        0        0     1069 2024-03-28 17:52:24.262000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_greater_than.py
--rw-r--r--   0        0        0     1094 2024-03-28 17:52:24.350000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_greater_than_or_equal.py
--rw-r--r--   0        0        0     1060 2024-03-28 17:52:24.437000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_less_than.py
--rw-r--r--   0        0        0     1085 2024-03-28 17:52:24.561000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_less_than_or_equal.py
--rw-r--r--   0        0        0     1060 2024-03-28 17:52:24.652000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_not_equal.py
--rw-r--r--   0        0        0      706 2024-03-28 17:52:24.732000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_string.py
--rw-r--r--   0        0        0     1046 2024-03-28 17:52:24.819000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_string_equal.py
--rw-r--r--   0        0        0     1057 2024-03-28 17:52:24.904000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_string_not_equal.py
--rw-r--r--   0        0        0     2415 2024-03-28 17:52:25.010000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp.py
--rw-r--r--   0        0        0     1166 2024-03-28 17:52:25.098000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_between.py
--rw-r--r--   0        0        0     1063 2024-03-28 17:52:25.189000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_equal.py
--rw-r--r--   0        0        0     1083 2024-03-28 17:52:25.277000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_greater_than.py
--rw-r--r--   0        0        0     1108 2024-03-28 17:52:25.363000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_greater_than_or_equal.py
--rw-r--r--   0        0        0      972 2024-03-28 17:52:25.451000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_is_not_null.py
--rw-r--r--   0        0        0      965 2024-03-28 17:52:25.539000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_is_null.py
--rw-r--r--   0        0        0     1074 2024-03-28 17:52:25.648000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_less_than.py
--rw-r--r--   0        0        0     1099 2024-03-28 17:52:25.734000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_less_than_or_equal.py
--rw-r--r--   0        0        0     1074 2024-03-28 17:52:25.833000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_not_equal.py
--rw-r--r--   0        0        0     3181 2024-03-28 17:52:25.975000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_optional.py
--rw-r--r--   0        0        0     1037 2024-03-28 17:52:26.062000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_equal.py
--rw-r--r--   0        0        0      960 2024-03-28 17:52:26.151000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_is_not_null.py
--rw-r--r--   0        0        0      953 2024-03-28 17:52:26.236000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_is_null.py
--rw-r--r--   0        0        0     1048 2024-03-28 17:52:26.321000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_not_equal.py
--rw-r--r--   0        0        0     1297 2024-03-28 17:52:26.415000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_optional.py
--rw-r--r--   0        0        0      806 2024-03-28 17:52:26.498000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/http_request_part.py
--rw-r--r--   0        0        0       82 2024-03-28 17:52:26.568000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/label_value.py
--rw-r--r--   0        0        0      155 2024-03-28 17:52:26.642000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/labels.py
--rw-r--r--   0        0        0     1755 2024-03-28 17:52:26.741000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_body_content.py
--rw-r--r--   0        0        0     1874 2024-03-28 17:52:26.835000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_conflict_resource.py
--rw-r--r--   0        0        0     1712 2024-03-28 17:52:26.941000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_forbidden.py
--rw-r--r--   0        0        0     1758 2024-03-28 17:52:27.048000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_internal_server_error.py
--rw-r--r--   0        0        0     1834 2024-03-28 17:52:27.145000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_method_not_allowed_resource_alive.py
--rw-r--r--   0        0        0     1838 2024-03-28 17:52:27.242000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_method_not_allowed_resource_deleted.py
--rw-r--r--   0        0        0     1791 2024-03-28 17:52:27.337000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_not_found_blob.py
--rw-r--r--   0        0        0     1811 2024-03-28 17:52:27.430000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_not_found_resource.py
--rw-r--r--   0        0        0     1820 2024-03-28 17:52:27.529000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_not_found_revision.py
--rw-r--r--   0        0        0     2050 2024-03-28 17:52:27.665000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_null_unicode.py
--rw-r--r--   0        0        0     1724 2024-03-28 17:52:27.758000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_unauthorized.py
--rw-r--r--   0        0        0     1830 2024-03-28 17:52:27.854000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_unsupported_media_type.py
--rw-r--r--   0        0        0     2061 2024-03-28 17:52:27.951000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_validation.py
--rw-r--r--   0        0        0     2123 2024-03-28 17:52:28.051000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource.py
--rw-r--r--   0        0        0       82 2024-03-28 17:52:28.123000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource_id.py
--rw-r--r--   0        0        0     1133 2024-03-28 17:52:28.210000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource_kind.py
--rw-r--r--   0        0        0       84 2024-03-28 17:52:28.281000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource_name.py
--rw-r--r--   0        0        0       87 2024-03-28 17:52:28.348000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource_version.py
--rw-r--r--   0        0        0       80 2024-03-28 17:52:28.418000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/revision.py
--rw-r--r--   0        0        0      487 2024-03-28 17:52:28.506000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/sort_order.py
--rw-r--r--   0        0        0     1020 2024-03-28 17:52:28.593000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/subject.py
--rw-r--r--   0        0        0      112 2024-03-28 17:52:28.667000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/timestamp.py
--rw-r--r--   0        0        0     1146 2024-03-28 17:52:28.906000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/upload_response.py
--rw-r--r--   0        0        0       75 2024-03-28 17:52:28.738000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/uri.py
--rw-r--r--   0        0        0       84 2024-03-28 17:52:28.813000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/uri_reference.py
--rw-r--r--   0        0        0     1416 2024-03-28 17:52:28.994000 truvity_sdk-0.0.7rc1/src/truvity_sdk/types/validation_error.py
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 truvity_sdk-0.0.7rc1/PKG-INFO
+-rw-r--r--   0        0        0     1772 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/README.md
+-rw-r--r--   0        0        0      461 2024-04-08 15:17:12.341611 truvity_sdk-0.0.7rc2/pyproject.toml
+-rw-r--r--   0        0        0     7208 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/__init__.py
+-rw-r--r--   0        0        0     4087 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/client.py
+-rw-r--r--   0        0        0      790 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/api_error.py
+-rw-r--r--   0        0        0     1185 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/core/request_options.py
+-rw-r--r--   0        0        0      163 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/environment.py
+-rw-r--r--   0        0        0      414 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/errors/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/errors/bad_request_error.py
+-rw-r--r--   0        0        0      293 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/errors/forbidden_error.py
+-rw-r--r--   0        0        0      330 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/errors/not_found_error.py
+-rw-r--r--   0        0        0      305 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/py.typed
+-rw-r--r--   0        0        0      118 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/resources/credentials/__init__.py
+-rw-r--r--   0        0        0   102754 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/resources/credentials/client.py
+-rw-r--r--   0        0        0     9255 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/annotation_value.py
+-rw-r--r--   0        0        0      175 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/annotations.py
+-rw-r--r--   0        0        0     1203 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/bad_request_error_body.py
+-rw-r--r--   0        0        0       78 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/blob_id.py
+-rw-r--r--   0        0        0       83 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/content_type.py
+-rw-r--r--   0        0        0     1862 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential.py
+-rw-r--r--   0        0        0     1803 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_11.py
+-rw-r--r--   0        0        0     1789 2024-04-08 15:16:31.113738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_20.py
+-rw-r--r--   0        0        0     2161 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_field.py
+-rw-r--r--   0        0        0     1883 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_filter.py
+-rw-r--r--   0        0        0     1301 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_filter_data.py
+-rw-r--r--   0        0        0      987 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_filter_kind.py
+-rw-r--r--   0        0        0       84 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_id.py
+-rw-r--r--   0        0        0     1463 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_input.py
+-rw-r--r--   0        0        0       88 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_issuer.py
+-rw-r--r--   0        0        0     1046 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_list.py
+-rw-r--r--   0        0        0     1502 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_resource.py
+-rw-r--r--   0        0        0     1103 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_sort.py
+-rw-r--r--   0        0        0      151 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_subject.py
+-rw-r--r--   0        0        0      114 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_type.py
+-rw-r--r--   0        0        0      122 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_valid_from.py
+-rw-r--r--   0        0        0      123 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_valid_until.py
+-rw-r--r--   0        0        0       87 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credentil_holder.py
+-rw-r--r--   0        0        0      687 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/data_model_credential.py
+-rw-r--r--   0        0        0       80 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/download.py
+-rw-r--r--   0        0        0       76 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/e_tag.py
+-rw-r--r--   0        0        0     1146 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id.py
+-rw-r--r--   0        0        0     1034 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_equal.py
+-rw-r--r--   0        0        0     1043 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_in.py
+-rw-r--r--   0        0        0     1045 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_not_equal.py
+-rw-r--r--   0        0        0     1050 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_not_in.py
+-rw-r--r--   0        0        0     2343 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer.py
+-rw-r--r--   0        0        0     1142 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_between.py
+-rw-r--r--   0        0        0     1049 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_equal.py
+-rw-r--r--   0        0        0     1069 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_greater_than.py
+-rw-r--r--   0        0        0     1094 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_greater_than_or_equal.py
+-rw-r--r--   0        0        0     1060 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_less_than.py
+-rw-r--r--   0        0        0     1085 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_less_than_or_equal.py
+-rw-r--r--   0        0        0     1060 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_not_equal.py
+-rw-r--r--   0        0        0      706 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_string.py
+-rw-r--r--   0        0        0     1046 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_string_equal.py
+-rw-r--r--   0        0        0     1057 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_string_not_equal.py
+-rw-r--r--   0        0        0     2415 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp.py
+-rw-r--r--   0        0        0     1166 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_between.py
+-rw-r--r--   0        0        0     1063 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_equal.py
+-rw-r--r--   0        0        0     1083 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_greater_than.py
+-rw-r--r--   0        0        0     1108 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_greater_than_or_equal.py
+-rw-r--r--   0        0        0      972 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_is_not_null.py
+-rw-r--r--   0        0        0      965 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_is_null.py
+-rw-r--r--   0        0        0     1074 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_less_than.py
+-rw-r--r--   0        0        0     1099 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_less_than_or_equal.py
+-rw-r--r--   0        0        0     1074 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_not_equal.py
+-rw-r--r--   0        0        0     3181 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_optional.py
+-rw-r--r--   0        0        0     1037 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_equal.py
+-rw-r--r--   0        0        0      960 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_is_not_null.py
+-rw-r--r--   0        0        0      953 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_is_null.py
+-rw-r--r--   0        0        0     1048 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_not_equal.py
+-rw-r--r--   0        0        0     1297 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_optional.py
+-rw-r--r--   0        0        0      806 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/http_request_part.py
+-rw-r--r--   0        0        0       82 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/label_value.py
+-rw-r--r--   0        0        0      155 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/labels.py
+-rw-r--r--   0        0        0     1755 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_body_content.py
+-rw-r--r--   0        0        0     1874 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_conflict_resource.py
+-rw-r--r--   0        0        0     1712 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_forbidden.py
+-rw-r--r--   0        0        0     1758 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_internal_server_error.py
+-rw-r--r--   0        0        0     1834 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_method_not_allowed_resource_alive.py
+-rw-r--r--   0        0        0     1838 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_method_not_allowed_resource_deleted.py
+-rw-r--r--   0        0        0     1791 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_not_found_blob.py
+-rw-r--r--   0        0        0     1811 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_not_found_resource.py
+-rw-r--r--   0        0        0     1820 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_not_found_revision.py
+-rw-r--r--   0        0        0     2050 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_null_unicode.py
+-rw-r--r--   0        0        0     1724 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_unauthorized.py
+-rw-r--r--   0        0        0     1830 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_unsupported_media_type.py
+-rw-r--r--   0        0        0     2061 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_validation.py
+-rw-r--r--   0        0        0     2123 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource.py
+-rw-r--r--   0        0        0       82 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource_id.py
+-rw-r--r--   0        0        0     1133 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource_kind.py
+-rw-r--r--   0        0        0       84 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource_name.py
+-rw-r--r--   0        0        0       87 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource_version.py
+-rw-r--r--   0        0        0       80 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/revision.py
+-rw-r--r--   0        0        0      487 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/sort_order.py
+-rw-r--r--   0        0        0     1020 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/subject.py
+-rw-r--r--   0        0        0      112 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/timestamp.py
+-rw-r--r--   0        0        0     1146 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/upload_response.py
+-rw-r--r--   0        0        0       75 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/uri.py
+-rw-r--r--   0        0        0       84 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/uri_reference.py
+-rw-r--r--   0        0        0     1416 2024-04-08 15:16:31.117738 truvity_sdk-0.0.7rc2/src/truvity_sdk/types/validation_error.py
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 truvity_sdk-0.0.7rc2/PKG-INFO
```

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/__init__.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/client.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/client.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/__init__.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/client_wrapper.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/client_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     def __init__(self, *, api_key: str, base_url: str):
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
-            "X-Fern-SDK-Name": "truvity_sdk",
-            "X-Fern-SDK-Version": "0.0.7rc1",
+            "X-Fern-SDK-Name": "truvity",
+            "X-Fern-SDK-Version": "0.0.0",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/datetime_utils.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/file.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/file.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/http_client.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/http_client.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/jsonable_encoder.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/core/request_options.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/core/request_options.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/resources/credentials/client.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/resources/credentials/client.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/__init__.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/bad_request_error_body.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/bad_request_error_body.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_11.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_11.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_20.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_20.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_field.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_field.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_filter.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_filter.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_filter_data.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_filter_data.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_filter_kind.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_filter_kind.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_input.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_input.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_list.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_list.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_resource.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_resource.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/credential_sort.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/credential_sort.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/data_model_credential.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/data_model_credential.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_in.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_in.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_not_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_not_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_id_not_in.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_id_not_in.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_between.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_between.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_greater_than.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_greater_than.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_greater_than_or_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_greater_than_or_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_less_than.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_less_than.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_less_than_or_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_less_than_or_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_integer_not_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_integer_not_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_string.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_string.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_string_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_string_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_string_not_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_string_not_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_between.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_between.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_greater_than.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_greater_than.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_greater_than_or_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_greater_than_or_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_is_not_null.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_is_not_null.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_is_null.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_is_null.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_less_than.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_less_than.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_less_than_or_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_less_than_or_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_not_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_not_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_timestamp_optional.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_timestamp_optional.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_is_not_null.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_is_not_null.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_is_null.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_is_null.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_not_equal.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_not_equal.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/filter_uri_optional.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/filter_uri_optional.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/http_request_part.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/http_request_part.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_body_content.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_body_content.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_conflict_resource.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_conflict_resource.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_forbidden.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_forbidden.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_internal_server_error.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_method_not_allowed_resource_alive.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_method_not_allowed_resource_alive.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_method_not_allowed_resource_deleted.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_method_not_allowed_resource_deleted.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_not_found_blob.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_not_found_blob.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_not_found_resource.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_not_found_resource.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_not_found_revision.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_not_found_revision.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_null_unicode.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_null_unicode.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_unauthorized.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_unauthorized.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_unsupported_media_type.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_unsupported_media_type.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/problem_validation.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/problem_validation.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/resource_kind.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/resource_kind.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/subject.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/subject.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/upload_response.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/upload_response.py`

 * *Files identical despite different names*

### Comparing `truvity_sdk-0.0.7rc1/src/truvity_sdk/types/validation_error.py` & `truvity_sdk-0.0.7rc2/src/truvity_sdk/types/validation_error.py`

 * *Files identical despite different names*

