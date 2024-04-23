# Comparing `tmp/python-aiconfig-1.1.8.tar.gz` & `tmp/python-aiconfig-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aiconfig-1.1.8.tar", last modified: Tue Dec 26 22:28:21 2023, max compression
+gzip compressed data, was "python-aiconfig-1.1.9.tar", last modified: Mon Jan  8 17:51:53 2024, max compression
```

## Comparing `python-aiconfig-1.1.8.tar` & `python-aiconfig-1.1.9.tar`

### file list

```diff
@@ -1,86 +1,92 @@
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.683895 python-aiconfig-1.1.8/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     1060 2023-12-01 00:43:09.000000 python-aiconfig-1.1.8/LICENSE
--rw-r--r--   0 rossdancraig   (501) staff       (20)       53 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/MANIFEST.in
--rw-r--r--   0 rossdancraig   (501) staff       (20)    24665 2023-12-26 22:28:21.683650 python-aiconfig-1.1.8/PKG-INFO
--rw-r--r--   0 rossdancraig   (501) staff       (20)    23607 2023-12-01 19:28:27.000000 python-aiconfig-1.1.8/README.md
--rw-r--r--   0 rossdancraig   (501) staff       (20)      905 2023-12-26 22:23:27.000000 python-aiconfig-1.1.8/pyproject.toml
--rw-r--r--   0 rossdancraig   (501) staff       (20)      279 2023-12-26 05:00:38.000000 python-aiconfig-1.1.8/requirements.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       38 2023-12-26 22:28:21.683932 python-aiconfig-1.1.8/setup.cfg
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.673081 python-aiconfig-1.1.8/src/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.675212 python-aiconfig-1.1.8/src/aiconfig/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     8554 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/ChatCompletion.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    17689 2023-12-26 04:43:24.000000 python-aiconfig-1.1.8/src/aiconfig/Config.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)      909 2023-11-28 20:37:07.000000 python-aiconfig-1.1.8/src/aiconfig/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     3763 2023-11-28 20:37:07.000000 python-aiconfig-1.1.8/src/aiconfig/callback.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.676504 python-aiconfig-1.1.8/src/aiconfig/default_parsers/
--rw-r--r--   0 rossdancraig   (501) staff       (20)        0 2023-11-16 17:04:29.000000 python-aiconfig-1.1.8/src/aiconfig/default_parsers/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     6895 2023-12-26 21:30:44.000000 python-aiconfig-1.1.8/src/aiconfig/default_parsers/dalle.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    10295 2023-12-26 21:30:44.000000 python-aiconfig-1.1.8/src/aiconfig/default_parsers/hf.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    18724 2023-12-26 22:15:01.000000 python-aiconfig-1.1.8/src/aiconfig/default_parsers/openai.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    13782 2023-12-26 22:15:01.000000 python-aiconfig-1.1.8/src/aiconfig/default_parsers/palm.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     5009 2023-11-29 05:38:04.000000 python-aiconfig-1.1.8/src/aiconfig/default_parsers/parameterized_model_parser.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.676782 python-aiconfig-1.1.8/src/aiconfig/editor/
--rw-r--r--   0 rossdancraig   (501) staff       (20)        0 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/__init__.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.676948 python-aiconfig-1.1.8/src/aiconfig/editor/client/
--rw-r--r--   0 rossdancraig   (501) staff       (20)        0 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/client/__init__.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.672126 python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.672185 python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/flatted/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.677249 python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/flatted/python/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     3879 2023-11-22 15:49:03.000000 python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     2129 2023-11-22 15:49:03.000000 python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/flatted/python/test.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)      760 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/example_aiconfig_model_registry.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.677651 python-aiconfig-1.1.8/src/aiconfig/editor/server/
--rw-r--r--   0 rossdancraig   (501) staff       (20)        0 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     7871 2023-12-26 20:13:07.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/server.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    12241 2023-12-26 20:13:07.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/server_utils.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.678249 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.678391 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/__pycache__/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      199 2023-12-22 00:03:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rossdancraig   (501) staff       (20)      366 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/asset-manifest.json
--rw-r--r--   0 rossdancraig   (501) staff       (20)      590 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/index.html
--rw-r--r--   0 rossdancraig   (501) staff       (20)      189 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/manifest.json
--rw-r--r--   0 rossdancraig   (501) staff       (20)       67 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/robots.txt
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.672704 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.678834 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/__pycache__/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      206 2023-12-22 00:03:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.679845 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     4512 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js
--rw-r--r--   0 rossdancraig   (501) staff       (20)    10597 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js.map
--rw-r--r--   0 rossdancraig   (501) staff       (20)   143442 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/main.612f69d0.js
--rw-r--r--   0 rossdancraig   (501) staff       (20)      971 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.LICENSE.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)   367448 2023-12-22 01:16:44.000000 python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.map
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.680700 python-aiconfig-1.1.8/src/aiconfig/eval/
--rw-r--r--   0 rossdancraig   (501) staff       (20)       13 2023-12-18 22:00:04.000000 python-aiconfig-1.1.8/src/aiconfig/eval/__init__.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.680820 python-aiconfig-1.1.8/src/aiconfig/eval/api/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      630 2023-12-19 21:39:11.000000 python-aiconfig-1.1.8/src/aiconfig/eval/api/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     6700 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/eval/common.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    11291 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/eval/lib.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    11797 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/eval/metrics.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     3152 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/eval/openai.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     9956 2023-12-21 20:10:47.000000 python-aiconfig-1.1.8/src/aiconfig/model_parser.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     5074 2023-12-01 00:35:47.000000 python-aiconfig-1.1.8/src/aiconfig/registry.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    28983 2023-12-26 21:30:44.000000 python-aiconfig-1.1.8/src/aiconfig/schema.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.681049 python-aiconfig-1.1.8/src/aiconfig/scripts/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     3760 2023-12-26 20:13:07.000000 python-aiconfig-1.1.8/src/aiconfig/scripts/aiconfig_cli.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     1506 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/src/aiconfig/scripts/run_aiconfig.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.681361 python-aiconfig-1.1.8/src/aiconfig/util/
--rw-r--r--   0 rossdancraig   (501) staff       (20)        0 2023-11-16 17:04:29.000000 python-aiconfig-1.1.8/src/aiconfig/util/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     1784 2023-12-24 03:51:28.000000 python-aiconfig-1.1.8/src/aiconfig/util/config_utils.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    11318 2023-12-19 21:39:26.000000 python-aiconfig-1.1.8/src/aiconfig/util/params.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.683348 python-aiconfig-1.1.8/src/python_aiconfig.egg-info/
--rw-r--r--   0 rossdancraig   (501) staff       (20)    24665 2023-12-26 22:28:21.000000 python-aiconfig-1.1.8/src/python_aiconfig.egg-info/PKG-INFO
--rw-r--r--   0 rossdancraig   (501) staff       (20)     2395 2023-12-26 22:28:21.000000 python-aiconfig-1.1.8/src/python_aiconfig.egg-info/SOURCES.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)        1 2023-12-26 22:28:21.000000 python-aiconfig-1.1.8/src/python_aiconfig.egg-info/dependency_links.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)      260 2023-12-26 22:28:21.000000 python-aiconfig-1.1.8/src/python_aiconfig.egg-info/requires.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)        9 2023-12-26 22:28:21.000000 python-aiconfig-1.1.8/src/python_aiconfig.egg-info/top_level.txt
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2023-12-26 22:28:21.683162 python-aiconfig-1.1.8/tests/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      614 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/tests/test_chatcompletion_mock_wrapper.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)      902 2023-11-28 20:37:07.000000 python-aiconfig-1.1.8/tests/test_dataclass.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     9517 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/tests/test_eval.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     4287 2023-12-20 19:19:58.000000 python-aiconfig-1.1.8/tests/test_eval_model_graded_openai.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     2428 2023-11-29 05:38:04.000000 python-aiconfig-1.1.8/tests/test_library_helpers.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     4506 2023-11-29 05:38:04.000000 python-aiconfig-1.1.8/tests/test_load_config.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    21058 2023-12-19 19:21:43.000000 python-aiconfig-1.1.8/tests/test_programmatically_create_an_AIConfig.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     5760 2023-11-29 22:38:36.000000 python-aiconfig-1.1.8/tests/test_registry.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)      944 2023-11-29 05:38:04.000000 python-aiconfig-1.1.8/tests/test_resolve.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     3732 2023-11-29 05:38:04.000000 python-aiconfig-1.1.8/tests/test_run_config.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.634981 python-aiconfig-1.1.9/
+-rw-r--r--   0 saqadri    (501) staff       (20)     1060 2023-12-09 08:36:12.000000 python-aiconfig-1.1.9/LICENSE
+-rw-r--r--   0 saqadri    (501) staff       (20)       53 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/MANIFEST.in
+-rw-r--r--   0 saqadri    (501) staff       (20)    24665 2024-01-08 17:51:53.634741 python-aiconfig-1.1.9/PKG-INFO
+-rw-r--r--   0 saqadri    (501) staff       (20)    23607 2023-12-09 08:36:12.000000 python-aiconfig-1.1.9/README.md
+-rw-r--r--   0 saqadri    (501) staff       (20)      972 2024-01-08 17:46:54.000000 python-aiconfig-1.1.9/pyproject.toml
+-rw-r--r--   0 saqadri    (501) staff       (20)      279 2023-12-28 22:15:56.000000 python-aiconfig-1.1.9/requirements.txt
+-rw-r--r--   0 saqadri    (501) staff       (20)       38 2024-01-08 17:51:53.635021 python-aiconfig-1.1.9/setup.cfg
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.619220 python-aiconfig-1.1.9/src/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.622429 python-aiconfig-1.1.9/src/aiconfig/
+-rw-r--r--   0 saqadri    (501) staff       (20)     8373 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/src/aiconfig/ChatCompletion.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    17842 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/src/aiconfig/Config.py
+-rw-r--r--   0 saqadri    (501) staff       (20)      934 2023-12-28 22:15:56.000000 python-aiconfig-1.1.9/src/aiconfig/__init__.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     3694 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/src/aiconfig/callback.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.623361 python-aiconfig-1.1.9/src/aiconfig/default_parsers/
+-rw-r--r--   0 saqadri    (501) staff       (20)        0 2023-10-17 16:38:21.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/__init__.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    10951 2024-01-05 19:02:46.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/anyscale_endpoint.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     7252 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/dalle.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    11163 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/hf.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    23698 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/openai.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    14537 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/palm.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     4906 2024-01-04 21:04:55.000000 python-aiconfig-1.1.9/src/aiconfig/default_parsers/parameterized_model_parser.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.623575 python-aiconfig-1.1.9/src/aiconfig/editor/
+-rw-r--r--   0 saqadri    (501) staff       (20)        0 2023-12-23 21:12:22.000000 python-aiconfig-1.1.9/src/aiconfig/editor/__init__.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.623682 python-aiconfig-1.1.9/src/aiconfig/editor/client/
+-rw-r--r--   0 saqadri    (501) staff       (20)        0 2023-12-23 21:12:22.000000 python-aiconfig-1.1.9/src/aiconfig/editor/client/__init__.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.618468 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.618311 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.618357 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.618406 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.623924 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/
+-rw-r--r--   0 saqadri    (501) staff       (20)     3879 2023-10-11 15:58:26.000000 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     2129 2023-10-11 15:58:26.000000 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/test.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.618510 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/flatted/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.625344 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/flatted/python/
+-rw-r--r--   0 saqadri    (501) staff       (20)     3879 2023-10-14 15:45:38.000000 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     2129 2023-10-14 15:45:38.000000 python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/flatted/python/test.py
+-rw-r--r--   0 saqadri    (501) staff       (20)      760 2023-12-23 21:12:22.000000 python-aiconfig-1.1.9/src/aiconfig/editor/example_aiconfig_model_registry.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.626107 python-aiconfig-1.1.9/src/aiconfig/editor/server/
+-rw-r--r--   0 saqadri    (501) staff       (20)        0 2023-12-23 21:12:22.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/__init__.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     1389 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/queue_iterator.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    18537 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/server.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    13006 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/server_utils.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.628718 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/
+-rw-r--r--   0 saqadri    (501) staff       (20)      366 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/asset-manifest.json
+-rw-r--r--   0 saqadri    (501) staff       (20)      590 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/index.html
+-rw-r--r--   0 saqadri    (501) staff       (20)      189 2024-01-02 18:17:09.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/manifest.json
+-rw-r--r--   0 saqadri    (501) staff       (20)       67 2024-01-02 18:17:09.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/robots.txt
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.618732 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.630345 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/
+-rw-r--r--   0 saqadri    (501) staff       (20)     4512 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js
+-rw-r--r--   0 saqadri    (501) staff       (20)    10597 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js.map
+-rw-r--r--   0 saqadri    (501) staff       (20)   143442 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/main.612f69d0.js
+-rw-r--r--   0 saqadri    (501) staff       (20)      971 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.LICENSE.txt
+-rw-r--r--   0 saqadri    (501) staff       (20)   367448 2024-01-03 17:08:36.000000 python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.map
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.631602 python-aiconfig-1.1.9/src/aiconfig/eval/
+-rw-r--r--   0 saqadri    (501) staff       (20)       13 2023-12-19 19:11:07.000000 python-aiconfig-1.1.9/src/aiconfig/eval/__init__.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.631712 python-aiconfig-1.1.9/src/aiconfig/eval/api/
+-rw-r--r--   0 saqadri    (501) staff       (20)      630 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/src/aiconfig/eval/api/__init__.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     6700 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/src/aiconfig/eval/common.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    11291 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/src/aiconfig/eval/lib.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    11797 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/src/aiconfig/eval/metrics.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     3152 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/src/aiconfig/eval/openai.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     9803 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/model_parser.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     5001 2024-01-02 18:12:58.000000 python-aiconfig-1.1.9/src/aiconfig/registry.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    36940 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/schema.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.631954 python-aiconfig-1.1.9/src/aiconfig/scripts/
+-rw-r--r--   0 saqadri    (501) staff       (20)     4666 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/src/aiconfig/scripts/aiconfig_cli.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     1490 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/src/aiconfig/scripts/run_aiconfig.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.632270 python-aiconfig-1.1.9/src/aiconfig/util/
+-rw-r--r--   0 saqadri    (501) staff       (20)        0 2023-10-17 16:38:26.000000 python-aiconfig-1.1.9/src/aiconfig/util/__init__.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     2505 2024-01-08 17:15:50.000000 python-aiconfig-1.1.9/src/aiconfig/util/config_utils.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    11182 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/src/aiconfig/util/params.py
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.634438 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/
+-rw-r--r--   0 saqadri    (501) staff       (20)    24665 2024-01-08 17:51:52.000000 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/PKG-INFO
+-rw-r--r--   0 saqadri    (501) staff       (20)     2588 2024-01-08 17:51:53.000000 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 saqadri    (501) staff       (20)        1 2024-01-08 17:51:52.000000 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 saqadri    (501) staff       (20)       64 2024-01-08 17:51:52.000000 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/entry_points.txt
+-rw-r--r--   0 saqadri    (501) staff       (20)      260 2024-01-08 17:51:52.000000 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/requires.txt
+-rw-r--r--   0 saqadri    (501) staff       (20)        9 2024-01-08 17:51:52.000000 python-aiconfig-1.1.9/src/python_aiconfig.egg-info/top_level.txt
+drwxr-xr-x   0 saqadri    (501) staff       (20)        0 2024-01-08 17:51:53.634276 python-aiconfig-1.1.9/tests/
+-rw-r--r--   0 saqadri    (501) staff       (20)      614 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/tests/test_chatcompletion_mock_wrapper.py
+-rw-r--r--   0 saqadri    (501) staff       (20)      902 2023-12-09 08:36:12.000000 python-aiconfig-1.1.9/tests/test_dataclass.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     9517 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/tests/test_eval.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     4287 2023-12-21 21:31:22.000000 python-aiconfig-1.1.9/tests/test_eval_model_graded_openai.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     2414 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_library_helpers.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     4414 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_load_config.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    14134 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_parameter_api.py
+-rw-r--r--   0 saqadri    (501) staff       (20)    23918 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_programmatically_create_an_AIConfig.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     5658 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_registry.py
+-rw-r--r--   0 saqadri    (501) staff       (20)      908 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_resolve.py
+-rw-r--r--   0 saqadri    (501) staff       (20)     3696 2024-01-05 22:02:44.000000 python-aiconfig-1.1.9/tests/test_run_config.py
```

### Comparing `python-aiconfig-1.1.8/LICENSE` & `python-aiconfig-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/PKG-INFO` & `python-aiconfig-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aiconfig
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python library for LastMile AI API
 Author-email: Sarmad Qadri <sarmad@lastmileai.dev>
 Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/aiconfig/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: black
 Requires-Dist: flake8
 Requires-Dist: flask-cors
 Requires-Dist: flask[async]
 Requires-Dist: google-generativeai
 Requires-Dist: huggingface_hub
 Requires-Dist: hypothesis==6.91.0
