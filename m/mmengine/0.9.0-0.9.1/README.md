# Comparing `tmp/mmengine-0.9.0.tar.gz` & `tmp/mmengine-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.9.0.tar", last modified: Tue Oct 10 11:04:22 2023, max compression
+gzip compressed data, was "dist/mmengine-0.9.1.tar", last modified: Fri Nov  3 08:17:55 2023, max compression
```

## Comparing `mmengine-0.9.0.tar` & `mmengine-0.9.1.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-10 11:02:55.000000 mmengine-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21630 2023-10-10 11:04:22.000000 mmengine-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2023-10-10 11:02:55.000000 mmengine-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39482 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22387 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/colossalai.py
--rw-r--r--   0 runner    (1001) docker     (127)    19013 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    28890 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/_strategy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13594 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26249 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (127)    31115 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74157 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/config/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18486 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34071 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20653 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43528 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21218 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18135 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27918 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    31140 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29994 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27712 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17565 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19045 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/efficient_conv_bn_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26125 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15161 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17881 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16538 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    64430 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    26948 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66496 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/_flexible_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/activation_checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    30359 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    24301 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17179 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)   103199 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24573 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)    13483 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17518 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/progressbar_rich.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52868 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    54112 2023-10-10 11:02:56.000000 mmengine-0.9.0/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21630 2023-10-10 11:04:21.000000 mmengine-0.9.0/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2023-10-10 11:04:22.000000 mmengine-0.9.0/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 11:04:21.000000 mmengine-0.9.0/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-10-10 11:04:21.000000 mmengine-0.9.0/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-10 11:04:21.000000 mmengine-0.9.0/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-10 11:04:22.000000 mmengine-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2023-10-10 11:02:56.000000 mmengine-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-03 08:16:14.000000 mmengine-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21630 2023-11-03 08:17:55.000000 mmengine-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2023-11-03 08:16:14.000000 mmengine-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39482 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22387 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/colossalai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20498 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28890 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13594 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26249 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31115 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74157 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18486 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34071 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43528 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21472 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18135 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27918 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31140 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29994 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17035 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27712 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19045 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/efficient_conv_bn_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26125 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15161 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17881 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16538 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64420 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26948 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66496 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/activation_checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30359 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24301 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17179 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103199 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13483 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17518 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/progressbar_rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52896 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54112 2023-11-03 08:16:14.000000 mmengine-0.9.1/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21630 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-03 08:17:55.000000 mmengine-0.9.1/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-03 08:17:55.000000 mmengine-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2023-11-03 08:16:14.000000 mmengine-0.9.1/setup.py
```

### Comparing `mmengine-0.9.0/PKG-INFO` & `mmengine-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.9.0
+Version: 0.9.1
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -62,25 +62,25 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.9.0 was released on 2023-10-10.
+        v0.9.1 was released on 2023-11-03.
         
         Highlights:
         
         - Support training with [ColossalAI](https://colossalai.org/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai) for more detailed usages.
         
         - Support gradient checkpointing. Refer to the [Save Memory on GPU](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing) for more details.
         
         - Supports multiple visualization backends, including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html) for more details.
         
