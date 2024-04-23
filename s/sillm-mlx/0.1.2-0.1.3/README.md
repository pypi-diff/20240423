# Comparing `tmp/sillm-mlx-0.1.2.tar.gz` & `tmp/sillm-mlx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sillm-mlx-0.1.2.tar", last modified: Fri Apr 19 14:22:42 2024, max compression
+gzip compressed data, was "sillm-mlx-0.1.3.tar", last modified: Tue Apr 23 18:35:44 2024, max compression
```

## Comparing `sillm-mlx-0.1.2.tar` & `sillm-mlx-0.1.3.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.813701 sillm-mlx-0.1.2/
--rw-r--r--   0 armin      (501) staff       (20)     1071 2024-01-14 11:43:40.000000 sillm-mlx-0.1.2/LICENSE
--rw-r--r--   0 armin      (501) staff       (20)     7829 2024-04-19 14:22:42.813526 sillm-mlx-0.1.2/PKG-INFO
--rw-r--r--   0 armin      (501) staff       (20)     7164 2024-04-16 14:05:30.000000 sillm-mlx-0.1.2/README.md
--rw-r--r--   0 armin      (501) staff       (20)       38 2024-04-19 14:22:42.813734 sillm-mlx-0.1.2/setup.cfg
--rw-r--r--   0 armin      (501) staff       (20)      921 2024-04-19 14:21:58.000000 sillm-mlx-0.1.2/setup.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.808797 sillm-mlx-0.1.2/sillm/
--rw-r--r--   0 armin      (501) staff       (20)      517 2024-04-19 12:35:05.000000 sillm-mlx-0.1.2/sillm/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)     4201 2024-04-19 12:42:57.000000 sillm-mlx-0.1.2/sillm/chat.py
--rw-r--r--   0 armin      (501) staff       (20)     1940 2024-04-10 11:04:13.000000 sillm-mlx-0.1.2/sillm/convert.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.809386 sillm-mlx-0.1.2/sillm/core/
--rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.2/sillm/core/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)     3344 2024-04-19 12:34:01.000000 sillm-mlx-0.1.2/sillm/core/conversation.py
--rw-r--r--   0 armin      (501) staff       (20)    14570 2024-04-19 11:37:42.000000 sillm-mlx-0.1.2/sillm/core/llm.py
--rw-r--r--   0 armin      (501) staff       (20)     9942 2024-04-19 11:08:30.000000 sillm-mlx-0.1.2/sillm/core/loader.py
--rw-r--r--   0 armin      (501) staff       (20)     3191 2024-04-19 12:34:44.000000 sillm-mlx-0.1.2/sillm/core/template.py
--rw-r--r--   0 armin      (501) staff       (20)    13270 2024-04-18 21:52:34.000000 sillm-mlx-0.1.2/sillm/core/tokenizer.py
--rw-r--r--   0 armin      (501) staff       (20)     7079 2024-03-19 07:56:55.000000 sillm-mlx-0.1.2/sillm/dpo.py
--rw-r--r--   0 armin      (501) staff       (20)     6749 2024-04-18 22:05:58.000000 sillm-mlx-0.1.2/sillm/lora.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.810466 sillm-mlx-0.1.2/sillm/models/
--rw-r--r--   0 armin      (501) staff       (20)      252 2024-04-05 12:50:36.000000 sillm-mlx-0.1.2/sillm/models/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)     5260 2024-04-10 07:23:26.000000 sillm-mlx-0.1.2/sillm/models/args.py
--rw-r--r--   0 armin      (501) staff       (20)     1550 2024-04-09 06:58:55.000000 sillm-mlx-0.1.2/sillm/models/base.py
--rw-r--r--   0 armin      (501) staff       (20)     5418 2024-04-19 10:57:13.000000 sillm-mlx-0.1.2/sillm/models/cohere.py
--rw-r--r--   0 armin      (501) staff       (20)     3586 2024-04-04 12:52:41.000000 sillm-mlx-0.1.2/sillm/models/dbrx.py
--rw-r--r--   0 armin      (501) staff       (20)     2887 2024-04-19 10:56:44.000000 sillm-mlx-0.1.2/sillm/models/gemma.py
--rw-r--r--   0 armin      (501) staff       (20)     6299 2024-04-09 06:59:25.000000 sillm-mlx-0.1.2/sillm/models/llama.py
--rw-r--r--   0 armin      (501) staff       (20)     7179 2024-04-15 20:30:32.000000 sillm-mlx-0.1.2/sillm/models/mixtral.py
--rw-r--r--   0 armin      (501) staff       (20)     4870 2024-04-09 07:03:25.000000 sillm-mlx-0.1.2/sillm/models/phi.py
--rw-r--r--   0 armin      (501) staff       (20)     3341 2024-04-19 10:57:38.000000 sillm-mlx-0.1.2/sillm/models/qwen2.py
--rw-r--r--   0 armin      (501) staff       (20)     4017 2024-04-19 10:56:55.000000 sillm-mlx-0.1.2/sillm/models/starcoder2.py
--rw-r--r--   0 armin      (501) staff       (20)     2284 2024-04-12 13:41:37.000000 sillm-mlx-0.1.2/sillm/quantize.py
--rw-r--r--   0 armin      (501) staff       (20)     2588 2024-04-19 12:38:43.000000 sillm-mlx-0.1.2/sillm/server.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.811678 sillm-mlx-0.1.2/sillm/templates/
--rw-r--r--   0 armin      (501) staff       (20)      785 2024-04-15 20:54:36.000000 sillm-mlx-0.1.2/sillm/templates/alpaca.jinja
--rw-r--r--   0 armin      (501) staff       (20)      203 2024-03-18 08:50:40.000000 sillm-mlx-0.1.2/sillm/templates/chatml.jinja
--rw-r--r--   0 armin      (501) staff       (20)     1189 2024-04-05 15:11:13.000000 sillm-mlx-0.1.2/sillm/templates/cohere.jinja
--rw-r--r--   0 armin      (501) staff       (20)       65 2024-04-15 13:34:23.000000 sillm-mlx-0.1.2/sillm/templates/empty.jinja
--rw-r--r--   0 armin      (501) staff       (20)      594 2024-03-18 08:50:40.000000 sillm-mlx-0.1.2/sillm/templates/gemma.jinja
--rw-r--r--   0 armin      (501) staff       (20)      791 2024-03-18 08:50:40.000000 sillm-mlx-0.1.2/sillm/templates/llama2.jinja
--rw-r--r--   0 armin      (501) staff       (20)      352 2024-04-18 21:30:19.000000 sillm-mlx-0.1.2/sillm/templates/llama3.jinja
--rw-r--r--   0 armin      (501) staff       (20)      443 2024-03-18 08:50:40.000000 sillm-mlx-0.1.2/sillm/templates/mistral.jinja
--rw-r--r--   0 armin      (501) staff       (20)      222 2024-04-02 07:37:25.000000 sillm-mlx-0.1.2/sillm/templates/openchat.jinja
--rw-r--r--   0 armin      (501) staff       (20)      364 2024-03-18 08:50:40.000000 sillm-mlx-0.1.2/sillm/templates/phi2.jinja
--rw-r--r--   0 armin      (501) staff       (20)      448 2024-03-18 08:50:40.000000 sillm-mlx-0.1.2/sillm/templates/qwen2.jinja
--rw-r--r--   0 armin      (501) staff       (20)      749 2024-04-15 20:52:40.000000 sillm-mlx-0.1.2/sillm/templates/vicuna.jinja
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.812058 sillm-mlx-0.1.2/sillm/training/
--rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.2/sillm/training/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)    15284 2024-04-18 20:42:44.000000 sillm-mlx-0.1.2/sillm/training/dataset.py
--rw-r--r--   0 armin      (501) staff       (20)     6480 2024-04-17 07:19:26.000000 sillm-mlx-0.1.2/sillm/training/dpo.py
--rw-r--r--   0 armin      (501) staff       (20)    18471 2024-04-10 09:02:01.000000 sillm-mlx-0.1.2/sillm/training/lora.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.812681 sillm-mlx-0.1.2/sillm/utils/
--rw-r--r--   0 armin      (501) staff       (20)      153 2024-03-22 08:26:17.000000 sillm-mlx-0.1.2/sillm/utils/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)      393 2024-03-22 08:25:51.000000 sillm-mlx-0.1.2/sillm/utils/common.py
--rw-r--r--   0 armin      (501) staff       (20)     1332 2024-04-08 13:25:32.000000 sillm-mlx-0.1.2/sillm/utils/log.py
--rw-r--r--   0 armin      (501) staff       (20)     8236 2024-04-16 09:00:07.000000 sillm-mlx-0.1.2/sillm/utils/mapping.py
--rw-r--r--   0 armin      (501) staff       (20)     1621 2024-03-08 12:33:03.000000 sillm-mlx-0.1.2/sillm/utils/plot.py
--rw-r--r--   0 armin      (501) staff       (20)     3303 2024-04-19 11:01:39.000000 sillm-mlx-0.1.2/sillm/utils/quantization.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-19 14:22:42.813187 sillm-mlx-0.1.2/sillm_mlx.egg-info/
--rw-r--r--   0 armin      (501) staff       (20)     7829 2024-04-19 14:22:42.000000 sillm-mlx-0.1.2/sillm_mlx.egg-info/PKG-INFO
--rw-r--r--   0 armin      (501) staff       (20)     1264 2024-04-19 14:22:42.000000 sillm-mlx-0.1.2/sillm_mlx.egg-info/SOURCES.txt
--rw-r--r--   0 armin      (501) staff       (20)        1 2024-04-19 14:22:42.000000 sillm-mlx-0.1.2/sillm_mlx.egg-info/dependency_links.txt
--rw-r--r--   0 armin      (501) staff       (20)      157 2024-04-19 14:22:42.000000 sillm-mlx-0.1.2/sillm_mlx.egg-info/requires.txt
--rw-r--r--   0 armin      (501) staff       (20)        6 2024-04-19 14:22:42.000000 sillm-mlx-0.1.2/sillm_mlx.egg-info/top_level.txt
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.284939 sillm-mlx-0.1.3/
+-rw-r--r--   0 armin      (501) staff       (20)     1071 2024-01-14 11:43:40.000000 sillm-mlx-0.1.3/LICENSE
+-rw-r--r--   0 armin      (501) staff       (20)     8222 2024-04-23 18:35:44.284731 sillm-mlx-0.1.3/PKG-INFO
+-rw-r--r--   0 armin      (501) staff       (20)     7557 2024-04-23 09:23:41.000000 sillm-mlx-0.1.3/README.md
+-rw-r--r--   0 armin      (501) staff       (20)       38 2024-04-23 18:35:44.284980 sillm-mlx-0.1.3/setup.cfg
+-rw-r--r--   0 armin      (501) staff       (20)      921 2024-04-23 18:35:40.000000 sillm-mlx-0.1.3/setup.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.278289 sillm-mlx-0.1.3/sillm/
+-rw-r--r--   0 armin      (501) staff       (20)      517 2024-04-19 12:35:05.000000 sillm-mlx-0.1.3/sillm/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)     4201 2024-04-19 20:27:08.000000 sillm-mlx-0.1.3/sillm/chat.py
+-rw-r--r--   0 armin      (501) staff       (20)     1940 2024-04-10 11:04:13.000000 sillm-mlx-0.1.3/sillm/convert.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.279064 sillm-mlx-0.1.3/sillm/core/
+-rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.3/sillm/core/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)     3344 2024-04-19 12:34:01.000000 sillm-mlx-0.1.3/sillm/core/conversation.py
+-rw-r--r--   0 armin      (501) staff       (20)    15038 2024-04-23 15:35:11.000000 sillm-mlx-0.1.3/sillm/core/llm.py
+-rw-r--r--   0 armin      (501) staff       (20)     9942 2024-04-19 11:08:30.000000 sillm-mlx-0.1.3/sillm/core/loader.py
+-rw-r--r--   0 armin      (501) staff       (20)     3211 2024-04-23 16:39:16.000000 sillm-mlx-0.1.3/sillm/core/template.py
+-rw-r--r--   0 armin      (501) staff       (20)    13393 2024-04-23 18:28:42.000000 sillm-mlx-0.1.3/sillm/core/tokenizer.py
+-rw-r--r--   0 armin      (501) staff       (20)     7079 2024-03-19 07:56:55.000000 sillm-mlx-0.1.3/sillm/dpo.py
+-rw-r--r--   0 armin      (501) staff       (20)     6754 2024-04-19 19:50:31.000000 sillm-mlx-0.1.3/sillm/lora.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.280611 sillm-mlx-0.1.3/sillm/models/
+-rw-r--r--   0 armin      (501) staff       (20)      282 2024-04-23 15:37:59.000000 sillm-mlx-0.1.3/sillm/models/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)     5468 2024-04-23 16:17:33.000000 sillm-mlx-0.1.3/sillm/models/args.py
+-rw-r--r--   0 armin      (501) staff       (20)     1550 2024-04-22 13:03:34.000000 sillm-mlx-0.1.3/sillm/models/base.py
+-rw-r--r--   0 armin      (501) staff       (20)     5418 2024-04-19 10:57:13.000000 sillm-mlx-0.1.3/sillm/models/cohere.py
+-rw-r--r--   0 armin      (501) staff       (20)     3586 2024-04-04 12:52:41.000000 sillm-mlx-0.1.3/sillm/models/dbrx.py
+-rw-r--r--   0 armin      (501) staff       (20)     2887 2024-04-19 10:56:44.000000 sillm-mlx-0.1.3/sillm/models/gemma.py
+-rw-r--r--   0 armin      (501) staff       (20)     6299 2024-04-09 06:59:25.000000 sillm-mlx-0.1.3/sillm/models/llama.py
+-rw-r--r--   0 armin      (501) staff       (20)     7179 2024-04-15 20:30:32.000000 sillm-mlx-0.1.3/sillm/models/mixtral.py
+-rw-r--r--   0 armin      (501) staff       (20)     4874 2024-04-23 18:17:57.000000 sillm-mlx-0.1.3/sillm/models/phi.py
+-rw-r--r--   0 armin      (501) staff       (20)     4160 2024-04-23 18:18:50.000000 sillm-mlx-0.1.3/sillm/models/phi3.py
+-rw-r--r--   0 armin      (501) staff       (20)     3341 2024-04-19 10:57:38.000000 sillm-mlx-0.1.3/sillm/models/qwen2.py
+-rw-r--r--   0 armin      (501) staff       (20)     4017 2024-04-19 10:56:55.000000 sillm-mlx-0.1.3/sillm/models/starcoder2.py
+-rw-r--r--   0 armin      (501) staff       (20)     2294 2024-04-19 17:58:09.000000 sillm-mlx-0.1.3/sillm/quantize.py
+-rw-r--r--   0 armin      (501) staff       (20)     2588 2024-04-19 12:38:43.000000 sillm-mlx-0.1.3/sillm/server.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.282612 sillm-mlx-0.1.3/sillm/templates/
+-rw-r--r--   0 armin      (501) staff       (20)      781 2024-04-20 20:30:19.000000 sillm-mlx-0.1.3/sillm/templates/alpaca.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      203 2024-03-18 08:50:40.000000 sillm-mlx-0.1.3/sillm/templates/chatml.jinja
+-rw-r--r--   0 armin      (501) staff       (20)     1189 2024-04-05 15:11:13.000000 sillm-mlx-0.1.3/sillm/templates/cohere.jinja
+-rw-r--r--   0 armin      (501) staff       (20)       65 2024-04-15 13:34:23.000000 sillm-mlx-0.1.3/sillm/templates/empty.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      594 2024-03-18 08:50:40.000000 sillm-mlx-0.1.3/sillm/templates/gemma.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      791 2024-03-18 08:50:40.000000 sillm-mlx-0.1.3/sillm/templates/llama2.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      352 2024-04-22 13:22:39.000000 sillm-mlx-0.1.3/sillm/templates/llama3.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      443 2024-03-18 08:50:40.000000 sillm-mlx-0.1.3/sillm/templates/mistral.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      222 2024-04-02 07:37:25.000000 sillm-mlx-0.1.3/sillm/templates/openchat.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      364 2024-03-18 08:50:40.000000 sillm-mlx-0.1.3/sillm/templates/phi2.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      206 2024-04-23 18:24:26.000000 sillm-mlx-0.1.3/sillm/templates/phi3.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      448 2024-03-18 08:50:40.000000 sillm-mlx-0.1.3/sillm/templates/qwen2.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      749 2024-04-15 20:52:40.000000 sillm-mlx-0.1.3/sillm/templates/vicuna.jinja
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.283134 sillm-mlx-0.1.3/sillm/training/
+-rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.3/sillm/training/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)    15303 2024-04-22 13:22:03.000000 sillm-mlx-0.1.3/sillm/training/dataset.py
+-rw-r--r--   0 armin      (501) staff       (20)     6480 2024-04-17 07:19:26.000000 sillm-mlx-0.1.3/sillm/training/dpo.py
+-rw-r--r--   0 armin      (501) staff       (20)    18435 2024-04-22 12:40:02.000000 sillm-mlx-0.1.3/sillm/training/lora.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.283837 sillm-mlx-0.1.3/sillm/utils/
+-rw-r--r--   0 armin      (501) staff       (20)      153 2024-03-22 08:26:17.000000 sillm-mlx-0.1.3/sillm/utils/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)      393 2024-03-22 08:25:51.000000 sillm-mlx-0.1.3/sillm/utils/common.py
+-rw-r--r--   0 armin      (501) staff       (20)     1332 2024-04-08 13:25:32.000000 sillm-mlx-0.1.3/sillm/utils/log.py
+-rw-r--r--   0 armin      (501) staff       (20)     8401 2024-04-23 16:26:02.000000 sillm-mlx-0.1.3/sillm/utils/mapping.py
+-rw-r--r--   0 armin      (501) staff       (20)     1661 2024-04-21 08:07:00.000000 sillm-mlx-0.1.3/sillm/utils/plot.py
+-rw-r--r--   0 armin      (501) staff       (20)     3303 2024-04-19 11:01:39.000000 sillm-mlx-0.1.3/sillm/utils/quantization.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-23 18:35:44.284355 sillm-mlx-0.1.3/sillm_mlx.egg-info/
+-rw-r--r--   0 armin      (501) staff       (20)     8222 2024-04-23 18:35:44.000000 sillm-mlx-0.1.3/sillm_mlx.egg-info/PKG-INFO
+-rw-r--r--   0 armin      (501) staff       (20)     1312 2024-04-23 18:35:44.000000 sillm-mlx-0.1.3/sillm_mlx.egg-info/SOURCES.txt
+-rw-r--r--   0 armin      (501) staff       (20)        1 2024-04-23 18:35:44.000000 sillm-mlx-0.1.3/sillm_mlx.egg-info/dependency_links.txt
+-rw-r--r--   0 armin      (501) staff       (20)      157 2024-04-23 18:35:44.000000 sillm-mlx-0.1.3/sillm_mlx.egg-info/requires.txt
+-rw-r--r--   0 armin      (501) staff       (20)        6 2024-04-23 18:35:44.000000 sillm-mlx-0.1.3/sillm_mlx.egg-info/top_level.txt
```

### Comparing `sillm-mlx-0.1.2/LICENSE` & `sillm-mlx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/PKG-INFO` & `sillm-mlx-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sillm-mlx
-Version: 0.1.2
+Version: 0.1.3
 Summary: Running and training LLMs on Apple Silicon via MLX
 Home-page: https://github.com/armbues/SiLLM
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mlx==0.11.0
+Requires-Dist: mlx==0.11.1
 Requires-Dist: transformers>=4.39.3
 Requires-Dist: sentencepiece==0.2.0
 Requires-Dist: protobuf>=5.26.1
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: psutil
 Requires-Dist: pyyaml