-Requires-Dist: lastmile-utils==0.0.13
+Requires-Dist: lastmile-utils==0.0.14
 Requires-Dist: mock
 Requires-Dist: nest_asyncio
 Requires-Dist: nltk
 Requires-Dist: openai<1.5,>=1.0.0
 Requires-Dist: prompt_toolkit
 Requires-Dist: pybars3
 Requires-Dist: pydantic>=2.1
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: python-aiconfig Version: 1.1.8 Summary: Python
+Metadata-Version: 2.1 Name: python-aiconfig Version: 1.1.9 Summary: Python
 library for LastMile AI API Author-email: Sarmad Qadri
 lastmileai.dev> Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/aiconfig/issues
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: black Requires-Dist: flake8 Requires-Dist:
 flask-cors Requires-Dist: flask[async] Requires-Dist: google-generativeai
 Requires-Dist: huggingface_hub Requires-Dist: hypothesis==6.91.0 Requires-Dist:
-lastmile-utils==0.0.13 Requires-Dist: mock Requires-Dist: nest_asyncio
+lastmile-utils==0.0.14 Requires-Dist: mock Requires-Dist: nest_asyncio
 Requires-Dist: nltk Requires-Dist: openai<1.5,>=1.0.0 Requires-Dist:
 prompt_toolkit Requires-Dist: pybars3 Requires-Dist: pydantic>=2.1 Requires-
 Dist: pylint Requires-Dist: pytest Requires-Dist: pytest-asyncio Requires-Dist:
 python-dotenv Requires-Dist: pyyaml Requires-Dist: requests Requires-Dist:
 result > Full documentation: **[aiconfig.lastmileai.dev](https://
 aiconfig.lastmileai.dev/)** ## Overview AIConfig saves prompts, models and
 model parameters as source control friendly configs. This allows you to iterate
```

### Comparing `python-aiconfig-1.1.8/README.md` & `python-aiconfig-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/pyproject.toml` & `python-aiconfig-1.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "python-aiconfig"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="Sarmad Qadri", email="sarmad@lastmileai.dev" },
 ]
 description = "Python library for LastMile AI API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,14 +19,17 @@
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 "Homepage" = "https://github.com/lastmile-ai/aiconfig"
 "Bug Tracker" = "https://github.com/lastmile-ai/aiconfig/issues"
 
