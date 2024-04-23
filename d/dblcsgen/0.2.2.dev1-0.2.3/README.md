# Comparing `tmp/dblcsgen-0.2.2.dev1.tar.gz` & `tmp/dblcsgen-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.2.dev1.tar", last modified: Wed Apr 17 09:17:29 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.3.tar", last modified: Tue Apr 23 09:51:20 2024, max compression
```

## Comparing `dblcsgen-0.2.2.dev1.tar` & `dblcsgen-0.2.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.029875 dblcsgen-0.2.2.dev1/
--rw-r--r--   0 theneault   (502) staff       (20)    11357 2024-04-17 09:17:27.000000 dblcsgen-0.2.2.dev1/LICENSE
--rw-r--r--   0 theneault   (502) staff       (20)    28301 2024-04-17 09:17:29.029629 dblcsgen-0.2.2.dev1/PKG-INFO
--rw-r--r--   0 theneault   (502) staff       (20)    14259 2024-04-17 09:17:27.000000 dblcsgen-0.2.2.dev1/README.md
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.028577 dblcsgen-0.2.2.dev1/dblcsgen.egg-info/
--rw-r--r--   0 theneault   (502) staff       (20)    28301 2024-04-17 09:17:29.000000 dblcsgen-0.2.2.dev1/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 theneault   (502) staff       (20)     1970 2024-04-17 09:17:29.000000 dblcsgen-0.2.2.dev1/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 theneault   (502) staff       (20)        1 2024-04-17 09:17:29.000000 dblcsgen-0.2.2.dev1/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 theneault   (502) staff       (20)      150 2024-04-17 09:17:29.000000 dblcsgen-0.2.2.dev1/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 theneault   (502) staff       (20)        7 2024-04-17 09:17:29.000000 dblcsgen-0.2.2.dev1/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 theneault   (502) staff       (20)     1017 2024-04-17 09:15:28.000000 dblcsgen-0.2.2.dev1/pyproject.toml
--rw-r--r--   0 theneault   (502) staff       (20)       38 2024-04-17 09:17:29.029923 dblcsgen-0.2.2.dev1/setup.cfg
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.020585 dblcsgen-0.2.2.dev1/sglang/
--rw-r--r--   0 theneault   (502) staff       (20)       96 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     4443 2024-04-17 09:15:09.000000 dblcsgen-0.2.2.dev1/sglang/api.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.020976 dblcsgen-0.2.2.dev1/sglang/backend/
--rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/backend/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     1831 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/backend/base_backend.py
--rw-r--r--   0 theneault   (502) staff       (20)     8319 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 theneault   (502) staff       (20)      797 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/global_config.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.021841 dblcsgen-0.2.2.dev1/sglang/lang/
--rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/lang/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     9633 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/lang/chat_template.py
--rw-r--r--   0 theneault   (502) staff       (20)     7527 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/lang/compiler.py
--rw-r--r--   0 theneault   (502) staff       (20)    26999 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/lang/interpreter.py
--rw-r--r--   0 theneault   (502) staff       (20)    13320 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/lang/ir.py
--rw-r--r--   0 theneault   (502) staff       (20)     8260 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/lang/tracer.py
--rw-r--r--   0 theneault   (502) staff       (20)      433 2024-04-16 18:25:50.000000 dblcsgen-0.2.2.dev1/sglang/launch_server.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.023370 dblcsgen-0.2.2.dev1/sglang/srt/
--rw-r--r--   0 theneault   (502) staff       (20)      227 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/backend_config.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.023906 dblcsgen-0.2.2.dev1/sglang/srt/constrained/
--rw-r--r--   0 theneault   (502) staff       (20)     1236 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/constrained/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     1405 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 theneault   (502) staff       (20)      902 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 theneault   (502) staff       (20)     2482 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 theneault   (502) staff       (20)    15496 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/conversation.py
--rw-r--r--   0 theneault   (502) staff       (20)     5285 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.024696 dblcsgen-0.2.2.dev1/sglang/srt/layers/
--rw-r--r--   0 theneault   (502) staff       (20)     5209 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 theneault   (502) staff       (20)    12622 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 theneault   (502) staff       (20)     6887 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 theneault   (502) staff       (20)     5597 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 theneault   (502) staff       (20)     8516 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.025237 dblcsgen-0.2.2.dev1/sglang/srt/managers/
--rw-r--r--   0 theneault   (502) staff       (20)     3292 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 theneault   (502) staff       (20)     3670 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/io_struct.py
--rw-r--r--   0 theneault   (502) staff       (20)     4563 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/openai_protocol.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.026082 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/
--rw-r--r--   0 theneault   (502) staff       (20)    19922 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 theneault   (502) staff       (20)     2682 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/manager.py
--rw-r--r--   0 theneault   (502) staff       (20)    28007 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 theneault   (502) staff       (20)    16926 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 theneault   (502) staff       (20)     6484 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 theneault   (502) staff       (20)     2818 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 theneault   (502) staff       (20)     9743 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 theneault   (502) staff       (20)     3609 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/memory_pool.py
--rw-r--r--   0 theneault   (502) staff       (20)     8889 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/mm_utils.py
--rw-r--r--   0 theneault   (502) staff       (20)     1546 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/model_config.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.027833 dblcsgen-0.2.2.dev1/sglang/srt/models/
--rw-r--r--   0 theneault   (502) staff       (20)    14112 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/dbrx.py
--rw-r--r--   0 theneault   (502) staff       (20)    11071 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 theneault   (502) staff       (20)    11587 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/gemma.py
--rw-r--r--   0 theneault   (502) staff       (20)    11611 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/llama2.py
--rw-r--r--   0 theneault   (502) staff       (20)    14922 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/llava.py
--rw-r--r--   0 theneault   (502) staff       (20)      254 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/mistral.py
--rw-r--r--   0 theneault   (502) staff       (20)    13915 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/mixtral.py
--rw-r--r--   0 theneault   (502) staff       (20)     9225 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/qwen.py
--rw-r--r--   0 theneault   (502) staff       (20)    11307 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/qwen2.py
--rw-r--r--   0 theneault   (502) staff       (20)    10816 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/stablelm.py
--rw-r--r--   0 theneault   (502) staff       (20)     4414 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/models/yivl.py
--rw-r--r--   0 theneault   (502) staff       (20)     2896 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/sampling_params.py
--rw-r--r--   0 theneault   (502) staff       (20)    27702 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/server.py
--rw-r--r--   0 theneault   (502) staff       (20)     9143 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/server_args.py
--rw-r--r--   0 theneault   (502) staff       (20)     7582 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/srt/utils.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:17:29.028358 dblcsgen-0.2.2.dev1/sglang/test/
--rw-r--r--   0 theneault   (502) staff       (20)     1592 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/test/test_conversation.py
--rw-r--r--   0 theneault   (502) staff       (20)     1657 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/test/test_openai_protocol.py
--rw-r--r--   0 theneault   (502) staff       (20)    11421 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/test/test_programs.py
--rw-r--r--   0 theneault   (502) staff       (20)     4830 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/test/test_utils.py
--rw-r--r--   0 theneault   (502) staff       (20)     6237 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev1/sglang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 09:51:18.000000 dblcsgen-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-23 09:51:18.000000 dblcsgen-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/dblcsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.827537 dblcsgen-0.2.3/sglang/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.827537 dblcsgen-0.2.3/sglang/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.827537 dblcsgen-0.2.3/sglang/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27168 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/launch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.831537 dblcsgen-0.2.3/sglang/srt/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.831537 dblcsgen-0.2.3/sglang/srt/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.831537 dblcsgen-0.2.3/sglang/srt/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.835537 dblcsgen-0.2.3/sglang/srt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/io_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/openai_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.835537 dblcsgen-0.2.3/sglang/srt/managers/router/
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28007 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/mm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.835537 dblcsgen-0.2.3/sglang/srt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/dbrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/qwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/qwen2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/stablelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/yivl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/server_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/sglang/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/utils.py
```

### Comparing `dblcsgen-0.2.2.dev1/LICENSE` & `dblcsgen-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/PKG-INFO` & `dblcsgen-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.2.dev1
+Version: 0.2.3
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.2.dev1/README.md` & `dblcsgen-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.3/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.2.dev1
+Version: 0.2.3
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.2.dev1/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.3/dblcsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/pyproject.toml` & `dblcsgen-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.2.dev1"
+version = "0.2.3"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
@@ -16,15 +16,17 @@
 dependencies = [
     "requests",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 srt = ["aiohttp", "fastapi", "psutil", "rpyc", "torch", "uvloop", "uvicorn",
-       "zmq", "vllm>=0.3.3", "interegular", "pydantic", "pillow", "outlines==0.0.34"]
+    "zmq", "vllm>=0.3.3", "interegular", "pydantic", "pillow",
+    "outlines==0.0.34" # There is a breaking change to regexes on 0.0.35, not handled by SGLang atm
+]
 all = ["sglang[srt]"]
 
 [project.urls]
 "Homepage" = "https://github.com/sgl-project/sglang"
 "Bug Tracker" = "https://github.com/sgl-project/sglang/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `dblcsgen-0.2.2.dev1/sglang/api.py` & `dblcsgen-0.2.3/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/backend/base_backend.py` & `dblcsgen-0.2.3/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.3/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/global_config.py` & `dblcsgen-0.2.3/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/lang/chat_template.py` & `dblcsgen-0.2.3/sglang/lang/chat_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,36 @@
             "user": ("[INST] ", " [/INST]"),
             "assistant": ("", " </s><s>"),
         },
         style=ChatTemplateStyle.LLAMA2,
     )
 )
 
