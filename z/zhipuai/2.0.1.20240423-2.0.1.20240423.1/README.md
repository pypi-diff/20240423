# Comparing `tmp/zhipuai-2.0.1.20240423.tar.gz` & `tmp/zhipuai-2.0.1.20240423.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-2.0.1.20240423.tar", last modified: Tue Apr 23 09:10:16 2024, max compression
+gzip compressed data, was "zhipuai-2.0.1.20240423.1.tar", last modified: Tue Apr 23 14:04:03 2024, max compression
```

## Comparing `zhipuai-2.0.1.20240423.tar` & `zhipuai-2.0.1.20240423.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.200056 zhipuai-2.0.1.20240423/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7982 2024-04-23 09:10:16.195052 zhipuai-2.0.1.20240423/PKG-INFO
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7371 2024-04-23 08:29:15.000000 zhipuai-2.0.1.20240423/README.md
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)       38 2024-04-23 09:10:16.201056 zhipuai-2.0.1.20240423/setup.cfg
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      937 2024-04-23 09:10:13.000000 zhipuai-2.0.1.20240423/setup.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.473164 zhipuai-2.0.1.20240423/tests/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3428 2024-04-22 06:48:52.000000 zhipuai-2.0.1.20240423/tests/test_charglm3.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4724 2024-04-23 08:24:48.000000 zhipuai-2.0.1.20240423/tests/test_chat.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      326 2024-04-18 02:32:31.000000 zhipuai-2.0.1.20240423/tests/test_embedding.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      650 2024-04-18 11:48:21.000000 zhipuai-2.0.1.20240423/tests/test_file.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1569 2024-04-18 11:50:17.000000 zhipuai-2.0.1.20240423/tests/test_finetuning.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      363 2024-04-18 11:50:56.000000 zhipuai-2.0.1.20240423/tests/test_images.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.518225 zhipuai-2.0.1.20240423/zhipuai/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      343 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)       23 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/__version__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)    13562 2024-04-22 03:42:28.000000 zhipuai-2.0.1.20240423/zhipuai/_base_models.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2431 2024-04-22 03:55:22.000000 zhipuai-2.0.1.20240423/zhipuai/_client.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.630859 zhipuai-2.0.1.20240423/zhipuai/api_resource/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      147 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/__init__.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.700849 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3230 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/async_completions.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      451 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/chat.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4464 2024-04-23 08:07:31.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/completions.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1694 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/embeddings.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2463 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/files.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.752654 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      311 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3757 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/jobs.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1885 2024-04-18 02:25:48.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/images.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.911214 zhipuai-2.0.1.20240423/zhipuai/core/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/core/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      406 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/core/_base_api.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     6405 2024-04-19 09:33:20.000000 zhipuai-2.0.1.20240423/zhipuai/core/_base_compat.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4484 2024-04-18 11:44:33.000000 zhipuai-2.0.1.20240423/zhipuai/core/_base_type.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2038 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423/zhipuai/core/_errors.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1384 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423/zhipuai/core/_files.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)    13808 2024-04-22 05:32:45.000000 zhipuai-2.0.1.20240423/zhipuai/core/_http_client.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      713 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/core/_jwt_token.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2346 2024-04-18 11:27:16.000000 zhipuai-2.0.1.20240423/zhipuai/core/_request_opt.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3640 2024-04-18 11:34:04.000000 zhipuai-2.0.1.20240423/zhipuai/core/_response.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4085 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423/zhipuai/core/_sse_client.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.965067 zhipuai-2.0.1.20240423/zhipuai/core/_utils/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1451 2024-04-18 10:47:00.000000 zhipuai-2.0.1.20240423/zhipuai/core/_utils/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3858 2024-04-18 10:47:00.000000 zhipuai-2.0.1.20240423/zhipuai/core/_utils/_typing.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)    11363 2024-04-18 10:49:15.000000 zhipuai-2.0.1.20240423/zhipuai/core/_utils/_utils.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.022095 zhipuai-2.0.1.20240423/zhipuai/types/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/__init__.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.112862 zhipuai-2.0.1.20240423/zhipuai/types/chat/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      557 2024-04-22 05:31:29.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/async_chat_completion.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      885 2024-04-22 05:23:09.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1257 2024-04-18 10:59:17.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion_chunk.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      171 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completions_create_param.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      434 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/embeddings.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      538 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/file_object.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.181752 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      244 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/__init__.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1113 2024-04-18 10:59:17.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1110 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      339 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/job_create_params.py
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)      382 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/image.py
-drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.575525 zhipuai-2.0.1.20240423/zhipuai.egg-info/
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7982 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/PKG-INFO
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1694 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/SOURCES.txt
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        1 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/dependency_links.txt
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)       64 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/requires.txt
--rw-r--r--   0 dmeck     (1000) dmeck     (1000)        8 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/top_level.txt
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:03.365862 zhipuai-2.0.1.20240423.1/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7984 2024-04-23 14:04:03.350804 zhipuai-2.0.1.20240423.1/PKG-INFO
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7371 2024-04-23 08:29:15.000000 zhipuai-2.0.1.20240423.1/README.md
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)       38 2024-04-23 14:04:03.365862 zhipuai-2.0.1.20240423.1/setup.cfg
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      939 2024-04-23 14:03:46.000000 zhipuai-2.0.1.20240423.1/setup.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:01.174406 zhipuai-2.0.1.20240423.1/tests/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3428 2024-04-22 06:48:52.000000 zhipuai-2.0.1.20240423.1/tests/test_charglm3.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4722 2024-04-23 13:57:44.000000 zhipuai-2.0.1.20240423.1/tests/test_chat.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      326 2024-04-18 02:32:31.000000 zhipuai-2.0.1.20240423.1/tests/test_embedding.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      650 2024-04-18 11:48:21.000000 zhipuai-2.0.1.20240423.1/tests/test_file.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1569 2024-04-18 11:50:17.000000 zhipuai-2.0.1.20240423.1/tests/test_finetuning.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      363 2024-04-18 11:50:56.000000 zhipuai-2.0.1.20240423.1/tests/test_images.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:01.331417 zhipuai-2.0.1.20240423.1/zhipuai/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      343 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)       23 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/__version__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)    13562 2024-04-22 03:42:28.000000 zhipuai-2.0.1.20240423.1/zhipuai/_base_models.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2431 2024-04-22 03:55:22.000000 zhipuai-2.0.1.20240423.1/zhipuai/_client.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:01.653731 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      147 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/__init__.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:01.868859 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3230 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/async_completions.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      451 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/chat.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4561 2024-04-23 13:56:27.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/completions.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1694 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/embeddings.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2463 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/files.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:02.004298 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/fine_tuning/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      311 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3757 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/fine_tuning/jobs.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1885 2024-04-18 02:25:48.000000 zhipuai-2.0.1.20240423.1/zhipuai/api_resource/images.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:02.506349 zhipuai-2.0.1.20240423.1/zhipuai/core/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      406 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_base_api.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     6405 2024-04-19 09:33:20.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_base_compat.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4484 2024-04-18 11:44:33.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_base_type.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2038 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_errors.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1384 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_files.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)    13808 2024-04-22 05:32:45.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_http_client.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      713 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_jwt_token.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2346 2024-04-18 11:27:16.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_request_opt.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3640 2024-04-18 11:34:04.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_response.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4085 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_sse_client.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:02.664266 zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1451 2024-04-18 10:47:00.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3858 2024-04-18 10:47:00.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/_typing.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)    11363 2024-04-18 10:49:15.000000 zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/_utils.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:02.810959 zhipuai-2.0.1.20240423.1/zhipuai/types/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/__init__.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:03.095394 zhipuai-2.0.1.20240423.1/zhipuai/types/chat/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/chat/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      557 2024-04-22 05:31:29.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/chat/async_chat_completion.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      885 2024-04-22 05:23:09.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/chat/chat_completion.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1257 2024-04-18 10:59:17.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      171 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/chat/chat_completions_create_param.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      434 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/embeddings.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      538 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/file_object.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:03.318738 zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      244 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1113 2024-04-18 10:59:17.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1110 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      339 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      382 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423.1/zhipuai/types/image.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 14:04:01.464225 zhipuai-2.0.1.20240423.1/zhipuai.egg-info/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7984 2024-04-23 14:04:00.000000 zhipuai-2.0.1.20240423.1/zhipuai.egg-info/PKG-INFO
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1694 2024-04-23 14:04:00.000000 zhipuai-2.0.1.20240423.1/zhipuai.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        1 2024-04-23 14:04:00.000000 zhipuai-2.0.1.20240423.1/zhipuai.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)       64 2024-04-23 14:04:00.000000 zhipuai-2.0.1.20240423.1/zhipuai.egg-info/requires.txt
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        8 2024-04-23 14:04:00.000000 zhipuai-2.0.1.20240423.1/zhipuai.egg-info/top_level.txt
```

### Comparing `zhipuai-2.0.1.20240423/PKG-INFO` & `zhipuai-2.0.1.20240423.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 2.0.1.20240423
+Version: 2.0.1.20240423.1
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Home-page: https://open.bigmodel.cn/
 Author: Zhipu AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `zhipuai-2.0.1.20240423/README.md` & `zhipuai-2.0.1.20240423.1/README.md`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/setup.py` & `zhipuai-2.0.1.20240423.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="zhipuai",
