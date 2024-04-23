# Comparing `tmp/zhipuai-2.0.1.tar.gz` & `tmp/zhipuai-2.0.1.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-2.0.1.tar", last modified: Tue Jan 16 11:43:44 2024, max compression
+gzip compressed data, was "zhipuai-2.0.1.20240423.tar", last modified: Tue Apr 23 09:10:16 2024, max compression
```

## Comparing `zhipuai-2.0.1.tar` & `zhipuai-2.0.1.20240423.tar`

### file list

```diff
@@ -1,57 +1,69 @@
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.278304 zhipuai-2.0.1/
--rw-r--r--   0 haowangai   (501) staff       (20)     2593 2024-01-16 11:43:44.278180 zhipuai-2.0.1/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)     2116 2024-01-16 10:54:57.000000 zhipuai-2.0.1/README.md
--rw-r--r--   0 haowangai   (501) staff       (20)       38 2024-01-16 11:43:44.278337 zhipuai-2.0.1/setup.cfg
--rw-r--r--   0 haowangai   (501) staff       (20)      928 2024-01-16 11:43:13.000000 zhipuai-2.0.1/setup.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.272148 zhipuai-2.0.1/zhipuai/
--rw-r--r--   0 haowangai   (501) staff       (20)      343 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)       23 2024-01-16 11:43:18.000000 zhipuai-2.0.1/zhipuai/__version__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     2377 2024-01-16 10:54:57.000000 zhipuai-2.0.1/zhipuai/_client.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.273510 zhipuai-2.0.1/zhipuai/api_resource/
--rw-r--r--   0 haowangai   (501) staff       (20)      147 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/__init__.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.274062 zhipuai-2.0.1/zhipuai/api_resource/chat/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-12-27 02:41:17.000000 zhipuai-2.0.1/zhipuai/api_resource/chat/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     3118 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/chat/async_completions.py
--rw-r--r--   0 haowangai   (501) staff       (20)      451 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/chat/chat.py
--rw-r--r--   0 haowangai   (501) staff       (20)     2790 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/chat/completions.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1633 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/embeddings.py
--rw-r--r--   0 haowangai   (501) staff       (20)     2323 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/files.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.274398 zhipuai-2.0.1/zhipuai/api_resource/fine_tuning/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/fine_tuning/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)      311 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0 haowangai   (501) staff       (20)     3470 2024-01-16 10:54:57.000000 zhipuai-2.0.1/zhipuai/api_resource/fine_tuning/jobs.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1818 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/api_resource/images.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.276068 zhipuai-2.0.1/zhipuai/core/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-12-27 02:41:17.000000 zhipuai-2.0.1/zhipuai/core/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)      406 2023-12-27 02:41:17.000000 zhipuai-2.0.1/zhipuai/core/_base_api.py
--rw-r--r--   0 haowangai   (501) staff       (20)     3356 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_base_type.py
--rw-r--r--   0 haowangai   (501) staff       (20)     2038 2023-12-27 02:45:35.000000 zhipuai-2.0.1/zhipuai/core/_errors.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1384 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_files.py
--rw-r--r--   0 haowangai   (501) staff       (20)    12297 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_http_client.py
--rw-r--r--   0 haowangai   (501) staff       (20)      713 2023-12-27 02:41:17.000000 zhipuai-2.0.1/zhipuai/core/_jwt_token.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1549 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_request_opt.py
--rw-r--r--   0 haowangai   (501) staff       (20)     3358 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_response.py
--rw-r--r--   0 haowangai   (501) staff       (20)     4085 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_sse_client.py
--rw-r--r--   0 haowangai   (501) staff       (20)      443 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/core/_utils.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.276678 zhipuai-2.0.1/zhipuai/types/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-12-27 02:45:45.000000 zhipuai-2.0.1/zhipuai/types/__init__.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.277308 zhipuai-2.0.1/zhipuai/types/chat/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-12-27 02:45:45.000000 zhipuai-2.0.1/zhipuai/types/chat/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)      550 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/types/chat/async_chat_completion.py
--rw-r--r--   0 haowangai   (501) staff       (20)      861 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/types/chat/chat_completion.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1208 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/types/chat/chat_completion_chunk.py
--rw-r--r--   0 haowangai   (501) staff       (20)      171 2023-12-27 02:45:35.000000 zhipuai-2.0.1/zhipuai/types/chat/chat_completions_create_param.py
--rw-r--r--   0 haowangai   (501) staff       (20)      428 2023-12-27 02:45:45.000000 zhipuai-2.0.1/zhipuai/types/embeddings.py
--rw-r--r--   0 haowangai   (501) staff       (20)      532 2024-01-16 11:40:53.000000 zhipuai-2.0.1/zhipuai/types/file_object.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.278008 zhipuai-2.0.1/zhipuai/types/fine_tuning/
--rw-r--r--   0 haowangai   (501) staff       (20)      244 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/types/fine_tuning/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1033 2024-01-16 11:40:53.000000 zhipuai-2.0.1/zhipuai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1103 2024-01-16 11:40:53.000000 zhipuai-2.0.1/zhipuai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0 haowangai   (501) staff       (20)      339 2024-01-16 10:53:04.000000 zhipuai-2.0.1/zhipuai/types/fine_tuning/job_create_params.py
--rw-r--r--   0 haowangai   (501) staff       (20)      376 2023-12-27 02:45:45.000000 zhipuai-2.0.1/zhipuai/types/image.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2024-01-16 11:43:44.272810 zhipuai-2.0.1/zhipuai.egg-info/
--rw-r--r--   0 haowangai   (501) staff       (20)     2593 2024-01-16 11:43:44.000000 zhipuai-2.0.1/zhipuai.egg-info/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)     1440 2024-01-16 11:43:44.000000 zhipuai-2.0.1/zhipuai.egg-info/SOURCES.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        1 2024-01-16 11:43:44.000000 zhipuai-2.0.1/zhipuai.egg-info/dependency_links.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       61 2024-01-16 11:43:44.000000 zhipuai-2.0.1/zhipuai.egg-info/requires.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        8 2024-01-16 11:43:44.000000 zhipuai-2.0.1/zhipuai.egg-info/top_level.txt
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.200056 zhipuai-2.0.1.20240423/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7982 2024-04-23 09:10:16.195052 zhipuai-2.0.1.20240423/PKG-INFO
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7371 2024-04-23 08:29:15.000000 zhipuai-2.0.1.20240423/README.md
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)       38 2024-04-23 09:10:16.201056 zhipuai-2.0.1.20240423/setup.cfg
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      937 2024-04-23 09:10:13.000000 zhipuai-2.0.1.20240423/setup.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.473164 zhipuai-2.0.1.20240423/tests/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3428 2024-04-22 06:48:52.000000 zhipuai-2.0.1.20240423/tests/test_charglm3.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4724 2024-04-23 08:24:48.000000 zhipuai-2.0.1.20240423/tests/test_chat.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      326 2024-04-18 02:32:31.000000 zhipuai-2.0.1.20240423/tests/test_embedding.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      650 2024-04-18 11:48:21.000000 zhipuai-2.0.1.20240423/tests/test_file.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1569 2024-04-18 11:50:17.000000 zhipuai-2.0.1.20240423/tests/test_finetuning.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      363 2024-04-18 11:50:56.000000 zhipuai-2.0.1.20240423/tests/test_images.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.518225 zhipuai-2.0.1.20240423/zhipuai/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      343 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)       23 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/__version__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)    13562 2024-04-22 03:42:28.000000 zhipuai-2.0.1.20240423/zhipuai/_base_models.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2431 2024-04-22 03:55:22.000000 zhipuai-2.0.1.20240423/zhipuai/_client.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.630859 zhipuai-2.0.1.20240423/zhipuai/api_resource/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      147 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/__init__.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.700849 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3230 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/async_completions.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      451 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/chat.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4464 2024-04-23 08:07:31.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/completions.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1694 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/embeddings.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2463 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/files.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.752654 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      311 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3757 2024-04-18 02:16:25.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/jobs.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1885 2024-04-18 02:25:48.000000 zhipuai-2.0.1.20240423/zhipuai/api_resource/images.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.911214 zhipuai-2.0.1.20240423/zhipuai/core/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/core/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      406 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/core/_base_api.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     6405 2024-04-19 09:33:20.000000 zhipuai-2.0.1.20240423/zhipuai/core/_base_compat.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4484 2024-04-18 11:44:33.000000 zhipuai-2.0.1.20240423/zhipuai/core/_base_type.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2038 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423/zhipuai/core/_errors.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1384 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423/zhipuai/core/_files.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)    13808 2024-04-22 05:32:45.000000 zhipuai-2.0.1.20240423/zhipuai/core/_http_client.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      713 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/core/_jwt_token.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     2346 2024-04-18 11:27:16.000000 zhipuai-2.0.1.20240423/zhipuai/core/_request_opt.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3640 2024-04-18 11:34:04.000000 zhipuai-2.0.1.20240423/zhipuai/core/_response.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     4085 2024-04-17 12:20:06.000000 zhipuai-2.0.1.20240423/zhipuai/core/_sse_client.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.965067 zhipuai-2.0.1.20240423/zhipuai/core/_utils/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1451 2024-04-18 10:47:00.000000 zhipuai-2.0.1.20240423/zhipuai/core/_utils/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     3858 2024-04-18 10:47:00.000000 zhipuai-2.0.1.20240423/zhipuai/core/_utils/_typing.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)    11363 2024-04-18 10:49:15.000000 zhipuai-2.0.1.20240423/zhipuai/core/_utils/_utils.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.022095 zhipuai-2.0.1.20240423/zhipuai/types/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/__init__.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.112862 zhipuai-2.0.1.20240423/zhipuai/types/chat/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        0 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      557 2024-04-22 05:31:29.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/async_chat_completion.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      885 2024-04-22 05:23:09.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1257 2024-04-18 10:59:17.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      171 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completions_create_param.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      434 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/embeddings.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      538 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/file_object.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:16.181752 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      244 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/__init__.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1113 2024-04-18 10:59:17.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1110 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      339 2024-04-15 03:34:35.000000 zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)      382 2024-04-18 10:55:02.000000 zhipuai-2.0.1.20240423/zhipuai/types/image.py
+drwxr-xr-x   0 dmeck     (1000) dmeck     (1000)        0 2024-04-23 09:10:15.575525 zhipuai-2.0.1.20240423/zhipuai.egg-info/
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     7982 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/PKG-INFO
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)     1694 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        1 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)       64 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/requires.txt
+-rw-r--r--   0 dmeck     (1000) dmeck     (1000)        8 2024-04-23 09:10:15.000000 zhipuai-2.0.1.20240423/zhipuai.egg-info/top_level.txt
```

### Comparing `zhipuai-2.0.1/setup.py` & `zhipuai-2.0.1.20240423/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="zhipuai",
-    version="v2.0.1",
+    version="v2.0.1.20240423",
     description="A SDK library for accessing big model apis from ZhipuAI",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Zhipu AI",
     url="https://open.bigmodel.cn/",
     packages=find_packages(exclude=['test', 'examples']),
     include_package_data=True,