+register_chat_template(
+    ChatTemplate(
+        name="llama-3-instruct",
+        default_system_prompt=None,
+        role_prefix_and_suffix={
+            "system": (
+                "<|start_header_id|>system<|end_header_id|>\n\n",
+                "<|eot_id|>",
+            ),
+            "user": (
+                "<|start_header_id|>user<|end_header_id|>\n\n",
+                "<|eot_id|>",
+            ),
+            "assistant": (
+                "<|start_header_id|>assistant<|end_header_id|>\n\n",
+                "<|eot_id|>",
+            ),
+        },
+        stop_str=("<|eot_id|>",),
+    )
+)
+
 # Reference: https://github.com/01-ai/Yi/tree/main/VL#major-difference-with-llava
 register_chat_template(
     ChatTemplate(
         name="yi",
         default_system_prompt=(
             "This is a chat between an inquisitive human and an AI assistant. Assume the role of the AI assistant. Read all the images carefully, and respond to the human's questions with informative, helpful, detailed and polite answers."
             "这是一个好奇的人类和一个人工智能助手之间的对话。假设你扮演这个AI助手的角色。仔细阅读所有的图像，并对人类的问题做出信息丰富、有帮助、详细的和礼貌的回答。"
@@ -230,14 +252,21 @@
     ) and "instruct" in model_path:
         return get_chat_template("llama-2-chat")
     if "codellama" in model_path and "instruct" in model_path:
         return get_chat_template("llama-2-chat")
 
 
 @register_chat_template_matching_function
+def match_llama3_instruct(model_path: str):
+    model_path = model_path.lower()
+    if "llama-3" in model_path and "instruct" in model_path:
+        return get_chat_template("llama-3-instruct")
+
+
+@register_chat_template_matching_function
 def match_chat_ml(model_path: str):
     model_path = model_path.lower()
     if "tinyllama" in model_path:
         return get_chat_template("chatml")
     if "qwen" in model_path and "chat" in model_path:
         return get_chat_template("chatml")
     if "llava-v1.6-34b" in model_path:
```

### Comparing `dblcsgen-0.2.2.dev1/sglang/lang/compiler.py` & `dblcsgen-0.2.3/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/lang/interpreter.py` & `dblcsgen-0.2.3/sglang/lang/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,17 +252,23 @@
         if name in self.variable_event:
             got = self.variable_event[name].wait(timeout)
             if not got:
                 raise TimeoutError(f"Timeout while waiting for event '{name}'")
         ret = self.meta_info.get(name, None)
         return ret
 
-    def fork(self, number: int, position_ids_offset: Optional[List[int]] = None):
-        self.submit(SglCommitLazy())
-        self.sync()
+    def fork(
+        self,
+        number: int,
+        position_ids_offset: Optional[List[int]] = None,
+        copy: bool = False,
+    ):
+        if number > 1 or copy:
+            self.submit(SglCommitLazy())
+            self.sync()
 
         number = int(number)
 
         exes = [
             StreamExecutor(
                 self.backend,
                 self.arguments,
@@ -637,23 +643,28 @@
 
     @contextmanager
     def var_scope(self, name: str):
         self.stream_executor.submit(SglVarScopeBegin(name))
         yield
         self.stream_executor.submit(SglVarScopeEnd(name))
 
-    def fork(self, number: int = 1, position_ids_offset: Optional[List[int]] = None):
-        stream_executors = self.stream_executor.fork(number, position_ids_offset)
+    def fork(
+        self,
+        number: int = 1,
+        position_ids_offset: Optional[List[int]] = None,
+        copy: bool = False,
+    ):
+        stream_executors = self.stream_executor.fork(number, position_ids_offset, copy)
         states = [ProgramState(x) for x in stream_executors]
         state_group = ProgramStateGroup(states, self)
         return state_group
 
     @contextmanager
     def copy(self, position_ids_offset: Optional[List[int]] = None):
-        state_group = self.fork(1, position_ids_offset)
+        state_group = self.fork(1, position_ids_offset, True)
         try:
             yield state_group[0]
         finally:
             state_group.join()
 
     def text(self):
         return self.stream_executor.text()
```

### Comparing `dblcsgen-0.2.2.dev1/sglang/lang/ir.py` & `dblcsgen-0.2.3/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/lang/tracer.py` & `dblcsgen-0.2.3/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.3/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.3/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.3/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.3/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/conversation.py` & `dblcsgen-0.2.3/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.3/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.3/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.3/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.3/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.3/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.3/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.3/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.3/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/openai_protocol.py` & `dblcsgen-0.2.3/sglang/srt/managers/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.3/sglang/srt/managers/router/infer_batch.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.3/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.3/sglang/srt/managers/router/model_rpc.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.3/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.3/sglang/srt/managers/router/radix_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,18 @@
             new_node.parent = node
             new_node.value = value
             node.children[key] = new_node
             self.evictable_size_ += len(value)
         return 0
 
     def _print_helper(self, node, indent):
-        for key, child in node.children.items():
-            print(" " * indent, len(key), key[:10], f"r={child.ref_counter}")
+        for _, child in node.children.items():
+            print(
+                " " * indent, len(child.key), child.key[:10], f"r={child.ref_counter}"
+            )
             self._print_helper(child, indent=indent + 2)
 
     def _delete_leaf(self, node):
         for k, v in node.parent.children.items():
             if v == node:
                 break
         del node.parent.children[k]
```

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.3/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.3/sglang/srt/managers/tokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/memory_pool.py` & `dblcsgen-0.2.3/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/mm_utils.py` & `dblcsgen-0.2.3/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/model_config.py` & `dblcsgen-0.2.3/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.3/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.3/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/gemma.py` & `dblcsgen-0.2.3/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/llama2.py` & `dblcsgen-0.2.3/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/llava.py` & `dblcsgen-0.2.3/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.3/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/qwen.py` & `dblcsgen-0.2.3/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.3/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.3/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/models/yivl.py` & `dblcsgen-0.2.3/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/sampling_params.py` & `dblcsgen-0.2.3/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/server.py` & `dblcsgen-0.2.3/sglang/srt/server.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/server_args.py` & `dblcsgen-0.2.3/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/srt/utils.py` & `dblcsgen-0.2.3/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/test/test_conversation.py` & `dblcsgen-0.2.3/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.3/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/test/test_programs.py` & `dblcsgen-0.2.3/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/test/test_utils.py` & `dblcsgen-0.2.3/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.2.dev1/sglang/utils.py` & `dblcsgen-0.2.3/sglang/utils.py`

 * *Files identical despite different names*