-    version="v2.0.1.20240423",
+    version="v2.0.1.20240423.1",
     description="A SDK library for accessing big model apis from ZhipuAI",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Zhipu AI",
     url="https://open.bigmodel.cn/",
     packages=find_packages(exclude=['test', 'examples']),
     include_package_data=True,
```

### Comparing `zhipuai-2.0.1.20240423/tests/test_charglm3.py` & `zhipuai-2.0.1.20240423.1/tests/test_charglm3.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/tests/test_chat.py` & `zhipuai-2.0.1.20240423.1/tests/test_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     import base64
     with open(image_path, "rb") as image_file:
         return base64.b64encode(image_file.read()).decode('utf-8')
 
 
 def test_completions_vis():
     client = ZhipuAI()  # 填写您自己的APIKey
-    base64_image  = encode_image("img/MetaGLM.png")
+    base64_image = encode_image("img/MetaGLM.png")
     response = client.chat.completions.create(
         model="glm-4v",  # 填写需要调用的模型名称
         extra_body={"temperature": 0.5, "max_tokens": 50},
         messages=[
             {
                 "role": "user",
                 "content": [
@@ -112,10 +112,9 @@
 
 def test_retrieve_completion_result():
     client = ZhipuAI()  # 请填写您自己的APIKey
     response = client.chat.asyncCompletions.retrieve_completion_result(id="1014908592669352541651237")
     print(response)
 
 
-
 if __name__ == "__main__":
     test_completions_vis()
```

### Comparing `zhipuai-2.0.1.20240423/tests/test_file.py` & `zhipuai-2.0.1.20240423.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/tests/test_finetuning.py` & `zhipuai-2.0.1.20240423.1/tests/test_finetuning.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/_base_models.py` & `zhipuai-2.0.1.20240423.1/zhipuai/_base_models.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/_client.py` & `zhipuai-2.0.1.20240423.1/zhipuai/_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/async_completions.py` & `zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/async_completions.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/completions.py` & `zhipuai-2.0.1.20240423.1/zhipuai/api_resource/chat/completions.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,21 +95,23 @@
                 extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=_cast_type,
             enable_stream=stream or False,
             stream_cls=_stream_cls,
         )
 
-    def _drop_prefix_image_data(self, content: List) -> List:
+    def _drop_prefix_image_data(self, content: Union[str,List[dict]]) -> Union[str,List[dict]]:
         """
         删除 ;base64, 前缀
         :param image_data:
         :return:
         """
-        for data in content:
-            if data.get('type') == 'image_url':
-                image_data = data.get("image_url").get("url")
-                if image_data.startswith("data:image/"):
-                    image_data = image_data.split("base64,")[-1]
-                    data["image_url"]["url"] = image_data
+        if isinstance(content, List):
+            for data in content:
+                if data.get('type') == 'image_url':
+                    image_data = data.get("image_url").get("url")
+                    if image_data.startswith("data:image/"):
+                        image_data = image_data.split("base64,")[-1]
+                        data["image_url"]["url"] = image_data
 
         return content
+
```

### Comparing `zhipuai-2.0.1.20240423/zhipuai/api_resource/embeddings.py` & `zhipuai-2.0.1.20240423.1/zhipuai/api_resource/embeddings.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/api_resource/files.py` & `zhipuai-2.0.1.20240423.1/zhipuai/api_resource/files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/jobs.py` & `zhipuai-2.0.1.20240423.1/zhipuai/api_resource/fine_tuning/jobs.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/api_resource/images.py` & `zhipuai-2.0.1.20240423.1/zhipuai/api_resource/images.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_base_compat.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_base_compat.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_base_type.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_base_type.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_errors.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_errors.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_files.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_http_client.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_http_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_jwt_token.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_request_opt.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_request_opt.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_response.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_response.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_sse_client.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_utils/__init__.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_utils/_typing.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/core/_utils/_utils.py` & `zhipuai-2.0.1.20240423.1/zhipuai/core/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/types/chat/async_chat_completion.py` & `zhipuai-2.0.1.20240423.1/zhipuai/types/chat/async_chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion.py` & `zhipuai-2.0.1.20240423.1/zhipuai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion_chunk.py` & `zhipuai-2.0.1.20240423.1/zhipuai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/types/file_object.py` & `zhipuai-2.0.1.20240423.1/zhipuai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job.py` & `zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job_event.py` & `zhipuai-2.0.1.20240423.1/zhipuai/types/fine_tuning/fine_tuning_job_event.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240423/zhipuai.egg-info/PKG-INFO` & `zhipuai-2.0.1.20240423.1/zhipuai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 2.0.1.20240423
+Version: 2.0.1.20240423.1
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Home-page: https://open.bigmodel.cn/
 Author: Zhipu AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `zhipuai-2.0.1.20240423/zhipuai.egg-info/SOURCES.txt` & `zhipuai-2.0.1.20240423.1/zhipuai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