-        Read [Changelog](./docs/en/notes/changelog.md#v090-10102023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v091-03112023) for more details.
         
         ## Table of Contents
         
         - [Introduction](#introduction)
         - [Installation](#installation)
         - [Get Started](#get-started)
         - [Learn More](#learn-more)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.9.0 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.9.1 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OOppeennMMMMLLaabb wweebbssiittee _H_O_T_      OOppeennMMMMLLaabb ppllaattffoorrmm _T_R_Y_ _I_T_ _O_U_T
@@ -16,25 +16,25 @@
  open-mmlab/mmengine/issues) [![issue resolution](https://isitmaintained.com/
    badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
 mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
      ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
-## What's New v0.9.0 was released on 2023-10-10. Highlights: - Support training
+## What's New v0.9.1 was released on 2023-11-03. Highlights: - Support training
 with [ColossalAI](https://colossalai.org/). Refer to the [Training Large
 Models](https://mmengine.readthedocs.io/en/latest/common_usage/
 large_model_training.html#colossalai) for more detailed usages. - Support
 gradient checkpointing. Refer to the [Save Memory on GPU](https://
 mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-
 checkpointing) for more details. - Supports multiple visualization backends,
 including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer
 to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/
 common_usage/visualize_training_log.html) for more details. Read [Changelog](./
-docs/en/notes/changelog.md#v090-10102023) for more details. ## Table of
+docs/en/notes/changelog.md#v091-03112023) for more details. ## Table of
 Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
 Started](#get-started) - [Learn More](#learn-more) - [Contributing]
 (#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
 (#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
 MMEngine is a foundational library for training deep learning models based on
 PyTorch. It provides a solid engineering foundation and frees developers from
 writing redundant codes on workflows. It serves as the training engine of all
```

### Comparing `mmengine-0.9.0/README.md` & `mmengine-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,25 @@
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
 </div>
 
 ## What's New
 
-v0.9.0 was released on 2023-10-10.
+v0.9.1 was released on 2023-11-03.
 
 Highlights:
 
 - Support training with [ColossalAI](https://colossalai.org/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai) for more detailed usages.
 
 - Support gradient checkpointing. Refer to the [Save Memory on GPU](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing) for more details.
 
 - Supports multiple visualization backends, including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html) for more details.
 
-Read [Changelog](./docs/en/notes/changelog.md#v090-10102023) for more details.
+Read [Changelog](./docs/en/notes/changelog.md#v091-03112023) for more details.
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Get Started](#get-started)
 - [Learn More](#learn-more)
```

### Comparing `mmengine-0.9.0/mmengine/_strategy/__init__.py` & `mmengine-0.9.1/mmengine/_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/_strategy/base.py` & `mmengine-0.9.1/mmengine/_strategy/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/_strategy/colossalai.py` & `mmengine-0.9.1/mmengine/_strategy/colossalai.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/_strategy/deepspeed.py` & `mmengine-0.9.1/mmengine/_strategy/deepspeed.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import torch.nn as nn
 
 import mmengine
 from mmengine.dist import init_dist
 from mmengine.optim import BaseOptimWrapper, _ParamScheduler
 from mmengine.registry import (MODEL_WRAPPERS, OPTIM_WRAPPERS, OPTIMIZERS,
                                STRATEGIES)
-from mmengine.utils import get_git_hash
+from mmengine.utils import apply_to, digit_version, get_git_hash
 from .base import BaseStrategy
 
 
 def register_deepspeed_optimizers() -> List[str]:
     """Register optimizers in ``deepspeed`` to the ``OPTIMIZERS`` registry.
 
     Returns:
@@ -184,26 +184,30 @@
 
         Returns:
             list or tuple or dict or None: Casted inputs.
         """
         if self._inputs_to_half is None:
             return inputs
 
+        dtype = next(self.model.parameters()).dtype
         if isinstance(inputs, (list, tuple)):
             new_inputs = []
             for i, v in enumerate(inputs):
                 if i in self._inputs_to_half:
-                    new_inputs.append(v.half())
+                    new_inputs.append(
+                        apply_to(v, lambda x: hasattr(x, 'to'),
+                                 lambda x: x.to(dtype)))
                 else:
                     new_inputs.append(v)
             return inputs.__class__(new_inputs)
         elif isinstance(inputs, dict):
             for k, v in inputs.items():
                 if k in self._inputs_to_half:
-                    inputs[k] = v.half()
+                    inputs[k] = apply_to(v, lambda x: hasattr(x, 'to'),
+                                         lambda x: x.to(dtype))
             return inputs
         else:
             raise TypeError('inputs should be list, tuple or dict, '
                             f'but got {type(inputs)}')
 
 
 @STRATEGIES.register_module()
@@ -241,14 +245,16 @@
             Defaults to None.
         train_micro_batch_size_per_gpu (int, optional): Batch size to be
             processed by one GPU in one step (without gradient accumulation).
             Defaults to None.
         gradient_accumulation_steps (int, optional): Number of training steps
             to accumulate gradients before averaging and applying them.
             Defaults to None.
+        exclude_frozen_parameters (bool, optional): Exclude frozen parameters
+            from saved checkpoint.
     """
 
     def __init__(
         self,
         *,
         # the following args are for deepspeed
         config: Union[str, dict, None] = None,
@@ -261,14 +267,15 @@
         activation_checkpointing: Optional[dict] = None,
         aio: Optional[dict] = None,
         train_micro_batch_size_per_gpu: Optional[int] = None,
         gradient_accumulation_steps: Optional[int] = None,
         # disable the log printed by deepseed
         steps_per_print: int = 10000000000000,
         # the following args are for BaseStrategy
+        exclude_frozen_parameters: Optional[bool] = None,
         **kwargs,
     ):
         assert deepspeed is not None, \
             'DeepSpeed is not installed. Please check ' \
             'https://github.com/microsoft/DeepSpeed#installation.'
 
         super().__init__(**kwargs)
@@ -294,14 +301,19 @@
         if gradient_accumulation_steps is not None:
             self.config['gradient_accumulation_steps'] = \
                 gradient_accumulation_steps
         else:
             self.config.setdefault('gradient_accumulation_steps', 1)
         self.config['steps_per_print'] = steps_per_print
         self._inputs_to_half = inputs_to_half
+        assert (exclude_frozen_parameters is None or
+                digit_version(deepspeed.__version__) >= digit_version('0.10.1')
+                ), ('DeepSpeed >= 0.10.1 is required to enable '
+                    'exclude_frozen_parameters')
+        self.exclude_frozen_parameters = exclude_frozen_parameters
 
         register_deepspeed_optimizers()
 
     def _parse_config(self, config):
         if config is None:
             config = dict()
         elif isinstance(config, str):
@@ -409,16 +421,23 @@
         Args:
             filename (str): Accept local filepath, URL, ``torchvision://xxx``,
                 ``open-mmlab://xxx``.
         """
         self.logger.info(f'Load checkpoint from {filename}')
 
         dirname, basename = osp.split(filename)
-        _, extra_ckpt = self.model.load_checkpoint(
-            dirname, tag=basename, load_optimizer_states=False)
+        if digit_version(deepspeed.__version__) >= digit_version('0.10.1'):
+            _, extra_ckpt = self.model.load_checkpoint(
+                dirname,
+                tag=basename,
+                load_optimizer_states=False,
+                load_module_strict=not self.exclude_frozen_parameters)
+        else:
+            _, extra_ckpt = self.model.load_checkpoint(
+                dirname, tag=basename, load_optimizer_states=False)
 
         return extra_ckpt
 
     def resume(
         self,
         filename: str,
         *,
@@ -506,9 +525,20 @@
             # when loading or resuming checkpoint.
             extra_ckpt['optim_wrapper'] = self.optim_state_dict()
 
         if save_param_scheduler and hasattr(self, 'param_schedulers'):
             extra_ckpt['param_schedulers'] = self.scheduler_state_dict()
 
         dirname, basename = osp.split(filename)
-        self.model.save_checkpoint(
-            dirname, tag=basename, client_state=extra_ckpt, save_latest=False)
+        if digit_version(deepspeed.__version__) >= digit_version('0.10.1'):
+            self.model.save_checkpoint(
+                dirname,
+                tag=basename,
+                client_state=extra_ckpt,
+                save_latest=False,
+                exclude_frozen_parameters=self.exclude_frozen_parameters)
+        else:
+            self.model.save_checkpoint(
+                dirname,
+                tag=basename,
+                client_state=extra_ckpt,
+                save_latest=False)
```

### Comparing `mmengine-0.9.0/mmengine/_strategy/distributed.py` & `mmengine-0.9.1/mmengine/_strategy/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/_strategy/fsdp.py` & `mmengine-0.9.1/mmengine/_strategy/fsdp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/_strategy/single_device.py` & `mmengine-0.9.1/mmengine/_strategy/single_device.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/_strategy/utils.py` & `mmengine-0.9.1/mmengine/_strategy/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/analysis/complexity_analysis.py` & `mmengine-0.9.1/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/analysis/jit_analysis.py` & `mmengine-0.9.1/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/analysis/jit_handles.py` & `mmengine-0.9.1/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/analysis/print_helper.py` & `mmengine-0.9.1/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/config/config.py` & `mmengine-0.9.1/mmengine/config/config.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/config/lazy.py` & `mmengine-0.9.1/mmengine/config/lazy.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/config/utils.py` & `mmengine-0.9.1/mmengine/config/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dataset/__init__.py` & `mmengine-0.9.1/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dataset/base_dataset.py` & `mmengine-0.9.1/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.9.1/mmengine/dataset/dataset_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
                     raise TypeError(
                         f'The type {cur_type} of {key} in the {i}-th dataset '
                         'should be the same with the first dataset '
                         f'{first_type}')
                 if (isinstance(self._metainfo[key], np.ndarray)
                         and not np.array_equal(self._metainfo[key],
                                                dataset.metainfo[key])
-                        or self._metainfo[key] != dataset.metainfo[key]):
+                        or (not isinstance(self._metainfo[key], np.ndarray)
+                            and self._metainfo[key] != dataset.metainfo[key])):
                     raise ValueError(
                         f'The meta information of the {i}-th dataset does not '
                         'match meta information of the first dataset')
 
         self._fully_initialized = False
         if not lazy_init:
             self.full_init()
```

### Comparing `mmengine-0.9.0/mmengine/dataset/sampler.py` & `mmengine-0.9.1/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dataset/utils.py` & `mmengine-0.9.1/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/device/utils.py` & `mmengine-0.9.1/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dist/__init__.py` & `mmengine-0.9.1/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dist/dist.py` & `mmengine-0.9.1/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/dist/utils.py` & `mmengine-0.9.1/mmengine/dist/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     # Not sure when this environment variable could be None, so use a fallback
     local_rank_env = os.environ.get('SLURM_LOCALID', None)
     if local_rank_env is not None:
         local_rank = int(local_rank_env)
     else:
         num_gpus = torch.cuda.device_count()
         local_rank = proc_id % num_gpus
-    torch.cuda.set_device(local_rank)
     addr = subprocess.getoutput(
         f'scontrol show hostname {node_list} | head -n1')
     # specify master port
     if port is not None:
         os.environ['MASTER_PORT'] = str(port)
     elif 'MASTER_PORT' in os.environ:
         pass  # use MASTER_PORT in the environment variable
@@ -202,30 +201,38 @@
     # use MASTER_ADDR in the environment variable if it already exists
     if 'MASTER_ADDR' not in os.environ:
         os.environ['MASTER_ADDR'] = addr
     os.environ['WORLD_SIZE'] = str(ntasks)
     os.environ['LOCAL_RANK'] = str(local_rank)
     os.environ['RANK'] = str(proc_id)
 
-    if init_backend == 'torch':
-        torch_dist.init_process_group(backend=backend, **kwargs)
-    elif init_backend == 'deepspeed':
-        import deepspeed
-        deepspeed.init_distributed(dist_backend=backend, **kwargs)
-    elif init_backend == 'colossalai':
-        import colossalai
-        colossalai.launch_from_slurm(
-            backend=backend,
-            host=os.environ['MASTER_ADDR'],
-            port=os.environ['MASTER_PORT'],
-            **kwargs,
-        )
+    if is_mlu_available():
+        import torch_mlu  # noqa: F401
+        torch.mlu.set_device(local_rank)
+        torch_dist.init_process_group(backend='cncl', **kwargs)
     else:
-        raise ValueError('supported "init_backend" is "torch" or "deepspeed", '
-                         f'but got {init_backend}')
+        torch.cuda.set_device(local_rank)
+
+        if init_backend == 'torch':
+            torch_dist.init_process_group(backend=backend, **kwargs)
+        elif init_backend == 'deepspeed':
+            import deepspeed
+            deepspeed.init_distributed(dist_backend=backend, **kwargs)
+        elif init_backend == 'colossalai':
+            import colossalai
+            colossalai.launch_from_slurm(
+                backend=backend,
+                host=os.environ['MASTER_ADDR'],
+                port=os.environ['MASTER_PORT'],
+                **kwargs,
+            )
+        else:
+            raise ValueError(
+                'supported "init_backend" is "torch" or "deepspeed", '
+                f'but got {init_backend}')
 
 
 def init_local_group(node_rank: int, num_gpus_per_node: int):
     """Setup the local process group.
 
     Setup a process group which only includes processes that on the same
     machine as the current process.
```

### Comparing `mmengine-0.9.0/mmengine/evaluator/evaluator.py` & `mmengine-0.9.1/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/evaluator/metric.py` & `mmengine-0.9.1/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/evaluator/utils.py` & `mmengine-0.9.1/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/__init__.py` & `mmengine-0.9.1/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/__init__.py` & `mmengine-0.9.1/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/base.py` & `mmengine-0.9.1/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/http_backend.py` & `mmengine-0.9.1/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.9.1/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/local_backend.py` & `mmengine-0.9.1/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.9.1/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.9.1/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.9.1/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/file_client.py` & `mmengine-0.9.1/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/handlers/base.py` & `mmengine-0.9.1/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.9.1/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.9.1/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.9.1/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.9.1/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/io.py` & `mmengine-0.9.1/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/fileio/parse.py` & `mmengine-0.9.1/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/__init__.py` & `mmengine-0.9.1/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.9.1/mmengine/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.9.1/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/ema_hook.py` & `mmengine-0.9.1/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.9.1/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/hook.py` & `mmengine-0.9.1/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.9.1/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/logger_hook.py` & `mmengine-0.9.1/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.9.1/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.9.1/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/profiler_hook.py` & `mmengine-0.9.1/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.9.1/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.9.1/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.9.1/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.9.1/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hub/hub.py` & `mmengine-0.9.1/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hub/mmcls.json` & `mmengine-0.9.1/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hub/openmmlab.json` & `mmengine-0.9.1/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/hub/torchvision_0.12.json` & `mmengine-0.9.1/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/infer/infer.py` & `mmengine-0.9.1/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/logging/history_buffer.py` & `mmengine-0.9.1/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/logging/logger.py` & `mmengine-0.9.1/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/logging/message_hub.py` & `mmengine-0.9.1/mmengine/logging/message_hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/__init__.py` & `mmengine-0.9.1/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/averaged_model.py` & `mmengine-0.9.1/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/base_model/base_model.py` & `mmengine-0.9.1/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.9.1/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/base_module.py` & `mmengine-0.9.1/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/efficient_conv_bn_eval.py` & `mmengine-0.9.1/mmengine/model/efficient_conv_bn_eval.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/test_time_aug.py` & `mmengine-0.9.1/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/utils.py` & `mmengine-0.9.1/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/weight_init.py` & `mmengine-0.9.1/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/wrappers/__init__.py` & `mmengine-0.9.1/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/wrappers/distributed.py` & `mmengine-0.9.1/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.9.1/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.9.1/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/model/wrappers/utils.py` & `mmengine-0.9.1/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/__init__.py` & `mmengine-0.9.1/mmengine/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/__init__.py` & `mmengine-0.9.1/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.9.1/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.9.1/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/base.py` & `mmengine-0.9.1/mmengine/optim/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/builder.py` & `mmengine-0.9.1/mmengine/optim/optimizer/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,33 +128,35 @@
 
 SOPHIA_OPTIMIZERS = register_sophia_optimizers()
 
 
 def register_bitsandbytes_optimizers() -> List[str]:
     """Register optimizers in ``bitsandbytes`` to the ``OPTIMIZERS`` registry.
 
+    In the `bitsandbytes` library, optimizers that have the same name as the
+    default optimizers in PyTorch are prefixed with ``bnb_``. For example,
+    ``bnb_Adagrad``.
+
     Returns:
         List[str]: A list of registered optimizers' name.
     """
     dadaptation_optimizers = []
     try:
         import bitsandbytes as bnb
     except ImportError:
         pass
     else:
-        for module_name in [
-                'AdamW8bit', 'Adam8bit', 'Adagrad8bit', 'PagedAdam8bit',
-                'PagedAdamW8bit', 'LAMB8bit', 'LARS8bit', 'RMSprop8bit',
-                'Lion8bit', 'PagedLion8bit', 'SGD8bit'
-        ]:
-            _optim = getattr(bnb.optim, module_name)
-            if inspect.isclass(_optim) and issubclass(_optim,
-                                                      torch.optim.Optimizer):
-                OPTIMIZERS.register_module(module=_optim)
-                dadaptation_optimizers.append(module_name)
+        optim_classes = inspect.getmembers(
+            bnb.optim, lambda _optim: (inspect.isclass(_optim) and issubclass(
+                _optim, torch.optim.Optimizer)))
+        for name, optim_cls in optim_classes:
+            if name in OPTIMIZERS:
+                name = f'bnb_{name}'
+            OPTIMIZERS.register_module(module=optim_cls, name=name)
+            dadaptation_optimizers.append(name)
     return dadaptation_optimizers
 
 
 BITSANDBYTES_OPTIMIZERS = register_bitsandbytes_optimizers()
 
 
 def register_transformers_optimizers():
```

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.9.1/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.9.1/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.9.1/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.9.1/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/scheduler/__init__.py` & `mmengine-0.9.1/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.9.1/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.9.1/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.9.1/mmengine/optim/scheduler/param_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,15 +980,15 @@
         # Validate total_steps
         if total_steps is not None:
             if total_steps <= 0 or not isinstance(total_steps, int):
                 raise ValueError('Expected positive integer total_steps, '
                                  f'but got {total_steps}')
             self.total_steps = total_steps
         else:
-            self.total_steps = self.end - self.begin
+            self.total_steps = end - begin
 
         # Validate pct_start
         if pct_start < 0 or pct_start > 1 or not isinstance(pct_start, float):
             raise ValueError('Expected float between 0 and 1 pct_start, '
                              f'but got {pct_start}')
 
         # Validate anneal_strategy
```

### Comparing `mmengine-0.9.0/mmengine/registry/__init__.py` & `mmengine-0.9.1/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/registry/build_functions.py` & `mmengine-0.9.1/mmengine/registry/build_functions.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/registry/default_scope.py` & `mmengine-0.9.1/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/registry/registry.py` & `mmengine-0.9.1/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/registry/root.py` & `mmengine-0.9.1/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/registry/utils.py` & `mmengine-0.9.1/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/__init__.py` & `mmengine-0.9.1/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/_flexible_runner.py` & `mmengine-0.9.1/mmengine/runner/_flexible_runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/activation_checkpointing.py` & `mmengine-0.9.1/mmengine/runner/activation_checkpointing.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/amp.py` & `mmengine-0.9.1/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/base_loop.py` & `mmengine-0.9.1/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/checkpoint.py` & `mmengine-0.9.1/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/log_processor.py` & `mmengine-0.9.1/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/loops.py` & `mmengine-0.9.1/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/priority.py` & `mmengine-0.9.1/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/runner.py` & `mmengine-0.9.1/mmengine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/runner/utils.py` & `mmengine-0.9.1/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/structures/base_data_element.py` & `mmengine-0.9.1/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/structures/instance_data.py` & `mmengine-0.9.1/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/structures/label_data.py` & `mmengine-0.9.1/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/structures/pixel_data.py` & `mmengine-0.9.1/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/testing/__init__.py` & `mmengine-0.9.1/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/testing/_internal/distributed.py` & `mmengine-0.9.1/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/testing/compare.py` & `mmengine-0.9.1/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/testing/runner_test_case.py` & `mmengine-0.9.1/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/__init__.py` & `mmengine-0.9.1/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/hub.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/misc.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/trace.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.9.1/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/manager.py` & `mmengine-0.9.1/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/misc.py` & `mmengine-0.9.1/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/package_utils.py` & `mmengine-0.9.1/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/path.py` & `mmengine-0.9.1/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/progressbar.py` & `mmengine-0.9.1/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/progressbar_rich.py` & `mmengine-0.9.1/mmengine/utils/progressbar_rich.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/timer.py` & `mmengine-0.9.1/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/utils/version_utils.py` & `mmengine-0.9.1/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/version.py` & `mmengine-0.9.1/mmengine/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.9.0/mmengine/visualization/__init__.py` & `mmengine-0.9.1/mmengine/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/visualization/utils.py` & `mmengine-0.9.1/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine/visualization/vis_backend.py` & `mmengine-0.9.1/mmengine/visualization/vis_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
 
         Args:
             config (Config): The Config object
         """
         assert isinstance(self._init_kwargs, dict)
         allow_val_change = self._init_kwargs.get('allow_val_change', False)
         self._wandb.config.update(
-            dict(config), allow_val_change=allow_val_change)
+            config.to_dict(), allow_val_change=allow_val_change)
         self._wandb.run.log_code(name=self._log_code_name)
 
     @force_init_env
     def add_graph(self, model: torch.nn.Module, data_batch: Sequence[dict],
                   **kwargs) -> None:
         """Record the model graph.
 
@@ -748,15 +748,15 @@
         """Record the config to mlflow.
 
         Args:
             config (Config): The Config object
         """
         self.cfg = config
         if self._tracked_config_keys is None:
-            self._mlflow.log_params(self._flatten(self.cfg))
+            self._mlflow.log_params(self._flatten(self.cfg.to_dict()))
         else:
             tracked_cfg = dict()
             for k in self._tracked_config_keys:
                 tracked_cfg[k] = self.cfg[k]
             self._mlflow.log_params(self._flatten(tracked_cfg))
         self._mlflow.log_text(self.cfg.pretty_text, 'config.py')
 
@@ -911,15 +911,15 @@
     def add_config(self, config: Config, **kwargs) -> None:
         """Record the config to clearml.
 
         Args:
             config (Config): The Config object
         """
         self.cfg = config
-        self._task.connect_configuration(vars(config))
+        self._task.connect_configuration(config.to_dict())
 
     @force_init_env
     def add_image(self,
                   name: str,
                   image: np.ndarray,
                   step: int = 0,
                   **kwargs) -> None:
@@ -1212,15 +1212,15 @@
         """Record the config to dvclive.
 
         Args:
             config (Config): The Config object
         """
         assert isinstance(config, Config)
         self.cfg = config
-        self._dvclive.log_params(self._to_dvc_paramlike(self.cfg))
+        self._dvclive.log_params(self._to_dvc_paramlike(self.cfg.to_dict()))
 
     @force_init_env
     def add_image(self,
                   name: str,
                   image: np.ndarray,
                   step: int = 0,
                   **kwargs) -> None:
```

### Comparing `mmengine-0.9.0/mmengine/visualization/visualizer.py` & `mmengine-0.9.1/mmengine/visualization/visualizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine.egg-info/PKG-INFO` & `mmengine-0.9.1/mmengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.9.0
+Version: 0.9.1
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -62,25 +62,25 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.9.0 was released on 2023-10-10.
+        v0.9.1 was released on 2023-11-03.
         
         Highlights:
         
         - Support training with [ColossalAI](https://colossalai.org/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai) for more detailed usages.
         
         - Support gradient checkpointing. Refer to the [Save Memory on GPU](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing) for more details.
         
         - Supports multiple visualization backends, including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html) for more details.
         
-        Read [Changelog](./docs/en/notes/changelog.md#v090-10102023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v091-03112023) for more details.
         
         ## Table of Contents
         
         - [Introduction](#introduction)
         - [Installation](#installation)
         - [Get Started](#get-started)
         - [Learn More](#learn-more)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.9.0 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.9.1 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OOppeennMMMMLLaabb wweebbssiittee _H_O_T_      OOppeennMMMMLLaabb ppllaattffoorrmm _T_R_Y_ _I_T_ _O_U_T
@@ -16,25 +16,25 @@
  open-mmlab/mmengine/issues) [![issue resolution](https://isitmaintained.com/
    badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
 mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
      ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
-## What's New v0.9.0 was released on 2023-10-10. Highlights: - Support training
+## What's New v0.9.1 was released on 2023-11-03. Highlights: - Support training
 with [ColossalAI](https://colossalai.org/). Refer to the [Training Large
 Models](https://mmengine.readthedocs.io/en/latest/common_usage/
 large_model_training.html#colossalai) for more detailed usages. - Support
 gradient checkpointing. Refer to the [Save Memory on GPU](https://
 mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-
 checkpointing) for more details. - Supports multiple visualization backends,
 including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer
 to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/
 common_usage/visualize_training_log.html) for more details. Read [Changelog](./
-docs/en/notes/changelog.md#v090-10102023) for more details. ## Table of
+docs/en/notes/changelog.md#v091-03112023) for more details. ## Table of
 Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
 Started](#get-started) - [Learn More](#learn-more) - [Contributing]
 (#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
 (#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
 MMEngine is a foundational library for training deep learning models based on
 PyTorch. It provides a solid engineering foundation and frees developers from
 writing redundant codes on workflows. It serves as the training engine of all
```

### Comparing `mmengine-0.9.0/mmengine.egg-info/SOURCES.txt` & `mmengine-0.9.1/mmengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/mmengine.egg-info/requires.txt` & `mmengine-0.9.1/mmengine.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.9.0/setup.py` & `mmengine-0.9.1/setup.py`

 * *Files identical despite different names*