@@ -48,15 +48,15 @@
 ```
 
 ## Usage
 
 ### Chat web application
 The web app uses [Chainlit](https://github.com/Chainlit/chainlit) to provide a frontend for conversational AI running locally on Apple Silicon hardware.
 
-https://github.com/armbues/SiLLM/assets/4117144/833d63ab-08b1-45ca-980f-474c7e9cc284
+https://github.com/armbues/SiLLM/assets/4117144/ab537795-5020-4241-aa89-3b19b9de263b
 
 To start the web app, clone the repository and start the app using chainlit:
 ``` sh
 git clone https://github.com/armbues/SiLLM.git
 cd SiLLM/app
 pip install -r requirements.txt
 python -m chainlit run app.py -w
@@ -115,36 +115,39 @@
 model = sillm.load("/path/to/model")
 for s, _ in model.generate("On a beautiful Sunday morning,"):
     print(s, flush=True, end="")
 ```
 
 ### Examples
 
-#### [LoRA Fine-tuning](examples/helpsteer/)
+The repository [SiLLM-examples](https://github.com/armbues/SiLLM-examples) contains Python code examples for using the SiLLM framework for training and running LLMs.
+
+#### LoRA Fine-tuning
 LoRA training [Mistral-7B-Instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) with the Nvidia [HelpSteer](https://huggingface.co/datasets/nvidia/HelpSteer) dataset.
 
-#### [DPO Fine-tuning](examples/dpo-mix-7k/)
+#### DPO Fine-tuning
 DPO training [Qwen1.5-7B-Chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat) with the [DPO Mix 7K](https://huggingface.co/datasets/argilla/dpo-mix-7k) dataset. The training consists of a supervised fine tuning (SFT) followed by direct preference optimization (DPO).
 
-#### [MMLU Benchmark](examples/mmlu/)
+#### MMLU Benchmark
 Implementation of the "Massive Multitask Language Understanding" benchmark using the [MMLU](https://huggingface.co/datasets/cais/mmlu) dataset.
 
-#### [Perplexity](examples/perplexity/)
+#### Perplexity
 Calculating perplexity scores for a sample [dataset](https://huggingface.co/datasets/Cohere/wikipedia-2023-11-embed-multilingual-v3) of entry paragraphs from Wikipedia articles.
 
 ## Model Support
 SiLLM generally supports loading LLMs of the following model architectures/families: *Llama 2*, *Mistral*, *Mixtral*, *Gemma*, *Phi*, *Qwen 2*, *StarCoder2*.
 
 Here is a list of models that were successfully tested with SiLLM:
 
 | Model Family | Models/Sizes (HF) | Models/Sizes (GGUF) | Models/Sizes (MLX) |
 | --- | --- | --- | --- |
-| Llama-2 | | [7b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF), [13b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-13B-chat-GGUF) | [7b](https://huggingface.co/mlx-community/Llama-2-7b-mlx), [7b-chat](https://huggingface.co/mlx-community/Llama-2-7b-chat-mlx) |
-| Mistral v0.2 | [7b-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | [7b-instruct-v0.2.Q8_0](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) | |
-| Mixtral v0.1 | | | [8x7B-Instruct](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1) |
+| Llama-3 | [8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct), [70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct/) | | |
+| Llama-2 | [7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf) | [7b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF), [13b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-13B-chat-GGUF) | [7b](https://huggingface.co/mlx-community/Llama-2-7b-mlx), [7b-chat](https://huggingface.co/mlx-community/Llama-2-7b-chat-mlx) |
+| Mistral | [7b-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | [7b-instruct-v0.2.Q8_0](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) | |
+| Mixtral | | | [8x7B-Instruct-v0.1 ](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1), [8x22B-Instruct-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-Instruct-v0.1) |
 | Gemma | [2b](https://huggingface.co/google/gemma-2b), [2b-it](https://huggingface.co/google/gemma-7b-it), [7b](https://huggingface.co/google/gemma-7b), [7b-it](https://huggingface.co/google/gemma-7b-it) | |
 | Phi-2 | [2.7b](https://huggingface.co/microsoft/phi-2) | |
 | Qwen 1.5 | [7b-chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat), [14b-chat](https://huggingface.co/Qwen/Qwen1.5-14B-Chat) | |
 | StarCoder2 | [3b](https://huggingface.co/bigcode/starcoder2-3b), [7b](https://huggingface.co/bigcode/starcoder2-7b), [15b](https://huggingface.co/bigcode/starcoder2-15b) | |
 | CodeLlama | | [70b-instruct.Q4_0](https://huggingface.co/TheBloke/CodeLlama-70B-Instruct-GGUF), [Phind-34b-v2.Q4_0](https://huggingface.co/TheBloke/Phind-CodeLlama-34B-v2-GGUF) | |
 | DBRX | (currently not supported) | | [dbrx-instruct-4bit](https://huggingface.co/mlx-community/dbrx-instruct-4bit) |
 | Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01), [Command-R+](CohereForAI/c4ai-command-r-plus) | |
```