```

### Comparing `zhipuai-2.0.1/zhipuai/_client.py` & `zhipuai-2.0.1.20240423/zhipuai/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from . import api_resource
 import os
 import httpx
 from httpx import Timeout
 
 
 class ZhipuAI(HttpClient):
-    chat: api_resource.chat
+    chat: api_resource.chat.Chat
     api_key: str
 
     def __init__(
             self,
             *,
             api_key: str | None = None,
             base_url: str | httpx.URL | None = None,
@@ -52,15 +52,16 @@
         self.files = api_resource.files.Files(self)
         self.fine_tuning = api_resource.fine_tuning.FineTuning(self)
 
     @property
     @override
     def _auth_headers(self) -> dict[str, str]:
         api_key = self.api_key
-        return {"Authorization": f"{_jwt_token.generate_token(api_key)}"}
+        # return {"Authorization": f"{_jwt_token.generate_token(api_key)}"}
+        return {"Authorization": f"{api_key}"}
 
     def __del__(self) -> None:
         if (not hasattr(self, "_has_custom_http_client")
                 or not hasattr(self, "close")
                 or not hasattr(self, "_client")):
             # if the '__init__' method raised an error, self would not have client attr
             return
```

### Comparing `zhipuai-2.0.1/zhipuai/api_resource/chat/async_completions.py` & `zhipuai-2.0.1.20240423/zhipuai/api_resource/chat/async_completions.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 from typing_extensions import Literal
 
 from ...core._base_api import BaseAPI
-from ...core._base_type import NotGiven, NOT_GIVEN, Headers
-from ...core._http_client import make_user_request_input
+from ...core._base_type import NotGiven, NOT_GIVEN, Headers, Body
+from ...core._http_client import make_request_options
 from ...types.chat.async_chat_completion import AsyncTaskStatus, AsyncCompletion
 
 if TYPE_CHECKING:
     from ..._client import ZhipuAI
 
 
 class AsyncCompletions(BaseAPI):
@@ -31,14 +31,15 @@
             seed: int | NotGiven = NOT_GIVEN,
             messages: Union[str, List[str], List[int], List[List[int]], None],
             stop: Optional[Union[str, List[str], None]] | NotGiven = NOT_GIVEN,
             sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
             tools: Optional[object] | NotGiven = NOT_GIVEN,
             tool_choice: str | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
             disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncTaskStatus:
         _cast_type = AsyncTaskStatus
 
         if disable_strict_validation:
             _cast_type = object
@@ -54,34 +55,34 @@
                 "seed": seed,
                 "messages": messages,
                 "stop": stop,
                 "sensitive_word_check": sensitive_word_check,
                 "tools": tools,
                 "tool_choice": tool_choice,
             },
