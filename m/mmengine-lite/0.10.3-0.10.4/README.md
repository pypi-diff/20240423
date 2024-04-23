# Comparing `tmp/mmengine-lite-0.10.3.tar.gz` & `tmp/mmengine-lite-0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-lite-0.10.3.tar", last modified: Wed Jan 24 04:50:06 2024, max compression
+gzip compressed data, was "dist/mmengine-lite-0.10.4.tar", last modified: Tue Apr 23 03:30:49 2024, max compression
```

## Comparing `mmengine-lite-0.10.3.tar` & `mmengine-lite-0.10.4.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21854 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/colossalai.py
--rw-r--r--   0 runner    (1001) docker     (127)    22446 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    28890 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/_strategy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26249 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (127)    31115 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74205 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/config/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18486 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34071 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18135 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27918 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29994 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27712 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19045 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/efficient_conv_bn_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26125 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15161 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17881 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    64420 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    26948 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66602 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/_flexible_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/activation_checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    30359 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)   103199 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24942 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17518 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/progressbar_rich.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52896 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    54108 2024-01-24 04:49:59.000000 mmengine-lite-0.10.3/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21854 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/mmengine_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-01-24 04:50:06.000000 mmengine-lite-0.10.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-01-24 04:50:04.000000 mmengine-lite-0.10.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21817 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18033 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/colossalai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22170 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28890 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26249 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31115 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74459 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18486 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34071 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18135 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27918 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29994 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27712 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19043 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/efficient_conv_bn_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26125 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17881 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64420 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26948 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66602 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/activation_checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30359 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103199 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24942 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17518 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/progressbar_rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53275 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54106 2024-04-23 03:30:46.000000 mmengine-lite-0.10.4/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21817 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/mmengine_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-23 03:30:49.000000 mmengine-lite-0.10.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-23 03:30:48.000000 mmengine-lite-0.10.4/setup.py
```

### Comparing `mmengine-lite-0.10.3/PKG-INFO` & `mmengine-lite-0.10.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine-lite
-Version: 0.10.3
+Version: 0.10.4
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -23,21 +23,22 @@
                 <i><font size="4">TRY IT OUT</font></i>
               </a>
             </sup>
           </div>
           <div>&nbsp;</div>
         
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mmengine)](https://pypi.org/project/mmengine/)
+        [![pytorch](https://img.shields.io/badge/pytorch-1.6~2.1-yellow)](#installation)
         [![PyPI](https://img.shields.io/pypi/v/mmengine)](https://pypi.org/project/mmengine)
         [![license](https://img.shields.io/github/license/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/blob/main/LICENSE)
-        [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/issues)
-        [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/issues)
         
+        [Introduction](#introduction) |
+        [Installation](#installation) |
+        [Get Started](#get-started) |
         [📘Documentation](https://mmengine.readthedocs.io/en/latest/) |
-        [🛠️Installation](https://mmengine.readthedocs.io/en/latest/get_started/installation.html) |
         [🤔Reporting Issues](https://github.com/open-mmlab/mmengine/issues/new/choose)
         
         </div>
         
         <div align="center">
         
         English | [简体中文](README_zh-CN.md)
@@ -62,65 +63,60 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.10.3 was released on 2024-1-24.
+        v0.10.4 was released on 2024-4-23.
         
         Highlights:
         
-        - Support installing mmengine-lite with no dependency on opencv. Refer to the [Installation](https://mmengine.readthedocs.io/en/latest/get_started/installation.html#install-mmengine) for more details.
+        - Support custom `artifact_location` in MLflowVisBackend [#1505](#1505)
+        - Enable `exclude_frozen_parameters` for `DeepSpeedEngine._zero3_consolidated_16bit_state_dict` [#1517](#1517)
         
-        - Support training with [ColossalAI](https://colossalai.org/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai) for more detailed usages.
+        Read [Changelog](./docs/en/notes/changelog.md#v0104-2342024) for more details.
         
-        - Support gradient checkpointing. Refer to the [Save Memory on GPU](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing) for more details.
-        
-        - Supports multiple visualization backends, including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html) for more details.
-        
-        Read [Changelog](./docs/en/notes/changelog.md#v0103-2412024) for more details.
+        ## Introduction
         
-        ## Table of Contents
+        MMEngine is a foundational library for training deep learning models based on PyTorch. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects. Its highlights are as follows:
         
-        - [Introduction](#introduction)
-        - [Installation](#installation)
-        - [Get Started](#get-started)
-        - [Learn More](#learn-more)
-        - [Contributing](#contributing)
-        - [Citation](#citation)
-        - [License](#license)
-        - [Ecosystem](#ecosystem)
-        - [Projects in OpenMMLab](#projects-in-openmmlab)
+        **Integrate mainstream large-scale model training frameworks**
         
-        ## Introduction
+        - [ColossalAI](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai)
+        - [DeepSpeed](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#deepspeed)
+        - [FSDP](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#fullyshardeddataparallel-fsdp)
         
-        MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
+        **Supports a variety of training strategies**
         
-        Major features:
+        - [Mixed Precision Training](https://mmengine.readthedocs.io/en/latest/common_usage/speed_up_training.html#mixed-precision-training)
+        - [Gradient Accumulation](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-accumulation)
+        - [Gradient Checkpointing](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing)
         
-        1. **A universal and powerful runner**:
+        **Provides a user-friendly configuration system**
         
-           - Supports training different tasks with a small amount of code, e.g., ImageNet can be trained with only 80 lines of code (400 lines of the original PyTorch example).
-           - Easily compatible with models from popular algorithm libraries such as TIMM, TorchVision, and Detectron2.
+        - [Pure Python-style configuration files, easy to navigate](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta)
+        - [Plain-text-style configuration files, supporting JSON and YAML](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html)
         
-        2. **Open architecture with unified interfaces**:
+        **Covers mainstream training monitoring platforms**
         
-           - Handles different algorithm tasks with unified APIs, e.g., implement a method and apply it to all compatible models.
-           - Provides a unified abstraction for upper-level algorithm libraries, which supports various back-end devices such as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training.
+        - [TensorBoard](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#tensorboard) | [WandB](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#wandb) | [MLflow](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#mlflow-wip)
+        - [ClearML](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) | [Neptune](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#neptune) | [DVCLive](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#dvclive) | [Aim](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#aim)
         
-        3. **Customizable training process**:
+        ## Installation
         
-           - Defines the training process just like playing with Legos.
-           - Provides rich components and strategies.
-           - Complete controls on the training process with different levels of APIs.
+        <details>
+        <summary>Supported PyTorch Versions</summary>
         
-        ![mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/267db9cb-72e4-4af2-a58b-877b30091acc)
+        | MMEngine           | PyTorch      | Python         |
+        | ------------------ | ------------ | -------------- |
+        | main               | >=1.6 \<=2.1 | >=3.8, \<=3.11 |
+        | >=0.9.0, \<=0.10.4 | >=1.6 \<=2.1 | >=3.8, \<=3.11 |
         
-        ## Installation
+        </details>
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
         
         ```bash
         pip install -U openmim
```

#### html2text {}

```diff
@@ -1,66 +1,69 @@
-Metadata-Version: 2.1 Name: mmengine-lite Version: 0.10.3 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine-lite Version: 0.10.4 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OOppeennMMMMLLaabb wweebbssiittee _H_O_T_      OOppeennMMMMLLaabb ppllaattffoorrmm _T_R_Y_ _I_T_ _O_U_T
                                         
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mmengine)]
- (https://pypi.org/project/mmengine/) [![PyPI](https://img.shields.io/pypi/v/
+(https://pypi.org/project/mmengine/) [![pytorch](https://img.shields.io/badge/
+pytorch-1.6~2.1-yellow)](#installation) [![PyPI](https://img.shields.io/pypi/v/
       mmengine)](https://pypi.org/project/mmengine) [![license](https://
   img.shields.io/github/license/open-mmlab/mmengine.svg)](https://github.com/
-        open-mmlab/mmengine/blob/main/LICENSE) [![open issues](https://
-  isitmaintained.com/badge/open/open-mmlab/mmengine.svg)](https://github.com/
- open-mmlab/mmengine/issues) [![issue resolution](https://isitmaintained.com/
-   badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
-mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
-     ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
-  get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
-                    open-mmlab/mmengine/issues/new/choose)
+    open-mmlab/mmengine/blob/main/LICENSE) [Introduction](#introduction) |
+        [Installation](#installation) | [Get Started](#get-started) |
+      [ðDocumentation](https://mmengine.readthedocs.io/en/latest/) |
+   [ð¤Reporting Issues](https://github.com/open-mmlab/mmengine/issues/new/
+                                    choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
-## What's New v0.10.3 was released on 2024-1-24. Highlights: - Support
-installing mmengine-lite with no dependency on opencv. Refer to the
-[Installation](https://mmengine.readthedocs.io/en/latest/get_started/
-installation.html#install-mmengine) for more details. - Support training with
-[ColossalAI](https://colossalai.org/). Refer to the [Training Large Models]
+## What's New v0.10.4 was released on 2024-4-23. Highlights: - Support custom
+`artifact_location` in MLflowVisBackend [#1505](#1505) - Enable
+`exclude_frozen_parameters` for
+`DeepSpeedEngine._zero3_consolidated_16bit_state_dict` [#1517](#1517) Read
+[Changelog](./docs/en/notes/changelog.md#v0104-2342024) for more details. ##
+Introduction MMEngine is a foundational library for training deep learning
+models based on PyTorch. It serves as the training engine of all OpenMMLab
+codebases, which support hundreds of algorithms in various research areas.
+Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects. Its
+highlights are as follows: **Integrate mainstream large-scale model training
+frameworks** - [ColossalAI](https://mmengine.readthedocs.io/en/latest/
+common_usage/large_model_training.html#colossalai) - [DeepSpeed](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+large_model_training.html#deepspeed) - [FSDP](https://mmengine.readthedocs.io/
+en/latest/common_usage/large_model_training.html#fullyshardeddataparallel-fsdp)
+**Supports a variety of training strategies** - [Mixed Precision Training]
 (https://mmengine.readthedocs.io/en/latest/common_usage/
-large_model_training.html#colossalai) for more detailed usages. - Support
-gradient checkpointing. Refer to the [Save Memory on GPU](https://
+speed_up_training.html#mixed-precision-training) - [Gradient Accumulation]
+(https://mmengine.readthedocs.io/en/latest/common_usage/
+save_gpu_memory.html#gradient-accumulation) - [Gradient Checkpointing](https://
 mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-
-checkpointing) for more details. - Supports multiple visualization backends,
-including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer
-to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/
-common_usage/visualize_training_log.html) for more details. Read [Changelog](./
-docs/en/notes/changelog.md#v0103-2412024) for more details. ## Table of
-Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
-Started](#get-started) - [Learn More](#learn-more) - [Contributing]
-(#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
-(#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
-MMEngine is a foundational library for training deep learning models based on
-PyTorch. It provides a solid engineering foundation and frees developers from
-writing redundant codes on workflows. It serves as the training engine of all
-OpenMMLab codebases, which support hundreds of algorithms in various research
-areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab
-projects. Major features: 1. **A universal and powerful runner**: - Supports
-training different tasks with a small amount of code, e.g., ImageNet can be
-trained with only 80 lines of code (400 lines of the original PyTorch example).
-- Easily compatible with models from popular algorithm libraries such as TIMM,
-TorchVision, and Detectron2. 2. **Open architecture with unified interfaces**:
-- Handles different algorithm tasks with unified APIs, e.g., implement a method
-and apply it to all compatible models. - Provides a unified abstraction for
-upper-level algorithm libraries, which supports various back-end devices such
-as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training. 3.
-**Customizable training process**: - Defines the training process just like
-playing with Legos. - Provides rich components and strategies. - Complete
-controls on the training process with different levels of APIs. !
-[mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/
-267db9cb-72e4-4af2-a58b-877b30091acc) ## Installation Before installing
+checkpointing) **Provides a user-friendly configuration system** - [Pure
+Python-style configuration files, easy to navigate](https://
+mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-
+style-configuration-file-beta) - [Plain-text-style configuration files,
+supporting JSON and YAML](https://mmengine.readthedocs.io/en/latest/
+advanced_tutorials/config.html) **Covers mainstream training monitoring
+platforms** - [TensorBoard](https://mmengine.readthedocs.io/en/latest/
+common_usage/visualize_training_log.html#tensorboard) | [WandB](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#wandb) | [MLflow](https://mmengine.readthedocs.io/
+en/latest/common_usage/visualize_training_log.html#mlflow-wip) - [ClearML]
+(https://mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#clearml) | [Neptune](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#neptune) | [DVCLive](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#dvclive) | [Aim](https://mmengine.readthedocs.io/
+en/latest/common_usage/visualize_training_log.html#aim) ## Installation
+Supported PyTorch Versions | MMEngine | PyTorch | Python | | -----------------
+- | ------------ | -------------- | | main | >=1.6 \<=2.1 | >=3.8, \<=3.11 | |
+>=0.9.0, \<=0.10.4 | >=1.6 \<=2.1 | >=3.8, \<=3.11 | Before installing
 MMEngine, please ensure that PyTorch has been successfully installed following
 the [official guide](https://pytorch.org/get-started/locally/). Install
 MMEngine ```bash pip install -U openmim mim install mmengine ``` Verify the
 installation ```bash python -c 'from mmengine.utils.dl_utils import
 collect_env;print(collect_env())' ``` ## Get Started Taking the training of a
 ResNet-50 model on the CIFAR-10 dataset as an example, we will use MMEngine to
 build a complete, configurable training and validation process in less than 80
```

### Comparing `mmengine-lite-0.10.3/README.md` & `mmengine-lite-0.10.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,21 +15,22 @@
         <i><font size="4">TRY IT OUT</font></i>
       </a>
     </sup>
   </div>
   <div>&nbsp;</div>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mmengine)](https://pypi.org/project/mmengine/)
+[![pytorch](https://img.shields.io/badge/pytorch-1.6~2.1-yellow)](#installation)
 [![PyPI](https://img.shields.io/pypi/v/mmengine)](https://pypi.org/project/mmengine)
 [![license](https://img.shields.io/github/license/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/blob/main/LICENSE)
-[![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/issues)
-[![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/issues)
 
+[Introduction](#introduction) |
+[Installation](#installation) |
+[Get Started](#get-started) |
 [📘Documentation](https://mmengine.readthedocs.io/en/latest/) |
-[🛠️Installation](https://mmengine.readthedocs.io/en/latest/get_started/installation.html) |
 [🤔Reporting Issues](https://github.com/open-mmlab/mmengine/issues/new/choose)
 
 </div>
 
 <div align="center">
 
 English | [简体中文](README_zh-CN.md)
@@ -54,65 +55,60 @@
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
 </div>
 
 ## What's New
 
-v0.10.3 was released on 2024-1-24.
+v0.10.4 was released on 2024-4-23.
 
 Highlights:
 
-- Support installing mmengine-lite with no dependency on opencv. Refer to the [Installation](https://mmengine.readthedocs.io/en/latest/get_started/installation.html#install-mmengine) for more details.
+- Support custom `artifact_location` in MLflowVisBackend [#1505](#1505)
+- Enable `exclude_frozen_parameters` for `DeepSpeedEngine._zero3_consolidated_16bit_state_dict` [#1517](#1517)
 
-- Support training with [ColossalAI](https://colossalai.org/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai) for more detailed usages.
+Read [Changelog](./docs/en/notes/changelog.md#v0104-2342024) for more details.
 
-- Support gradient checkpointing. Refer to the [Save Memory on GPU](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing) for more details.
-
-- Supports multiple visualization backends, including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html) for more details.
-
-Read [Changelog](./docs/en/notes/changelog.md#v0103-2412024) for more details.
+## Introduction
 
-## Table of Contents
+MMEngine is a foundational library for training deep learning models based on PyTorch. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects. Its highlights are as follows:
 
-- [Introduction](#introduction)
-- [Installation](#installation)
-- [Get Started](#get-started)
-- [Learn More](#learn-more)
-- [Contributing](#contributing)
-- [Citation](#citation)
-- [License](#license)
-- [Ecosystem](#ecosystem)
-- [Projects in OpenMMLab](#projects-in-openmmlab)
+**Integrate mainstream large-scale model training frameworks**
 
-## Introduction
+- [ColossalAI](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai)
+- [DeepSpeed](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#deepspeed)
+- [FSDP](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#fullyshardeddataparallel-fsdp)
 
-MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
+**Supports a variety of training strategies**
 
-Major features:
+- [Mixed Precision Training](https://mmengine.readthedocs.io/en/latest/common_usage/speed_up_training.html#mixed-precision-training)
+- [Gradient Accumulation](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-accumulation)
+- [Gradient Checkpointing](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing)
 
-1. **A universal and powerful runner**:
+**Provides a user-friendly configuration system**
 
-   - Supports training different tasks with a small amount of code, e.g., ImageNet can be trained with only 80 lines of code (400 lines of the original PyTorch example).
-   - Easily compatible with models from popular algorithm libraries such as TIMM, TorchVision, and Detectron2.
+- [Pure Python-style configuration files, easy to navigate](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta)
+- [Plain-text-style configuration files, supporting JSON and YAML](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html)
 
-2. **Open architecture with unified interfaces**:
+**Covers mainstream training monitoring platforms**
 
-   - Handles different algorithm tasks with unified APIs, e.g., implement a method and apply it to all compatible models.
-   - Provides a unified abstraction for upper-level algorithm libraries, which supports various back-end devices such as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training.
+- [TensorBoard](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#tensorboard) | [WandB](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#wandb) | [MLflow](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#mlflow-wip)
+- [ClearML](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) | [Neptune](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#neptune) | [DVCLive](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#dvclive) | [Aim](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#aim)
 
-3. **Customizable training process**:
+## Installation
 
-   - Defines the training process just like playing with Legos.
-   - Provides rich components and strategies.
-   - Complete controls on the training process with different levels of APIs.
+<details>
+<summary>Supported PyTorch Versions</summary>
 
-![mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/267db9cb-72e4-4af2-a58b-877b30091acc)
+| MMEngine           | PyTorch      | Python         |
+| ------------------ | ------------ | -------------- |
+| main               | >=1.6 \<=2.1 | >=3.8, \<=3.11 |
+| >=0.9.0, \<=0.10.4 | >=1.6 \<=2.1 | >=3.8, \<=3.11 |
 
-## Installation
+</details>
 
 Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
 
 Install MMEngine
 
 ```bash
 pip install -U openmim
```

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/__init__.py` & `mmengine-lite-0.10.4/mmengine/_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/base.py` & `mmengine-lite-0.10.4/mmengine/_strategy/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/colossalai.py` & `mmengine-lite-0.10.4/mmengine/_strategy/colossalai.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/deepspeed.py` & `mmengine-lite-0.10.4/mmengine/_strategy/deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,16 +307,16 @@
             self.config['gradient_accumulation_steps'] = \
                 gradient_accumulation_steps
         else:
             self.config.setdefault('gradient_accumulation_steps', 1)
         self.config['steps_per_print'] = steps_per_print
         self._inputs_to_half = inputs_to_half
         assert (exclude_frozen_parameters is None or
-                digit_version(deepspeed.__version__) >= digit_version('0.10.1')
-                ), ('DeepSpeed >= 0.10.1 is required to enable '
+                digit_version(deepspeed.__version__) >= digit_version('0.13.2')
+                ), ('DeepSpeed >= 0.13.2 is required to enable '
                     'exclude_frozen_parameters')
         self.exclude_frozen_parameters = exclude_frozen_parameters
 
         register_deepspeed_optimizers()
 
     def _parse_config(self, config):
         if config is None:
@@ -426,15 +426,15 @@
         Args:
             filename (str): Accept local filepath, URL, ``torchvision://xxx``,
                 ``open-mmlab://xxx``.
         """
         self.logger.info(f'Load checkpoint from {filename}')
 
         dirname, basename = osp.split(filename)
-        if digit_version(deepspeed.__version__) >= digit_version('0.10.1'):
+        if digit_version(deepspeed.__version__) >= digit_version('0.13.2'):
             _, extra_ckpt = self.model.load_checkpoint(
                 dirname,
                 tag=basename,
                 load_optimizer_states=False,
                 load_module_strict=not self.exclude_frozen_parameters)
         else:
             _, extra_ckpt = self.model.load_checkpoint(
@@ -464,15 +464,15 @@
                 Defaults to True.
             resume_param_scheduler (bool): Whether to resume param scheduler
                 state. Defaults to True.
         """
         self.logger.info(f'Resume checkpoint from {filename}')
 
         dirname, basename = osp.split(filename)
-        if digit_version(deepspeed.__version__) >= digit_version('0.10.1'):
+        if digit_version(deepspeed.__version__) >= digit_version('0.13.2'):
             _, extra_ckpt = self.model.load_checkpoint(
                 dirname,
                 tag=basename,
                 load_optimizer_states=resume_optimizer,
                 load_module_strict=not self.exclude_frozen_parameters)
         else:
             _, extra_ckpt = self.model.load_checkpoint(
@@ -547,38 +547,35 @@
                 'To support `save_optimizer=False`, please set '
                 '`gather_16bit_weights_on_model_save=True` in your '
                 'DeepSpeed config.',
                 logger='current',
                 level=logging.WARNING)
             save_optimizer = True
 
+        state_dict_kwargs = {}
+        if digit_version(deepspeed.__version__) >= digit_version('0.13.2'):
+            state_dict_kwargs[
+                'exclude_frozen_parameters'] = self.exclude_frozen_parameters
+
         if save_optimizer:
             if hasattr(self, 'optim_wrapper'):
                 # The key can not be 'optimizer', otherwise error will be
                 # thrown when loading or resuming checkpoint.
                 extra_ckpt['optim_wrapper'] = self.optim_state_dict()
 
             dirname, basename = osp.split(filename)
-            if digit_version(deepspeed.__version__) >= digit_version('0.10.1'):
-                self.model.save_checkpoint(
-                    dirname,
-                    tag=basename,
-                    client_state=extra_ckpt,
-                    save_latest=False,
-                    exclude_frozen_parameters=self.exclude_frozen_parameters)
-            else:
-                self.model.save_checkpoint(
-                    dirname,
-                    tag=basename,
-                    client_state=extra_ckpt,
-                    save_latest=False)
+            self.model.save_checkpoint(
+                dirname,
+                tag=basename,
+                client_state=extra_ckpt,
+                save_latest=False,
+                **state_dict_kwargs)
         else:
             if self.model.zero_optimization_partition_weights():
-                # TODO: `_zero3_consolidated_16bit_state_dict` doesn't support
-                # `exclude_frozen_parameters`.
-                state_dict = self.model._zero3_consolidated_16bit_state_dict()
+                state_dict = self.model._zero3_consolidated_16bit_state_dict(
+                    **state_dict_kwargs)
             else:
-                state_dict = self.model.module_state_dict(
-                    exclude_frozen_parameters=self.exclude_frozen_parameters)
+                state_dict = self.model.module_state_dict(**state_dict_kwargs)
+
             if is_main_process():
                 ckpt = {'state_dict': weights_to_cpu(state_dict), **extra_ckpt}
                 save_checkpoint(ckpt, filename)
```

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/distributed.py` & `mmengine-lite-0.10.4/mmengine/_strategy/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/fsdp.py` & `mmengine-lite-0.10.4/mmengine/_strategy/fsdp.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/single_device.py` & `mmengine-lite-0.10.4/mmengine/_strategy/single_device.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/_strategy/utils.py` & `mmengine-lite-0.10.4/mmengine/_strategy/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/analysis/complexity_analysis.py` & `mmengine-lite-0.10.4/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/analysis/jit_analysis.py` & `mmengine-lite-0.10.4/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/analysis/jit_handles.py` & `mmengine-lite-0.10.4/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/analysis/print_helper.py` & `mmengine-lite-0.10.4/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/config/config.py` & `mmengine-lite-0.10.4/mmengine/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,14 +440,16 @@
 
         Args:
             filename (str or Path): Name of config file.
             use_predefined_variables (bool, optional): Whether to use
                 predefined variables. Defaults to True.
             import_custom_modules (bool, optional): Whether to support
                 importing custom modules in config. Defaults to None.
+            use_environment_variables (bool, optional): Whether to use
+                environment variables. Defaults to True.
             lazy_import (bool): Whether to load config in `lazy_import` mode.
                 If it is `None`, it will be deduced by the content of the
                 config file. Defaults to None.
             format_python_code (bool): Whether to format Python code by yapf.
                 Defaults to True.
 
         Returns:
@@ -827,14 +829,16 @@
             lazy_import: Optional[bool] = None) -> Tuple[dict, str, dict]:
         """Transform file to variables dictionary.
 
         Args:
             filename (str): Name of config file.
             use_predefined_variables (bool, optional): Whether to use
                 predefined variables. Defaults to True.
+            use_environment_variables (bool, optional): Whether to use
+                environment variables. Defaults to True.
             lazy_import (bool): Whether to load config in `lazy_import` mode.
                 If it is `None`, it will be deduced by the content of the
                 config file. Defaults to None.
 
         Returns:
             Tuple[dict, str]: Variables dictionary and text of Config.
         """
@@ -897,15 +901,15 @@
                             f'Duplicate keys: {duplicate_keys}')
 
                     # _dict_to_config_dict will do the following things:
                     # 1. Recursively converts ``dict`` to :obj:`ConfigDict`.
                     # 2. Set `_scope_` for the outer dict variable for the base
                     # config.
                     # 3. Set `scope` attribute for each base variable.
-                    # Different from `_scope_`， `scope` is not a key of base
+                    # Different from `_scope_`, `scope` is not a key of base
                     # dict, `scope` attribute will be parsed to key `_scope_`
                     # by function `_parse_scope` only if the base variable is
                     # accessed by the current config.
                     _cfg_dict = Config._dict_to_config_dict(_cfg_dict, scope)
                     base_cfg_dict.update(_cfg_dict)
 
                 if filename.endswith('.py'):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmengine-lite-0.10.3/mmengine/config/lazy.py` & `mmengine-lite-0.10.4/mmengine/config/lazy.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/config/utils.py` & `mmengine-lite-0.10.4/mmengine/config/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dataset/__init__.py` & `mmengine-lite-0.10.4/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dataset/base_dataset.py` & `mmengine-lite-0.10.4/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dataset/dataset_wrapper.py` & `mmengine-lite-0.10.4/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dataset/sampler.py` & `mmengine-lite-0.10.4/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dataset/utils.py` & `mmengine-lite-0.10.4/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/device/__init__.py` & `mmengine-lite-0.10.4/mmengine/device/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/device/utils.py` & `mmengine-lite-0.10.4/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dist/__init__.py` & `mmengine-lite-0.10.4/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dist/dist.py` & `mmengine-lite-0.10.4/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/dist/utils.py` & `mmengine-lite-0.10.4/mmengine/dist/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/evaluator/evaluator.py` & `mmengine-lite-0.10.4/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/evaluator/metric.py` & `mmengine-lite-0.10.4/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/evaluator/utils.py` & `mmengine-lite-0.10.4/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/__init__.py` & `mmengine-lite-0.10.4/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/__init__.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/base.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/http_backend.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/local_backend.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/memcached_backend.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/petrel_backend.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/backends/registry_utils.py` & `mmengine-lite-0.10.4/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/file_client.py` & `mmengine-lite-0.10.4/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/handlers/base.py` & `mmengine-lite-0.10.4/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/handlers/json_handler.py` & `mmengine-lite-0.10.4/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-lite-0.10.4/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/handlers/registry_utils.py` & `mmengine-lite-0.10.4/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-lite-0.10.4/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/io.py` & `mmengine-lite-0.10.4/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/fileio/parse.py` & `mmengine-lite-0.10.4/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/__init__.py` & `mmengine-lite-0.10.4/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/checkpoint_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/early_stopping_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/ema_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/empty_cache_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/iter_timer_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/logger_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/naive_visualization_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/param_scheduler_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/profiler_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/runtime_info_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/sampler_seed_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/sync_buffer_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hooks/test_time_aug_hook.py` & `mmengine-lite-0.10.4/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hub/hub.py` & `mmengine-lite-0.10.4/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hub/mmcls.json` & `mmengine-lite-0.10.4/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hub/openmmlab.json` & `mmengine-lite-0.10.4/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/hub/torchvision_0.12.json` & `mmengine-lite-0.10.4/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/infer/infer.py` & `mmengine-lite-0.10.4/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/logging/history_buffer.py` & `mmengine-lite-0.10.4/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/logging/logger.py` & `mmengine-lite-0.10.4/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/logging/message_hub.py` & `mmengine-lite-0.10.4/mmengine/logging/message_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
 
         Returns:
             Any: A copy of corresponding runtime information if the key exists.
         """
         if key not in self.runtime_info:
             return default
         else:
-            # TODO： There are restrictions on objects that can be saved
+            # TODO: There are restrictions on objects that can be saved
             # return copy.deepcopy(self._runtime_info[key])
             return self._runtime_info[key]
 
     def _get_valid_value(
         self,
         value: Union['torch.Tensor', np.ndarray, np.number, int, float],
     ) -> Union[int, float]:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmengine-lite-0.10.3/mmengine/model/__init__.py` & `mmengine-lite-0.10.4/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/averaged_model.py` & `mmengine-lite-0.10.4/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/base_model/base_model.py` & `mmengine-lite-0.10.4/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/base_model/data_preprocessor.py` & `mmengine-lite-0.10.4/mmengine/model/base_model/data_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         else:
             self._enable_normalize = False
         self._channel_conversion = rgb_to_bgr or bgr_to_rgb
         self.pad_size_divisor = pad_size_divisor
         self.pad_value = pad_value
 
     def forward(self, data: dict, training: bool = False) -> Union[dict, list]:
-        """Performs normalization、padding and bgr2rgb conversion based on
+        """Performs normalization, padding and bgr2rgb conversion based on
         ``BaseDataPreprocessor``.
 
         Args:
             data (dict): Data sampled from dataset. If the collate
                 function of DataLoader is :obj:`pseudo_collate`, data will be a
                 list of dict. If collate function is :obj:`default_collate`,
                 data will be a tuple with batch input tensor and list of data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmengine-lite-0.10.3/mmengine/model/base_module.py` & `mmengine-lite-0.10.4/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/efficient_conv_bn_eval.py` & `mmengine-lite-0.10.4/mmengine/model/efficient_conv_bn_eval.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/test_time_aug.py` & `mmengine-lite-0.10.4/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/utils.py` & `mmengine-lite-0.10.4/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/weight_init.py` & `mmengine-lite-0.10.4/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/wrappers/__init__.py` & `mmengine-lite-0.10.4/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/wrappers/distributed.py` & `mmengine-lite-0.10.4/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-lite-0.10.4/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-lite-0.10.4/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/model/wrappers/utils.py` & `mmengine-lite-0.10.4/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/__init__.py` & `mmengine-lite-0.10.4/mmengine/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/__init__.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/base.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/builder.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/default_constructor.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/default_constructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,18 @@
                 print_log(
                     f'{prefix} is duplicate. It is skipped since '
                     f'bypass_duplicate={bypass_duplicate}',
                     logger='current',
                     level=logging.WARNING)
                 continue
             if not param.requires_grad:
-                params.append(param_group)
+                print_log((f'{prefix}.{name} is skipped since its '
+                           f'requires_grad={param.requires_grad}'),
+                          logger='current',
+                          level=logging.WARNING)
                 continue
 
             # if the parameter match one of the custom keys, ignore other rules
             is_custom = False
             for key in sorted_keys:
                 if key in f'{prefix}.{name}':
                     is_custom = True
```

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-lite-0.10.4/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/scheduler/__init__.py` & `mmengine-lite-0.10.4/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-lite-0.10.4/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-lite-0.10.4/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-lite-0.10.4/mmengine/optim/scheduler/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/registry/__init__.py` & `mmengine-lite-0.10.4/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/registry/build_functions.py` & `mmengine-lite-0.10.4/mmengine/registry/build_functions.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/registry/default_scope.py` & `mmengine-lite-0.10.4/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/registry/registry.py` & `mmengine-lite-0.10.4/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/registry/root.py` & `mmengine-lite-0.10.4/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/registry/utils.py` & `mmengine-lite-0.10.4/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/__init__.py` & `mmengine-lite-0.10.4/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/_flexible_runner.py` & `mmengine-lite-0.10.4/mmengine/runner/_flexible_runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/activation_checkpointing.py` & `mmengine-lite-0.10.4/mmengine/runner/activation_checkpointing.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/amp.py` & `mmengine-lite-0.10.4/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/base_loop.py` & `mmengine-lite-0.10.4/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/checkpoint.py` & `mmengine-lite-0.10.4/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/log_processor.py` & `mmengine-lite-0.10.4/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/loops.py` & `mmengine-lite-0.10.4/mmengine/runner/loops.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
 
         while self._epoch < self._max_epochs and not self.stop_training:
             self.run_epoch()
 
             self._decide_current_val_interval()
             if (self.runner.val_loop is not None
                     and self._epoch >= self.val_begin
-                    and self._epoch % self.val_interval == 0):
+                    and (self._epoch % self.val_interval == 0
+                         or self._epoch == self._max_epochs)):
                 self.runner.val_loop.run()
 
         self.runner.call_hook('after_train')
         return self.runner.model
 
     def run_epoch(self) -> None:
         """Iterate one epoch."""
@@ -284,15 +285,16 @@
 
             data_batch = next(self.dataloader_iterator)
             self.run_iter(data_batch)
 
             self._decide_current_val_interval()
             if (self.runner.val_loop is not None
                     and self._iter >= self.val_begin
-                    and self._iter % self.val_interval == 0):
+                    and (self._iter % self.val_interval == 0
+                         or self._iter == self._max_iters)):
                 self.runner.val_loop.run()
 
         self.runner.call_hook('after_train_epoch')
         self.runner.call_hook('after_train')
         return self.runner.model
 
     def run_iter(self, data_batch: Sequence[dict]) -> None:
```

### Comparing `mmengine-lite-0.10.3/mmengine/runner/priority.py` & `mmengine-lite-0.10.4/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/runner.py` & `mmengine-lite-0.10.4/mmengine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/runner/utils.py` & `mmengine-lite-0.10.4/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/structures/base_data_element.py` & `mmengine-lite-0.10.4/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/structures/instance_data.py` & `mmengine-lite-0.10.4/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/structures/label_data.py` & `mmengine-lite-0.10.4/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/structures/pixel_data.py` & `mmengine-lite-0.10.4/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/testing/__init__.py` & `mmengine-lite-0.10.4/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/testing/_internal/distributed.py` & `mmengine-lite-0.10.4/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/testing/compare.py` & `mmengine-lite-0.10.4/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/testing/runner_test_case.py` & `mmengine-lite-0.10.4/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/__init__.py` & `mmengine-lite-0.10.4/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/__init__.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/collect_env.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/hub.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/misc.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/setup_env.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/time_counter.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/trace.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/dl_utils/visualize.py` & `mmengine-lite-0.10.4/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/manager.py` & `mmengine-lite-0.10.4/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/misc.py` & `mmengine-lite-0.10.4/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/package_utils.py` & `mmengine-lite-0.10.4/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/path.py` & `mmengine-lite-0.10.4/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/progressbar.py` & `mmengine-lite-0.10.4/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/progressbar_rich.py` & `mmengine-lite-0.10.4/mmengine/utils/progressbar_rich.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/timer.py` & `mmengine-lite-0.10.4/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/utils/version_utils.py` & `mmengine-lite-0.10.4/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/version.py` & `mmengine-lite-0.10.4/mmengine/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.10.3'
+__version__ = '0.10.4'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-lite-0.10.3/mmengine/visualization/__init__.py` & `mmengine-lite-0.10.4/mmengine/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/visualization/utils.py` & `mmengine-lite-0.10.4/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine/visualization/vis_backend.py` & `mmengine-lite-0.10.4/mmengine/visualization/vis_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,34 +665,40 @@
         tracking_uri (str, optional): The tracking uri. Defaults to None.
         artifact_suffix (Tuple[str] or str, optional): The artifact suffix.
             Defaults to ('.json', '.log', '.py', 'yaml').
         tracked_config_keys (dict, optional): The top level keys of config that
             will be added to the experiment. If it is None, which means all
             the config will be added. Defaults to None.
             `New in version 0.7.4.`
+        artifact_location (str, optional): The location to store run artifacts.
+            If None, the server picks an appropriate default.
+            Defaults to None.
+            `New in version 0.10.4.`
     """
 
     def __init__(self,
                  save_dir: str,
                  exp_name: Optional[str] = None,
                  run_name: Optional[str] = None,
                  tags: Optional[dict] = None,
                  params: Optional[dict] = None,
                  tracking_uri: Optional[str] = None,
                  artifact_suffix: SUFFIX_TYPE = ('.json', '.log', '.py',
                                                  'yaml'),
-                 tracked_config_keys: Optional[dict] = None):
+                 tracked_config_keys: Optional[dict] = None,
+                 artifact_location: Optional[str] = None):
         super().__init__(save_dir)
         self._exp_name = exp_name
         self._run_name = run_name
         self._tags = tags
         self._params = params
         self._tracking_uri = tracking_uri
         self._artifact_suffix = artifact_suffix
         self._tracked_config_keys = tracked_config_keys
+        self._artifact_location = artifact_location
 
     def _init_env(self):
         """Setup env for MLflow."""
         if not os.path.exists(self._save_dir):
             os.makedirs(self._save_dir, exist_ok=True)  # type: ignore
 
         try:
@@ -722,15 +728,16 @@
             else:
                 file_url = f'file://{os.path.abspath(self._save_dir)}'
             self._mlflow.set_tracking_uri(file_url)
 
         self._exp_name = self._exp_name or 'Default'
 
         if self._mlflow.get_experiment_by_name(self._exp_name) is None:
-            self._mlflow.create_experiment(self._exp_name)
+            self._mlflow.create_experiment(
+                self._exp_name, artifact_location=self._artifact_location)
 
         self._mlflow.set_experiment(self._exp_name)
 
         if self._run_name is not None:
             self._mlflow.set_tag('mlflow.runName', self._run_name)
         if self._tags is not None:
             self._mlflow.set_tags(self._tags)
```

### Comparing `mmengine-lite-0.10.3/mmengine/visualization/visualizer.py` & `mmengine-lite-0.10.4/mmengine/visualization/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -875,15 +875,15 @@
             'The dtype of binary_masks should be np.bool_, '
             f'but got {binary_masks.dtype}')
         binary_masks = binary_masks.astype('uint8') * 255
         img = self.get_image()
         if binary_masks.ndim == 2:
             binary_masks = binary_masks[None]
         assert img.shape[:2] == binary_masks.shape[
-                                1:], '`binary_marks` must have ' \
+                                1:], '`binary_masks` must have ' \
                                      'the same shape with image'
         binary_mask_len = binary_masks.shape[0]
 
         check_type_and_length('colors', colors, (str, tuple, list),
                               binary_mask_len)
         colors = value2list(colors, (str, tuple), binary_mask_len)
         colors = [
@@ -985,15 +985,15 @@
 
             if overlaid_image.shape[:2] != featmap.shape[1:]:
                 warnings.warn(
                     f'Since the spatial dimensions of '
                     f'overlaid_image: {overlaid_image.shape[:2]} and '
                     f'featmap: {featmap.shape[1:]} are not same, '
                     f'the feature map will be interpolated. '
-                    f'This may cause mismatch problems ！')
+                    f'This may cause mismatch problems !')
                 if resize_shape is None:
                     featmap = F.interpolate(
                         featmap[None],
                         overlaid_image.shape[:2],
                         mode='bilinear',
                         align_corners=False)[0]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmengine-lite-0.10.3/mmengine_lite.egg-info/PKG-INFO` & `mmengine-lite-0.10.4/mmengine_lite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine-lite
-Version: 0.10.3
+Version: 0.10.4
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -23,21 +23,22 @@
                 <i><font size="4">TRY IT OUT</font></i>
               </a>
             </sup>
           </div>
           <div>&nbsp;</div>
         
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mmengine)](https://pypi.org/project/mmengine/)
+        [![pytorch](https://img.shields.io/badge/pytorch-1.6~2.1-yellow)](#installation)
         [![PyPI](https://img.shields.io/pypi/v/mmengine)](https://pypi.org/project/mmengine)
         [![license](https://img.shields.io/github/license/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/blob/main/LICENSE)
-        [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/issues)
-        [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/mmengine/issues)
         
+        [Introduction](#introduction) |
+        [Installation](#installation) |
+        [Get Started](#get-started) |
         [📘Documentation](https://mmengine.readthedocs.io/en/latest/) |
-        [🛠️Installation](https://mmengine.readthedocs.io/en/latest/get_started/installation.html) |
         [🤔Reporting Issues](https://github.com/open-mmlab/mmengine/issues/new/choose)
         
         </div>
         
         <div align="center">
         
         English | [简体中文](README_zh-CN.md)
@@ -62,65 +63,60 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.10.3 was released on 2024-1-24.
+        v0.10.4 was released on 2024-4-23.
         
         Highlights:
         
-        - Support installing mmengine-lite with no dependency on opencv. Refer to the [Installation](https://mmengine.readthedocs.io/en/latest/get_started/installation.html#install-mmengine) for more details.
+        - Support custom `artifact_location` in MLflowVisBackend [#1505](#1505)
+        - Enable `exclude_frozen_parameters` for `DeepSpeedEngine._zero3_consolidated_16bit_state_dict` [#1517](#1517)
         
-        - Support training with [ColossalAI](https://colossalai.org/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai) for more detailed usages.
+        Read [Changelog](./docs/en/notes/changelog.md#v0104-2342024) for more details.
         
-        - Support gradient checkpointing. Refer to the [Save Memory on GPU](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing) for more details.
-        
-        - Supports multiple visualization backends, including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html) for more details.
-        
-        Read [Changelog](./docs/en/notes/changelog.md#v0103-2412024) for more details.
+        ## Introduction
         
-        ## Table of Contents
+        MMEngine is a foundational library for training deep learning models based on PyTorch. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects. Its highlights are as follows:
         
-        - [Introduction](#introduction)
-        - [Installation](#installation)
-        - [Get Started](#get-started)
-        - [Learn More](#learn-more)
-        - [Contributing](#contributing)
-        - [Citation](#citation)
-        - [License](#license)
-        - [Ecosystem](#ecosystem)
-        - [Projects in OpenMMLab](#projects-in-openmmlab)
+        **Integrate mainstream large-scale model training frameworks**
         
-        ## Introduction
+        - [ColossalAI](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#colossalai)
+        - [DeepSpeed](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#deepspeed)
+        - [FSDP](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html#fullyshardeddataparallel-fsdp)
         
-        MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
+        **Supports a variety of training strategies**
         
-        Major features:
+        - [Mixed Precision Training](https://mmengine.readthedocs.io/en/latest/common_usage/speed_up_training.html#mixed-precision-training)
+        - [Gradient Accumulation](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-accumulation)
+        - [Gradient Checkpointing](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-checkpointing)
         
-        1. **A universal and powerful runner**:
+        **Provides a user-friendly configuration system**
         
-           - Supports training different tasks with a small amount of code, e.g., ImageNet can be trained with only 80 lines of code (400 lines of the original PyTorch example).
-           - Easily compatible with models from popular algorithm libraries such as TIMM, TorchVision, and Detectron2.
+        - [Pure Python-style configuration files, easy to navigate](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta)
+        - [Plain-text-style configuration files, supporting JSON and YAML](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html)
         
-        2. **Open architecture with unified interfaces**:
+        **Covers mainstream training monitoring platforms**
         
-           - Handles different algorithm tasks with unified APIs, e.g., implement a method and apply it to all compatible models.
-           - Provides a unified abstraction for upper-level algorithm libraries, which supports various back-end devices such as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training.
+        - [TensorBoard](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#tensorboard) | [WandB](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#wandb) | [MLflow](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#mlflow-wip)
+        - [ClearML](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) | [Neptune](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#neptune) | [DVCLive](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#dvclive) | [Aim](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#aim)
         
-        3. **Customizable training process**:
+        ## Installation
         
-           - Defines the training process just like playing with Legos.
-           - Provides rich components and strategies.
-           - Complete controls on the training process with different levels of APIs.
+        <details>
+        <summary>Supported PyTorch Versions</summary>
         
-        ![mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/267db9cb-72e4-4af2-a58b-877b30091acc)
+        | MMEngine           | PyTorch      | Python         |
+        | ------------------ | ------------ | -------------- |
+        | main               | >=1.6 \<=2.1 | >=3.8, \<=3.11 |
+        | >=0.9.0, \<=0.10.4 | >=1.6 \<=2.1 | >=3.8, \<=3.11 |
         
-        ## Installation
+        </details>
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
         
         ```bash
         pip install -U openmim
```

#### html2text {}

```diff
@@ -1,66 +1,69 @@
-Metadata-Version: 2.1 Name: mmengine-lite Version: 0.10.3 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine-lite Version: 0.10.4 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OOppeennMMMMLLaabb wweebbssiittee _H_O_T_      OOppeennMMMMLLaabb ppllaattffoorrmm _T_R_Y_ _I_T_ _O_U_T
                                         
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mmengine)]
- (https://pypi.org/project/mmengine/) [![PyPI](https://img.shields.io/pypi/v/
+(https://pypi.org/project/mmengine/) [![pytorch](https://img.shields.io/badge/
+pytorch-1.6~2.1-yellow)](#installation) [![PyPI](https://img.shields.io/pypi/v/
       mmengine)](https://pypi.org/project/mmengine) [![license](https://
   img.shields.io/github/license/open-mmlab/mmengine.svg)](https://github.com/
-        open-mmlab/mmengine/blob/main/LICENSE) [![open issues](https://
-  isitmaintained.com/badge/open/open-mmlab/mmengine.svg)](https://github.com/
- open-mmlab/mmengine/issues) [![issue resolution](https://isitmaintained.com/
-   badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
-mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
-     ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
-  get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
-                    open-mmlab/mmengine/issues/new/choose)
+    open-mmlab/mmengine/blob/main/LICENSE) [Introduction](#introduction) |
+        [Installation](#installation) | [Get Started](#get-started) |
+      [ðDocumentation](https://mmengine.readthedocs.io/en/latest/) |
+   [ð¤Reporting Issues](https://github.com/open-mmlab/mmengine/issues/new/
+                                    choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
-## What's New v0.10.3 was released on 2024-1-24. Highlights: - Support
-installing mmengine-lite with no dependency on opencv. Refer to the
-[Installation](https://mmengine.readthedocs.io/en/latest/get_started/
-installation.html#install-mmengine) for more details. - Support training with
-[ColossalAI](https://colossalai.org/). Refer to the [Training Large Models]
+## What's New v0.10.4 was released on 2024-4-23. Highlights: - Support custom
+`artifact_location` in MLflowVisBackend [#1505](#1505) - Enable
+`exclude_frozen_parameters` for
+`DeepSpeedEngine._zero3_consolidated_16bit_state_dict` [#1517](#1517) Read
+[Changelog](./docs/en/notes/changelog.md#v0104-2342024) for more details. ##
+Introduction MMEngine is a foundational library for training deep learning
+models based on PyTorch. It serves as the training engine of all OpenMMLab
+codebases, which support hundreds of algorithms in various research areas.
+Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects. Its
+highlights are as follows: **Integrate mainstream large-scale model training
+frameworks** - [ColossalAI](https://mmengine.readthedocs.io/en/latest/
+common_usage/large_model_training.html#colossalai) - [DeepSpeed](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+large_model_training.html#deepspeed) - [FSDP](https://mmengine.readthedocs.io/
+en/latest/common_usage/large_model_training.html#fullyshardeddataparallel-fsdp)
+**Supports a variety of training strategies** - [Mixed Precision Training]
 (https://mmengine.readthedocs.io/en/latest/common_usage/
-large_model_training.html#colossalai) for more detailed usages. - Support
-gradient checkpointing. Refer to the [Save Memory on GPU](https://
+speed_up_training.html#mixed-precision-training) - [Gradient Accumulation]
+(https://mmengine.readthedocs.io/en/latest/common_usage/
+save_gpu_memory.html#gradient-accumulation) - [Gradient Checkpointing](https://
 mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#gradient-
-checkpointing) for more details. - Supports multiple visualization backends,
-including `NeptuneVisBackend`, `DVCLiveVisBackend` and `AimVisBackend`. Refer
-to [Visualization Backends](https://mmengine.readthedocs.io/en/latest/
-common_usage/visualize_training_log.html) for more details. Read [Changelog](./
-docs/en/notes/changelog.md#v0103-2412024) for more details. ## Table of
-Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
-Started](#get-started) - [Learn More](#learn-more) - [Contributing]
-(#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
-(#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
-MMEngine is a foundational library for training deep learning models based on
-PyTorch. It provides a solid engineering foundation and frees developers from
-writing redundant codes on workflows. It serves as the training engine of all
-OpenMMLab codebases, which support hundreds of algorithms in various research
-areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab
-projects. Major features: 1. **A universal and powerful runner**: - Supports
-training different tasks with a small amount of code, e.g., ImageNet can be
-trained with only 80 lines of code (400 lines of the original PyTorch example).
-- Easily compatible with models from popular algorithm libraries such as TIMM,
-TorchVision, and Detectron2. 2. **Open architecture with unified interfaces**:
-- Handles different algorithm tasks with unified APIs, e.g., implement a method
-and apply it to all compatible models. - Provides a unified abstraction for
-upper-level algorithm libraries, which supports various back-end devices such
-as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training. 3.
-**Customizable training process**: - Defines the training process just like
-playing with Legos. - Provides rich components and strategies. - Complete
-controls on the training process with different levels of APIs. !
-[mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/
-267db9cb-72e4-4af2-a58b-877b30091acc) ## Installation Before installing
+checkpointing) **Provides a user-friendly configuration system** - [Pure
+Python-style configuration files, easy to navigate](https://
+mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-
+style-configuration-file-beta) - [Plain-text-style configuration files,
+supporting JSON and YAML](https://mmengine.readthedocs.io/en/latest/
+advanced_tutorials/config.html) **Covers mainstream training monitoring
+platforms** - [TensorBoard](https://mmengine.readthedocs.io/en/latest/
+common_usage/visualize_training_log.html#tensorboard) | [WandB](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#wandb) | [MLflow](https://mmengine.readthedocs.io/
+en/latest/common_usage/visualize_training_log.html#mlflow-wip) - [ClearML]
+(https://mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#clearml) | [Neptune](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#neptune) | [DVCLive](https://
+mmengine.readthedocs.io/en/latest/common_usage/
+visualize_training_log.html#dvclive) | [Aim](https://mmengine.readthedocs.io/
+en/latest/common_usage/visualize_training_log.html#aim) ## Installation
+Supported PyTorch Versions | MMEngine | PyTorch | Python | | -----------------
+- | ------------ | -------------- | | main | >=1.6 \<=2.1 | >=3.8, \<=3.11 | |
+>=0.9.0, \<=0.10.4 | >=1.6 \<=2.1 | >=3.8, \<=3.11 | Before installing
 MMEngine, please ensure that PyTorch has been successfully installed following
 the [official guide](https://pytorch.org/get-started/locally/). Install
 MMEngine ```bash pip install -U openmim mim install mmengine ``` Verify the
 installation ```bash python -c 'from mmengine.utils.dl_utils import
 collect_env;print(collect_env())' ``` ## Get Started Taking the training of a
 ResNet-50 model on the CIFAR-10 dataset as an example, we will use MMEngine to
 build a complete, configurable training and validation process in less than 80
```

### Comparing `mmengine-lite-0.10.3/mmengine_lite.egg-info/SOURCES.txt` & `mmengine-lite-0.10.4/mmengine_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/mmengine_lite.egg-info/requires.txt` & `mmengine-lite-0.10.4/mmengine_lite.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mmengine-lite-0.10.3/setup.py` & `mmengine-lite-0.10.4/setup.py`

 * *Files identical despite different names*