### Comparing `sillm-mlx-0.1.2/README.md` & `sillm-mlx-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ```
 
 ## Usage
 
 ### Chat web application
 The web app uses [Chainlit](https://github.com/Chainlit/chainlit) to provide a frontend for conversational AI running locally on Apple Silicon hardware.
 
-https://github.com/armbues/SiLLM/assets/4117144/833d63ab-08b1-45ca-980f-474c7e9cc284
+https://github.com/armbues/SiLLM/assets/4117144/ab537795-5020-4241-aa89-3b19b9de263b
 
 To start the web app, clone the repository and start the app using chainlit:
 ``` sh
 git clone https://github.com/armbues/SiLLM.git
 cd SiLLM/app
 pip install -r requirements.txt
 python -m chainlit run app.py -w
@@ -92,36 +92,39 @@
 model = sillm.load("/path/to/model")
 for s, _ in model.generate("On a beautiful Sunday morning,"):
     print(s, flush=True, end="")
 ```
 
 ### Examples
 
-#### [LoRA Fine-tuning](examples/helpsteer/)
+The repository [SiLLM-examples](https://github.com/armbues/SiLLM-examples) contains Python code examples for using the SiLLM framework for training and running LLMs.
+
+#### LoRA Fine-tuning
 LoRA training [Mistral-7B-Instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) with the Nvidia [HelpSteer](https://huggingface.co/datasets/nvidia/HelpSteer) dataset.
 
-#### [DPO Fine-tuning](examples/dpo-mix-7k/)
+#### DPO Fine-tuning
 DPO training [Qwen1.5-7B-Chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat) with the [DPO Mix 7K](https://huggingface.co/datasets/argilla/dpo-mix-7k) dataset. The training consists of a supervised fine tuning (SFT) followed by direct preference optimization (DPO).
 
-#### [MMLU Benchmark](examples/mmlu/)
+#### MMLU Benchmark
 Implementation of the "Massive Multitask Language Understanding" benchmark using the [MMLU](https://huggingface.co/datasets/cais/mmlu) dataset.
 
-#### [Perplexity](examples/perplexity/)
+#### Perplexity
 Calculating perplexity scores for a sample [dataset](https://huggingface.co/datasets/Cohere/wikipedia-2023-11-embed-multilingual-v3) of entry paragraphs from Wikipedia articles.
 
 ## Model Support
 SiLLM generally supports loading LLMs of the following model architectures/families: *Llama 2*, *Mistral*, *Mixtral*, *Gemma*, *Phi*, *Qwen 2*, *StarCoder2*.
 
 Here is a list of models that were successfully tested with SiLLM:
 
 | Model Family | Models/Sizes (HF) | Models/Sizes (GGUF) | Models/Sizes (MLX) |
 | --- | --- | --- | --- |
-| Llama-2 | | [7b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF), [13b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-13B-chat-GGUF) | [7b](https://huggingface.co/mlx-community/Llama-2-7b-mlx), [7b-chat](https://huggingface.co/mlx-community/Llama-2-7b-chat-mlx) |
-| Mistral v0.2 | [7b-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | [7b-instruct-v0.2.Q8_0](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) | |
-| Mixtral v0.1 | | | [8x7B-Instruct](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1) |
+| Llama-3 | [8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct), [70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct/) | | |
+| Llama-2 | [7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf) | [7b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF), [13b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-13B-chat-GGUF) | [7b](https://huggingface.co/mlx-community/Llama-2-7b-mlx), [7b-chat](https://huggingface.co/mlx-community/Llama-2-7b-chat-mlx) |
+| Mistral | [7b-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | [7b-instruct-v0.2.Q8_0](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) | |
+| Mixtral | | | [8x7B-Instruct-v0.1 ](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1), [8x22B-Instruct-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-Instruct-v0.1) |
 | Gemma | [2b](https://huggingface.co/google/gemma-2b), [2b-it](https://huggingface.co/google/gemma-7b-it), [7b](https://huggingface.co/google/gemma-7b), [7b-it](https://huggingface.co/google/gemma-7b-it) | |
 | Phi-2 | [2.7b](https://huggingface.co/microsoft/phi-2) | |
 | Qwen 1.5 | [7b-chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat), [14b-chat](https://huggingface.co/Qwen/Qwen1.5-14B-Chat) | |
 | StarCoder2 | [3b](https://huggingface.co/bigcode/starcoder2-3b), [7b](https://huggingface.co/bigcode/starcoder2-7b), [15b](https://huggingface.co/bigcode/starcoder2-15b) | |
 | CodeLlama | | [70b-instruct.Q4_0](https://huggingface.co/TheBloke/CodeLlama-70B-Instruct-GGUF), [Phind-34b-v2.Q4_0](https://huggingface.co/TheBloke/Phind-CodeLlama-34B-v2-GGUF) | |
 | DBRX | (currently not supported) | | [dbrx-instruct-4bit](https://huggingface.co/mlx-community/dbrx-instruct-4bit) |
 | Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01), [Command-R+](CohereForAI/c4ai-command-r-plus) | |
```

### Comparing `sillm-mlx-0.1.2/setup.py` & `sillm-mlx-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pkg_dir = pathlib.Path(__file__).parent.resolve()
 readme = (pkg_dir / "README.md").read_text(encoding="utf-8")
 requirements = (pkg_dir / "requirements.txt").read_text(encoding="utf-8").splitlines()
 requirements_server = (pkg_dir / "requirements-server.txt").read_text(encoding="utf-8").splitlines()
 
 setup(
     name = "sillm-mlx",
-    version = "0.1.2",
+    version = "0.1.3",
     description = "Running and training LLMs on Apple Silicon via MLX",
     long_description = readme,
     long_description_content_type = "text/markdown",
     readme="README.md",
     url = "https://github.com/armbues/SiLLM",
     install_requires=requirements,
     extras_require={
```

### Comparing `sillm-mlx-0.1.2/sillm/__init__.py` & `sillm-mlx-0.1.3/sillm/__init__.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/chat.py` & `sillm-mlx-0.1.3/sillm/chat.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/convert.py` & `sillm-mlx-0.1.3/sillm/convert.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/core/conversation.py` & `sillm-mlx-0.1.3/sillm/core/conversation.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/core/llm.py` & `sillm-mlx-0.1.3/sillm/core/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 model_map = {
     "llama":        models.llama.Model,
     "mistral":      models.llama.Model,
     "gemma":        models.gemma.Model,
     "mixtral":      models.mixtral.Model,   
     "phi":          models.phi.Model,
+    "phi3":         models.phi3.Model,
     "starcoder2":   models.starcoder2.Model,
     "qwen2":        models.qwen2.Model,
     "dbrx":         models.dbrx.Model,
     "cohere":       models.cohere.Model,
 }
 
 class LLM():
@@ -290,16 +291,24 @@
                     output_dims, input_dims = weight.shape
                     linear = nn.Linear(input_dims, output_dims, bias=bias)
                     linear.weight = weight
                     if bias:
                         linear.bias = module.bias
 
                     layers.append((name, linear))
+                elif isinstance(module, nn.QuantizedEmbedding):
+                    weight = mx.dequantize(module.weight, module.scales, module.biases, module.group_size, module.bits).astype(mx.float16)
+                    num_embeddings, dims = weight.shape
+                    embedding = nn.Embedding(num_embeddings, dims)
+                    embedding.weight = weight
+                    layers.append((name, embedding))
             
-            self.model.update_modules(tree_unflatten(layers))
+            if len(layers) > 0:
+                self.model.update_modules(tree_unflatten(layers))
+
             self._quantization = None
             self.args.quantization = None
 
             logger.info(f"Dequantized model")
 
     def perplexity(self,
                    dataset: Dataset,
@@ -382,19 +391,39 @@
     metadata = {
         "timing": timing,
         "usage": usage,
         "logprobs": [],
         "finish_reason": "length"
     }
 
+    def sample(logits):
+        if temperature > 0:
+            return mx.random.categorical(logits * (1 / temperature))
+        else:
+            return mx.argmax(logits, axis=-1)
+        # TODO add top-p sampling
+
+    def generate_step(model, inputs):
+        y = inputs
+        cache = None
+        while True:
+            logits, cache = model(y[None], cache=cache)
+            logits = logits[:, -1, :]
+            y = sample(logits)
+
+            p = 0.0
+            if logprobs:
+                p = nn.log_softmax(logits, axis=-1)[0,y].item()
+            
+            yield y, p
+
     tokens, text, buffer, prefix = [], "", [], ""
-    for (token,p) , i in zip(generate_step(model, inputs, temperature, logprobs), range(max_tokens)):
+    for (token,p), i in zip(generate_step(model, inputs), range(max_tokens)):
         if i == 0:
             mx.eval(token)
-
             timing["eval_time"] = time.perf_counter() - start
 
         if token.item() in stop_tokens:
             metadata["finish_reason"] = "stop"
             break
 
         tokens.append(token.item())
@@ -417,45 +446,22 @@
 
             timing["runtime"] = time.perf_counter() - start
             usage["completion_tokens"] = i+1
             usage["total_tokens"] = usage["prompt_tokens"] + usage["completion_tokens"]
 
             yield text, metadata
 
-    mx.eval(tokens)
-    
     text = tokenizer.decode(tokens)
     window = tokenizer.decode(buffer + tokens)
     if prefix + " " + text == window:
         prefix = text
         text = " " + text
     else:
         prefix = text
     buffer = tokens
     tokens = []
 
     timing["runtime"] = time.perf_counter() - start
     usage["completion_tokens"] = i+1
     usage["total_tokens"] = usage["prompt_tokens"] + usage["completion_tokens"]
 
-    yield text, metadata
-
-def generate_step(model, inputs, temperature, logprobs=False):
-    y = inputs
-    cache = None
-    while True:
-        logits, cache = model(y[None], cache=cache)
-        logits = logits[:, -1, :]
-        y = sample(logits, temperature)
-
-        p = 0.0
-        if logprobs:
-            p = nn.log_softmax(logits, axis=-1)[0,y].item()
-        
-        yield y, p
-
-def sample(logits, temperature):
-    if temperature > 0:
-        return mx.random.categorical(logits * (1 / temperature))
-    else:
-        return mx.argmax(logits, axis=-1)
-    # TODO add top-p sampling
+    yield text, metadata
```

### Comparing `sillm-mlx-0.1.2/sillm/core/loader.py` & `sillm-mlx-0.1.3/sillm/core/loader.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/core/template.py` & `sillm-mlx-0.1.3/sillm/core/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "mistral": "mistral",
     "gemma": "gemma",
     "mixtral": "mistral",
     "phi": "phi2",
     "qwen2": "qwen2",
     "dbrx": "chatml",
     "cohere": "cohere",
+    "phi3": "phi3",
 }
 
 class Template(object):
     def __init__(self,
                  tokenizer,
                  template_name: str = "chatml",
                  exception_callback = None
```

### Comparing `sillm-mlx-0.1.2/sillm/core/tokenizer.py` & `sillm-mlx-0.1.3/sillm/core/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         """
         Special tokens map.
         """
         special_tokens_map = {
             "bos_token": self._model.id_to_piece(self.bos_id),
             "eos_token": self._model.id_to_piece(self.eos_id),
         }
-        
+
         return special_tokens_map
     
     def save(self,
             tokenizer_path: str
             ):
         tokenizer_path = pathlib.Path(tokenizer_path) / "tokenizer.model"
 
@@ -183,14 +183,17 @@
             self.pad_id = args.pad_token_id
 
         self.special_ids = set([self.bos_id, self.eos_id] + self._model.all_special_ids)
 
         # Hack for Llama-3
         if "<|eot_id|>" in self._model.vocab:
             self.special_ids.add(self._model.vocab["<|eot_id|>"])
+        # Hack for Phi-3
+        if "<|end|>" in self._model.vocab:
+            self.special_ids.add(self._model.vocab["<|end|>"])
 
     def encode(self,
                s: str,
                bos: bool = True,
                eos: bool = False
                ) -> List[int]:
         """
```

### Comparing `sillm-mlx-0.1.2/sillm/dpo.py` & `sillm-mlx-0.1.3/sillm/dpo.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/lora.py` & `sillm-mlx-0.1.3/sillm/lora.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     # Initialize plot
     if args.plot is not None:
         plot = utils.Plot()
 
     # Set conversation template
     if args.template:
-        template = sillm.Template(model.tokenizer, template=args.template)
+        template = sillm.Template(model.tokenizer, template_name=args.template)
     else:
         template = None
 
     # Log memory usage
     utils.log_memory_usage()
 
     if args.train is not None:
```

### Comparing `sillm-mlx-0.1.2/sillm/models/args.py` & `sillm-mlx-0.1.3/sillm/models/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
                 ArgsClass = Qwen2Args
             elif config["model_type"] == "starcoder2":
                 ArgsClass = Starcoder2Args
             elif config["model_type"] == "dbrx":
                 ArgsClass = DbrxArgs
             elif config["model_type"] == "cohere":
                 ArgsClass = CohereArgs
+            elif config["model_type"] == "phi3":
+                ArgsClass = Phi3Args
             else:
                 ArgsClass = LlamaArgs
         if ArgsClass is None:
             ArgsClass = LlamaArgs
             config["model_type"] = "llama"
             logger.warn(f"No model type specified - falling back to `llama` config")
 
@@ -186,8 +188,15 @@
 @dataclasses.dataclass
 class CohereArgs(ModelArgs):
     """
     Cohere model arguments.
     """
     norm_bias: bool = False
     logit_scale: float = 0.0625
-    use_qk_norm: bool = False
+    use_qk_norm: bool = False
+
+@dataclasses.dataclass
+class Phi3Args(ModelArgs):
+    """
+    Phi-3 model arguments.
+    """
+    embd_pdrop: float = 0.0
```

### Comparing `sillm-mlx-0.1.2/sillm/models/base.py` & `sillm-mlx-0.1.3/sillm/models/base.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/cohere.py` & `sillm-mlx-0.1.3/sillm/models/cohere.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/dbrx.py` & `sillm-mlx-0.1.3/sillm/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/gemma.py` & `sillm-mlx-0.1.3/sillm/models/gemma.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/llama.py` & `sillm-mlx-0.1.3/sillm/models/llama.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/mixtral.py` & `sillm-mlx-0.1.3/sillm/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/phi.py` & `sillm-mlx-0.1.3/sillm/models/phi.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """
     def __init__(self, args: ModelArgs):
         """
         Args:
             args: Model arguments.
         """
         nn.Module.__init__(self)
+        
         self.args = args
 
         self.n_heads: int = args.n_heads
         self.n_kv_heads: int = args.n_kv_heads
 
         self.repeats = self.n_heads // self.n_kv_heads
         self.scale = self.args.head_dim ** -0.5
@@ -104,15 +105,16 @@
     Transformer block.
     """
     def __init__(self, args: ModelArgs):
         """
         Args:
             args: Model arguments.
         """
-        nn.Module.__init__(self)
+        super().__init__()
+
         self.args = args
 
         self.n_heads = args.n_heads
         self.dim = args.dim
 
         self.attention = Attention(args=args)
         self.attention_norm = nn.LayerNorm(args.dim, eps=args.norm_eps)
```

### Comparing `sillm-mlx-0.1.2/sillm/models/qwen2.py` & `sillm-mlx-0.1.3/sillm/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/models/starcoder2.py` & `sillm-mlx-0.1.3/sillm/models/starcoder2.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/quantize.py` & `sillm-mlx-0.1.3/sillm/quantize.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sillm.core.tokenizer import TransformerTokenizer, SentencePieceTokenizer
 
 if __name__ == "__main__":
     # Parse commandline arguments
     parser = argparse.ArgumentParser(description="A simple CLI for generating text with SiLLM.")
     parser.add_argument("input", type=str, help="The input model directory or file")
     parser.add_argument("output", type=str, help="The output model directory or file")
-    parser.add_argument("--bits", default=4, help="Quantization bits")
+    parser.add_argument("--bits", type=int, default=4, help="Quantization bits")
     parser.add_argument("--group_size", default=32, help="Quantization group size")
     parser.add_argument("-v", "--verbose", default=1, action="count", help="Increase output verbosity")
     args = parser.parse_args()
 
     # Initialize logging
     log_level = 40 - (10 * args.verbose) if args.verbose > 0 else 0
     logger = utils.init_logger(log_level)
```

### Comparing `sillm-mlx-0.1.2/sillm/server.py` & `sillm-mlx-0.1.3/sillm/server.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/templates/alpaca.jinja` & `sillm-mlx-0.1.3/sillm/templates/alpaca.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{{ system_message }}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ '### Instruction:\n' + message['content'].strip() + '\n\n' }}{% elif message['role'] == 'assistant' %}{{ '### Response:\n' + message['content'].strip() + '</s>\n\n' }}{% endif %}{% if loop.last and message['role'] == 'user' and add_generation_prompt %}{{ '### Instruction:\n' }}{% endif %}{% endfor %}
+{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{{ system_message }}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ '### Instruction:\n' + message['content'].strip() + '\n\n' }}{% elif message['role'] == 'assistant' %}{{ '### Response:\n' + message['content'].strip() + '\n\n' }}{% endif %}{% if loop.last and message['role'] == 'user' and add_generation_prompt %}{{ '### Instruction:\n' }}{% endif %}{% endfor %}
```

### Comparing `sillm-mlx-0.1.2/sillm/templates/cohere.jinja` & `sillm-mlx-0.1.3/sillm/templates/cohere.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/templates/gemma.jinja` & `sillm-mlx-0.1.3/sillm/templates/gemma.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/templates/llama2.jinja` & `sillm-mlx-0.1.3/sillm/templates/llama2.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/templates/vicuna.jinja` & `sillm-mlx-0.1.3/sillm/templates/vicuna.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/training/dataset.py` & `sillm-mlx-0.1.3/sillm/training/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                     batch_arr[j, : lengths[j]] = batch[j]
                 batch = mx.array(batch_arr)
 
                 inputs = batch[:, :-1]
                 targets = batch[:, 1:]
 
                 lengths = mx.array(lengths)
-                loss_masks = mx.arange(inputs.shape[1])[None, :] < lengths[:, None]
+                loss_masks = mx.arange(inputs.shape[1])[None, :] < lengths[:, None] - 1
 
                 yield inputs, targets, loss_masks
 
             if not train:
                 break
     
 class DatasetMessages(Dataset):
@@ -188,16 +188,16 @@
 
                 inputs = batch[:, :-1]
                 targets = batch[:, 1:]
 
                 lengths = mx.array(lengths)
                 prompt_lengths = mx.array([len(x) for x in prompts])
                 loss_masks = mx.logical_and(
-                    mx.arange(inputs.shape[1])[None, :] < lengths[:, None],
-                    mx.arange(inputs.shape[1])[None, :] > prompt_lengths[:, None]
+                    mx.arange(inputs.shape[1])[None, :] >= prompt_lengths[:, None],
+                    mx.arange(inputs.shape[1])[None, :] < lengths[:, None] - 1
                 )
 
                 yield inputs, targets, loss_masks
 
             if not train:
                 break
 
@@ -347,20 +347,20 @@
                     rejected[j, : rejected_lengths[j]] = batch[j][2]
 
                 # Mask prompt and padding tokens
                 chosen_lengths = mx.array(chosen_lengths)
                 rejected_lengths = mx.array(rejected_lengths)
                 prompt_lengths = mx.array([len(x[0]) for x in batch])
                 chosen_masks = mx.logical_and(
-                    mx.arange(chosen.shape[1] - 1)[None, :] < chosen_lengths[:, None],
-                    mx.arange(chosen.shape[1] - 1)[None, :] > prompt_lengths[:, None]
+                    mx.arange(chosen.shape[1] - 1)[None, :] < chosen_lengths[:, None] - 1,
+                    mx.arange(chosen.shape[1] - 1)[None, :] >= prompt_lengths[:, None]
                 )
                 rejected_masks = mx.logical_and(
-                    mx.arange(rejected.shape[1] - 1)[None, :] < rejected_lengths[:, None],
-                    mx.arange(rejected.shape[1] - 1)[None, :] > prompt_lengths[:, None]
+                    mx.arange(rejected.shape[1] - 1)[None, :] < rejected_lengths[:, None] - 1,
+                    mx.arange(rejected.shape[1] - 1)[None, :] >= prompt_lengths[:, None]
                 )
                 
                 yield mx.array(chosen), mx.array(rejected), chosen_masks, rejected_masks
 
             if not train:
                 break
```

### Comparing `sillm-mlx-0.1.2/sillm/training/dpo.py` & `sillm-mlx-0.1.3/sillm/training/dpo.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/training/lora.py` & `sillm-mlx-0.1.3/sillm/training/lora.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         output_dims, input_dims = linear.weight.shape
         if isinstance(linear, nn.QuantizedLinear):
             input_dims *= 32 // linear.bits
         bias = "bias" in linear
 
         lora_lin = LoRALinear(input_dims, output_dims, rank, alpha, dropout, scale, bias)
         lora_lin.linear = linear
-        lora_lin.name = linear.name
 
         return lora_lin
 
     def __init__(self,
                  input_dims: int,
                  output_dims: int,
                  rank: int = 8,
```

### Comparing `sillm-mlx-0.1.2/sillm/utils/log.py` & `sillm-mlx-0.1.3/sillm/utils/log.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm/utils/mapping.py` & `sillm-mlx-0.1.3/sillm/utils/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,18 @@
         k = re.sub(r"\.mlp\.fc1\.", ".feed_forward.w1.", k)
         k = re.sub(r"\.mlp\.fc2\.", ".feed_forward.w2.", k)
 
         # Starcoder2 mapping
         k = re.sub(r"\.mlp\.c_fc\.", ".feed_forward.w1.", k)
         k = re.sub(r"\.mlp\.c_proj\.", ".feed_forward.w2.", k)
 
+        # Phi-3 mapping
+        k = re.sub(r"\.mlp\.gate_up_proj\.", ".feed_forward.w1.", k)
+        k = re.sub(r"\.self_attn\.qkv_proj\.", r".attention.wqkv.", k)
+
         return k
     # GGUF keys
     elif k.startswith("output_norm."):
         return re.sub(r"^output_norm\.", "norm.", k)
     elif k.startswith("token_embd."):
         return re.sub(r"^token_embd\.", "tok_embeddings.", k)
     elif k.startswith("blk."):
```

### Comparing `sillm-mlx-0.1.2/sillm/utils/plot.py` & `sillm-mlx-0.1.3/sillm/utils/plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         """
         Save the plot to a file.
         Args:
             fpath: File path
         """
         self.plot()
         plt.savefig(fpath)
+        plt.close()
 
     def show(self):
         """
         Show the plot.
         """
         self.plot()
-        plt.show()
+        plt.show()
+        plt.close()
```

### Comparing `sillm-mlx-0.1.2/sillm/utils/quantization.py` & `sillm-mlx-0.1.3/sillm/utils/quantization.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.2/sillm_mlx.egg-info/PKG-INFO` & `sillm-mlx-0.1.3/sillm_mlx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sillm-mlx
-Version: 0.1.2
+Version: 0.1.3
 Summary: Running and training LLMs on Apple Silicon via MLX
 Home-page: https://github.com/armbues/SiLLM
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mlx==0.11.0
+Requires-Dist: mlx==0.11.1
 Requires-Dist: transformers>=4.39.3
 Requires-Dist: sentencepiece==0.2.0
 Requires-Dist: protobuf>=5.26.1
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: psutil
 Requires-Dist: pyyaml
@@ -48,15 +48,15 @@
 ```
 
 ## Usage
 
 ### Chat web application
 The web app uses [Chainlit](https://github.com/Chainlit/chainlit) to provide a frontend for conversational AI running locally on Apple Silicon hardware.
 
-https://github.com/armbues/SiLLM/assets/4117144/833d63ab-08b1-45ca-980f-474c7e9cc284
+https://github.com/armbues/SiLLM/assets/4117144/ab537795-5020-4241-aa89-3b19b9de263b
 
 To start the web app, clone the repository and start the app using chainlit:
 ``` sh
 git clone https://github.com/armbues/SiLLM.git
 cd SiLLM/app
 pip install -r requirements.txt
 python -m chainlit run app.py -w
@@ -115,36 +115,39 @@
 model = sillm.load("/path/to/model")
 for s, _ in model.generate("On a beautiful Sunday morning,"):
     print(s, flush=True, end="")
 ```
 
 ### Examples
 
-#### [LoRA Fine-tuning](examples/helpsteer/)
+The repository [SiLLM-examples](https://github.com/armbues/SiLLM-examples) contains Python code examples for using the SiLLM framework for training and running LLMs.
+
+#### LoRA Fine-tuning
 LoRA training [Mistral-7B-Instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) with the Nvidia [HelpSteer](https://huggingface.co/datasets/nvidia/HelpSteer) dataset.
 
-#### [DPO Fine-tuning](examples/dpo-mix-7k/)
+#### DPO Fine-tuning
 DPO training [Qwen1.5-7B-Chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat) with the [DPO Mix 7K](https://huggingface.co/datasets/argilla/dpo-mix-7k) dataset. The training consists of a supervised fine tuning (SFT) followed by direct preference optimization (DPO).
 
-#### [MMLU Benchmark](examples/mmlu/)
+#### MMLU Benchmark
 Implementation of the "Massive Multitask Language Understanding" benchmark using the [MMLU](https://huggingface.co/datasets/cais/mmlu) dataset.
 
-#### [Perplexity](examples/perplexity/)
+#### Perplexity
 Calculating perplexity scores for a sample [dataset](https://huggingface.co/datasets/Cohere/wikipedia-2023-11-embed-multilingual-v3) of entry paragraphs from Wikipedia articles.
 
 ## Model Support
 SiLLM generally supports loading LLMs of the following model architectures/families: *Llama 2*, *Mistral*, *Mixtral*, *Gemma*, *Phi*, *Qwen 2*, *StarCoder2*.
 
 Here is a list of models that were successfully tested with SiLLM:
 
 | Model Family | Models/Sizes (HF) | Models/Sizes (GGUF) | Models/Sizes (MLX) |
 | --- | --- | --- | --- |
-| Llama-2 | | [7b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF), [13b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-13B-chat-GGUF) | [7b](https://huggingface.co/mlx-community/Llama-2-7b-mlx), [7b-chat](https://huggingface.co/mlx-community/Llama-2-7b-chat-mlx) |
-| Mistral v0.2 | [7b-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | [7b-instruct-v0.2.Q8_0](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) | |
-| Mixtral v0.1 | | | [8x7B-Instruct](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1) |
+| Llama-3 | [8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct), [70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct/) | | |
+| Llama-2 | [7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf) | [7b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF), [13b-chat.Q8_0](https://huggingface.co/TheBloke/Llama-2-13B-chat-GGUF) | [7b](https://huggingface.co/mlx-community/Llama-2-7b-mlx), [7b-chat](https://huggingface.co/mlx-community/Llama-2-7b-chat-mlx) |
+| Mistral | [7b-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | [7b-instruct-v0.2.Q8_0](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) | |
+| Mixtral | | | [8x7B-Instruct-v0.1 ](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1), [8x22B-Instruct-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-Instruct-v0.1) |
 | Gemma | [2b](https://huggingface.co/google/gemma-2b), [2b-it](https://huggingface.co/google/gemma-7b-it), [7b](https://huggingface.co/google/gemma-7b), [7b-it](https://huggingface.co/google/gemma-7b-it) | |
 | Phi-2 | [2.7b](https://huggingface.co/microsoft/phi-2) | |
 | Qwen 1.5 | [7b-chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat), [14b-chat](https://huggingface.co/Qwen/Qwen1.5-14B-Chat) | |
 | StarCoder2 | [3b](https://huggingface.co/bigcode/starcoder2-3b), [7b](https://huggingface.co/bigcode/starcoder2-7b), [15b](https://huggingface.co/bigcode/starcoder2-15b) | |
 | CodeLlama | | [70b-instruct.Q4_0](https://huggingface.co/TheBloke/CodeLlama-70B-Instruct-GGUF), [Phind-34b-v2.Q4_0](https://huggingface.co/TheBloke/Phind-CodeLlama-34B-v2-GGUF) | |
 | DBRX | (currently not supported) | | [dbrx-instruct-4bit](https://huggingface.co/mlx-community/dbrx-instruct-4bit) |
 | Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01), [Command-R+](CohereForAI/c4ai-command-r-plus) | |
```

### Comparing `sillm-mlx-0.1.2/sillm_mlx.egg-info/SOURCES.txt` & `sillm-mlx-0.1.3/sillm_mlx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,28 @@
 sillm/models/base.py
 sillm/models/cohere.py
 sillm/models/dbrx.py
 sillm/models/gemma.py
 sillm/models/llama.py
 sillm/models/mixtral.py
 sillm/models/phi.py
+sillm/models/phi3.py
 sillm/models/qwen2.py
 sillm/models/starcoder2.py
 sillm/templates/alpaca.jinja
 sillm/templates/chatml.jinja
 sillm/templates/cohere.jinja
 sillm/templates/empty.jinja
 sillm/templates/gemma.jinja
 sillm/templates/llama2.jinja
 sillm/templates/llama3.jinja
 sillm/templates/mistral.jinja
 sillm/templates/openchat.jinja
 sillm/templates/phi2.jinja
+sillm/templates/phi3.jinja
 sillm/templates/qwen2.jinja
 sillm/templates/vicuna.jinja
 sillm/training/__init__.py
 sillm/training/dataset.py
 sillm/training/dpo.py
 sillm/training/lora.py
 sillm/utils/__init__.py
```