-            options=make_user_request_input(
-                extra_headers=extra_headers, timeout=timeout
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=_cast_type,
             enable_stream=False,
         )
 
     def retrieve_completion_result(
         self,
         id: str,
         extra_headers: Headers | None = None,
+        extra_body: Body | None = None,
         disable_strict_validation: Optional[bool] | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Union[AsyncCompletion, AsyncTaskStatus]:
         _cast_type = Union[AsyncCompletion,AsyncTaskStatus]
         if disable_strict_validation:
             _cast_type = object
         return self._get(
             path=f"/async-result/{id}",
             cast_type=_cast_type,
-            options=make_user_request_input(
-                extra_headers=extra_headers,
-                timeout=timeout
-            )
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
+            ),
         )
```

### Comparing `zhipuai-2.0.1/zhipuai/api_resource/chat/completions.py` & `zhipuai-2.0.1.20240423/zhipuai/api_resource/files.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 from __future__ import annotations
 
-from typing import Union, List, Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
 import httpx
-from typing_extensions import Literal
 
-from ...core._base_api import BaseAPI
-from ...core._base_type import NotGiven, NOT_GIVEN, Headers
-from ...core._http_client import make_user_request_input
-from ...core._sse_client import StreamResponse
-from ...types.chat.chat_completion import Completion
-from ...types.chat.chat_completion_chunk import ChatCompletionChunk
+from ..core._base_api import BaseAPI
+from ..core._base_type import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
+from ..core._files import is_file_content
+from ..core._http_client import (
+    make_request_options,
+)
+from ..types.file_object import FileObject, ListOfFileObject
 
 if TYPE_CHECKING:
-    from ..._client import ZhipuAI
+    from .._client import ZhipuAI
 
+__all__ = ["Files"]
+
+
+class Files(BaseAPI):
 
