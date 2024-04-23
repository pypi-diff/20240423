# Comparing `tmp/types-tensorflow-2.15.0.20240417.tar.gz` & `tmp/types-tensorflow-2.15.0.20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.15.0.20240417.tar", last modified: Wed Apr 17 02:17:36 2024, max compression
+gzip compressed data, was "types-tensorflow-2.15.0.20240422.tar", last modified: Mon Apr 22 02:19:04 2024, max compression
```

## Comparing `types-tensorflow-2.15.0.20240417.tar` & `types-tensorflow-2.15.0.20240422.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/_aliases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/audio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autodiff.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/bitwise.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (127)    79109 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    81470 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.389538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.393538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    74211 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    50609 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/experimental/coordinator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/dtensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/losses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/linalg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/nn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/distribute/distribute_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/framework/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/ressource.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/training/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/training/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/training/tracking/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/random.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/raw_ops.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/sparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/summary.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/types/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.804945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/_aliases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/audio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autodiff.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.804945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/bitwise.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.804945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.808945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    79109 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    81470 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.808945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.808945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.812945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.816945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    74211 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.816945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    50609 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/experimental/coordinator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/dtensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/losses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/linalg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/nn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/distribute/distribute_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/framework/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/ressource.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/training/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/training/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/training/tracking/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/random.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/raw_ops.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/sparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/summary.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/types/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.15.0.20240417/CHANGELOG.md` & `types-tensorflow-2.15.0.20240422/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.15.0.20240422 (2024-04-22)
+
+Simplify protoc install in protobuf generation scripts (#11785)
+
 ## 2.15.0.20240417 (2024-04-17)
 
 Remove remaining bare `Incomplete`s (#11768)
 
 Enable Y065
 
 ## 2.15.0.20240412 (2024-04-12)
```

### Comparing `types-tensorflow-2.15.0.20240417/PKG-INFO` & `types-tensorflow-2.15.0.20240422/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240417
+Version: 2.15.0.20240422
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,17 +27,17 @@
 
 This version of `types-tensorflow` aims to provide accurate annotations
 for `tensorflow==2.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.12.1.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.15.0.20240417/setup.py` & `types-tensorflow-2.15.0.20240422/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
 This version of `types-tensorflow` aims to provide accurate annotations
 for `tensorflow==2.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.12.1.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.15.0.20240417",
+      version="2.15.0.20240422",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
```

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/autodiff.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/autodiff.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/experimental.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/bitwise.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/bitwise.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/experimental.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/experimental.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/dtensor.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/dtensor.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/activations.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/activations.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/callbacks.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/callbacks.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/losses.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/losses.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/metrics.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/metrics.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/models.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/models.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/linalg.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/linalg.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/math.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/nn.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/nn.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/random.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/raw_ops.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/raw_ops.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/experimental.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/strings.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/strings.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/summary.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/summary.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/__init__.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/tensorflow-stubs/types/experimental.pyi` & `types-tensorflow-2.15.0.20240422/tensorflow-stubs/types/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240417
+Version: 2.15.0.20240422
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,17 +27,17 @@
 
 This version of `types-tensorflow` aims to provide accurate annotations
 for `tensorflow==2.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.12.1.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