+[project.scripts]
+aiconfig = "aiconfig.scripts.aiconfig_cli:main"
+
 # Black formatting
 [tool.black]
 line-length = 99
 include = '\.pyi?$'
 exclude = '''
 /(
       .eggs         # exclude a few common directories in the
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/ChatCompletion.py` & `python-aiconfig-1.1.9/src/aiconfig/ChatCompletion.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,15 @@
         prompts (List[Prompt]): List of prompts to be validated and added.
         aiconfig (AIConfigRuntime): Configuration runtime instance to which the prompts are to be added.
     """
     for i, new_prompt in enumerate(prompts):
         in_config = False
         for config_prompt in aiconfig.prompts:
             # check for duplicates (same input and settings.)
-            if (
-                config_prompt.input == new_prompt.input
-                and new_prompt.metadata == config_prompt.metadata
-            ):
+            if config_prompt.input == new_prompt.input and new_prompt.metadata == config_prompt.metadata:
                 in_config = True
                 # update outputs if different
                 if config_prompt.outputs != new_prompt.outputs:
                     config_prompt.outputs = new_prompt.outputs
                 break
         if not in_config:
             new_prompt_name = "prompt_{}".format(str(len(aiconfig.prompts)))
@@ -54,17 +51,15 @@
     Returns:
         List[Output]: A list of outputs extracted and formatted from the response.
     """
     outputs = []
 
     response = response.model_dump(exclude_none=True)
 
-    response_without_choices = {
-        key: copy.deepcopy(value) for key, value in response.items() if key != "choices"
-    }
+    response_without_choices = {key: copy.deepcopy(value) for key, value in response.items() if key != "choices"}
     for i, choice in enumerate(response.get("choices")):
         response_without_choices.update({"finish_reason": choice.get("finish_reason")})
         output = ExecuteResult(
             **{
                 "output_type": "execute_result",
                 "data": choice["message"],
                 "execution_count": i,
@@ -72,26 +67,27 @@
             }
         )
 
         outputs.append(output)
     return outputs
 
 
-def async_run_serialize_helper(aiconfig: AIConfigRuntime, request_kwargs: Dict):
+def async_run_serialize_helper(
+    aiconfig: AIConfigRuntime,
+    request_kwargs: Dict,
+) -> List[Prompt]:
     """
     Method serialize() of AIConfig is an async method. If not, create a new one and await serialize().
     """
     in_event_loop = asyncio.get_event_loop().is_running()
 
     serialized_prompts = None
 
     async def run_and_await_serialize():
-        result = await aiconfig.serialize(
-            request_kwargs.get("model"), request_kwargs, "prompt"
-        )
+        result = await aiconfig.serialize(request_kwargs.get("model"), request_kwargs, "prompt")
         return result
 
     # serialize prompts from ChatCompletion kwargs
     if in_event_loop:
         nest_asyncio.apply(loop=asyncio.get_event_loop())
         serialized_prompts = asyncio.run(run_and_await_serialize())
 
@@ -118,39 +114,29 @@
 
     def _get_aiconfig_runtime(output_aiconfig_path: str) -> AIConfigRuntime:
         try:
             return AIConfigRuntime.load(output_aiconfig_path)
         except IOError:
             return AIConfigRuntime.create(**(aiconfig_settings or {}))
 
-    output_aiconfig = (
-        output_aiconfig_ref
-        if isinstance(output_aiconfig_ref, AIConfigRuntime)
-        else _get_aiconfig_runtime(output_aiconfig_ref)
-    )
-
-    output_config_file_path = (
-        output_aiconfig_ref
-        if isinstance(output_aiconfig_ref, str)
-        else output_aiconfig_ref.file_path
-    )
+    output_aiconfig = output_aiconfig_ref if isinstance(output_aiconfig_ref, AIConfigRuntime) else _get_aiconfig_runtime(output_aiconfig_ref)
+
+    output_config_file_path = output_aiconfig_ref if isinstance(output_aiconfig_ref, str) else output_aiconfig_ref.file_path
 
     # TODO: openai makes it hard to statically annotate.
     def _create_chat_completion_with_config_saving(*args, **kwargs) -> Any:  # type: ignore
         response = openai_api.chat.completions.create(*args, **kwargs)
 
         serialized_prompts = async_run_serialize_helper(output_aiconfig, kwargs)
 
         # serialize output from response
         outputs = []
 
         # Check if response is a stream
-        stream = kwargs.get("stream", False) is True and isinstance(
-            response, openai.Stream
-        )
+        stream = kwargs.get("stream", False) is True and isinstance(response, openai.Stream)
 
         # Convert Response to output for last prompt
         if not stream:
             outputs = extract_outputs_from_response(response)
 
             # Add outputs to last prompt
             serialized_prompts[-1].outputs = outputs
@@ -182,17 +168,15 @@
                             output_type="execute_result",
                             data=copy.deepcopy(accumulated_message_for_choice),
                             execution_count=index,
                             metadata={"finish_reason": choice.get("finish_reason")},
                         )
                         stream_outputs[index] = output
                     yield chunk
-                stream_outputs = [
-                    stream_outputs[i] for i in sorted(list(stream_outputs.keys()))
-                ]
+                stream_outputs = [stream_outputs[i] for i in sorted(list(stream_outputs.keys()))]
 
                 # Add outputs to last prompt
                 serialized_prompts[-1].outputs = stream_outputs
 
                 validate_and_add_prompts_to_config(serialized_prompts, output_aiconfig)
 
                 # Save config to file
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/Config.py` & `python-aiconfig-1.1.9/src/aiconfig/Config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import json
 import os
-import yaml
 from typing import Any, Dict, List, Literal, Optional, Tuple
 
 import requests
+import yaml
 from aiconfig.callback import CallbackEvent, CallbackManager
+from aiconfig.default_parsers.anyscale_endpoint import DefaultAnyscaleEndpointParser
 from aiconfig.default_parsers.openai import DefaultOpenAIParser
 from aiconfig.default_parsers.palm import PaLMChatParser, PaLMTextParser
 from aiconfig.model_parser import InferenceOptions, ModelParser
+
 from aiconfig.schema import JSONObject
 
 from .default_parsers.dalle import DalleImageGenerationParser
 from .default_parsers.hf import HuggingFaceTextGenerationParser
-from .registry import (
-    ModelParserRegistry,
-    update_model_parser_registry_with_config_runtime,
-)
+from .registry import ModelParserRegistry, update_model_parser_registry_with_config_runtime
 from .schema import AIConfig, Prompt
 from .util.config_utils import is_yaml_ext
 
 gpt_models = [
     "gpt-4",
-    "GPT-4",
     "gpt-4-0314",
     "gpt-4-0613",
     "gpt-4-32k",
     "gpt-4-32k-0314",
     "gpt-4-32k-0613",
     "gpt-3.5-turbo",
     "gpt-3.5-turbo-16k",
     "gpt-3.5-turbo-0301",
     "gpt-3.5-turbo-0613",
     "gpt-3.5-turbo-16k-0613",
 ]
 for model in gpt_models:
     ModelParserRegistry.register_model_parser(DefaultOpenAIParser(model))
+ModelParserRegistry.register_model_parser(DefaultAnyscaleEndpointParser("AnyscaleEndpoint"))
 ModelParserRegistry.register_model_parser(PaLMChatParser())
 ModelParserRegistry.register_model_parser(PaLMTextParser())
 ModelParserRegistry.register_model_parser(HuggingFaceTextGenerationParser())
 dalle_image_generation_models = [
     "dall-e-2",
     "dall-e-3",
 ]
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/__init__.py` & `python-aiconfig-1.1.9/src/aiconfig/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .schema import (
     AIConfig,
     ConfigMetadata,
     ExecuteResult,
     JSONObject,
     ModelMetadata,
     Output,
+    OutputDataWithValue,
     Prompt,
     PromptInput,
     PromptMetadata,
     SchemaVersion,
 )
 from .util.config_utils import get_api_key_from_environment
 from .util.params import resolve_prompt
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/callback.py` & `python-aiconfig-1.1.9/src/aiconfig/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 # Standard Libraries
 import asyncio
 import logging
 import time
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Coroutine,
-    Final,
-    List,
-    Sequence,
-    TypeAlias,
-    Union,
-)
+from typing import Any, Awaitable, Callable, Coroutine, Final, List, Sequence, TypeAlias, Union
 
 from pydantic import BaseModel, ConfigDict
 
 # Third Party Libraries
 from result import Err, Ok
 
 # Constants
@@ -39,17 +29,15 @@
 
 
 # Type Aliases
 Callback = Callable[[CallbackEvent], Awaitable[Any]]
 Result: TypeAlias = Union[Ok[Any], Err[Any]]
 
 
-async def execute_coroutine_with_timeout(
-    coroutine: Coroutine[Any, Any, Any], timeout: int
-) -> Result:
+async def execute_coroutine_with_timeout(coroutine: Coroutine[Any, Any, Any], timeout: int) -> Result:
     """
     Execute a coroutine with a timeout, return an Ok result or an Err on Exception
 
     Args:
         coroutine: The coroutine to execute
         timeout: The timeout in seconds
 
@@ -119,17 +107,15 @@
         log_file = "callbacks.log"
 
     def setup_logger():
         level = logging.DEBUG
         name = "my-logger"
         log_file = "aiconfig.log"
 
-        formatter = logging.Formatter(
-            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-        )
+        formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         handler = logging.FileHandler(log_file)
         handler.setFormatter(formatter)
 
         logger = logging.getLogger(name)
         logger.setLevel(level)
         logger.addHandler(handler)
         return logger
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/default_parsers/dalle.py` & `python-aiconfig-1.1.9/src/aiconfig/default_parsers/dalle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import copy
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 import openai
 from aiconfig.default_parsers.parameterized_model_parser import ParameterizedModelParser
 from aiconfig.util.config_utils import get_api_key_from_environment
 from aiconfig.util.params import resolve_prompt
 from openai import OpenAI
 
 # Dall-E API imports
 from openai.types import Image, ImagesResponse
 
-from aiconfig.schema import ExecuteResult, Output, Prompt, PromptMetadata
+from aiconfig.schema import ExecuteResult, Output, OutputDataWithStringValue, Prompt, PromptMetadata
 
 # ModelParser Utils
 # Type hint imports
 
 
 # Circuluar Dependency Type Hints
 if TYPE_CHECKING:
@@ -37,18 +37,25 @@
         if key.lower() in supported_keys:
             completion_data[key.lower()] = model_settings[key]
 
     return completion_data
 
 
 def construct_output(image_data: Image, execution_count: int) -> Output:
+    data = None
+    if image_data.b64_json is not None:
+        data = OutputDataWithStringValue(kind="base64", value=str(image_data.b64_json))
+    elif image_data.url is not None:
+        data = OutputDataWithStringValue(kind="file_uri", value=str(image_data.url))
+    else:
+        raise ValueError(f"Did not receive a valid image type from image_data: {image_data}")
     output = ExecuteResult(
         **{
             "output_type": "execute_result",
-            "data": image_data.b64_json or image_data.url,
+            "data": data,
             "execution_count": execution_count,
             "metadata": {"revised_prompt": image_data.revised_prompt},
             "mime_type": "image/png",
         }
     )
     return output
 
@@ -72,18 +79,15 @@
         super().__init__()
 
         supported_models = {
             "dall-e-2",
             "dall-e-3",
         }
         if model_id.lower() not in supported_models:
-            raise ValueError(
-                "{model_id}"
-                + " is not a valid model ID for Dall-E image generation. Supported models: {supported_models}."
-            )
+            raise ValueError("{model_id}" + " is not a valid model ID for Dall-E image generation. Supported models: {supported_models}.")
         self.model_id = model_id
 
         self.client = None
 
     def id(self) -> str:
         """
         Returns an identifier for the model (e.g. dall-e-2, dall-e-3, etc.).
@@ -93,15 +97,15 @@
     async def serialize(
         self,
         prompt_name: str,
         data: Any,
         ai_config: "AIConfigRuntime",
         parameters: Optional[Dict] = None,
         **kwargs,
-    ) -> Prompt:
+    ) -> List[Prompt]:
         """
         Defines how a prompt and model inference settings get serialized in the .aiconfig.
 
         Args:
             prompt (str): The prompt to be serialized.
             inference_settings (dict): Model-specific inference settings to be serialized.
 
@@ -116,24 +120,20 @@
         # Prompt is handled, remove from data
         data.pop("prompt", None)
 
         model_metadata = ai_config.get_model_metadata(data, self.id())
         prompt = Prompt(
             name=prompt_name,
             input=prompt_input,
-            metadata=PromptMetadata(
-                model=model_metadata, parameters=parameters, **kwargs
-            ),
+            metadata=PromptMetadata(model=model_metadata, parameters=parameters, **kwargs),
         )
         return [prompt]
 
     # TODO (rossdanlm): Update documentation for args
-    async def deserialize(
-        self, prompt: Prompt, aiconfig: "AIConfigRuntime", params: Optional[Dict] = {}
-    ) -> Dict:
+    async def deserialize(self, prompt: Prompt, aiconfig: "AIConfigRuntime", params: Optional[Dict] = {}) -> Dict:
         """
         Defines how to parse a prompt in the .aiconfig for a particular model
         and constructs the completion params for that model.
 
         Args:
             Update this documentation... serialized_data (str): Serialized data from the .aiconfig.
 
@@ -145,39 +145,35 @@
         model_settings = self.get_model_settings(prompt, aiconfig)
 
         # Build Completion data
         completion_data = refine_image_completion_params(model_settings)
         completion_data["prompt"] = resolved_prompt
         return completion_data
 
-    async def run_inference(
-        self, prompt: Prompt, aiconfig, _options, parameters
-    ) -> Output:
+    async def run_inference(self, prompt: Prompt, aiconfig, _options, parameters) -> List[Output]:
         """
         Invoked to run a prompt in the .aiconfig. This method should perform
         the actual model inference based on the provided prompt and inference settings.
 
         Args:
             prompt (str): The input prompt.
             inference_settings (dict): Model-specific inference settings.
 
         Returns:
             InferenceResponse: The response from the model.
         """
         # If needed, certify the API key and initialize the OpenAI client
         if not openai.api_key:
-            openai.api_key = get_api_key_from_environment("OPENAI_API_KEY")
+            openai.api_key = get_api_key_from_environment("OPENAI_API_KEY").unwrap()
         if not self.client:
             self.client = OpenAI(api_key=openai.api_key)
 
         completion_data = await self.deserialize(prompt, aiconfig, parameters)
 
-        print(
-            "Calling image generation. This can take several seconds, please hold on..."
-        )
+        print("Calling image generation. This can take several seconds, please hold on...")
         response: ImagesResponse = self.client.images.generate(**completion_data)
 
         outputs = []
         # ImageResponse object also contains a "created" field for timestamp, should I store that somewhere?
         # Ex: response=ImagesResponse(created=1700347843, data=[...])
         for execution_count, image_data in enumerate(response.data):
             output = construct_output(image_data, execution_count)
@@ -197,11 +193,12 @@
 
         if not output:
             return ""
 
         # TODO (rossdanlm): Handle multiple outputs in list
         # https://github.com/lastmile-ai/aiconfig/issues/467
         if output.output_type == "execute_result":
-            if isinstance(output.data, str):
+            if isinstance(output.data, OutputDataWithStringValue):
+                return output.data.value
+            elif isinstance(output.data, str):
                 return output.data
-        else:
-            return ""
+        return ""
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/default_parsers/hf.py` & `python-aiconfig-1.1.9/src/aiconfig/default_parsers/hf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 import copy
-from typing import TYPE_CHECKING, Any, Dict, Optional
+import json
+from typing import TYPE_CHECKING, Any, Iterable, List, Optional, Union
 
 from aiconfig.default_parsers.parameterized_model_parser import ParameterizedModelParser
 from aiconfig.model_parser import InferenceOptions
 from aiconfig.util.config_utils import get_api_key_from_environment
+from aiconfig.util.params import resolve_prompt
 
 # HuggingFace API imports
 from huggingface_hub import InferenceClient
-from huggingface_hub.inference._text_generation import (
-    TextGenerationResponse,
-    TextGenerationStreamResponse,
-)
+from huggingface_hub.inference._text_generation import TextGenerationResponse, TextGenerationStreamResponse
 
-from aiconfig.schema import ExecuteResult, Output, Prompt, PromptMetadata
 from aiconfig import CallbackEvent
-
-from aiconfig.util.params import resolve_prompt
-
-# ModelParser Utils
-# Type hint imports
+from aiconfig.schema import ExecuteResult, Output, OutputDataWithValue, Prompt, PromptMetadata
 
 # Circuluar Dependency Type Hints
 if TYPE_CHECKING:
     from aiconfig.Config import AIConfigRuntime
 
 
 # Step 1: define Helpers
@@ -59,15 +53,15 @@
         if key.lower() in supported_keys:
             completion_data[key.lower()] = model_settings[key]
 
     return completion_data
 
 
 def construct_stream_output(
-    response: TextGenerationStreamResponse,
+    response: Union[Iterable[TextGenerationStreamResponse], Iterable[str]],
     response_includes_details: bool,
     options: InferenceOptions,
 ) -> Output:
     """
     Constructs the output for a stream response.
 
     Args:
@@ -75,66 +69,62 @@
         response_includes_details (bool): Whether or not the response includes details.
         options (InferenceOptions): The inference options. Used to determine the stream callback.
 
     """
     accumulated_message = ""
     for iteration in response:
         metadata = {}
-        data = iteration
+        # If response_includes_details is false, `iteration` will be a string,
+        # otherwise, `iteration` is a TextGenerationStreamResponse
+        new_text = iteration
         if response_includes_details:
             iteration: TextGenerationStreamResponse
-            data = iteration.token.text
+            new_text = iteration.token.text
             metadata = {"token": iteration.token, "details": iteration.details}
-        else:
-            data: str
 
         # Reduce
-        accumulated_message += data
+        accumulated_message += new_text
 
         index = 0  # HF Text Generation api doesn't support multiple outputs
-        delta = data
         if options and options.stream_callback:
-            options.stream_callback(delta, accumulated_message, index)
-
+            options.stream_callback(new_text, accumulated_message, index)
         output = ExecuteResult(
             **{
                 "output_type": "execute_result",
-                "data": copy.deepcopy(accumulated_message),
+                "data": accumulated_message,
                 "execution_count": index,
                 "metadata": metadata,
             }
         )
 
     return output
 
 
-def construct_regular_output(response: TextGenerationResponse, response_includes_details: bool) -> Output:
-    metadata = {}
-    data = response
+def construct_regular_output(response: str, response_includes_details: bool) -> Output:
+    metadata = {"raw_response": response}
     if response_includes_details:
-        data = response.generated_text
-        metadata = {"details": response.details}
+        metadata["details"] = response.details
 
     output = ExecuteResult(
         **{
             "output_type": "execute_result",
-            "data": data,
+            "data": response,
             "execution_count": 0,
             "metadata": metadata,
         }
     )
     return output
 
 
 class HuggingFaceTextGenerationParser(ParameterizedModelParser):
     """
     A model parser for HuggingFace text generation models.
     """
 
-    def __init__(self, model_id: str = None, use_api_token=False):
+    def __init__(self, model_id: str = None, use_api_token=True):
         """
         Args:
             model_id (str): The model ID of the model to use.
             no_token (bool): Whether or not to require an API token. Set to False if you don't have an api key.
 
         Returns:
             HuggingFaceTextParser: The HuggingFaceTextParser object.
@@ -151,15 +141,17 @@
 
         """
         super().__init__()
 
         token = None
 
         if use_api_token:
-            token = get_api_key_from_environment("HUGGING_FACE_API_TOKEN")
+            # You are allowed to use Hugging Face for a bit before you get
+            # rate limited, in which case you will receive a clear error
+            token = get_api_key_from_environment("HUGGING_FACE_API_TOKEN", required=False).unwrap()
 
         self.client = InferenceClient(model_id, token=token)
 
     def id(self) -> str:
         """
         Returns an identifier for the Model Parser
         """
@@ -168,15 +160,15 @@
     async def serialize(
         self,
         prompt_name: str,
         data: Any,
         ai_config: "AIConfigRuntime",
         parameters: Optional[dict[Any, Any]] = None,
         **kwargs,
-    ) -> list[Prompt]:
+    ) -> List[Prompt]:
         """
         Defines how a prompt and model inference settings get serialized in the .aiconfig.
 
         Args:
             prompt (str): The prompt to be serialized.
             inference_settings (dict): Model-specific inference settings to be serialized.
 
@@ -206,23 +198,21 @@
 
         prompts = []
 
         model_metadata = ai_config.get_model_metadata(data, self.id())
         prompt = Prompt(
             name=prompt_name,
             input=prompt_input,
-            metadata=PromptMetadata(
-                model=model_metadata, parameters=parameters, **kwargs
-            ),
+            metadata=PromptMetadata(model=model_metadata, parameters=parameters, **kwargs),
         )
 
         prompts.append(prompt)
-        
-        await ai_config.callback_manager.run_callbacks(CallbackEvent("on_serialize_complete", __name__, {"result": prompts }))
-        
+
+        await ai_config.callback_manager.run_callbacks(CallbackEvent("on_serialize_complete", __name__, {"result": prompts}))
+
         return prompts
 
     async def deserialize(
         self,
         prompt: Prompt,
         aiconfig: "AIConfigRuntime",
         params: Optional[dict[Any, Any]] = {},
@@ -248,17 +238,15 @@
 
         completion_data["prompt"] = resolved_prompt
 
         await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_deserialize_complete", __name__, {"output": completion_data}))
 
         return completion_data
 
-    async def run_inference(
-        self, prompt: Prompt, aiconfig: "AIConfigRuntime", options: InferenceOptions, parameters: dict[Any, Any]
-    ) -> Output:
+    async def run_inference(self, prompt: Prompt, aiconfig: "AIConfigRuntime", options: InferenceOptions, parameters: dict[Any, Any]) -> List[Output]:
         """
         Invoked to run a prompt in the .aiconfig. This method should perform
         the actual model inference based on the provided prompt and inference settings.
 
         Args:
             prompt (str): The input prompt.
             inference_settings (dict): Model-specific inference settings.
@@ -314,11 +302,23 @@
         if not output:
             output = aiconfig.get_latest_output(prompt)
 
         if not output:
             return ""
 
         if output.output_type == "execute_result":
-            if isinstance(output.data, str):
-                return output.data
-        else:
-            return ""
+            output_data = output.data
+            if isinstance(output_data, str):
+                return output_data
+            if isinstance(output_data, OutputDataWithValue):
+                if isinstance(output_data.value, str):
+                    return output_data.value
+                # HuggingFace Text generation does not support function
+                # calls so shouldn't get here, but just being safe
+                return json.dumps(output_data.value, indent=2)
+
+            # Doing this to be backwards-compatible with old output format
+            # where we used to save the TextGenerationResponse or
+            # TextGenerationStreamResponse in output.data
+            if hasattr(output_data, "generated_text"):
+                return output_data.generated_text
+        return ""
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/default_parsers/palm.py` & `python-aiconfig-1.1.9/src/aiconfig/default_parsers/palm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import json
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 import google.generativeai as palm
+from aiconfig.callback import CallbackEvent
 from aiconfig.default_parsers.parameterized_model_parser import ParameterizedModelParser
+from aiconfig.model_parser import InferenceOptions
 from aiconfig.util.params import resolve_parameters, resolve_prompt
 from google.generativeai.text import Completion
+from google.generativeai.types.discuss_types import MessageDict
 
-from ..callback import CallbackEvent
-from ..model_parser import InferenceOptions
-from ..schema import ExecuteResult, Output, Prompt, PromptMetadata
+from aiconfig.schema import ExecuteResult, Output, OutputDataWithValue, Prompt, PromptMetadata
 
 if TYPE_CHECKING:
     from aiconfig.Config import AIConfigRuntime
 
 
 class PaLMTextParser(ParameterizedModelParser):
     def __init__(self):
@@ -69,56 +71,46 @@
         ]
 
         event = CallbackEvent("on_serialize_complete", __name__, {"result": prompts})
         await ai_config.callback_manager.run_callbacks(event)
 
         return prompts
 
-    async def deserialize(
-        self, prompt: Prompt, aiconfig: "AIConfigRuntime", params: Optional[Dict] = {}
-    ) -> Dict:
+    async def deserialize(self, prompt: Prompt, aiconfig: "AIConfigRuntime", params: Optional[Dict] = {}) -> Dict:
         """
         Defines how to parse a prompt in the .aiconfig for a particular model
         and constructs the completion params for that model.
 
         Args:
             serialized_data (str): Serialized data from the .aiconfig.
 
         Returns:
             dict: Model-specific completion parameters.
         """
-        await aiconfig.callback_manager.run_callbacks(
-            CallbackEvent(
-                "on_deserialize_start", __name__, {"prompt": prompt, "params": params}
-            )
-        )
+        await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_deserialize_start", __name__, {"prompt": prompt, "params": params}))
         # Build Completion data
         model_settings = self.get_model_settings(prompt, aiconfig)
 
         completion_data = refine_chat_completion_params(model_settings)
 
         prompt_str = resolve_prompt(prompt, params, aiconfig)
 
         # pass in the user prompt
         completion_data["prompt"] = prompt_str
 
-        await aiconfig.callback_manager.run_callbacks(
-            CallbackEvent(
-                "on_deserialize_complete", __name__, {"output": completion_data}
-            )
-        )
+        await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_deserialize_complete", __name__, {"output": completion_data}))
         return completion_data
 
     async def run_inference(
         self,
         prompt: Prompt,
         aiconfig: "AIConfigRuntime",
         options: InferenceOptions,
         parameters,
-    ) -> Output:
+    ) -> List[Output]:
         """
         Invoked to run a prompt in the .aiconfig. This method should perform
         the actual model inference based on the provided prompt and inference settings.
 
         Output is deconstructed into two parts:
             data: the output text
             metadata: Candidate data from the model
@@ -142,27 +134,28 @@
         completion_data = await self.deserialize(prompt, aiconfig, parameters)
         # Return Type is of type Completion from Google Library
         completion: Completion = palm.generate_text(**completion_data)
 
         outputs = []
         # completion.candidates has all outputs. Candidates is an attribute of completion. Candidates is a dict. Taken from Google API impl
         for i, candidate in enumerate(completion.candidates):
+            # candidate is a TextCompletion obj (https://shorturl.at/emuG2),
+            # but Pydantic TypedDict breaks for Python v<3.12  so using
+            # generic Dict type
             candidate: Dict
             output = ExecuteResult(
                 output_type="execute_result",
                 execution_count=i,
-                data=candidate.get("output"),
-                metadata=candidate,
+                data=candidate.get("output", ""),
+                metadata={"raw_response": candidate},
             )
             outputs.append(output)
 
         prompt.outputs = outputs
-        await aiconfig.callback_manager.run_callbacks(
-            CallbackEvent("on_run_complete", __name__, {"result": prompt.outputs})
-        )
+        await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_run_complete", __name__, {"result": prompt.outputs}))
         return outputs
 
     def get_output_text(
         self,
         prompt: Prompt,
         aiconfig: "AIConfigRuntime",
         output: Optional[Output] = None,
@@ -230,94 +223,80 @@
                     **kwargs,
                 ),
             )
         ]
 
         event = CallbackEvent("on_serialize_complete", __name__, {"result": prompts})
         await ai_config.callback_manager.run_callbacks(event)
+        return prompts
 
-    async def deserialize(
-        self, prompt: Prompt, aiconfig: "AIConfigRuntime", params: Optional[Dict] = {}
-    ) -> Dict:
+    async def deserialize(self, prompt: Prompt, aiconfig: "AIConfigRuntime", params: Optional[Dict] = {}) -> Dict:
         """
         Defines how to parse a prompt in the .aiconfig for a particular model
         and constructs the completion params for that model.
 
         Args:
             serialized_data (str): Serialized data from the .aiconfig.
 
         Returns:
             dict: Model-specific completion parameters.
         """
-        await aiconfig.callback_manager.run_callbacks(
-            CallbackEvent(
-                "on_deserialize_start", __name__, {"prompt": prompt, "params": params}
-            )
-        )
+        await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_deserialize_start", __name__, {"prompt": prompt, "params": params}))
         resolved_prompt = resolve_prompt(prompt, params, aiconfig)
 
         # Build Completion data
         model_settings = self.get_model_settings(prompt, aiconfig)
 
         completion_data = refine_chat_completion_params(model_settings)
 
         # TODO: handle if user specifies previous messages in settings
         completion_data["messages"] = []
 
         # Default to always use chat contextjkl;
         if not hasattr(prompt.metadata, "remember_chat_context") or (
-            hasattr(prompt.metadata, "remember_chat_context")
-            and prompt.metadata.remember_chat_context != False
+            hasattr(prompt.metadata, "remember_chat_context") and prompt.metadata.remember_chat_context != False
         ):
             # handle chat history. check previous prompts for the same model. if same model, add prompt and its output to completion data if it has a completed output
             for i, previous_prompt in enumerate(aiconfig.prompts):
                 # include prompts upto the current one
                 if previous_prompt.name == prompt.name:
                     break
 
                 # check if prompt is of the same model
                 if aiconfig.get_model_name(previous_prompt) == self.id():
                     # add prompt and its output to completion data
                     # constructing this prompt will take into account available parameters.
 
                     # check if prompt has an output. PaLM Api requires this
                     if len(previous_prompt.outputs) > 0:
-                        resolved_previous_prompt = resolve_parameters(
-                            {}, previous_prompt, aiconfig
-                        )
-                        completion_data["messages"].append(
-                            {"content": resolved_previous_prompt, "author": "0"}
-                        )
+                        resolved_previous_prompt = resolve_parameters({}, previous_prompt, aiconfig)
+                        completion_data["messages"].append({"content": resolved_previous_prompt, "author": "0"})
 
                         completion_data["messages"].append(
                             {
                                 "content": aiconfig.get_output_text(
                                     previous_prompt,
                                     aiconfig.get_latest_output(previous_prompt),
                                 ),
                                 "author": "1",
                             }
                         )
 
         # pass in the user prompt
         completion_data["messages"].append({"content": resolved_prompt, "author": "0"})
-        await aiconfig.callback_manager.run_callbacks(
-            CallbackEvent(
-                "on_deserialize_complete", __name__, {"output": completion_data}
-            )
-        )
+        await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_deserialize_complete", __name__, {"output": completion_data}))
         return completion_data
 
     async def run_inference(
         self,
         prompt: Prompt,
         aiconfig: "AIConfigRuntime",
         options: InferenceOptions,
         parameters,
-    ) -> Output:
+    ) -> List[Output]:
         """
         Invoked to run a prompt in the .aiconfig. This method should perform
         the actual model inference based on the provided prompt and inference settings.
 
         Args:
             prompt (str): The input prompt.
             inference_settings (dict): Model-specific inference settings.
@@ -334,28 +313,30 @@
         )
 
         # TODO: check and handle api key here
         completion_data = await self.deserialize(prompt, aiconfig, parameters)
         response = palm.chat(**completion_data)
         outputs = []
         for i, candidate in enumerate(response.candidates):
+            # candidate is a MessageDict obj (https://shorturl.at/jKY35),
+            # but Pydantic TypedDict breaks for Python v<3.12  so using
+            # generic Dict type
+            candidate: Dict
             output = ExecuteResult(
                 **{
                     "output_type": "execute_result",
-                    "data": candidate,
+                    "data": candidate.get("content", ""),
                     "execution_count": i,
-                    "metadata": {"response": response},
+                    "metadata": {"raw_response": response},
                 }
             )
             outputs.append(output)
 
         prompt.outputs = outputs
-        await aiconfig.callback_manager.run_callbacks(
-            CallbackEvent("on_run_complete", __name__, {"result": prompt.outputs})
-        )
+        await aiconfig.callback_manager.run_callbacks(CallbackEvent("on_run_complete", __name__, {"result": prompt.outputs}))
         return prompt.outputs
 
     def get_output_text(
         self,
         prompt: Prompt,
         aiconfig: "AIConfigRuntime",
         output: Optional[Output] = None,
@@ -363,21 +344,30 @@
         if not output:
             output = aiconfig.get_latest_output(prompt)
 
         if not output:
             return ""
 
         if output.output_type == "execute_result":
-            message = output.data
-            if message.get("content"):
-                return message.get("content")
-            else:
-                return ""
-        else:
-            return ""
+            output_data = output.data
+            if isinstance(output_data, str):
+                return output_data
+            if isinstance(output_data, OutputDataWithValue):
+                if isinstance(output_data.value, str):
+                    return output_data.value
+                # PaLM does not support function calls so shouldn't get here,
+                # but just being safe
+                return json.dumps(output_data.value, indent=2)
+
+            # Doing this to be backwards-compatible with old output format
+            # where we used to save the MessageDict in output.data
+            if isinstance(output_data, MessageDict):
+                if output_data.get("content"):
+                    return output_data("content")
+        return ""
 
 
 def refine_chat_completion_params(model_settings):
     # completion parameters to be used for Palm's chat completion api
     # messages handled seperately
     supported_keys = {
         "candidate_count",
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/default_parsers/parameterized_model_parser.py` & `python-aiconfig-1.1.9/src/aiconfig/default_parsers/parameterized_model_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # TODO: plaese improve the file name on this file. This is an abstract class that handles parameterization for a model parser.
 
 
 import typing
 from abc import abstractmethod
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
 from aiconfig.model_parser import InferenceOptions, ModelParser
 from aiconfig.util.params import get_dependency_graph, resolve_prompt_string
 
-from aiconfig.schema import AIConfig, ExecuteResult, JSONObject, Prompt, PromptInput
+from aiconfig.schema import AIConfig, JSONObject, Output, Prompt, PromptInput
 
 if typing.TYPE_CHECKING:
     from aiconfig import AIConfigRuntime
 
 
 class ParameterizedModelParser(ModelParser):
     @abstractmethod
@@ -32,50 +32,44 @@
             params (dict): A dictionary of parameters to substitute into the prompt.
 
         Returns:
             dict: Model-specific completion parameters.
         """
 
     @abstractmethod
-    async def run_inference(self):
+    async def run_inference(self) -> List[Output]:
         pass
 
     async def run(
         self,
         prompt: Prompt,
         aiconfig: AIConfig,
         options: Optional[InferenceOptions] = None,
         parameters: Dict = {},
         **kwargs,
-    ) -> ExecuteResult:
+    ) -> List[Output]:
         # maybe use prompt metadata instead of kwargs?
         if kwargs.get("run_with_dependencies", False):
-            return await self.run_with_dependencies(
-                prompt, aiconfig, options, parameters
-            )
+            return await self.run_with_dependencies(prompt, aiconfig, options, parameters)
         else:
             return await self.run_inference(prompt, aiconfig, options, parameters)
 
-    async def run_with_dependencies(
-        self, prompt: Prompt, aiconfig: AIConfig, options=None, parameters: Dict = {}
-    ) -> ExecuteResult:
+    async def run_with_dependencies(self, prompt: Prompt, aiconfig: AIConfig, options=None, parameters: Dict = {}) -> List[Output]:
         """
         Executes the AI model with the resolved dependencies and prompt references and returns the API response.
 
         Args:
             prompt: The prompt to be used.
             aiconfig: The AIConfig object containing all prompts and parameters.
             parameters (dict): The resolved parameters to use for inference.
 
         Returns:
             ExecuteResult: An Object containing the response from the AI model.
         """
-        dependency_graph = get_dependency_graph(
-            prompt, aiconfig.prompts, aiconfig.prompt_index
-        )
+        dependency_graph = get_dependency_graph(prompt, aiconfig.prompts, aiconfig.prompt_index)
 
         # Create a set to keep track of visited prompts
         visited_prompts = set()
 
         async def execute_recursive(prompt_name):
             """
             Execute the AI model for a given prompt and its dependencies recursively.
@@ -91,19 +85,19 @@
                 return  # Skip already visited prompts
             visited_prompts.add(prompt_name)
 
             # Iterate through dependencies of the current prompt
             for dependency_prompt_name in dependency_graph[prompt_name]:
                 await execute_recursive(dependency_prompt_name)
 
-            output = await aiconfig.run(prompt_name, parameters, options)
+            outputs = await aiconfig.run(prompt_name, parameters, options)
 
             # Return the output of the original prompt being executed
             if prompt_name == prompt.name:
-                return output
+                return outputs
 
         return await execute_recursive(prompt.name)
 
     def resolve_prompt_template(
         prompt_template: str,
         prompt: Prompt,
         ai_config: "AIConfigRuntime",
@@ -125,15 +119,11 @@
 
     def get_prompt_template(self, prompt: Prompt, aiConfig: "AIConfigRuntime") -> str:
         """
         An overrideable method that returns a template for a prompt.
         """
         if isinstance(prompt.input, str):
             return prompt.input
-        elif isinstance(prompt.input, PromptInput) and isinstance(
-            prompt.input.data, str
-        ):
+        elif isinstance(prompt.input, PromptInput) and isinstance(prompt.input.data, str):
             return prompt.input.data
         else:
-            raise Exception(
-                f"Cannot get prompt template string from prompt input: {prompt.input}"
-            )
+            raise Exception(f"Cannot get prompt template string from prompt input: {prompt.input}")
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py` & `python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/flatted.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/client/node_modules/flatted/python/test.py` & `python-aiconfig-1.1.9/src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/test.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/example_aiconfig_model_registry.py` & `python-aiconfig-1.1.9/src/aiconfig/editor/example_aiconfig_model_registry.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/server_utils.py` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/server_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import importlib
 import importlib.util
 import logging
 import os
 import sys
+import typing
 from dataclasses import dataclass
 from enum import Enum
 from types import ModuleType
-from typing import Any, Callable, NewType, Optional, Type, TypeVar, cast
-import typing
+from typing import Any, Callable, NewType, Type, TypeVar, cast
 
 import lastmile_utils.lib.core.api as core_utils
 import result
 from aiconfig.Config import AIConfigRuntime
+from aiconfig.registry import ModelParserRegistry
 from flask import Flask
 from pydantic import field_validator
 from result import Err, Ok, Result
 
+from aiconfig.schema import Prompt, PromptMetadata
+
 MethodName = NewType("MethodName", str)
 
 logging.getLogger("werkzeug").disabled = True
 
 logging.basicConfig(format=core_utils.LOGGER_FMT)
 LOGGER = logging.getLogger(__name__)
 
@@ -50,17 +53,17 @@
     DEBUG_SERVERS = "DEBUG_SERVERS"
     DEBUG_BACKEND = "DEBUG_BACKEND"
     PROD = "PROD"
 
 
 class EditServerConfig(core_utils.Record):
     server_port: int = 8080
-    aiconfig_path: Optional[str] = None
+    aiconfig_path: str = "my_aiconfig.aiconfig.json"
     log_level: str | int = "INFO"
-    server_mode: ServerMode
+    server_mode: ServerMode = ServerMode.PROD
     parsers_module_path: str = "aiconfig_model_registry.py"
 
     @field_validator("server_mode", mode="before")
     def convert_to_mode(cls, value: Any) -> ServerMode:  # pylint: disable=no-self-argument
         if isinstance(value, str):
             try:
                 return ServerMode[value.upper()]
@@ -103,15 +106,15 @@
     return app.server_state  # type: ignore
 
 
 def resolve_path(path: str) -> str:
     return os.path.abspath(os.path.expanduser(path))
 
 
-def get_validated_path(raw_path: str, allow_create: bool = False) -> Result[ValidatedPath, str]:
+def get_validated_path(raw_path: str | None, allow_create: bool = False) -> Result[ValidatedPath, str]:
     LOGGER.debug(f"{allow_create=}")
     if not raw_path:
         return Err("No path provided")
     resolved = resolve_path(raw_path)
     if not allow_create and not os.path.isfile(resolved):
         return Err(f"File does not exist: {resolved}")
     return Ok(ValidatedPath(resolved))
@@ -198,32 +201,43 @@
 
 def init_server_state(app: Flask, edit_config: EditServerConfig) -> Result[None, str]:
     LOGGER.info("Initializing server state")
     _load_user_parser_module_if_exists(edit_config.parsers_module_path)
     state = get_server_state(app)
 
     assert state.aiconfig is None
-    if edit_config.aiconfig_path:
+    if os.path.exists(edit_config.aiconfig_path):
         LOGGER.info(f"Loading AIConfig from {edit_config.aiconfig_path}")
         val_path = get_validated_path(edit_config.aiconfig_path)
         aiconfig_runtime = val_path.and_then(safe_load_from_disk)
-        LOGGER.debug(f"{aiconfig_runtime.is_ok()=}")
         match aiconfig_runtime:
             case Ok(aiconfig_runtime_):
                 state.aiconfig = aiconfig_runtime_
                 LOGGER.info(f"Loaded AIConfig from {edit_config.aiconfig_path}")
                 return Ok(None)
             case Err(e):
                 LOGGER.error(f"Failed to load AIConfig from {edit_config.aiconfig_path}: {e}")
                 return Err(f"Failed to load AIConfig from {edit_config.aiconfig_path}: {e}")
     else:
+        LOGGER.info(f"Creating new AIConfig at {edit_config.aiconfig_path}")
         aiconfig_runtime = AIConfigRuntime.create()  # type: ignore
+        model_ids = ModelParserRegistry.parser_ids()
+        if len(model_ids) > 0:
+            aiconfig_runtime.add_prompt("prompt_1", Prompt(name="prompt_1", input="", metadata=PromptMetadata(model=model_ids[0])))
+
         state.aiconfig = aiconfig_runtime
         LOGGER.info("Created new AIConfig")
-        return Ok(None)
+        try:
+            aiconfig_runtime.save(edit_config.aiconfig_path)
+            LOGGER.info(f"Saved new AIConfig to {edit_config.aiconfig_path}")
+            state.aiconfig = aiconfig_runtime
+            return Ok(None)
+        except Exception as e:
+            LOGGER.error(f"Failed to create new AIConfig at {edit_config.aiconfig_path}: {e}")
+            return core_utils.ErrWithTraceback(e)
 
 
 def _safe_run_aiconfig_method(aiconfig: AIConfigRuntime, method_name: MethodName, method_args: OpArgs) -> Result[None, str]:
     # TODO: use `out`
     try:
         method = getattr(aiconfig, method_name)
         out = method(**method_args)
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/static/index.html` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/static/index.html`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js.map` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js.map`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/main.612f69d0.js` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/main.612f69d0.js`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.LICENSE.txt` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.map` & `python-aiconfig-1.1.9/src/aiconfig/editor/server/static/static/js/main.612f69d0.js.map`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/eval/api/__init__.py` & `python-aiconfig-1.1.9/src/aiconfig/eval/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/eval/common.py` & `python-aiconfig-1.1.9/src/aiconfig/eval/common.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/eval/lib.py` & `python-aiconfig-1.1.9/src/aiconfig/eval/lib.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/eval/metrics.py` & `python-aiconfig-1.1.9/src/aiconfig/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/eval/openai.py` & `python-aiconfig-1.1.9/src/aiconfig/eval/openai.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/src/aiconfig/model_parser.py` & `python-aiconfig-1.1.9/src/aiconfig/model_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from abc import ABC, abstractmethod
 import asyncio
 import copy
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 from aiconfig.schema import AIConfig, ExecuteResult, Output, Prompt
 
 if TYPE_CHECKING:
     from aiconfig.Config import AIConfigRuntime
 
 
@@ -20,27 +20,28 @@
     async def serialize(
         self,
         prompt_name: str,
         data: Any,
         ai_config: "AIConfigRuntime",
         parameters: Optional[Dict] = None,
         **kwargs,
-    ) -> Prompt:
+    ) -> List[Prompt]:
         """
-        Serialize a prompt and additional metadata/model settings into a Prompt object that can be saved in the AIConfig.
+        Serialize a prompt and additional metadata/model settings into a
+        list of Prompt objects that can be saved in the AIConfig.
 
         Args:
             prompt_name (str): Name to identify the prompt.
             data (Any): The prompt data to be serialized.
             ai_config (AIConfig): The AIConfig that the prompt belongs to.
             parameters (dict, optional): Optional parameters to include in the serialization.
             **kwargs: Additional keyword arguments, if needed.
 
         Returns:
-            Prompt: Serialized representation of the input data.
+            List[Prompt]: Serialized representation of the input data.
         """
 
     @abstractmethod
     async def deserialize(
         self,
         prompt: Prompt,
         aiConfig: "AIConfigRuntime",
@@ -138,74 +139,59 @@
             prompt (Prompt): The prompt to be used for inference.
             aiconfig (AIConfig): The AIConfig object containing all prompts and parameters.
 
         Returns:
             str: The output text from the model inference response.
         """
 
-    def get_model_settings(
-        self, prompt: Prompt, aiconfig: "AIConfigRuntime"
-    ) -> Dict[str, Any]:
+    def get_model_settings(self, prompt: Prompt, aiconfig: "AIConfigRuntime") -> Dict[str, Any]:
         """
         Extracts the AI model's settings from the configuration. If both prompt and config level settings are defined, merge them with prompt settings taking precedence.
 
         Args:
             prompt: The prompt object.
 
         Returns:
             dict: The settings of the model used by the prompt.
         """
         if not prompt:
             return aiconfig.get_global_settings(self.id())
 
         # Check if the prompt exists in the config
-        if (
-            prompt.name not in aiconfig.prompt_index
-            or aiconfig.prompt_index[prompt.name] != prompt
-        ):
+        if prompt.name not in aiconfig.prompt_index or aiconfig.prompt_index[prompt.name] != prompt:
             raise IndexError(f"Prompt '{prompt.name}' not in config.")
 
         model_metadata = prompt.metadata.model if prompt.metadata else None
 
         if model_metadata is None:
             # Use Default Model
             default_model = aiconfig.get_default_model()
             if not default_model:
-                raise KeyError(
-                    f"No default model specified in AIConfigMetadata, and prompt `{prompt.name}` does not specify a model."
-                )
+                raise KeyError(f"No default model specified in AIConfigMetadata, and prompt `{prompt.name}` does not specify a model.")
             return aiconfig.get_global_settings(default_model)
         elif isinstance(model_metadata, str):
             # Use Global settings
             return aiconfig.get_global_settings(model_metadata)
         else:
             # Merge config and prompt settings with prompt settings taking precedent
             model_settings = {}
             global_settings = aiconfig.get_global_settings(model_metadata.name)
-            prompt_setings = (
-                prompt.metadata.model.settings
-                if prompt.metadata.model.settings is not None
-                else {}
-            )
+            prompt_setings = prompt.metadata.model.settings if prompt.metadata.model.settings is not None else {}
 
             model_settings.update(global_settings)
             model_settings.update(prompt_setings)
 
             return model_settings
 
 
 def print_stream_callback(data, accumulated_data, index: int):
     """
     Default streamCallback function that prints the output to the console.
     """
-    print(
-        "\ndata: {}\naccumulated_data:{}\nindex:{}\n".format(
-            data, accumulated_data, index
-        )
-    )
+    print("\ndata: {}\naccumulated_data:{}\nindex:{}\n".format(data, accumulated_data, index))
 
 
 def print_stream_delta(data, accumulated_data, index: int):
     """
     Default streamCallback function that prints the output to the console.
     """
     if "content" in data:
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/registry.py` & `python-aiconfig-1.1.9/src/aiconfig/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,42 +8,43 @@
 if typing.TYPE_CHECKING:
     from aiconfig.Config import AIConfigRuntime
 
 
 class ModelParserRegistry:
     """
     A dictionary to store registered model parsers by their IDs. It stores both:
-        1) model_name --> model_parser (ex: "mistralai/Mistral-7B-v0.1" --> 
+        1) model_name --> model_parser (ex: "mistralai/Mistral-7B-v0.1" -->
             HuggingFaceTextGenerationTransformer)
-        2) moder_parser.id() --> model_parser (ex: HuggingFaceTextGenerationTransformer 
-            works with many different Text Generation models) so is saved as 
-            HuggingFaceTextGenerationTransformer.id() (str) (usually it's classname) --> 
-            HuggingFaceTextGenerationTransformer (obj) 
-        
-    The reason we allow 2) above is so that you can define the relationship between a 
+        2) moder_parser.id() --> model_parser (ex: HuggingFaceTextGenerationTransformer
+            works with many different Text Generation models) so is saved as
+            HuggingFaceTextGenerationTransformer.id() (str) (usually it's classname) -->
+            HuggingFaceTextGenerationTransformer (obj)
+
+    The reason we allow 2) above is so that you can define the relationship between a
     model name and a model parser in the AIConfig instead of the model parser class (ex:
     https://github.com/lastmile-ai/aiconfig/blob/main/cookbooks/HuggingFace/Mistral-aiconfig.json#L16-L18).
-    This then gets updated into the desired format 1) by calling the 
+    This then gets updated into the desired format 1) by calling the
     `update_model_parser_registry_with_config_runtime()` command
-    
-    Each model_name is only allowed to map to a single model_parser for an 
+
+    Each model_name is only allowed to map to a single model_parser for an
     AIConfigRuntime.
     """
+
     _parsers: Dict[str, ModelParser] = {}
 
     @staticmethod
     def register_model_parser(model_parser: ModelParser, ids: Optional[List[str]] = None):
         """
-        Adds a model parser to the registry. This model parser is used to parse Prompts 
+        Adds a model parser to the registry. This model parser is used to parse Prompts
         in the AIConfig that use the given model.
 
         Args:
             model_parser (ModelParser): The model parser to add to the registry.
-            ids (list, optional): Optional list of IDs (typically model names) to 
-                register the model parser under. If unspecified, the model parser will 
+            ids (list, optional): Optional list of IDs (typically model names) to
+                register the model parser under. If unspecified, the model parser will
                 be resgistered under its own ID.
         """
         if ids:
             for id in ids:
                 ModelParserRegistry._parsers[id] = model_parser
         ModelParserRegistry._parsers[model_parser.id()] = model_parser
 
@@ -89,47 +90,42 @@
     def clear_registry():
         """
         Removes all model parsers from the Registry.
         """
         ModelParserRegistry._parsers.clear()
 
     @staticmethod
-    def parser_ids() -> list:
+    def parser_ids() -> list[str]:
         """
         Retrieves a list of model parser IDs from the ModelParserRegistry.
 
         Returns:
             list: A list of model parser IDs.
         """
         return list(ModelParserRegistry._parsers.keys())
 
     @staticmethod
     def display_parsers() -> Dict[str, str]:
         """
         returns a dictionary of model names and their correspondings model parser ids
         """
-        return {
-            model_name: model_parser.id()
-            for model_name, model_parser in ModelParserRegistry._parsers.items()
-        }
+        return {model_name: model_parser.id() for model_name, model_parser in ModelParserRegistry._parsers.items()}
 
 
 def update_model_parser_registry_with_config_runtime(config_runtime: "AIConfigRuntime"):
     """
     Updates the model parser registry with any model parsers specified in the AIConfig.
 
     Args:
         config_runtime (AIConfigRuntime): The AIConfigRuntime.
     """
     if not config_runtime.metadata.model_parsers:
         return
     for model_id, model_parser_id in config_runtime.metadata.model_parsers.items():
-        retrieved_model_parser = ModelParserRegistry.get_model_parser(
-            model_parser_id
-        )  # Fix
+        retrieved_model_parser = ModelParserRegistry.get_model_parser(model_parser_id)  # Fix
         if retrieved_model_parser is None:
             error_message = (
                 f"Unable to load AIConfig: It specifies {config_runtime.metadata.model_parsers}, "
                 f"but ModelParser {model_parser_id} for {model_id} does not exist. "
                 "Make sure you have registered the ModelParser using AIConfigRuntime.registerModelParser "
                 "before loading the AIConfig."
             )
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/schema.py` & `python-aiconfig-1.1.9/src/aiconfig/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,34 +7,88 @@
 # Pydantic doesn't handle circular type references very well, TODO: handle this better than defining as type Any
 # JSONObject represents a JSON object as a dictionary with string keys and JSONValue values
 JSONObject = Dict[str, Any]
 # InferenceSettings represents settings for model inference as a JSON object
 InferenceSettings = JSONObject
 
 
-class OutputData(BaseModel):
+class OutputDataWithStringValue(BaseModel):
     """
-    OutputData represents the output content in a standard format.
+    This represents the output content that is storied as a string, but we use
+    both the `kind` field here and the `mime_type` in ExecuteResult to convert
+    the string into the output format we want.
     """
 
-    kind: Literal["string", "file_uri", "base64"]
+    kind: Literal["file_uri", "base64"]
     value: str
 
 
+class FunctionCallData(BaseModel):
+    """
+    Function call data reprsenting a single function call
+    """
+
+    arguments: str
+    """
+    The arguments to call the function with, as generated by the model in JSON
+    format. Note that the model does not always generate valid JSON, and may
+    hallucinate parameters not defined by your function schema. Validate the
+    arguments in your code before calling your function.
+    """
+
+    name: str
+    """The name of the function to call."""
+
+    class Config:
+        extra = "allow"
+
+
+class ToolCallData(BaseModel):
+    """
+    Generic tool call data
+    """
+
+    id: Optional[str]
+    """
+    Note: the `id` field is non-optional in OpenAI but we're keeping
+    it optional for practical purposes. See:
+    https://github.com/lastmile-ai/aiconfig/pull/636#discussion_r1437087325
+    """
+
+    function: FunctionCallData
+    type: Literal["function"]
+
+
+class OutputDataWithToolCallsValue(BaseModel):
+    """
+    This based off of ChatCompletionMessageToolCall from openai.types.chat
+    and is used for general tool calls.
+    """
+
+    kind: Literal["tool_calls"]
+    value: List[ToolCallData]
+
+
+OutputDataWithValue = Union[
+    OutputDataWithStringValue,
+    OutputDataWithToolCallsValue,
+]
+
+
 class ExecuteResult(BaseModel):
     """
     ExecuteResult represents the result of executing a prompt.
     """
 
     # Type of output
     output_type: Literal["execute_result"]
     # nth choice.
     execution_count: Union[int, None] = None
     # The result of the executing prompt.
-    data: Union[Any, OutputData]
+    data: Union[OutputDataWithValue, str, Any]
     # The MIME type of the result. If not specified, the MIME type will be assumed to be plain text.
     mime_type: Optional[str] = None
     # Output metadata
     metadata: Dict[str, Any]
 
 
 class Error(BaseModel):
@@ -278,35 +332,176 @@
         if prompt_name:
             if prompt_name not in self.prompt_index:
                 raise IndexError(f"Prompt '{prompt_name}' not found in config.")
             return self.prompt_index[prompt_name].metadata
         else:
             return self.metadata
 
-    def set_parameter(self, parameter_name: str, parameter_value, prompt_name: Optional[str] = None):
+    def get_parameters(
+        self,
+        prompt_or_prompt_name: Optional[str | Prompt] = None,
+    ) -> JSONObject:
+        """
+        Get the parameters for a prompt, using the global parameters if
+        needed.
+
+        Args:
+            prompt_or_prompt_name Optional[str | Prompt]: The name of the
+                prompt or the prompt object. If not specified, use the
+                global parameters.
+        """
+        prompt = prompt_or_prompt_name
+        if isinstance(prompt_or_prompt_name, str):
+            if prompt_or_prompt_name not in self.prompt_index:
+                raise IndexError(f"Prompt '{prompt_or_prompt_name}' not found in config, available prompts are:\n {list(self.prompt_index.keys())}")
+            prompt = self.prompt_index[prompt_or_prompt_name]
+
+        assert prompt is None or isinstance(prompt, Prompt)
+        if prompt is None or not prompt.metadata or not prompt.metadata.parameters:
+            return self.get_global_parameters()
+
+        return self.get_prompt_parameters(prompt)
+
+    # pylint: disable=W0102
+    def get_global_parameters(
+        self,
+        default_return_value: JSONObject = {},
+    ) -> JSONObject:
+        """
+        Get the global parameters for the AIConfig. If they're not defined,
+        return a default value ({} unless overridden)
+
+        Args:
+            default_return_value JSONObject - Default value to return if
+                global parameters are not defined.
+        """
+        return self._get_global_parameters_exact() or default_return_value
+
+    # pylint: enable=W0102
+
+    def _get_global_parameters_exact(self) -> JSONObject | None:
+        """
+        Get the global parameters for the AIConfig. This should be the
+        the explicit value (ie: if parameters is None, return None, not {})
+        """
+        return self.metadata.parameters
+
+    # pylint: disable=W0102
+    def get_prompt_parameters(
+        self,
+        prompt: Prompt,
+        default_return_value: JSONObject = {},
+    ) -> JSONObject:
+        """
+        Get the prompt's local parameters. If they're not defined,
+        return a default value ({} unless overridden)
+
+        Args:
+            default_return_value JSONObject - Default value to return if
+                prompt parameters are not defined.
+        """
+        return self._get_prompt_parameters_exact(prompt) or default_return_value
+
+    # pylint: enable=W0102
+
+    def _get_prompt_parameters_exact(
+        self,
+        prompt: Prompt,
+    ) -> JSONObject | None:
+        """
+        Get the global parameters for the AIConfig. This should be the
+        the explicit value (ie: if parameters is None, return None, not {})
+        """
+        if not prompt.metadata:
+            return prompt.metadata
+        return prompt.metadata.parameters
+
+    def set_parameter(self, parameter_name: str, parameter_value: Union[str, JSONObject], prompt_name: Optional[str] = None):
         """
-        Sets a parameter in the AI configuration metadata. If a prompt_name is specified, it adds the parameter to
-        a specific prompt's metadata in the AI configuration. Otherwise, it adds the parameter to the global metadata.
+        Sets a parameter in the AI configuration metadata. If a prompt_name
+        is specified, it adds the parameter to a specific prompt's metadata
+        in the AI configuration. Otherwise, it adds the parameter to the
+        global metadata.
 
         Args:
             parameter_name (str): The name of the parameter.
-            parameter_value: The value of the parameter. It can be more than just a string. It can be a string or a JSON object. For example:
-                {
-                person: {
-                    firstname: "john",
-                    lastname: "smith",
-                    },
-                }
-                Using the parameter in a prompt with handlebars syntax would look like this:
-                "{{person.firstname}} {{person.lastname}}"
-            prompt_name (str, optional): The name of the prompt to add the parameter to. Defaults to None.
+            parameter_value: The value of the parameter. It can be more than
+                just a string. It can be a string or a JSON object. For
+                example:
+                    {
+                    person: {
+                        firstname: "john",
+                        lastname: "smith",
+                        },
+                    }
+                Using the parameter in a prompt with handlebars syntax would
+                look like this:
+                    "{{person.firstname}} {{person.lastname}}"
+            prompt_name (str, optional): The name of the prompt to add the
+                parameter to. Defaults to None.
         """
         target_metadata = self.get_metadata(prompt_name)
+        if not target_metadata:
+            # Technically this check is not needed since the metadata is a
+            # required field in Config while it is not required in Prompt.
+            # Therefore, if it's not defined, we can infer that it should
+            # be a PromptMetadata type, but this is just good robustness
+            # in case we ever change our schema in the future
+            if prompt_name:
+                prompt = self.get_prompt(prompt_name)
+                # check next line not needed since it's already assumed
+                # we got here because target_metadata is None, just being
+                # extra safe
+                if not prompt.metadata:
+                    target_metadata = PromptMetadata(parameters={})
+                    prompt.metadata = target_metadata
+            else:
+                if not self.metadata:
+                    target_metadata = ConfigMetadata()
+                    self.metadata = target_metadata
+
+        assert target_metadata is not None
+        if target_metadata.parameters is None:
+            target_metadata.parameters = {}
         target_metadata.parameters[parameter_name] = parameter_value
 
+    def set_parameters(self, parameters: JSONObject, prompt_name: Optional[str] = None) -> None:
+        """
+        Set the entire parameters dict for either a prompt (if specified)
+        or the AIConfig (if prompt is not specified). It overwrites whatever
+        was previously stored as parameters for the prompt or AIConfig.
+
+        Args:
+            parameters (JSONObject): The entire set of parameters. Ex:
+                {
+                    "city": "New York",
+                    "sort_by": "geographical location",
+                }
+                In this example, we call `set_parameter` twice:
+                    1) set_parameter("city", "New York", prompt_name)
+                    2) set_parameter("sort_by", "geographical location", prompt_name)
+
+            prompt_name (str, optional): The name of the prompt to add the
+                parameters dict to. If none is provided, we update the
+                AIConfig-level parameters instead
+        """
+        # Clear all existing parameters before setting new ones
+        parameter_names_to_delete = []
+        if prompt_name:
+            prompt = self.get_prompt(prompt_name)
+            parameter_names_to_delete = list(self.get_prompt_parameters(prompt).keys())
+        else:
+            parameter_names_to_delete = list(self.get_global_parameters().keys())
+
+        for parameter_name in parameter_names_to_delete:
+            self.delete_parameter(parameter_name, prompt_name)
+
+        for parameter_name, parameter_value in parameters.items():
+            self.set_parameter(parameter_name, parameter_value, prompt_name)
+
     def update_parameter(
         self,
         parameter_name: str,
         parameter_value: str,
         prompt_name: Optional[str] = None,
     ):
         """
@@ -387,14 +582,16 @@
             raise IndexError("Prompt '{}' not found in config, available prompts are:\n {}".format(prompt_name, list(self.prompt_index.keys())))
 
         self.prompt_index[prompt_name] = prompt_data
         # update prompt list
         for i, prompt in enumerate(self.prompts):
             if prompt.name == prompt_name:
                 self.prompts[i] = prompt_data
+                del self.prompt_index[prompt_name]
+                self.prompt_index[prompt_data.name] = prompt_data
                 break
 
     def delete_prompt(self, prompt_name: str):
         """
         Given a prompt name, deletes the prompt from the .aiconfig.
 
         Args:
@@ -624,29 +821,50 @@
             else:
                 raise KeyError(f"Metadata '{key}' does not exist in config.")
 
     # TODO: rename _get_metadata to get_metadata
 
     def add_output(self, prompt_name: str, output: Output, overwrite: bool = False):
         """
-        Add an output to the [rompt with the given name in the AIConfig
+        Add an output to the prompt with the given name in the AIConfig
 
         Args:
             prompt_name (str): The name of the prompt to add the output to.
             output (Output): The output to add.
             overwrite (bool, optional): Overwrites the existing output if True. Otherwise appends the output to the prompt's output list. Defaults to False.
         """
         prompt = self.get_prompt(prompt_name)
         if not prompt:
-            raise IndexError(f"Cannot out output. Prompt '{prompt_name}' not found in config.")
-        if overwrite or not output:
+            raise IndexError(f"Cannot add output. Prompt '{prompt_name}' not found in config.")
+        if not output:
+            raise ValueError(f"Cannot add output to prompt '{prompt_name}'. Output is not defined.")
+        if overwrite:
             prompt.outputs = [output]
         else:
             prompt.outputs.append(output)
 
+    def add_outputs(self, prompt_name: str, outputs: List[Output], overwrite: bool = False):
+        """
+        Add multiple outputs to the prompt with the given name in the AIConfig
+
+        Args:
+            prompt_name (str): The name of the prompt to add the outputs to.
+            outputs (List[Output]): List of outputs to add.
+            overwrite (bool, optional): Overwrites the existing output if True. Otherwise appends the outputs to the prompt's output list. Defaults to False.
+        """
+        prompt = self.get_prompt(prompt_name)
+        if not prompt:
+            raise IndexError(f"Cannot add outputs. Prompt '{prompt_name}' not found in config.")
+        if not outputs:
+            raise ValueError(f"Cannot add outputs. No outputs provided for prompt '{prompt_name}'.")
+        if overwrite:
+            prompt.outputs = outputs
+        else:
+            prompt.outputs.extend(outputs)
+
     def delete_output(self, prompt_name: str):
         """
         Deletes the outputs for the prompt with the given prompt_name.
 
         Args:
             prompt_name (str): The name of the prompt to delete the outputs for.
 
@@ -676,22 +894,14 @@
         """
         Gets the string representing the output from a prompt.
 
         Args:
             prompt (str|Prompt): The name of the prompt or the prompt object.
         """
 
-    def get_prompt_parameters(self, prompt: Prompt):
-        """
-        Gets the prompt's local parameters for a prompt.
-        """
-        if not prompt.metadata:
-            return {}
-        return prompt.metadata.parameters
-
     """
     Library Helpers
     """
 
     def get_global_settings(self, model_name: str):
         """
         Gets the global settings for a model.
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/scripts/aiconfig_cli.py` & `python-aiconfig-1.1.9/src/aiconfig/scripts/aiconfig_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import asyncio
 import logging
 import signal
+import socket
 import subprocess
 import sys
 
 import lastmile_utils.lib.core.api as core_utils
 import result
-from result import Err, Ok, Result
 from aiconfig.editor.server.server import run_backend_server
-
 from aiconfig.editor.server.server_utils import EditServerConfig, ServerMode
+from result import Err, Ok, Result
 
 
 class AIConfigCLIConfig(core_utils.Record):
     log_level: str | int = "WARNING"
 
 
 logging.basicConfig(format=core_utils.LOGGER_FMT)
 LOGGER = logging.getLogger(__name__)
 
 
-async def main(argv: list[str]) -> int:
+async def main_with_args(argv: list[str]) -> int:
     final_result = run_subcommand(argv)
     match final_result:
         case Ok(msg):
             LOGGER.info("Final result: Ok:\n%s", msg)
             return 0
         case Err(e):
             LOGGER.critical("Final result err: %s", e)
             return core_utils.result_to_exitcode(Err(e))
 
 
 def run_subcommand(argv: list[str]) -> Result[str, str]:
     LOGGER.info("Running subcommand")
     subparser_record_types = {"edit": EditServerConfig}
-    main_parser = core_utils.argparsify(AIConfigCLIConfig, subparser_rs=subparser_record_types)
+    main_parser = core_utils.argparsify(AIConfigCLIConfig, subparser_record_types=subparser_record_types)
 
     res_cli_config = core_utils.parse_args(main_parser, argv[1:], AIConfigCLIConfig)
     res_cli_config.and_then(_process_cli_config)
 
     subparser_name = core_utils.get_subparser_name(main_parser, argv[1:])
     LOGGER.info(f"Running subcommand: {subparser_name}")
 
@@ -61,15 +61,40 @@
 def _sigint(procs: list[subprocess.Popen[bytes]]) -> Result[str, str]:
     LOGGER.info("sigint")
     for p in procs:
         p.send_signal(signal.SIGINT)
     return Ok("Sent SIGINT to frontend servers.")
 
 
+def is_port_in_use(port: int) -> bool:
+    """
+    Checks if a port is in use at localhost.
+
+    Creates a temporary connection.
+    Context manager will automatically close the connection
+    """
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex(("localhost", port)) == 0
+
+
 def _run_editor_servers(edit_config: EditServerConfig) -> Result[list[str], str]:
+    port = edit_config.server_port
+
+    while is_port_in_use(port):
+        LOGGER.warning(f"Port {port} is in use. Checking next port.")
+        port += 1
+
+    # Must reconstruct, EditServerConfig is an immutable type (frozen dataclass)
+    edit_config_dict = edit_config.model_dump()
+    edit_config_dict["server_port"] = port
+    edit_config = EditServerConfig(**edit_config_dict)
+
+    LOGGER.warning(f"Using {port}.")
+
+    # Check if server is already running
     LOGGER.info("Running editor servers")
     frontend_procs = _run_frontend_server_background() if edit_config.server_mode in [ServerMode.DEBUG_SERVERS] else Ok([])
     match frontend_procs:
         case Ok(_):
             pass
         case Err(e):
             return Err(e)
@@ -112,10 +137,16 @@
         p2.stdin.write(b"n\n")
     except Exception as e:
         return core_utils.ErrWithTraceback(e)
 
     return Ok([p1, p2])
 
 
+def main() -> int:
+    print("Running main")
+    argv = sys.argv
+    return asyncio.run(main_with_args(argv))
+
+
 if __name__ == "__main__":
-    retcode: int = asyncio.run(main(sys.argv))
+    retcode: int = main()
     sys.exit(retcode)
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/scripts/run_aiconfig.py` & `python-aiconfig-1.1.9/src/aiconfig/scripts/run_aiconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import asyncio
 import logging
 import sys
 
-from result import Ok, Result
-
-
+import lastmile_utils.lib.core.api as core_utils
 from aiconfig.Config import AIConfigRuntime
 from aiconfig.eval.lib import run_aiconfig_helper
-import lastmile_utils.lib.core.api as core_utils
+from result import Ok, Result
 
 logging.basicConfig(format=core_utils.LOGGER_FMT)
 LOGGER = logging.getLogger(__name__)
 
 
 class Settings(core_utils.Record):
     prompt_name: str
@@ -31,17 +29,15 @@
             return core_utils.ErrWithTraceback(e)
 
     # TODO: Need do_async for a different reason: the async expression can't be defined
     # before the do because it's a function of the stuff unwrapped in the do.
     settings = res_settings.unwrap()
     res_aiconfig = _load_aiconfig(settings)
     aiconfig = res_aiconfig.unwrap()
-    final_value = await run_aiconfig_helper(
-        runtime=aiconfig, prompt_name=settings.prompt_name, question=question
-    )
+    final_value = await run_aiconfig_helper(runtime=aiconfig, prompt_name=settings.prompt_name, question=question)
 
     print(final_value.unwrap_or_else(str))
 
     LOGGER.info("Final value: %s", final_value)
 
 
 def _load_settings(settings_path: str) -> Result[Settings, str]:
```

### Comparing `python-aiconfig-1.1.8/src/aiconfig/util/params.py` & `python-aiconfig-1.1.9/src/aiconfig/util/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,15 @@
     """Paramterizes input Prompt"""
     compiler = Compiler()
     template = compiler.compile(raw_prompt)
     resolved_prompt = template(params)
     return resolved_prompt
 
 
-def find_dependencies_in_prompt(
-    prompt_template: str, current_prompt_name: str, prompt_list: List[Prompt]
-) -> Set[str]:
+def find_dependencies_in_prompt(prompt_template: str, current_prompt_name: str, prompt_list: List[Prompt]) -> Set[str]:
     """
     Finds and returns a set of prompt IDs that are dependencies of the given prompt.
 
     :param prompt_template: The prompt template string to search for dependencies.
     :param current_prompt_id: The ID of the current prompt being analyzed.
     :param prompt_list: A list of all prompts in the configuration.
 
@@ -154,17 +152,15 @@
             dependencies.add(prompt.name)
 
     # Exclude references to prompts ahead of the current prompt
     # because including them could result in cyclic dependencies
     return dependencies
 
 
-def get_dependency_graph(
-    root_prompt: Prompt, all_prompts: List[Prompt], prompt_dict: Dict[str, Prompt]
-) -> dict[str, List[str]]:
+def get_dependency_graph(root_prompt: Prompt, all_prompts: List[Prompt], prompt_dict: Dict[str, Prompt]) -> dict[str, List[str]]:
     """
     Generates an upstream dependency graph of prompts in the configuration, with each entry representing only its direct dependencies.
     Traversal is required to identify all upstream dependencies. The specified prompt serves as the root.
 
     :param root_prompt: The starting point for generating the dependency graph.
     :param all_prompts: A list of all prompts in the configuration.
     :param prompt_dict: A dictionary mapping prompt names to prompt objects.
@@ -180,17 +176,15 @@
         :param current_prompt_name: The name of the current prompt being processed.
         """
         if current_prompt_name in visited:
             return
         visited.add(current_prompt_name)
 
         prompt_template = prompt_dict[current_prompt_name].get_raw_prompt_from_config()
-        prompt_dependencies = find_dependencies_in_prompt(
-            prompt_template, current_prompt_name, all_prompts
-        )
+        prompt_dependencies = find_dependencies_in_prompt(prompt_template, current_prompt_name, all_prompts)
 
         for prompt_dependency in prompt_dependencies:
             dependency_graph[current_prompt_name].append(prompt_dependency)
             build_dependency_graph_recursive(prompt_dependency)
 
     build_dependency_graph_recursive(root_prompt.name)
     return dependency_graph
@@ -232,46 +226,36 @@
         return model_parser.get_prompt_template(prompt, aiconfig)
 
     if isinstance(prompt.input, str):
         return prompt.input
     elif isinstance(prompt.input.data, str):
         return prompt.input.data
     else:
-        raise Exception(
-            f"Cannot get prompt template string from prompt: {prompt.input}"
-        )
+        raise Exception(f"Cannot get prompt template string from prompt: {prompt.input}")
 
 
 def collect_prompt_references(current_prompt: Prompt, ai_config: "AIConfigRuntime"):
     """
     Collects references to all other prompts in the AIConfig. Only prompts that appear before the current prompt are collected.
     """
     prompt_references = {}
     for previous_prompt in ai_config.prompts:
         if current_prompt.name == previous_prompt.name:
             break
 
         prompt_input = get_prompt_template(previous_prompt, ai_config)
-        prompt_output = (
-            ai_config.get_output_text(
-                previous_prompt, ai_config.get_latest_output(previous_prompt)
-            )
-            if previous_prompt.outputs
-            else None
-        )
+        prompt_output = ai_config.get_output_text(previous_prompt, ai_config.get_latest_output(previous_prompt)) if previous_prompt.outputs else None
         prompt_references[previous_prompt.name] = {
             "input": prompt_input,
             "output": prompt_output,
         }
     return prompt_references
 
 
-def resolve_prompt(
-    current_prompt: Prompt, input_params: Dict, ai_config: "AIConfigRuntime"
-) -> str:
+def resolve_prompt(current_prompt: Prompt, input_params: Dict, ai_config: "AIConfigRuntime") -> str:
     """
     Parameterizes a prompt using provided parameters, references to other prompts, and parameters stored in config..
     """
     raw_prompt = get_prompt_template(current_prompt, ai_config)
 
     return resolve_prompt_string(current_prompt, input_params, ai_config, raw_prompt)
 
@@ -306,15 +290,15 @@
         str: The parameterized prompt with placeholders replaced by values.
     """
 
     # augment params with prompt-reference params
     augmented_params = collect_prompt_references(current_prompt, ai_config)
 
     # augment params with config-level params
-    augmented_params.update(ai_config.metadata.parameters)
+    augmented_params.update(ai_config.get_global_parameters())
 
     # augment params with prompt level params
     augmented_params.update(ai_config.get_prompt_parameters(current_prompt))
 
     # Combine input_params and augmented_params
     combined_params = dict(augmented_params, **input_params)
```

### Comparing `python-aiconfig-1.1.8/src/python_aiconfig.egg-info/PKG-INFO` & `python-aiconfig-1.1.9/src/python_aiconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aiconfig
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python library for LastMile AI API
 Author-email: Sarmad Qadri <sarmad@lastmileai.dev>
 Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/aiconfig/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: black
 Requires-Dist: flake8
 Requires-Dist: flask-cors
 Requires-Dist: flask[async]
 Requires-Dist: google-generativeai
 Requires-Dist: huggingface_hub
 Requires-Dist: hypothesis==6.91.0
-Requires-Dist: lastmile-utils==0.0.13
+Requires-Dist: lastmile-utils==0.0.14
 Requires-Dist: mock
 Requires-Dist: nest_asyncio
 Requires-Dist: nltk
 Requires-Dist: openai<1.5,>=1.0.0
 Requires-Dist: prompt_toolkit
 Requires-Dist: pybars3
 Requires-Dist: pydantic>=2.1
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: python-aiconfig Version: 1.1.8 Summary: Python
+Metadata-Version: 2.1 Name: python-aiconfig Version: 1.1.9 Summary: Python
 library for LastMile AI API Author-email: Sarmad Qadri
 lastmileai.dev> Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/aiconfig/issues
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: black Requires-Dist: flake8 Requires-Dist:
 flask-cors Requires-Dist: flask[async] Requires-Dist: google-generativeai
 Requires-Dist: huggingface_hub Requires-Dist: hypothesis==6.91.0 Requires-Dist:
-lastmile-utils==0.0.13 Requires-Dist: mock Requires-Dist: nest_asyncio
+lastmile-utils==0.0.14 Requires-Dist: mock Requires-Dist: nest_asyncio
 Requires-Dist: nltk Requires-Dist: openai<1.5,>=1.0.0 Requires-Dist:
 prompt_toolkit Requires-Dist: pybars3 Requires-Dist: pydantic>=2.1 Requires-
 Dist: pylint Requires-Dist: pytest Requires-Dist: pytest-asyncio Requires-Dist:
 python-dotenv Requires-Dist: pyyaml Requires-Dist: requests Requires-Dist:
 result > Full documentation: **[aiconfig.lastmileai.dev](https://
 aiconfig.lastmileai.dev/)** ## Overview AIConfig saves prompts, models and
 model parameters as source control friendly configs. This allows you to iterate
```

### Comparing `python-aiconfig-1.1.8/src/python_aiconfig.egg-info/SOURCES.txt` & `python-aiconfig-1.1.9/src/python_aiconfig.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,33 +7,35 @@
 src/aiconfig/Config.py
 src/aiconfig/__init__.py
 src/aiconfig/callback.py
 src/aiconfig/model_parser.py
 src/aiconfig/registry.py
 src/aiconfig/schema.py
 src/aiconfig/default_parsers/__init__.py
+src/aiconfig/default_parsers/anyscale_endpoint.py
 src/aiconfig/default_parsers/dalle.py
 src/aiconfig/default_parsers/hf.py
 src/aiconfig/default_parsers/openai.py
 src/aiconfig/default_parsers/palm.py
 src/aiconfig/default_parsers/parameterized_model_parser.py
 src/aiconfig/editor/__init__.py
 src/aiconfig/editor/example_aiconfig_model_registry.py
 src/aiconfig/editor/client/__init__.py
+src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/flatted.py
+src/aiconfig/editor/client/node_modules/aiconfig/node_modules/flatted/python/test.py
 src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
 src/aiconfig/editor/client/node_modules/flatted/python/test.py
 src/aiconfig/editor/server/__init__.py
+src/aiconfig/editor/server/queue_iterator.py
 src/aiconfig/editor/server/server.py
 src/aiconfig/editor/server/server_utils.py
 src/aiconfig/editor/server/static/asset-manifest.json
 src/aiconfig/editor/server/static/index.html
 src/aiconfig/editor/server/static/manifest.json
 src/aiconfig/editor/server/static/robots.txt
-src/aiconfig/editor/server/static/__pycache__/__init__.cpython-311.pyc
-src/aiconfig/editor/server/static/static/__pycache__/__init__.cpython-311.pyc
 src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js
 src/aiconfig/editor/server/static/static/js/787.d5fa4d18.chunk.js.map
 src/aiconfig/editor/server/static/static/js/main.612f69d0.js
 src/aiconfig/editor/server/static/static/js/main.612f69d0.js.LICENSE.txt
 src/aiconfig/editor/server/static/static/js/main.612f69d0.js.map
 src/aiconfig/eval/__init__.py
 src/aiconfig/eval/common.py
@@ -45,19 +47,21 @@
 src/aiconfig/scripts/run_aiconfig.py
 src/aiconfig/util/__init__.py
 src/aiconfig/util/config_utils.py
 src/aiconfig/util/params.py
 src/python_aiconfig.egg-info/PKG-INFO
 src/python_aiconfig.egg-info/SOURCES.txt
 src/python_aiconfig.egg-info/dependency_links.txt
+src/python_aiconfig.egg-info/entry_points.txt
 src/python_aiconfig.egg-info/requires.txt
 src/python_aiconfig.egg-info/top_level.txt
 tests/test_chatcompletion_mock_wrapper.py
 tests/test_dataclass.py
 tests/test_eval.py
 tests/test_eval_model_graded_openai.py
 tests/test_library_helpers.py
 tests/test_load_config.py
+tests/test_parameter_api.py
 tests/test_programmatically_create_an_AIConfig.py
 tests/test_registry.py
 tests/test_resolve.py
 tests/test_run_config.py
```

### Comparing `python-aiconfig-1.1.8/tests/test_chatcompletion_mock_wrapper.py` & `python-aiconfig-1.1.9/tests/test_chatcompletion_mock_wrapper.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/tests/test_dataclass.py` & `python-aiconfig-1.1.9/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/tests/test_eval.py` & `python-aiconfig-1.1.9/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/tests/test_eval_model_graded_openai.py` & `python-aiconfig-1.1.9/tests/test_eval_model_graded_openai.py`

 * *Files identical despite different names*

### Comparing `python-aiconfig-1.1.8/tests/test_library_helpers.py` & `python-aiconfig-1.1.9/tests/test_library_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     with four prompts. Prompt 4, which is after the third prompt in the sequence, is expected
     to not be included in the collected references.
     """
 
     # input is an aiconfig with a 4 prompts. Test collects prompt references for the 3rd prompt
     # collect_prompt_references should return references to 1 and 2. 3 is the prompt we are collecting references for, 4 is after. Both are expected to be skipped
     config_relative_path = "aiconfigs/GPT4 Coding Assistant_aiconfig.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     aiconfig = AIConfigRuntime.load(config_absolute_path)
 
     prompt3 = aiconfig.prompts[2]
 
     prompt_references = collect_prompt_references(prompt3, aiconfig)
 
     assert prompt_references == {
```

### Comparing `python-aiconfig-1.1.8/tests/test_load_config.py` & `python-aiconfig-1.1.9/tests/test_load_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,39 +8,33 @@
 from .util.file_path_utils import get_absolute_file_path_from_relative
 
 
 @pytest.mark.asyncio
 async def test_load_basic_chatgpt_query_config(set_temporary_env_vars):
     """Test loading a basic chatgpt query config"""
     config_relative_path = "aiconfigs/basic_chatgpt_query_config.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     config = AIConfigRuntime.load(config_absolute_path)
 
     data_for_inference = await config.resolve("prompt1")
 
     assert data_for_inference == {
         "model": "gpt-3.5-turbo",
         "top_p": 1,
         "temperature": 1,
         "stream": False,
-        "messages": [
-            {"content": "Hi! Tell me 10 cool things to do in NYC.", "role": "user"}
-        ],
+        "messages": [{"content": "Hi! Tell me 10 cool things to do in NYC.", "role": "user"}],
     }
 
 
 @pytest.mark.asyncio
 async def test_load_basic_dalle2_config(set_temporary_env_vars):
     """Test loading a basic Dall-E 2 config"""
     config_relative_path = "aiconfigs/basic_dalle2_config.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     config = AIConfigRuntime.load(config_absolute_path)
 
     data_for_inference = await config.resolve("panda_eating_dumplings")
 
     assert data_for_inference == {
         "model": "dall-e-2",
         "n": 4,
@@ -49,17 +43,15 @@
     }
 
 
 @pytest.mark.asyncio
 async def test_load_basic_dalle3_config(set_temporary_env_vars):
     """Test loading a basic Dall-E 3 config"""
     config_relative_path = "aiconfigs/basic_dalle3_config.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     config = AIConfigRuntime.load(config_absolute_path)
 
     data_for_inference = await config.resolve("panda_eating_dumplings")
 
     assert data_for_inference == {
         "model": "dall-e-3",
         "n": 1,
@@ -68,17 +60,15 @@
     }
 
 
 @pytest.mark.asyncio
 async def test_chained_gpt_config(set_temporary_env_vars):
     """Test loading a chained gpt config and resolving it, with chat context enabled"""
     config_relative_path = "aiconfigs/chained_gpt_config.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     config = AIConfigRuntime.load(config_absolute_path)
 
     data_for_inference1 = await config.resolve("prompt1")
 
     assert data_for_inference1 == {
         "model": "gpt-3.5-turbo",
         "top_p": 1,
@@ -115,17 +105,15 @@
 
 @pytest.mark.asyncio
 async def test_resolve_system_prompt():
     """
     Resolves a system prompt with a provided parameter
     """
     config_relative_path = "aiconfigs/system_prompt_parameters_config.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     config = AIConfigRuntime.load(config_absolute_path)
 
     data_for_inference = await config.resolve("prompt1", {"system": "skip odd numbers"})
     assert data_for_inference == {
         "temperature": 1,
         "model": "gpt-3.5-turbo",
         "top_p": 1,
```

### Comparing `python-aiconfig-1.1.8/tests/test_programmatically_create_an_AIConfig.py` & `python-aiconfig-1.1.9/tests/test_programmatically_create_an_AIConfig.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import pytest
 from aiconfig.Config import AIConfigRuntime
 from aiconfig.util.config_utils import extract_override_settings
 
-from aiconfig.schema import (
-    AIConfig,
-    ConfigMetadata,
-    ExecuteResult,
-    ModelMetadata,
-    Prompt,
-    PromptMetadata,
-)
+from aiconfig.schema import AIConfig, ConfigMetadata, ExecuteResult, ModelMetadata, Prompt, PromptMetadata
 
 
 @pytest.fixture
 def ai_config_runtime():
     runtime = AIConfigRuntime.create("Untitled AIConfig")
     return runtime
 
@@ -64,17 +57,15 @@
 def test_delete_nonexistent_model(ai_config: AIConfig):
     """
     Test deleting a non-existent model (expect an exception).
     """
     non_existent_model = "non_existent_model"
 
     # Ensure trying to delete a non-existent model raises an exception
-    with pytest.raises(
-        Exception, match=f"Model '{non_existent_model}' does not exist."
-    ):
+    with pytest.raises(Exception, match=f"Model '{non_existent_model}' does not exist."):
         ai_config.delete_model(non_existent_model)
 
 
 def test_add_prompt_to_config(ai_config_runtime: AIConfigRuntime):
     """
     Test adding a prompt to the AIConfig.
     """
@@ -234,115 +225,25 @@
     prompt_name = "nonexistent_prompt"
 
     # Ensure that attempting to retrieve metadata for a non-existent prompt raises an exception
     with pytest.raises(IndexError, match=f"Prompt '{prompt_name}' not found in config"):
         config.get_metadata(prompt_name)
 
 
-def test_delete_nonexistent_parameter(ai_config_runtime: AIConfigRuntime):
-    """
-    Test deleting a nonexistent parameter.
-    """
-    config = ai_config_runtime
-    parameter_name_to_delete = "param1"
-    config.add_prompt(
-        "prompt1",
-        Prompt(
-            name="prompt_name",
-            input="This is a prompt",
-            metadata=PromptMetadata(model="fakemodel"),
-        ),
-    )
-
-    # Ensure deleting a nonexistent parameter raises a KeyError
-    with pytest.raises(
-        KeyError, match=f"Parameter '{parameter_name_to_delete}' does not exist."
-    ):
-        config.delete_parameter(parameter_name_to_delete)
-
-
 @pytest.fixture
 def ai_config():
     config = AIConfig(
         name="Untitled AIConfig",
         schema_version="latest",
         metadata=ConfigMetadata(),
         prompts=[],
     )
     return config
 
 
-def test_set_global_parameter(ai_config: AIConfig):
-    """
-    Test setting a global parameter.
-    """
-    parameter_name = "global_param"
-    parameter_value = "global_value"
-
-    ai_config.set_parameter(parameter_name, parameter_value, prompt_name=None)
-
-    # Ensure the global parameter is set correctly
-    assert ai_config.metadata.parameters[parameter_name] == parameter_value
-
-
-def test_set_parameter_for_prompt(ai_config: AIConfig):
-    """
-    Test setting a parameter for a specific prompt.
-    """
-    prompt_name = "prompt1"
-    parameter_name = "prompt_param"
-    parameter_value = "prompt_value"
-
-    # Create a sample prompt for testing
-    prompt_data = Prompt(
-        name=prompt_name,
-        input="This is a prompt",
-        metadata=PromptMetadata(model="fakemodel"),
-    )
-    ai_config.add_prompt(prompt_name, prompt_data)
-
-    ai_config.set_parameter(parameter_name, parameter_value, prompt_name=prompt_name)
-
-    # Ensure the parameter is set for the specific prompt
-    assert (
-        ai_config.prompt_index[prompt_name].metadata.parameters[parameter_name]
-        == parameter_value
-    )
-    assert ai_config.prompts[0].metadata.parameters[parameter_name] == parameter_value
-
-
-def test_update_existing_parameter(ai_config: AIConfig):
-    """
-    Test updating an existing parameter.
-    """
-    parameter_name = "existing_param"
-    initial_value = "initial_value"
-    updated_value = "updated_value"
-
-    ai_config.set_parameter(parameter_name, initial_value, prompt_name=None)
-    ai_config.update_parameter(parameter_name, updated_value, prompt_name=None)
-
-    # Ensure the existing parameter is updated correctly
-    assert ai_config.metadata.parameters[parameter_name] == updated_value
-
-
-def test_delete_existing_parameter(ai_config: AIConfig):
-    """
-    Test deleting an existing parameter.
-    """
-    parameter_name_to_delete = "param_to_delete"
-    parameter_value = "param_value"
-
-    ai_config.set_parameter(parameter_name_to_delete, parameter_value, prompt_name=None)
-    ai_config.delete_parameter(parameter_name_to_delete, prompt_name=None)
-
-    # Ensure the existing parameter is deleted correctly
-    assert parameter_name_to_delete not in ai_config.metadata.parameters
-
-
 def test_load_saved_config(tmp_path):
     """
     Test loading a saved AIConfig from a JSON file.
     """
     config_runtime = AIConfigRuntime.create("My AIConfig")
 
     # Create a configuration-level parameter
@@ -364,17 +265,16 @@
 
     loaded_config = AIConfigRuntime.load(json_config_filepath)
 
     # Ensure the loaded AIConfig contains the expected data
     assert loaded_config.name == "My AIConfig"
     assert loaded_config.metadata.parameters == {"config_param": "config_value"}
     assert "prompt1" in loaded_config.prompt_index
-    assert loaded_config.prompt_index["prompt1"].metadata.parameters == {
-        "prompt_param": "prompt_value"
-    }
+    assert loaded_config.prompt_index["prompt1"].metadata is not None
+    assert loaded_config.prompt_index["prompt1"].metadata.parameters == {"prompt_param": "prompt_value"}
 
 
 def test_set_config_name(ai_config_runtime: AIConfigRuntime):
     ai_config_runtime.set_name("My AIConfig")
     assert ai_config_runtime.name == "My AIConfig"
 
 
@@ -410,17 +310,15 @@
     ai_config_runtime.add_prompt(prompt2.name, prompt2)
     ai_config_runtime.delete_prompt("GreetingPrompt")
     retrieved_prompt = ai_config_runtime.get_prompt("GoodbyePrompt")
     assert retrieved_prompt == prompt2
 
 
 def test_get_prompt_nonexistent(ai_config_runtime: AIConfigRuntime):
-    with pytest.raises(
-        IndexError, match=r"Prompt 'GreetingPrompt' not found in config"
-    ):
+    with pytest.raises(IndexError, match=r"Prompt 'GreetingPrompt' not found in config"):
         ai_config_runtime.get_prompt("GreetingPrompt")
 
 
 def test_update_model_for_ai_config(ai_config_runtime: AIConfigRuntime):
     """Test updating model without a specific prompt."""
     # New model name, new settings --> update
     model_name = "testmodel"
@@ -449,77 +347,75 @@
     pytest.warns(match=f"No prompt name was given to update the model name to '{new_model_name}'.")
     assert ai_config_runtime.metadata.models is not None
     assert ai_config_runtime.metadata.models[new_model_name] == {}
 
 
 def test_update_model_for_prompt(ai_config_runtime: AIConfigRuntime):
     """Test updating model for a specific prompt."""
-    #New model name, new settings, no prompt metadata --> update
-    prompt1 = Prompt(
-        name="GreetingPrompt",
-        input="Hello, how are you?"
-    )
+    # New model name, new settings, no prompt metadata --> update
+    prompt1 = Prompt(name="GreetingPrompt", input="Hello, how are you?")
     ai_config_runtime.add_prompt(prompt1.name, prompt1)
     model_name = "testmodel"
     settings = {"topP": 0.9}
     ai_config_runtime.update_model(model_name, settings, prompt1.name)
     prompt = ai_config_runtime.get_prompt(prompt1.name)
     assert prompt.metadata is not None
     assert prompt.metadata.model == ModelMetadata(name=model_name, settings=settings)
-    
+
     # New model name, no settings --> update name only
     new_model_name = "testmodel_new_name"
     ai_config_runtime.update_model(new_model_name, None, prompt1.name)
     prompt = ai_config_runtime.get_prompt(prompt1.name)
     assert prompt.metadata is not None
     assert prompt.metadata.model == ModelMetadata(name=new_model_name, settings=settings)
-    
+
     # Same model name, new settings --> update settings only
     settings = {"topP": 0.9}
     ai_config_runtime.update_model(new_model_name, settings, prompt1.name)
     prompt = ai_config_runtime.get_prompt(prompt1.name)
     assert prompt.metadata is not None
     assert prompt.metadata.model == ModelMetadata(name=new_model_name, settings=settings)
-    
+
     # New name, no settings, prompt with model name as string --> update
     prompt2 = Prompt(
         name="GreetingPromptModelAsStr",
         input="Hello, how are you?",
-        metadata=PromptMetadata(model= "some_random_model"),
+        metadata=PromptMetadata(model="some_random_model"),
     )
     ai_config_runtime.add_prompt(prompt2.name, prompt2)
     new_name_again = "testmodel_new_name_model_as_str"
     ai_config_runtime.update_model(new_name_again, None, prompt2.name)
     prompt = ai_config_runtime.get_prompt(prompt2.name)
     assert prompt.metadata is not None
     assert prompt.metadata.model == ModelMetadata(name=new_name_again, settings={})
 
     # New name, no settings, prompt with metadata but no model --> update
     tags = ["my_fancy_tags"]
     prompt3 = Prompt(
         name="GreetingsNumber3",
         input="Hello, how are you?",
-        metadata=PromptMetadata(tags= tags),
+        metadata=PromptMetadata(tags=tags),
     )
     ai_config_runtime.add_prompt(prompt3.name, prompt3)
     new_name_3 = "new_name_number_3"
     ai_config_runtime.update_model(new_name_3, None, prompt3.name)
     prompt = ai_config_runtime.get_prompt(prompt3.name)
     assert prompt.metadata is not None
     assert prompt.metadata.model == ModelMetadata(name=new_name_3, settings={})
     assert prompt.metadata.tags == tags
 
+
 def test_update_model_with_invalid_arguments(ai_config_runtime: AIConfigRuntime):
     """Test trying to update model with invalid arguments."""
     with pytest.raises(
         ValueError,
         match=r"Cannot update model. Either model name or model settings must be specified.",
     ):
         ai_config_runtime.update_model(model_name=None, settings=None)
-    
+
     with pytest.raises(
         ValueError,
         match=r"Cannot update model. There are two things you are trying:",
     ):
         ai_config_runtime.update_model(model_name=None, settings={"top": 0.9}, prompt_name=None)
 
 
@@ -532,85 +428,219 @@
     ai_config_runtime.delete_metadata("testkey")
 
     assert hasattr(ai_config_runtime.get_metadata(), "testkey") is False
 
 
 def test_set_and_delete_metadata_ai_config_prompt(ai_config_runtime: AIConfigRuntime):
     """Test deleting a non-existent metadata key at the AIConfig level."""
-    prompt1 = Prompt(
+    prompt = Prompt(
         name="GreetingPrompt",
         input="Hello, how are you?",
         metadata=PromptMetadata(model="fakemodel"),
     )
-    ai_config_runtime.add_prompt(prompt1.name, prompt1)
+    ai_config_runtime.add_prompt(prompt.name, prompt)
     ai_config_runtime.set_metadata("testkey", "testvalue", "GreetingPrompt")
 
-    assert (
-        ai_config_runtime.get_prompt("GreetingPrompt").metadata.testkey == "testvalue"
-    )
+    assert ai_config_runtime.get_prompt("GreetingPrompt").metadata.testkey == "testvalue"
 
     ai_config_runtime.delete_metadata("testkey", "GreetingPrompt")
 
-    assert (
-        hasattr(ai_config_runtime.get_prompt("GreetingPrompt").metadata, "testkey")
-        is False
-    )
+    assert hasattr(ai_config_runtime.get_prompt("GreetingPrompt").metadata, "testkey") is False
 
 
 def test_add_output_existing_prompt_no_overwrite(ai_config_runtime: AIConfigRuntime):
     """Test adding an output to an existing prompt without overwriting."""
-    prompt1 = Prompt(
+    prompt = Prompt(
         name="GreetingPrompt",
         input="Hello, how are you?",
         metadata=PromptMetadata(model="fakemodel"),
     )
-    ai_config_runtime.add_prompt(prompt1.name, prompt1)
+    ai_config_runtime.add_prompt(prompt.name, prompt)
     test_result = ExecuteResult(
         output_type="execute_result",
-        execution_count=0.0,
-        data={"role": "assistant", "content": "test output"},
-        metadata={"finish_reason": "stop"},
+        execution_count=0,
+        data="test output",
+        metadata={"raw_response": {"role": "assistant", "content": "test output"}},
     )
     ai_config_runtime.add_output("GreetingPrompt", test_result)
 
     assert ai_config_runtime.get_latest_output("GreetingPrompt") == test_result
 
     test_result2 = ExecuteResult(
         output_type="execute_result",
-        execution_count=0.0,
-        data={"role": "assistant", "content": "test output"},
-        metadata={"finish_reason": "stop"},
+        execution_count=0,
+        data="test output",
+        metadata={"raw_response": {"role": "assistant", "content": "test output for second time"}},
     )
+
     ai_config_runtime.add_output("GreetingPrompt", test_result2)
     assert ai_config_runtime.get_latest_output("GreetingPrompt") == test_result2
 
     ai_config_runtime.delete_output("GreetingPrompt")
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == None
+
+
+def test_add_outputs_existing_prompt_no_overwrite(ai_config_runtime: AIConfigRuntime):
+    """Test adding outputs to an existing prompt without overwriting."""
+    original_result = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="original result",
+        metadata={"raw_response": {"role": "assistant", "content": "original result"}},
+    )
+    prompt = Prompt(
+        name="GreetingPrompt",
+        input="Hello, how are you?",
+        metadata=PromptMetadata(model="fakemodel"),
+        outputs=[original_result],
+    )
+    ai_config_runtime.add_prompt(prompt.name, prompt)
+
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == original_result
+
+    test_result1 = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="test output 1",
+        metadata={"raw_response": {"role": "assistant", "content": "test output 1"}},
+    )
+    test_result2 = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="test output 2",
+        metadata={"raw_response": {"role": "assistant", "content": "test output 2"}},
+    )
+    ai_config_runtime.add_outputs("GreetingPrompt", [test_result1, test_result2])
+
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == test_result2
+    assert prompt.outputs == [original_result, test_result1, test_result2]
+
+
+def test_add_outputs_existing_prompt_with_overwrite(ai_config_runtime: AIConfigRuntime):
+    """Test adding outputs to an existing prompt with overwriting."""
+    original_result = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="original result",
+        metadata={"raw_response": {"role": "assistant", "content": "original result"}},
+    )
+    prompt = Prompt(
+        name="GreetingPrompt",
+        input="Hello, how are you?",
+        metadata=PromptMetadata(model="fakemodel"),
+        outputs=[original_result],
+    )
+    ai_config_runtime.add_prompt(prompt.name, prompt)
+
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == original_result
+
+    test_result1 = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="test output 1",
+        metadata={"raw_response": {"role": "assistant", "content": "test output 1"}},
+    )
+    test_result2 = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="test output 2",
+        metadata={"raw_response": {"role": "assistant", "content": "test output 2"}},
+    )
+    ai_config_runtime.add_outputs("GreetingPrompt", [test_result1, test_result2], True)
+
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == test_result2
+    assert prompt.outputs == [test_result1, test_result2]
 
+
+def test_add_undefined_outputs_to_prompt(ai_config_runtime: AIConfigRuntime):
+    """Test for adding undefined outputs to an existing prompt with/without overwriting. Should result in an error."""
+    prompt = Prompt(
+        name="GreetingPrompt",
+        input="Hello, how are you?",
+        metadata=PromptMetadata(model="fakemodel"),
+    )
+    ai_config_runtime.add_prompt(prompt.name, prompt)
     assert ai_config_runtime.get_latest_output("GreetingPrompt") == None
+    # Case 1: No outputs, overwrite param not defined
+    with pytest.raises(
+        ValueError,
+        match=r"Cannot add outputs. No outputs provided for prompt 'GreetingPrompt'.",
+    ):
+        ai_config_runtime.add_outputs("GreetingPrompt", [])
+    # Case 2: No outputs, overwrite param set to True
+    with pytest.raises(
+        ValueError,
+        match=r"Cannot add outputs. No outputs provided for prompt 'GreetingPrompt'.",
+    ):
+        ai_config_runtime.add_outputs("GreetingPrompt", [], True)
+
+
+def test_add_output_existing_prompt_overwrite(ai_config_runtime: AIConfigRuntime):
+    """Test adding an output to an existing prompt with overwriting."""
+    original_output = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="original output",
+        metadata={"raw_response": {"role": "assistant", "content": "original output"}},
+    )
+    prompt = Prompt(
+        name="GreetingPrompt",
+        input="Hello, how are you?",
+        metadata=PromptMetadata(model="fakemodel"),
+        outputs=[original_output],
+    )
+    ai_config_runtime.add_prompt(prompt.name, prompt)
+    # check that the original_output is there
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == original_output
+    expected_output = ExecuteResult(
+        output_type="execute_result",
+        execution_count=0,
+        data="original output",
+        metadata={"raw_response": {"role": "assistant", "content": "original output"}},
+    )
+    # overwrite the original_output
+    ai_config_runtime.add_output("GreetingPrompt", expected_output, True)
+    assert ai_config_runtime.get_latest_output("GreetingPrompt") == expected_output
+
+
+def test_add_undefined_output_to_prompt(ai_config_runtime: AIConfigRuntime):
+    """Test for adding an undefined output to a prompt with/without overwriting. Should result in an error."""
+    prompt = Prompt(
+        name="GreetingPrompt",
+        input="Hello, how are you?",
+        metadata=PromptMetadata(model="fakemodel"),
+    )
+    ai_config_runtime.add_prompt(prompt.name, prompt)
+    # Case 1: No output, overwrite param not defined
+    with pytest.raises(
+        ValueError,
+        match=r"Cannot add output to prompt 'GreetingPrompt'. Output is not defined.",
+    ):
+        ai_config_runtime.add_output("GreetingPrompt", None)
+    # Case 2: No output, overwrite param set to True
+    with pytest.raises(
+        ValueError,
+        match=r"Cannot add output to prompt 'GreetingPrompt'. Output is not defined.",
+    ):
+        ai_config_runtime.add_output("GreetingPrompt", None, True)
 
 
 def test_extract_override_settings(ai_config_runtime: AIConfigRuntime):
     initial_settings = {"topP": 0.9}
 
     # Test Case 1: No global setting, Expect an override
-    override = extract_override_settings(
-        ai_config_runtime, initial_settings, "testmodel"
-    )
+    override = extract_override_settings(ai_config_runtime, initial_settings, "testmodel")
     assert override == {"topP": 0.9}
 
     # Test Case 2: Global Settings differ, expect override
     ai_config_runtime.add_model("testmodel", {"topP": 0.8})
-    override = extract_override_settings(
-        ai_config_runtime, initial_settings, "testmodel"
-    )
+    override = extract_override_settings(ai_config_runtime, initial_settings, "testmodel")
     assert override == {"topP": 0.9}
 
     # Test Case 3: Global Settings match settings, expect no override
     ai_config_runtime.update_model(model_name="testmodel", settings={"topP": 0.9})
-    override = extract_override_settings(
-        ai_config_runtime, initial_settings, "testmodel"
-    )
+    override = extract_override_settings(ai_config_runtime, initial_settings, "testmodel")
     assert override == {}
 
     # Test Case 4: Global settings defined and empty settings defined. Expect no override
     override = extract_override_settings(ai_config_runtime, {}, "testmodel")
     assert override == {}
```

### Comparing `python-aiconfig-1.1.8/tests/test_registry.py` & `python-aiconfig-1.1.9/tests/test_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,15 @@
         assert ModelParserRegistry.get_model_parser("id1") == mock_model_parser
         assert ModelParserRegistry.get_model_parser("id2") == mock_model_parser
 
     def test_register_single_model_parser(self):
         mock_model_parser = MockModelParser()
         ModelParserRegistry.register_model_parser(mock_model_parser)
 
-        assert (
-            ModelParserRegistry.get_model_parser(mock_model_parser.id())
-            == mock_model_parser
-        )
+        assert ModelParserRegistry.get_model_parser(mock_model_parser.id()) == mock_model_parser
 
     def test_register_multiple_model_parsers_with_different_ids(self):
         # Create model parsers
         model_parser_1 = MockModelParser()
         model_parser_2 = MockModelParser()
 
         # Register the model parsers with different IDs
@@ -92,39 +89,33 @@
                 "input": "I am the prompt's input",
                 "metadata": {"model": "model-7"},
             }
         )
         ai_config_runtime.add_prompt(prompt.name, prompt)
 
         # Retrieve the model parser for the Prompt
-        retrieved_parser = ModelParserRegistry.get_model_parser_for_prompt(
-            prompt, ai_config_runtime
-        )
+        retrieved_parser = ModelParserRegistry.get_model_parser_for_prompt(prompt, ai_config_runtime)
 
         # Assert that the retrieved model parser is the same as the registered one
         assert retrieved_parser == model_parser
 
-    def test_retrieve_model_parser_for_prompt_with_nonexistent_model(
-        self, ai_config_runtime: AIConfigRuntime
-    ):
+    def test_retrieve_model_parser_for_prompt_with_nonexistent_model(self, ai_config_runtime: AIConfigRuntime):
         # Create a Prompt object with a model name that is not registered
         prompt = Prompt(
             **{
                 "name": "prompt1",
                 "input": "I am the prompt's input",
                 "metadata": {"model": "test_model"},
             }
         )
         ai_config_runtime.add_prompt(prompt.name, prompt)
 
         # Attempt to retrieve a model parser for the Prompt
         with pytest.raises(KeyError):
-            ModelParserRegistry.get_model_parser_for_prompt(
-                prompt, ai_config_runtime
-            ).id()
+            ModelParserRegistry.get_model_parser_for_prompt(prompt, ai_config_runtime).id()
 
     def test_remove_model_parser(self):
         # Create a model parser
         model_parser = MockModelParser()
 
         # Register the model parser
         ModelParserRegistry.register_model_parser(model_parser, ids=["model-8"])
```

### Comparing `python-aiconfig-1.1.8/tests/test_resolve.py` & `python-aiconfig-1.1.9/tests/test_resolve.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,17 @@
 
 @pytest.mark.asyncio
 async def test_resolve_default_model_config_with_openai_parser():
     """
     Test that the default model config is resolved correctly. `basic_default_model_aiconfig.json` is an aiconfig with 1 prompt that has no settings or model defined besides the default.
     """
     config_relative_path = "aiconfigs/basic_default_model_aiconfig.json"
-    config_absolute_path = get_absolute_file_path_from_relative(
-        __file__, config_relative_path
-    )
+    config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
     config = AIConfigRuntime.load(config_absolute_path)
     resolved_params = await config.resolve("prompt1")
 
     assert resolved_params == {
-        "messages": [
-            {"content": "Hi! Tell me 10 cool things to do in NYC.", "role": "user"}
-        ],
+        "messages": [{"content": "Hi! Tell me 10 cool things to do in NYC.", "role": "user"}],
         "model": "gpt-3.5-turbo",
         "temperature": 1,
         "top_p": 1,
     }
```

### Comparing `python-aiconfig-1.1.8/tests/test_run_config.py` & `python-aiconfig-1.1.9/tests/test_run_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 
 @pytest.mark.asyncio
 async def test_load_parametrized_data_config(set_temporary_env_vars):
     """Test loading a parametrized data config and resolving it
 
     Config has 2 prompts. Prompt2 uses prompt1.output in its input.
     """
-    with patch.object(
-        openai.chat.completions, "create", side_effect=mock_openai_chat_completion
-    ):
+    with patch.object(openai.chat.completions, "create", side_effect=mock_openai_chat_completion):
         config_relative_path = "aiconfigs/parametrized_data_config.json"
-        config_absolute_path = get_absolute_file_path_from_relative(
-            __file__, config_relative_path
-        )
+        config_absolute_path = get_absolute_file_path_from_relative(__file__, config_relative_path)
         config = AIConfigRuntime.load(config_absolute_path)
 
         prompt1_params = {
             "sql_language": "MySQL",
             "output_data": "total revenue from sales for each product category",
             "table_relationships": "Employees are related to Departments through the 'DepartmentID' field.",
         }
```