-class Completions(BaseAPI):
     def __init__(self, client: "ZhipuAI") -> None:
         super().__init__(client)
 
     def create(
             self,
             *,
-            model: str,
-            request_id: Optional[str] | NotGiven = NOT_GIVEN,
-            do_sample: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
-            stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
-            temperature: Optional[float] | NotGiven = NOT_GIVEN,
-            top_p: Optional[float] | NotGiven = NOT_GIVEN,
-            max_tokens: int | NotGiven = NOT_GIVEN,
-            seed: int | NotGiven = NOT_GIVEN,
-            messages: Union[str, List[str], List[int], object, None],
-            stop: Optional[Union[str, List[str], None]] | NotGiven = NOT_GIVEN,
-            sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
-            tools: Optional[object] | NotGiven = NOT_GIVEN,
-            tool_choice: str | NotGiven = NOT_GIVEN,
+            file: FileTypes,
+            purpose: str,
             extra_headers: Headers | None = None,
-            disable_strict_validation: Optional[bool] | None = None,
+            extra_body: Body | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Completion | StreamResponse[ChatCompletionChunk]:
-        _cast_type = Completion
-        _stream_cls = StreamResponse[ChatCompletionChunk]
-        if disable_strict_validation:
-            _cast_type = object
-            _stream_cls = StreamResponse[object]
+    ) -> FileObject:
+        if not is_file_content(file):
+            prefix = f"Expected file input `{file!r}`"
+            raise RuntimeError(
+                f"{prefix} to be bytes, an io.IOBase instance, PathLike or a tuple but received {type(file)} instead."
+            ) from None
+        files = [("file", file)]
+
+        extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
+
         return self._post(
-            "/chat/completions",
+            "/files",
             body={
-                "model": model,
-                "request_id": request_id,
-                "temperature": temperature,
-                "top_p": top_p,
-                "do_sample": do_sample,
-                "max_tokens": max_tokens,
-                "seed": seed,
-                "messages": messages,
-                "stop": stop,
-                "sensitive_word_check": sensitive_word_check,
-                "stream": stream,
-                "tools": tools,
-                "tool_choice": tool_choice,
+                "purpose": purpose,
             },
-            options=make_user_request_input(
+            files=files,
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
+            ),
+            cast_type=FileObject,
+        )
+
+    def list(
+            self,
+            *,
+            purpose: str | NotGiven = NOT_GIVEN,
+            limit: int | NotGiven = NOT_GIVEN,
+            after: str | NotGiven = NOT_GIVEN,
+            order: str | NotGiven = NOT_GIVEN,
+            extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
+            timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> ListOfFileObject:
+        return self._get(
+            "/files",
+            cast_type=ListOfFileObject,
+            options=make_request_options(
                 extra_headers=extra_headers,
+                extra_body=extra_body,
+                timeout=timeout,
+                query={
+                    "purpose": purpose,
+                    "limit": limit,
+                    "after": after,
+                    "order": order,
+                },
             ),
-            cast_type=_cast_type,
-            enable_stream=stream or False,
-            stream_cls=_stream_cls,
         )
```

### Comparing `zhipuai-2.0.1/zhipuai/api_resource/embeddings.py` & `zhipuai-2.0.1.20240423/zhipuai/api_resource/embeddings.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 
 from ..core._base_api import BaseAPI
 from ..core._base_type import NotGiven, NOT_GIVEN, Headers
-from ..core._http_client import make_user_request_input
+from ..core._http_client import make_request_options
 from ..types.embeddings import EmbeddingsResponded
 
 if TYPE_CHECKING:
     from .._client import ZhipuAI
 
 
 class Embeddings(BaseAPI):
@@ -22,14 +22,15 @@
             *,
             input: Union[str, List[str], List[int], List[List[int]]],
             model: Union[str],
             encoding_format: str | NotGiven = NOT_GIVEN,
             user: str | NotGiven = NOT_GIVEN,
             sensitive_word_check: Optional[object] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
             disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> EmbeddingsResponded:
         _cast_type = EmbeddingsResponded
         if disable_strict_validation:
             _cast_type = object
         return self._post(
@@ -37,13 +38,13 @@
             body={
                 "input": input,
                 "model": model,
                 "encoding_format": encoding_format,
                 "user": user,
                 "sensitive_word_check": sensitive_word_check,
             },
-            options=make_user_request_input(
-                extra_headers=extra_headers, timeout=timeout
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=_cast_type,
             enable_stream=False,
         )
```

### Comparing `zhipuai-2.0.1/zhipuai/api_resource/files.py` & `zhipuai-2.0.1.20240423/zhipuai/api_resource/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,56 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import Union, List, Optional, TYPE_CHECKING
 
 import httpx
 
 from ..core._base_api import BaseAPI
-from ..core._base_type import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
-from ..core._files import is_file_content
-from ..core._http_client import (
-    make_user_request_input,
-)
-from ..types.file_object import FileObject, ListOfFileObject
+from ..core._base_type import NotGiven, NOT_GIVEN, Headers, Body
+from ..core._http_client import make_request_options
+from ..types.image import ImagesResponded
 
 if TYPE_CHECKING:
     from .._client import ZhipuAI
 
-__all__ = ["Files"]
-
-
-class Files(BaseAPI):
 
+class Images(BaseAPI):
     def __init__(self, client: "ZhipuAI") -> None:
         super().__init__(client)
 
-    def create(
+    def generations(
             self,
             *,
-            file: FileTypes,
-            purpose: str,
+            prompt: str,
+            model: str | NotGiven = NOT_GIVEN,
+            n: Optional[int] | NotGiven = NOT_GIVEN,
+            quality: Optional[str] | NotGiven = NOT_GIVEN,
+            response_format: Optional[str] | NotGiven = NOT_GIVEN,
+            size: Optional[str] | NotGiven = NOT_GIVEN,
+            style: Optional[str] | NotGiven = NOT_GIVEN,
+            user: str | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
+            disable_strict_validation: Optional[bool] | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> FileObject:
-        if not is_file_content(file):
-            prefix = f"Expected file input `{file!r}`"
-            raise RuntimeError(
-                f"{prefix} to be bytes, an io.IOBase instance, PathLike or a tuple but received {type(file)} instead."
-            ) from None
-        files = [("file", file)]
-
-        extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
-
+    ) -> ImagesResponded:
+        _cast_type = ImagesResponded
+        if disable_strict_validation:
+            _cast_type = object
         return self._post(
-            "/files",
+            "/images/generations",
             body={
-                "purpose": purpose,
+                "prompt": prompt,
+                "model": model,
+                "n": n,
+                "quality": quality,
+                "response_format": response_format,
+                "size": size,
+                "style": style,
+                "user": user,
             },
-            files=files,
-            options=make_user_request_input(
-                extra_headers=extra_headers, timeout=timeout
-            ),
-            cast_type=FileObject,
-        )
-
-    def list(
-            self,
-            *,
-            purpose: str | NotGiven = NOT_GIVEN,
-            limit: int  | NotGiven = NOT_GIVEN,
-            after: str | NotGiven = NOT_GIVEN,
-            order: str | NotGiven = NOT_GIVEN,
-            extra_headers: Headers | None = None,
-            timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ListOfFileObject:
-        return self._get(
-            "/files",
-            cast_type=ListOfFileObject,
-            options=make_user_request_input(
-                extra_headers=extra_headers,
-                timeout=timeout,
-                query={
-                    "purpose": purpose,
-                    "limit": limit,
-                    "after": after,
-                    "order": order,
-                },
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
+            cast_type=_cast_type,
+            enable_stream=False,
         )
```

### Comparing `zhipuai-2.0.1/zhipuai/api_resource/fine_tuning/jobs.py` & `zhipuai-2.0.1.20240423/zhipuai/api_resource/fine_tuning/jobs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
 
 import httpx
 
 from ...core._base_api import BaseAPI
-from ...core._base_type import NOT_GIVEN, Headers, NotGiven
+from ...core._base_type import NOT_GIVEN, Headers, NotGiven, Body
 from ...core._http_client import (
-    make_user_request_input,
+    make_request_options,
 )
 from ...types.fine_tuning import (
     FineTuningJob,
     job_create_params,
     ListOfFineTuningJob,
     FineTuningJobEvent,
 )
@@ -33,60 +33,64 @@
             model: str,
             training_file: str,
             hyperparameters: job_create_params.Hyperparameters | NotGiven = NOT_GIVEN,
             suffix: Optional[str] | NotGiven = NOT_GIVEN,
             request_id: Optional[str] | NotGiven = NOT_GIVEN,
             validation_file: Optional[str] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> FineTuningJob:
         return self._post(
             "/fine_tuning/jobs",
             body={
                 "model": model,
                 "training_file": training_file,
                 "hyperparameters": hyperparameters,
                 "suffix": suffix,
                 "validation_file": validation_file,
                 "request_id": request_id,
             },
-            options=make_user_request_input(
-                extra_headers=extra_headers, timeout=timeout
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=FineTuningJob,
         )
 
     def retrieve(
             self,
             fine_tuning_job_id: str,
             *,
             extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> FineTuningJob:
         return self._get(
             f"/fine_tuning/jobs/{fine_tuning_job_id}",
-            options=make_user_request_input(
-                extra_headers=extra_headers, timeout=timeout
+            options=make_request_options(
+                extra_headers=extra_headers, extra_body=extra_body, timeout=timeout
             ),
             cast_type=FineTuningJob,
         )
 
     def list(
             self,
             *,
             after: str | NotGiven = NOT_GIVEN,
             limit: int | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
+            extra_body: Body | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> ListOfFineTuningJob:
         return self._get(
             "/fine_tuning/jobs",
             cast_type=ListOfFineTuningJob,
-            options=make_user_request_input(
+            options=make_request_options(
                 extra_headers=extra_headers,
+                extra_body=extra_body,
                 timeout=timeout,
                 query={
                     "after": after,
                     "limit": limit,
                 },
             ),
         )
@@ -94,22 +98,24 @@
     def list_events(
         self,
         fine_tuning_job_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         extra_headers: Headers | None = None,
+        extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> FineTuningJobEvent:
 
         return self._get(
             f"/fine_tuning/jobs/{fine_tuning_job_id}/events",
             cast_type=FineTuningJobEvent,
-            options=make_user_request_input(
+            options=make_request_options(
                 extra_headers=extra_headers,
+                extra_body=extra_body,
                 timeout=timeout,
                 query={
                     "after": after,
                     "limit": limit,
                 },
             ),
         )
```

### Comparing `zhipuai-2.0.1/zhipuai/core/_base_type.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_base_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 from os import PathLike
 from typing import (
+    IO,
     TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
     Type,
+    Tuple,
     Union,
     Mapping,
-    TypeVar, IO, Tuple, Sequence, Any, List,
+    TypeVar,
+    Callable,
+    Optional,
+    Sequence,
 )
-
 import pydantic
-from typing_extensions import (
-    Literal,
-    override,
-)
-
-
+from httpx import Response
+from typing_extensions import Literal, Protocol, TypeAlias, TypedDict, override, runtime_checkable
 Query = Mapping[str, object]
 Body = object
 AnyMapping = Mapping[str, object]
 PrimitiveData = Union[str, int, float, bool, None]
 Data = Union[PrimitiveData, List[Any], Tuple[Any], "Mapping[str, Any]"]
 ModelT = TypeVar("ModelT", bound=pydantic.BaseModel)
 _T = TypeVar("_T")
@@ -76,21 +79,65 @@
     ```
     """
 
     def __bool__(self) -> Literal[False]:
         return False
 
 
+@runtime_checkable
+class ModelBuilderProtocol(Protocol):
+    @classmethod
+    def build(
+            cls: type[_T],
+            *,
+            response: Response,
+            data: object,
+    ) -> _T:
+        ...
+
+
 Headers = Mapping[str, Union[str, Omit]]
 
+
+class HeadersLikeProtocol(Protocol):
+    def get(self, __key: str) -> str | None:
+        ...
+
+
+HeadersLike = Union[Headers, HeadersLikeProtocol]
+
 ResponseT = TypeVar(
     "ResponseT",
     bound="Union[str, None, BaseModel, List[Any], Dict[str, Any], Response, UnknownResponse, ModelBuilderProtocol, BinaryResponseContent]",
 )
 
+StrBytesIntFloat = Union[str, bytes, int, float]
+
+# Note: copied from Pydantic
+# https://github.com/pydantic/pydantic/blob/32ea570bf96e84234d2992e1ddf40ab8a565925a/pydantic/main.py#L49
+IncEx: TypeAlias = "set[int] | set[str] | dict[int, Any] | dict[str, Any] | None"
+
+PostParser = Callable[[Any], Any]
+
+
+@runtime_checkable
+class InheritsGeneric(Protocol):
+    """Represents a type that has inherited from `Generic`
+
+    The `__orig_bases__` property can be used to determine the resolved
+    type variable for a given base class.
+    """
+
+    __orig_bases__: tuple[_GenericAlias]
+
+
+class _GenericAlias(Protocol):
+    __origin__: type[object]
+
+
 # for user input files
 if TYPE_CHECKING:
     FileContent = Union[IO[bytes], bytes, PathLike[str]]
 else:
     FileContent = Union[IO[bytes], bytes, PathLike]
 
 FileTypes = Union[
```

### Comparing `zhipuai-2.0.1/zhipuai/core/_errors.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_errors.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1/zhipuai/core/_files.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_files.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1/zhipuai/core/_http_client.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 
 import inspect
 from typing import (
     Any,
     Type,
     Union,
     cast,
-    Mapping,
+    Mapping, TypeVar, Dict,
 )
 
 import httpx
 import pydantic
 from httpx import URL, Timeout
 
 from . import _errors
-from ._base_type import NotGiven, ResponseT, Body, Headers, NOT_GIVEN, RequestFiles, Query, Data
+from ._base_compat import parse_obj
+from ._base_type import NotGiven, ResponseT, Body, Headers, NOT_GIVEN, RequestFiles, Query, Data, Omit, AnyMapping, \
+    ModelBuilderProtocol
 from ._errors import APIResponseValidationError, APIStatusError, APITimeoutError
 from ._files import make_httpx_files
 from ._request_opt import ClientRequestParam, UserRequestInput
 from ._response import HttpResponse
 from ._sse_client import StreamResponse
-from ._utils import flatten
+from ._utils import flatten, is_mapping
+from .._base_models import construct_type
+
+_T = TypeVar("_T")
+_T_co = TypeVar("_T_co", covariant=True)
+
 
 headers = {
     "Accept": "application/json",
     "Content-Type": "application/json; charset=UTF-8",
 }
 
 
-def _merge_map(map1: Mapping, map2: Mapping) -> Mapping:
-    merged = {**map1, **map2}
-    return {key: val for key, val in merged.items() if val is not None}
-
-
 from httpx._config import DEFAULT_TIMEOUT_CONFIG as HTTPX_DEFAULT_TIMEOUT
 
 ZHIPUAI_DEFAULT_TIMEOUT = httpx.Timeout(timeout=300.0, connect=8.0)
 ZHIPUAI_DEFAULT_MAX_RETRIES = 3
 ZHIPUAI_DEFAULT_LIMITS = httpx.Limits(max_connections=50, max_keepalive_connections=10)
 
 
@@ -103,31 +105,43 @@
 
     @property
     def _auth_headers(self):
         return {}
 
     def _prepare_headers(self, request_param: ClientRequestParam) -> httpx.Headers:
         custom_headers = request_param.headers or {}
-        headers_dict = _merge_map(self._default_headers, custom_headers)
+        headers_dict = _merge_mappings(self._default_headers, custom_headers)
 
         httpx_headers = httpx.Headers(headers_dict)
 
         return httpx_headers
 
-    def _prepare_request(
+    def _build_request(
             self,
             request_param: ClientRequestParam
     ) -> httpx.Request:
         kwargs: dict[str, Any] = {}
-        json_data = request_param.json_data
         headers = self._prepare_headers(request_param)
         url = self._prepare_url(request_param.url)
         json_data = request_param.json_data
+        if request_param.extra_json is not None:
+            if json_data is None:
+                json_data = cast(Body, request_param.extra_json)
+            elif is_mapping(json_data):
+                json_data = _merge_mappings(json_data, request_param.extra_json)
+            else:
+                raise RuntimeError(f"Unexpected JSON data type, {type(json_data)}, cannot merge with `extra_body`")
+
+        content_type = headers.get("Content-Type")
+        # multipart/form-data; boundary=---abc--
         if headers.get("Content-Type") == "multipart/form-data":
-            headers.pop("Content-Type")
+            if "boundary" not in content_type:
+                # only remove the header if the boundary hasn't been explicitly set
+                # as the caller doesn't want httpx to come up with their own boundary
+                headers.pop("Content-Type")
 
             if json_data:
                 kwargs["data"] = self._make_multipartform(json_data)
 
         return self._client.build_request(
             headers=headers,
             timeout=self.timeout if isinstance(request_param.timeout, NotGiven) else request_param.timeout,
@@ -200,22 +214,26 @@
     def _process_response_data(
             self,
             *,
             data: object,
             cast_type: type[ResponseT],
             response: httpx.Response,
     ) -> ResponseT:
+
         if data is None:
             return cast(ResponseT, None)
 
+        if cast_type is object:
+            return cast(ResponseT, data)
+
         try:
-            if inspect.isclass(cast_type) and issubclass(cast_type, pydantic.BaseModel):
-                return cast(ResponseT, cast_type.model_validate(data))
+            if inspect.isclass(cast_type) and issubclass(cast_type, ModelBuilderProtocol):
+                return cast(ResponseT, cast_type.build(response=response, data=data))
 
-            return cast(ResponseT, pydantic.TypeAdapter(cast_type).validate_python(data))
+            return cast(ResponseT, construct_type(type_=cast_type, value=data))
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(response=response, json_data=data) from err
 
     def is_closed(self) -> bool:
         return self._client.is_closed
 
     def close(self):
@@ -225,21 +243,21 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def request(
             self,
-            *,
             cast_type: Type[ResponseT],
             params: ClientRequestParam,
+            *,
             enable_stream: bool = False,
             stream_cls: type[StreamResponse[Any]] | None = None,
     ) -> ResponseT | StreamResponse:
-        request = self._prepare_request(params)
+        request = self._build_request(params)
 
         try:
             response = self._client.send(
                 request,
                 stream=enable_stream,
             )
             response.raise_for_status()
@@ -353,25 +371,45 @@
         elif status_code == 500:
             return _errors.APIInternalError(message=error_msg, response=response)
         elif status_code == 503:
             return _errors.APIServerFlowExceedError(message=error_msg, response=response)
         return APIStatusError(message=error_msg, response=response)
 
 
-def make_user_request_input(
-        max_retries: int | None = None,
-        timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
-        extra_headers: Headers = None,
+def make_request_options(
+        *,
         query: Query | None = None,
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN
 ) -> UserRequestInput:
+    """Create a dict of type RequestOptions without keys of NotGiven values."""
     options: UserRequestInput = {}
-
     if extra_headers is not None:
         options["headers"] = extra_headers
-    if max_retries is not None:
-        options["max_retries"] = max_retries
-    if not isinstance(timeout, NotGiven):
-        options['timeout'] = timeout
+
+    if extra_body is not None:
+        options["extra_json"] = cast(AnyMapping, extra_body)
+
     if query is not None:
         options["params"] = query
 
+    if extra_query is not None:
+        options["params"] = {**options.get("params", {}), **extra_query}
+
+    if not isinstance(timeout, NotGiven):
+        options["timeout"] = timeout
+
     return options
+
+
+def _merge_mappings(
+        obj1: Mapping[_T_co, Union[_T, Omit]],
+        obj2: Mapping[_T_co, Union[_T, Omit]],
+) -> Dict[_T_co, _T]:
+    """Merge two mappings of the same type, removing any values that are instances of `Omit`.
+
+    In cases with duplicate keys the second mapping takes precedence.
+    """
+    merged = {**obj1, **obj2}
+    return {key: value for key, value in merged.items() if not isinstance(value, Omit)}
```

### Comparing `zhipuai-2.0.1/zhipuai/core/_jwt_token.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1/zhipuai/core/_request_opt.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_request_opt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from __future__ import annotations
 
-from typing import Union, Any, cast
+from typing import Union, Any, cast, TYPE_CHECKING
 
+from ._base_compat import ConfigDict, PYDANTIC_V2
 import pydantic.generics
 from httpx import Timeout
-from pydantic import ConfigDict
 from typing_extensions import (
     final, Unpack, ClassVar, TypedDict
 
 )
 
-from ._base_type import Body, NotGiven, Headers, HttpxRequestFiles, Query
-from ._utils import remove_notgiven_indict
+from ._base_type import Body, NotGiven, Headers, HttpxRequestFiles, Query, AnyMapping
+from ._utils import remove_notgiven_indict, strip_not_given
 
 
 class UserRequestInput(TypedDict, total=False):
+    headers: Headers
     max_retries: int
     timeout: float | Timeout | None
-    headers: Headers
-    params: Query | None
+    params: Query
+    extra_json: AnyMapping
 
 
 @final
 class ClientRequestParam(pydantic.BaseModel):
     method: str
     url: str
     max_retries: Union[int, NotGiven] = NotGiven()
     timeout: Union[float, Timeout, NotGiven] = NotGiven()
     headers: Union[Headers, NotGiven] = NotGiven()
-    json_data: Union[Body, None] = None
     files: Union[HttpxRequestFiles, None] = None
     params: Query = {}
-    model_config: ClassVar[ConfigDict] = ConfigDict(arbitrary_types_allowed=True)
+
+    json_data: Union[Body, None] = None
+    extra_json: Union[AnyMapping, None] = None
+
+    if PYDANTIC_V2:
+        model_config: ClassVar[ConfigDict] = ConfigDict(arbitrary_types_allowed=True)
+    else:
+
+        class Config(pydantic.BaseConfig):  # pyright: ignore[reportDeprecated]
+            arbitrary_types_allowed: bool = True
 
     def get_max_retries(self, max_retries) -> int:
         if isinstance(self.max_retries, NotGiven):
             return max_retries
         return self.max_retries
 
     @classmethod
@@ -43,11 +52,21 @@
             cls,
             _fields_set: set[str] | None = None,
             **values: Unpack[UserRequestInput],
     ) -> ClientRequestParam :
         kwargs: dict[str, Any] = {
             key: remove_notgiven_indict(value) for key, value in values.items()
         }
-        return cast(ClientRequestParam, super().model_construct(_fields_set, **kwargs))
+        kwargs: dict[str, Any] = {
+            # we unconditionally call `strip_not_given` on any value
+            # as it will just ignore any non-mapping types
+            key: strip_not_given(value)
+            for key, value in values.items()
+        }
+        if PYDANTIC_V2:
+            return cast(ClientRequestParam, super().model_construct(_fields_set, **kwargs))
 
-    model_construct = construct
+        return cast(ClientRequestParam, super().construct(_fields_set, **kwargs))  # pyright: ignore[reportDeprecated]
 
+    if not TYPE_CHECKING:
+        # type checkers incorrectly complain about this assignment
+        model_construct = construct
```

### Comparing `zhipuai-2.0.1/zhipuai/core/_response.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import datetime
 from typing import TypeVar, Generic, cast, Any, TYPE_CHECKING
 
 import httpx
-import pydantic
+import logging
 from typing_extensions import ParamSpec, get_origin, get_args
 
 from ._base_type import NoneType
 from ._sse_client import StreamResponse
+from .._base_models import is_basemodel
 
 if TYPE_CHECKING:
     from ._http_client import HttpClient
 
 P = ParamSpec("P")
 R = TypeVar("R")
-
+log: logging.Logger = logging.getLogger(__name__)
 
 class HttpResponse(Generic[R]):
     _cast_type: type[R]
     _client: "HttpClient"
     _parsed: R | None
     _enable_stream: bool
     _stream_cls: type[StreamResponse[Any]]
@@ -62,21 +63,25 @@
         http_response = self.http_response
         if cast_type == str:
             return cast(R, http_response.text)
 
         content_type, *_ = http_response.headers.get("content-type", "application/json").split(";")
         origin = get_origin(cast_type) or cast_type
         if content_type != "application/json":
-            if issubclass(origin, pydantic.BaseModel):
-                data = http_response.json()
-                return self._client._process_response_data(
-                    data=data,
-                    cast_type=cast_type,  # type: ignore
-                    response=http_response,
-                )
+            if is_basemodel(cast_type):
+                try:
+                    data = http_response.json()
+                except Exception as exc:
+                    log.debug("Could not read JSON from response data due to %s - %s", type(exc), exc)
+                else:
+                    return self._client._process_response_data(
+                        data=data,
+                        cast_to=cast_type,  # type: ignore
+                        response=http_response,
+                    )
 
             return http_response.text
 
         data = http_response.json()
 
         return self._client._process_response_data(
             data=data,
```

### Comparing `zhipuai-2.0.1/zhipuai/core/_sse_client.py` & `zhipuai-2.0.1.20240423/zhipuai/core/_sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1/zhipuai/types/chat/async_chat_completion.py` & `zhipuai-2.0.1.20240423/zhipuai/types/chat/async_chat_completion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List, Optional
 
-from pydantic import BaseModel
-
+from ..._base_models import BaseModel
 from .chat_completion import CompletionChoice, CompletionUsage
 
 __all__ = ["AsyncTaskStatus"]
 
 
 class AsyncTaskStatus(BaseModel):
     id: Optional[str] = None
@@ -16,8 +15,8 @@
 
 class AsyncCompletion(BaseModel):
     id: Optional[str] = None
     request_id: Optional[str] = None
     model: Optional[str] = None
     task_status: str
     choices: List[CompletionChoice]
-    usage: CompletionUsage
+    usage: CompletionUsage
```

### Comparing `zhipuai-2.0.1/zhipuai/types/chat/chat_completion.py` & `zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import List, Optional
+from typing import List, Optional, Union, Dict, Any
 
-from pydantic import BaseModel
+from ..._base_models import BaseModel
 
 __all__ = ["Completion", "CompletionUsage"]
 
 
 class Function(BaseModel):
     arguments: str
     name: str
@@ -38,8 +38,7 @@
     model: Optional[str] = None
     created: Optional[int] = None
     choices: List[CompletionChoice]
     request_id: Optional[str] = None
     id: Optional[str] = None
     usage: CompletionUsage
 
-
```

### Comparing `zhipuai-2.0.1/zhipuai/types/chat/chat_completion_chunk.py` & `zhipuai-2.0.1.20240423/zhipuai/types/chat/chat_completion_chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import List, Optional
+from typing import List, Optional, Dict, Any
 
-from pydantic import BaseModel
+from ..._base_models import BaseModel
 
 __all__ = [
     "ChatCompletionChunk",
     "Choice",
     "ChoiceDelta",
     "ChoiceDeltaFunctionCall",
     "ChoiceDeltaToolCall",
@@ -49,7 +49,8 @@
 
 class ChatCompletionChunk(BaseModel):
     id: Optional[str] = None
     choices: List[Choice]
     created: Optional[int] = None
     model: Optional[str] = None
     usage: Optional[CompletionUsage] = None
+    extra_json: Dict[str, Any]
```

### Comparing `zhipuai-2.0.1/zhipuai/types/file_object.py` & `zhipuai-2.0.1.20240423/zhipuai/types/file_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, List
 
-from pydantic import BaseModel
+from .._base_models import BaseModel
 
 __all__ = ["FileObject"]
 
 
 class FileObject(BaseModel):
 
     id: Optional[str] = None
```

### Comparing `zhipuai-2.0.1/zhipuai/types/fine_tuning/fine_tuning_job.py` & `zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Dict, Any
 from typing_extensions import Literal
 
-from pydantic import BaseModel
+from ..._base_models import BaseModel
 
 __all__ = ["FineTuningJob", "Error", "Hyperparameters", "ListOfFineTuningJob" ]
 
 
 class Error(BaseModel):
     code: str
     message: str
@@ -40,13 +40,15 @@
     status: str
 
     trained_tokens: Optional[int] = None
 
     training_file: str
 
     validation_file: Optional[str] = None
+    extra_json: Dict[str, Any]
 
 
 class ListOfFineTuningJob(BaseModel):
     object: Optional[str] = None
     data: List[FineTuningJob]
     has_more: Optional[bool] = None
+    extra_json: Dict[str, Any]
```

### Comparing `zhipuai-2.0.1/zhipuai/types/fine_tuning/fine_tuning_job_event.py` & `zhipuai-2.0.1.20240423/zhipuai/types/fine_tuning/fine_tuning_job_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Union, Optional
 from typing_extensions import Literal
 
-from pydantic import BaseModel
+from ..._base_models import BaseModel
 
 __all__ = ["FineTuningJobEvent", "Metric", "JobEvent"]
 
 
 class Metric(BaseModel):
     epoch: Optional[Union[str, int, float]] = None
     current_steps: Optional[int] = None
```

