# Comparing `tmp/speechless-0.8.0.tar.gz` & `tmp/speechless-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechless-0.8.0.tar", last modified: Sat Feb  3 08:50:15 2024, max compression
+gzip compressed data, was "speechless-0.9.0.tar", last modified: Tue Apr 23 02:28:48 2024, max compression
```

## Comparing `speechless-0.8.0.tar` & `speechless-0.9.0.tar`

### file list

```diff
@@ -1,305 +1,449 @@
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.407728 speechless-0.8.0/
--rw-r--r--   0 sujiangwen   (501) staff       (20)    11357 2023-09-17 11:16:20.000000 speechless-0.8.0/LICENSE
--rw-r--r--   0 sujiangwen   (501) staff       (20)    31079 2024-02-03 08:50:15.407515 speechless-0.8.0/PKG-INFO
--rw-r--r--   0 sujiangwen   (501) staff       (20)    30209 2024-01-27 03:56:14.000000 speechless-0.8.0/README.md
--rw-r--r--   0 sujiangwen   (501) staff       (20)      521 2024-02-03 08:49:49.000000 speechless-0.8.0/pyproject.toml
--rw-r--r--   0 sujiangwen   (501) staff       (20)       38 2024-02-03 08:50:15.407780 speechless-0.8.0/setup.cfg
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4100 2023-11-04 02:56:31.000000 speechless-0.8.0/setup.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.346064 speechless-0.8.0/speechless/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)       88 2024-01-21 16:49:42.000000 speechless-0.8.0/speechless/__version__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.346978 speechless-0.8.0/speechless/agents/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 12:01:05.000000 speechless-0.8.0/speechless/agents/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.348867 speechless-0.8.0/speechless/agents/algorithms/
--rw-r--r--   0 sujiangwen   (501) staff       (20)    17343 2023-11-15 15:49:42.000000 speechless-0.8.0/speechless/agents/algorithms/DFS.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8058 2023-11-05 13:34:43.000000 speechless-0.8.0/speechless/agents/algorithms/Tree.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/algorithms/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      931 2023-11-04 14:21:42.000000 speechless-0.8.0/speechless/agents/algorithms/base_env.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1233 2023-11-04 14:21:42.000000 speechless-0.8.0/speechless/agents/algorithms/base_search.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3656 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/algorithms/rank_candidate.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8203 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/algorithms/single_chain.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.351140 speechless-0.8.0/speechless/agents/llms/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)       43 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/base_io.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4899 2023-12-31 14:55:44.000000 speechless-0.8.0/speechless/agents/llms/chatgpt_function_model.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6031 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/compression.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6939 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/llama_model.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9816 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/model_adapter.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2359 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/retriever.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7110 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/tool_llama_lora_model.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8706 2023-11-05 08:23:36.000000 speechless-0.8.0/speechless/agents/llms/tool_llama_model.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9184 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/llms/utils.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    12907 2023-11-12 20:04:28.000000 speechless-0.8.0/speechless/agents/llms/vllm_model.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.352078 speechless-0.8.0/speechless/agents/prompts/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1858 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/prompts/ReAct_prompts.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      528 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/prompts/Tree_search_prompts.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/prompts/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      838 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/prompts/rank_prompts.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    10925 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/prompts/tool_conversation.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.353168 speechless-0.8.0/speechless/agents/rapidapi/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/rapidapi/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7812 2023-11-08 11:03:48.000000 speechless-0.8.0/speechless/agents/rapidapi/rapidapi_server.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    36282 2023-11-21 09:58:04.000000 speechless-0.8.0/speechless/agents/rapidapi/run_rapidapi.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6825 2023-11-05 23:59:20.000000 speechless-0.8.0/speechless/agents/rapidapi/toolbench_cache.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.355261 speechless-0.8.0/speechless/agents/tooleval/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5237 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/automatic_eval_sample.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1283 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/convert_answers.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8517 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/convert_to_answer_format.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.355540 speechless-0.8.0/speechless/agents/tooleval/dataset/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/dataset/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7879 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/eval_and_update_leaderboard.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8749 2023-11-10 13:22:46.000000 speechless-0.8.0/speechless/agents/tooleval/eval_pass_rate.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    13767 2023-11-12 19:12:12.000000 speechless-0.8.0/speechless/agents/tooleval/eval_preference.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.356143 speechless-0.8.0/speechless/agents/tooleval/evaluation/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      139 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluation/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    10248 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluation/dataclass.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1292 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluation/methodcls.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2478 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluation/usereval.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.356324 speechless-0.8.0/speechless/agents/tooleval/evaluators/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      794 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.357313 speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      633 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4534 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/base.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9367 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/rtl.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7837 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/tooleval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2534 2023-12-31 14:55:44.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/utils.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5457 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/tooleval/evaluators_comparison.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8591 2023-11-10 13:22:46.000000 speechless-0.8.0/speechless/agents/tooleval/utils.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6432 2023-11-04 13:09:17.000000 speechless-0.8.0/speechless/agents/utils.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.358159 speechless-0.8.0/speechless/api/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3011 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/client.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.359221 speechless-0.8.0/speechless/api/llms/
--rw-r--r--   0 sujiangwen   (501) staff       (20)       99 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/llms/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1292 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/llms/base_llm.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7556 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/llms/exllama.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7416 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/llms/huggingface.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7935 2023-11-05 09:16:27.000000 speechless-0.8.0/speechless/api/llms/vllm.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.359736 speechless-0.8.0/speechless/api/protocol/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/protocol/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6712 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/protocol/openai.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3144 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/protocol/sampling_params.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    13969 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/api/server.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3796 2024-01-06 02:32:59.000000 speechless-0.8.0/speechless/api/settings.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.360647 speechless-0.8.0/speechless/chat/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)       72 2024-01-21 04:46:16.000000 speechless-0.8.0/speechless/chat/__main__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.361684 speechless-0.8.0/speechless/chat/app/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      167 2024-01-24 00:08:37.000000 speechless-0.8.0/speechless/chat/app/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3127 2024-01-24 00:08:37.000000 speechless-0.8.0/speechless/chat/app/app.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3314 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/app/session_manager.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1047 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/app/session_store.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.362681 speechless-0.8.0/speechless/chat/ces/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      185 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/ces/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/ces/client.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3085 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/ces/common.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    19123 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/ces/environment.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    18247 2024-01-24 00:08:37.000000 speechless-0.8.0/speechless/chat/chat.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.363453 speechless-0.8.0/speechless/chat/config/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/config/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9187 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/config/config_mgt.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1546 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/config/module_config.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.363744 speechless-0.8.0/speechless/chat/logging/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4322 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/logging/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.365726 speechless-0.8.0/speechless/chat/memory/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      228 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2903 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/attachment.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2586 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/conversation.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1595 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/memory.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    10411 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/plugin.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3338 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/post.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2523 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/round.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      150 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/memory/type_vars.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.366197 speechless-0.8.0/speechless/chat/misc/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/misc/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3042 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/misc/component_registry.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      564 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/misc/example.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.366804 speechless-0.8.0/speechless/chat/session/
--rw-r--r--   0 sujiangwen   (501) staff       (20)       28 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/session/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8825 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/session/session.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2146 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/utils.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.367177 speechless-0.8.0/speechless/chat/workspace/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/workspace/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      702 2024-01-19 22:20:56.000000 speechless-0.8.0/speechless/chat/workspace/workspace.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.369869 speechless-0.8.0/speechless/eval/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-26 10:21:46.000000 speechless-0.8.0/speechless/eval/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2065 2024-01-26 08:42:38.000000 speechless-0.8.0/speechless/eval/__main__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    15929 2023-12-31 14:55:44.000000 speechless-0.8.0/speechless/eval/async_openai.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    15990 2023-12-27 07:43:41.000000 speechless-0.8.0/speechless/eval/bigcode_eval.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.371343 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1654 2023-12-15 00:18:34.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/arguments.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2711 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/base.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4214 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/evaluator.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6115 2023-12-15 00:18:34.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/generation.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.376849 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1632 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4142 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/apps.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    10884 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_code_to_text.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4050 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_text_to_text.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3995 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/conala.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3914 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/concode.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.377568 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7446 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/codexglue_code_to_text_bleu.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    13459 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/diff_eval.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.383267 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3170 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/containerized_eval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1164 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cpp.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2102 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cs.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2235 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_dlang.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1112 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_go.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1498 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_java.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1562 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_javascript.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      582 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_julia.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      390 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_lua.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      446 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_php.py
--rwxr-xr-x   0 sujiangwen   (501) staff       (20)      469 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_pl.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      461 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_python.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1404 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_r.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1225 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_racket.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1361 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ruby.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1644 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_rust.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1303 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_scala.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      578 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_sh.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      864 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_swift.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      911 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ts.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2692 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/evaluation.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4829 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/generic_eval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1325 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/libeval.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.383816 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2803 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2877 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/module_test.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      548 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/single_experiment_pass_k.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.384520 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4410 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/pal_code_exec.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6186 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/python_executor.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7069 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/ds1000.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7496 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/gsm.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5335 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/humaneval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    30239 2023-12-16 08:26:01.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8807 2023-12-31 14:55:44.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack_openai.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5903 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_humaneval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5267 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_wizard_humaneval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5319 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/mbpp.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7066 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/multiple.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5348 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/parity.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4740 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/python_bugs.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5146 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/quixbugs.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7436 2023-12-13 16:02:27.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/recode.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    15958 2023-12-29 10:34:15.000000 speechless-0.8.0/speechless/eval/bigcode_eval_qwen/utils.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.385438 speechless-0.8.0/speechless/eval/evalplus/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      120 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.386552 speechless-0.8.0/speechless/eval/evalplus/data/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      224 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/data/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3144 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/data/humaneval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5215 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/data/mbpp.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5303 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/data/utils.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.387409 speechless-0.8.0/speechless/eval/evalplus/eval/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9102 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/eval/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      600 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/eval/_special_oracle.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5110 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/eval/utils.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    10285 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/evaluate.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.388644 speechless-0.8.0/speechless/eval/evalplus/gen/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      753 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/gen/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3186 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/gen/chatgpt_gen.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1052 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/gen/mut_gen.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    10914 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/gen/type_mut.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.389209 speechless-0.8.0/speechless/eval/evalplus/gen/util/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      899 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/gen/util/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1662 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/gen/util/api_request.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3987 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/evalplus/inputgen.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.390525 speechless-0.8.0/speechless/eval/human_eval/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/eval/human_eval/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1553 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/eval/human_eval/data.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      635 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/eval/human_eval/evaluate_functional_correctness.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3959 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/eval/human_eval/evaluation.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6405 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/eval/human_eval/execution.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6323 2023-11-30 09:01:22.000000 speechless-0.8.0/speechless/eval/humaneval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4027 2023-12-31 14:55:44.000000 speechless-0.8.0/speechless/eval/llm_api.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.391702 speechless-0.8.0/speechless/eval/lm_eval/
--rw-r--r--   0 sujiangwen   (501) staff       (20)       49 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8995 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/__main__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.394246 speechless-0.8.0/speechless/eval/lm_eval/api/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2046 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/filter.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      970 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/instance.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    11336 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/metrics.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9176 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/model.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4575 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/registry.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4931 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/samplers.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    49758 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/api/task.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.395664 speechless-0.8.0/speechless/eval/lm_eval/decontamination/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/decontamination/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5664 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/decontamination/archiver.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6928 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/decontamination/decontaminate.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    13175 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/decontamination/janitor.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    24764 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/evaluator.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.396830 speechless-0.8.0/speechless/eval/lm_eval/filters/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1516 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/filters/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      630 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/filters/decontamination.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1771 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/filters/extraction.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1606 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/filters/selection.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1532 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/filters/transformation.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.399103 speechless-0.8.0/speechless/eval/lm_eval/models/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      207 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6605 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/anthropic_llms.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)      799 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/dummy.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4629 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/gguf.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    41090 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/huggingface.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    18075 2024-01-29 09:49:27.000000 speechless-0.8.0/speechless/eval/lm_eval/models/openai_completions.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5537 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/textsynth.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    13972 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/models/vllm_causallms.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.399432 speechless-0.8.0/speechless/eval/lm_eval/prompts/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4436 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/prompts/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.399681 speechless-0.8.0/speechless/eval/lm_eval/tasks/
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9319 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/tasks/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    20713 2024-01-28 08:02:08.000000 speechless-0.8.0/speechless/eval/lm_eval/utils.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    32052 2023-11-29 03:23:20.000000 speechless-0.8.0/speechless/eval/lmeval.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5696 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/eval/multiple.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5646 2024-01-06 02:32:59.000000 speechless-0.8.0/speechless/eval/multiple_gen.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.401730 speechless-0.8.0/speechless/finetune/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/finetune/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     3843 2024-01-25 01:52:42.000000 speechless-0.8.0/speechless/finetune/__main__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    72615 2024-02-03 08:45:52.000000 speechless-0.8.0/speechless/finetune/finetune.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    72615 2024-02-03 08:45:52.000000 speechless-0.8.0/speechless/finetune/finetune_conversations.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    47140 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/finetune/finetune_instruction_response.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     7664 2023-11-20 16:10:37.000000 speechless-0.8.0/speechless/finetune/sophia.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.402688 speechless-0.8.0/speechless/infer/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.8.0/speechless/infer/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4068 2024-01-27 03:56:14.000000 speechless-0.8.0/speechless/infer/__main__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     4153 2023-12-31 14:55:44.000000 speechless-0.8.0/speechless/infer/infer.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     6057 2024-01-25 00:31:23.000000 speechless-0.8.0/speechless/infer/openrouter.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.403081 speechless-0.8.0/speechless/quant/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-25 00:31:23.000000 speechless-0.8.0/speechless/quant/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2294 2024-01-28 00:01:49.000000 speechless-0.8.0/speechless/quant/__main__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.403455 speechless-0.8.0/speechless/rag/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-12 03:42:36.000000 speechless-0.8.0/speechless/rag/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.403941 speechless-0.8.0/speechless/rag/document/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-11 12:42:03.000000 speechless-0.8.0/speechless/rag/document/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2336 2024-01-13 06:22:06.000000 speechless-0.8.0/speechless/rag/document/pdf.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    26505 2024-01-13 06:22:06.000000 speechless-0.8.0/speechless/rag/document/pdf2txt.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.404329 speechless-0.8.0/speechless/synthetic_data/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-30 10:07:54.000000 speechless-0.8.0/speechless/synthetic_data/__init__.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.405623 speechless-0.8.0/speechless/synthetic_data/nuggets/
--rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-30 10:07:54.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    14147 2024-02-01 02:29:23.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/__main__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1416 2024-02-01 02:29:23.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/kmeans_sample.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     2160 2024-01-31 07:15:13.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/meta_optimizer.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)    14147 2024-02-01 02:29:23.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/nuggets.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1767 2024-02-01 02:29:23.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/plt.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.407172 speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/
--rw-r--r--   0 sujiangwen   (501) staff       (20)      245 2024-01-31 07:15:13.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/__init__.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     5254 2024-01-31 07:15:13.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/alpaca.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     9459 2024-02-01 02:29:23.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/base.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     8553 2024-01-31 07:15:13.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/loader.py
--rw-r--r--   0 sujiangwen   (501) staff       (20)     1733 2024-02-01 02:29:23.000000 speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/rng_ctx.py
-drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-02-03 08:50:15.346753 speechless-0.8.0/speechless.egg-info/
--rw-r--r--   0 sujiangwen   (501) staff       (20)    31079 2024-02-03 08:50:15.000000 speechless-0.8.0/speechless.egg-info/PKG-INFO
--rw-r--r--   0 sujiangwen   (501) staff       (20)    11615 2024-02-03 08:50:15.000000 speechless-0.8.0/speechless.egg-info/SOURCES.txt
--rw-r--r--   0 sujiangwen   (501) staff       (20)        1 2024-02-03 08:50:15.000000 speechless-0.8.0/speechless.egg-info/dependency_links.txt
--rw-r--r--   0 sujiangwen   (501) staff       (20)      140 2024-02-03 08:50:15.000000 speechless-0.8.0/speechless.egg-info/requires.txt
--rw-r--r--   0 sujiangwen   (501) staff       (20)       11 2024-02-03 08:50:15.000000 speechless-0.8.0/speechless.egg-info/top_level.txt
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.299091 speechless-0.9.0/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    11357 2023-09-17 11:16:20.000000 speechless-0.9.0/LICENSE
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    34155 2024-04-23 02:28:48.298847 speechless-0.9.0/PKG-INFO
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    33285 2024-03-13 15:12:36.000000 speechless-0.9.0/README.md
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      656 2024-04-19 03:30:16.000000 speechless-0.9.0/pyproject.toml
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       38 2024-04-23 02:28:48.299127 speechless-0.9.0/setup.cfg
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4100 2023-11-04 02:56:31.000000 speechless-0.9.0/setup.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.230660 speechless-0.9.0/speechless/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       88 2024-04-23 02:28:14.000000 speechless-0.9.0/speechless/__version__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.231600 speechless-0.9.0/speechless/agents/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 12:01:05.000000 speechless-0.9.0/speechless/agents/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.233419 speechless-0.9.0/speechless/agents/algorithms/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    17343 2023-11-15 15:49:42.000000 speechless-0.9.0/speechless/agents/algorithms/DFS.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8058 2023-11-05 13:34:43.000000 speechless-0.9.0/speechless/agents/algorithms/Tree.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/algorithms/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      931 2023-11-04 14:21:42.000000 speechless-0.9.0/speechless/agents/algorithms/base_env.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1233 2023-11-04 14:21:42.000000 speechless-0.9.0/speechless/agents/algorithms/base_search.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3656 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/algorithms/rank_candidate.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8203 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/algorithms/single_chain.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.233688 speechless-0.9.0/speechless/agents/functionary/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-04-17 09:33:10.000000 speechless-0.9.0/speechless/agents/functionary/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.235731 speechless-0.9.0/speechless/agents/llms/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       43 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/base_io.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4899 2023-12-31 14:55:44.000000 speechless-0.9.0/speechless/agents/llms/chatgpt_function_model.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6031 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/compression.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6939 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/llama_model.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9816 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/model_adapter.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2359 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/retriever.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7110 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/tool_llama_lora_model.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8706 2023-11-05 08:23:36.000000 speechless-0.9.0/speechless/agents/llms/tool_llama_model.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9184 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/llms/utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    12907 2023-11-12 20:04:28.000000 speechless-0.9.0/speechless/agents/llms/vllm_model.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.236148 speechless-0.9.0/speechless/agents/octopus/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-04-22 03:32:31.000000 speechless-0.9.0/speechless/agents/octopus/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1132 2024-04-22 03:32:52.000000 speechless-0.9.0/speechless/agents/octopus/octopusv2.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.236391 speechless-0.9.0/speechless/agents/openfunctionsv2/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-04-19 03:30:16.000000 speechless-0.9.0/speechless/agents/openfunctionsv2/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.237069 speechless-0.9.0/speechless/agents/prompts/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1858 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/prompts/ReAct_prompts.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      528 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/prompts/Tree_search_prompts.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/prompts/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      838 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/prompts/rank_prompts.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10925 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/prompts/tool_conversation.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.237954 speechless-0.9.0/speechless/agents/rapidapi/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/rapidapi/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7812 2023-11-08 11:03:48.000000 speechless-0.9.0/speechless/agents/rapidapi/rapidapi_server.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    36282 2023-11-21 09:58:04.000000 speechless-0.9.0/speechless/agents/rapidapi/run_rapidapi.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6825 2023-11-05 23:59:20.000000 speechless-0.9.0/speechless/agents/rapidapi/toolbench_cache.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.239461 speechless-0.9.0/speechless/agents/tooleval/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5237 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/automatic_eval_sample.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1283 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/convert_answers.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8517 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/convert_to_answer_format.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.239596 speechless-0.9.0/speechless/agents/tooleval/dataset/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/dataset/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7879 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/eval_and_update_leaderboard.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8749 2023-11-10 13:22:46.000000 speechless-0.9.0/speechless/agents/tooleval/eval_pass_rate.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13767 2023-11-12 19:12:12.000000 speechless-0.9.0/speechless/agents/tooleval/eval_preference.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.240097 speechless-0.9.0/speechless/agents/tooleval/evaluation/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      139 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluation/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10248 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluation/dataclass.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1292 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluation/methodcls.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2478 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluation/usereval.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.240218 speechless-0.9.0/speechless/agents/tooleval/evaluators/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      794 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.240980 speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      633 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4534 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/base.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9367 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/rtl.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7837 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/tooleval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2534 2023-12-31 14:55:44.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5457 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/tooleval/evaluators_comparison.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8591 2023-11-10 13:22:46.000000 speechless-0.9.0/speechless/agents/tooleval/utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6432 2023-11-04 13:09:17.000000 speechless-0.9.0/speechless/agents/utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.241566 speechless-0.9.0/speechless/api/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3011 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/client.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.242464 speechless-0.9.0/speechless/api/llms/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       99 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/llms/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1292 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/llms/base_llm.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7556 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/llms/exllama.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7416 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/llms/huggingface.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7935 2023-11-05 09:16:27.000000 speechless-0.9.0/speechless/api/llms/vllm.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.242822 speechless-0.9.0/speechless/api/protocol/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/protocol/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6712 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/protocol/openai.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3144 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/protocol/sampling_params.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13969 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/api/server.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3796 2024-01-06 02:32:59.000000 speechless-0.9.0/speechless/api/settings.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.243611 speechless-0.9.0/speechless/chat/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       72 2024-01-21 04:46:16.000000 speechless-0.9.0/speechless/chat/__main__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.244112 speechless-0.9.0/speechless/chat/app/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      167 2024-01-24 00:08:37.000000 speechless-0.9.0/speechless/chat/app/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3127 2024-01-24 00:08:37.000000 speechless-0.9.0/speechless/chat/app/app.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3314 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/app/session_manager.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1047 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/app/session_store.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.244572 speechless-0.9.0/speechless/chat/ces/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      185 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/ces/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/ces/client.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3085 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/ces/common.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    19123 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/ces/environment.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    18247 2024-01-24 00:08:37.000000 speechless-0.9.0/speechless/chat/chat.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.245222 speechless-0.9.0/speechless/chat/config/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/config/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9187 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/config/config_mgt.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1546 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/config/module_config.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.245448 speechless-0.9.0/speechless/chat/logging/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4322 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/logging/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.246853 speechless-0.9.0/speechless/chat/memory/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      228 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2903 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/attachment.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2586 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/conversation.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1595 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/memory.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10411 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/plugin.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3338 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/post.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2523 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/round.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      150 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/memory/type_vars.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.247331 speechless-0.9.0/speechless/chat/misc/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/misc/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3042 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/misc/component_registry.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      564 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/misc/example.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.247596 speechless-0.9.0/speechless/chat/session/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       28 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/session/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8825 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/session/session.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2146 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.247848 speechless-0.9.0/speechless/chat/workspace/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/workspace/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      702 2024-01-19 22:20:56.000000 speechless-0.9.0/speechless/chat/workspace/workspace.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.247978 speechless-0.9.0/speechless/data_selection/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.249742 speechless-0.9.0/speechless/data_selection/ifd/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6198 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/data_analysis.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7240 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/data_analysis_vic.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5076 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/data_by_IFD.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6376 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/data_by_IFD_vic.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4533 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/data_by_cluster.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3827 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/filter.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1010 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/ifd/select_from_ifd_json.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.251221 speechless-0.9.0/speechless/data_selection/less/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    15012 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/collect_grad_reps.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7420 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/get_info.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7931 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/get_test_dataset.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10213 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/get_training_dataset.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13077 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/get_validation_dataset.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3700 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/matching.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4470 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/less/write_selected_data.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.251384 speechless-0.9.0/speechless/data_selection/mods/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.251939 speechless-0.9.0/speechless/data_selection/mods/diverse-data-selection/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/diverse-data-selection/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5046 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/diverse-data-selection/kcenter_greedy.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2467 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/diverse-data-selection/run.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1419 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/diverse-data-selection/sampling_def.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.252590 speechless-0.9.0/speechless/data_selection/mods/necessity-evaluation/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/necessity-evaluation/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1572 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/necessity-evaluation/merge.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3039 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/necessity-evaluation/necessity-evaluation.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2092 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/necessity-evaluation/necessity-instruction-extraction.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.252984 speechless-0.9.0/speechless/data_selection/mods/quality-evaluation/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/quality-evaluation/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2984 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/quality-evaluation/high-quality-data-extraction.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3022 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/data_selection/mods/quality-evaluation/quality-evaluation.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.253964 speechless-0.9.0/speechless/data_selection/nuggets/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    14147 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/__main__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1416 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/kmeans_sample.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2160 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/meta_optimizer.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    14147 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/nuggets.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1767 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/plt.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.255053 speechless-0.9.0/speechless/data_selection/nuggets/tasks/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      245 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/tasks/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5254 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/tasks/alpaca.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9459 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/tasks/base.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8553 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/tasks/loader.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1733 2024-02-10 19:03:12.000000 speechless-0.9.0/speechless/data_selection/nuggets/tasks/rng_ctx.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.255174 speechless-0.9.0/speechless/decoding/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.255754 speechless-0.9.0/speechless/decoding/ouroboros/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       32 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.256174 speechless-0.9.0/speechless/decoding/ouroboros/cache_engine/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       37 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/cache_engine/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4581 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/cache_engine/cache_engine.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10792 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/kv_cache_model.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.256860 speechless-0.9.0/speechless/decoding/ouroboros/models/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       56 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/models/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    12557 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/models/mask_making_llama.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)   110568 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/models/modeling_llama.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7459 2024-02-25 10:43:16.000000 speechless-0.9.0/speechless/decoding/ouroboros/ouroboros.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.259387 speechless-0.9.0/speechless/eval/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-26 10:21:46.000000 speechless-0.9.0/speechless/eval/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2065 2024-01-26 08:42:38.000000 speechless-0.9.0/speechless/eval/__main__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    15929 2023-12-31 14:55:44.000000 speechless-0.9.0/speechless/eval/async_openai.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    15990 2023-12-27 07:43:41.000000 speechless-0.9.0/speechless/eval/bigcode_eval.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.260581 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1654 2023-12-15 00:18:34.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/arguments.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2711 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/base.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4214 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/evaluator.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6115 2023-12-15 00:18:34.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/generation.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.263845 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1632 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4142 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/apps.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10884 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_code_to_text.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4050 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_text_to_text.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3995 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/conala.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3914 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/concode.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.264209 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7446 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/codexglue_code_to_text_bleu.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13459 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/diff_eval.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.267762 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3170 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/containerized_eval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1164 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cpp.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2102 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cs.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2235 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_dlang.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1112 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_go.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1498 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_java.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1562 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_javascript.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      582 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_julia.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      390 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_lua.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      446 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_php.py
+-rwxr-xr-x   0 sujiangwen   (501) staff       (20)      469 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_pl.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      461 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_python.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1404 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_r.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1225 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_racket.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1361 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ruby.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1644 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_rust.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1303 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_scala.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      578 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_sh.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      864 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_swift.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      911 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ts.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2692 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/evaluation.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4829 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/generic_eval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1325 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/libeval.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.268012 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2803 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2877 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/module_test.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      548 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/single_experiment_pass_k.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.268384 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4410 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/pal_code_exec.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6186 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/python_executor.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7069 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/ds1000.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7496 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/gsm.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5335 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/humaneval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    30239 2023-12-16 08:26:01.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8807 2023-12-31 14:55:44.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack_openai.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5903 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_humaneval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5267 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_wizard_humaneval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5319 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/mbpp.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7066 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/multiple.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5348 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/parity.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4740 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/python_bugs.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5146 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/quixbugs.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7436 2023-12-13 16:02:27.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/recode.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    15958 2023-12-29 10:34:15.000000 speechless-0.9.0/speechless/eval/bigcode_eval_qwen/utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.268930 speechless-0.9.0/speechless/eval/evalplus/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      120 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.269509 speechless-0.9.0/speechless/eval/evalplus/data/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      224 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/data/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3144 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/data/humaneval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5215 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/data/mbpp.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5303 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/data/utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.270054 speechless-0.9.0/speechless/eval/evalplus/eval/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9102 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/eval/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      600 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/eval/_special_oracle.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5110 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/eval/utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10285 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/evaluate.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.270531 speechless-0.9.0/speechless/eval/evalplus/gen/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      753 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/gen/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3186 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/gen/chatgpt_gen.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1052 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/gen/mut_gen.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10914 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/gen/type_mut.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.271079 speechless-0.9.0/speechless/eval/evalplus/gen/util/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      899 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/gen/util/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1662 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/gen/util/api_request.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3987 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/evalplus/inputgen.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.271628 speechless-0.9.0/speechless/eval/human_eval/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/eval/human_eval/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1553 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/eval/human_eval/data.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      635 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/eval/human_eval/evaluate_functional_correctness.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3959 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/eval/human_eval/evaluation.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6405 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/eval/human_eval/execution.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6323 2023-11-30 09:01:22.000000 speechless-0.9.0/speechless/eval/humaneval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4027 2023-12-31 14:55:44.000000 speechless-0.9.0/speechless/eval/llm_api.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.272583 speechless-0.9.0/speechless/eval/lm_eval/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       49 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8995 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/__main__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.274472 speechless-0.9.0/speechless/eval/lm_eval/api/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2046 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/filter.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      970 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/instance.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    11336 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/metrics.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9176 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/model.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4575 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/registry.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4931 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/samplers.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    49758 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/api/task.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.275066 speechless-0.9.0/speechless/eval/lm_eval/decontamination/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/decontamination/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5664 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/decontamination/archiver.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6928 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/decontamination/decontaminate.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13175 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/decontamination/janitor.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    24764 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/evaluator.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.275870 speechless-0.9.0/speechless/eval/lm_eval/filters/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1516 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/filters/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      630 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/filters/decontamination.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1771 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/filters/extraction.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1606 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/filters/selection.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1532 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/filters/transformation.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.277488 speechless-0.9.0/speechless/eval/lm_eval/models/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      207 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6605 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/anthropic_llms.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      799 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/dummy.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4629 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/gguf.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    41090 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/huggingface.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    18075 2024-01-29 09:49:27.000000 speechless-0.9.0/speechless/eval/lm_eval/models/openai_completions.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5537 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/textsynth.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13972 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/models/vllm_causallms.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.277787 speechless-0.9.0/speechless/eval/lm_eval/prompts/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4436 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/prompts/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.277950 speechless-0.9.0/speechless/eval/lm_eval/tasks/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     9319 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/tasks/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    20713 2024-01-28 08:02:08.000000 speechless-0.9.0/speechless/eval/lm_eval/utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    32052 2023-11-29 03:23:20.000000 speechless-0.9.0/speechless/eval/lmeval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5696 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/eval/multiple.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5646 2024-01-06 02:32:59.000000 speechless-0.9.0/speechless/eval/multiple_gen.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.281139 speechless-0.9.0/speechless/finetune/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/finetune/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4214 2024-02-08 18:26:32.000000 speechless-0.9.0/speechless/finetune/__main__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6938 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/callbacks.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    38818 2024-02-11 18:52:12.000000 speechless-0.9.0/speechless/finetune/dataset_utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    34917 2024-03-11 09:59:52.000000 speechless-0.9.0/speechless/finetune/finetune.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    34917 2024-03-11 09:59:52.000000 speechless-0.9.0/speechless/finetune/finetune_conversations.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    47140 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/finetune/finetune_instruction_response.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1679 2024-04-22 06:35:41.000000 speechless-0.9.0/speechless/finetune/generate_llamacpp_finetune_data.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1747 2024-04-23 02:27:09.000000 speechless-0.9.0/speechless/finetune/generate_mlx_finetune_data.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.282717 speechless-0.9.0/speechless/finetune/hparams/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      494 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3871 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/data_args.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1462 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/evaluation_args.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    10631 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/finetuning_args.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1915 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/generating_args.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7154 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/model_args.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    12908 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/hparams/parser.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2912 2024-04-11 17:38:41.000000 speechless-0.9.0/speechless/finetune/lisa.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       23 2024-04-23 02:27:09.000000 speechless-0.9.0/speechless/finetune/llamacpp.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.283919 speechless-0.9.0/speechless/finetune/model/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      287 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/model/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7443 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/model/adapter.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7386 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/finetune/model/loader.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    18050 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/model/patcher.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7177 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/model/utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.285843 speechless-0.9.0/speechless/finetune/moe/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-08 07:24:18.000000 speechless-0.9.0/speechless/finetune/moe/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    16580 2024-02-19 22:09:20.000000 speechless-0.9.0/speechless/finetune/moe/__main__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5889 2024-02-11 18:52:12.000000 speechless-0.9.0/speechless/finetune/moe/merge_moe.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.286509 speechless-0.9.0/speechless/finetune/moe/sparsetral/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-08 07:24:18.000000 speechless-0.9.0/speechless/finetune/moe/sparsetral/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7469 2024-02-08 07:24:18.000000 speechless-0.9.0/speechless/finetune/moe/sparsetral/configuration_sparsetral.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    68141 2024-02-08 07:24:18.000000 speechless-0.9.0/speechless/finetune/moe/sparsetral/modeling_sparsetral.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    16580 2024-02-19 22:09:20.000000 speechless-0.9.0/speechless/finetune/moe/train_moe.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    22289 2024-02-08 07:24:18.000000 speechless-0.9.0/speechless/finetune/moe/transformers_utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.287306 speechless-0.9.0/speechless/finetune/patches/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/patches/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8841 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/patches/llama_patch.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    13935 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/finetune/pretrain.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7664 2023-11-20 16:10:37.000000 speechless-0.9.0/speechless/finetune/sophia.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.288914 speechless-0.9.0/speechless/generate/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-14 09:45:37.000000 speechless-0.9.0/speechless/generate/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2325 2024-03-28 22:48:42.000000 speechless-0.9.0/speechless/generate/anthropic.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2469 2024-04-03 01:57:18.000000 speechless-0.9.0/speechless/generate/groq.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2678 2024-02-19 08:44:53.000000 speechless-0.9.0/speechless/generate/llamacpp.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3711 2024-04-11 17:38:41.000000 speechless-0.9.0/speechless/generate/mlx.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2655 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/generate/openai.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4202 2024-02-19 08:44:53.000000 speechless-0.9.0/speechless/generate/wasmedge.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.289744 speechless-0.9.0/speechless/infer/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2023-11-04 02:56:31.000000 speechless-0.9.0/speechless/infer/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4112 2024-02-08 07:24:18.000000 speechless-0.9.0/speechless/infer/__main__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4153 2023-12-31 14:55:44.000000 speechless-0.9.0/speechless/infer/infer.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6057 2024-01-25 00:31:23.000000 speechless-0.9.0/speechless/infer/openrouter.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.290088 speechless-0.9.0/speechless/quant/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-25 00:31:23.000000 speechless-0.9.0/speechless/quant/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2519 2024-02-17 23:36:53.000000 speechless-0.9.0/speechless/quant/__main__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.290320 speechless-0.9.0/speechless/rag/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-12 03:42:36.000000 speechless-0.9.0/speechless/rag/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.290746 speechless-0.9.0/speechless/rag/document/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-01-11 12:42:03.000000 speechless-0.9.0/speechless/rag/document/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2336 2024-01-13 06:22:06.000000 speechless-0.9.0/speechless/rag/document/pdf.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    26505 2024-01-13 06:22:06.000000 speechless-0.9.0/speechless/rag/document/pdf2txt.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.291197 speechless-0.9.0/speechless/synthetic_data/
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.291709 speechless-0.9.0/speechless/synthetic_data/Humback/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       40 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7916 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/data.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.293089 speechless-0.9.0/speechless/synthetic_data/Humback/utils/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1060 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/config.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      102 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/constant.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      850 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/convert_vllm_to_alpaca_eval.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1387 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/io.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      122 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/print.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1575 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/Humback/utils/template.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.293429 speechless-0.9.0/speechless/synthetic_data/ada_instruct/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       48 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.294089 speechless-0.9.0/speechless/synthetic_data/ada_instruct/config/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      109 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/config/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1347 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/config/generation_config.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      666 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/config/verification_config.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     7296 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/synthesize_instructions.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.294488 speechless-0.9.0/speechless/synthetic_data/ada_instruct/tasks/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      609 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/tasks/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1341 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/ada_instruct/tasks/base.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.294786 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/__init__.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.294971 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/control_flow_functions/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/control_flow_functions/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    74261 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/control_flow_functions/control_flow_functions.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.297769 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        0 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2129 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/async_llamacpp_api_call.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     1010 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/character_card_helpers.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      998 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/constants.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     4838 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/engine_wrapper_class.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      704 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/extract_name.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      592 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/extract_question_answer.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      413 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/format_qatuples.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5786 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/generation_step_class.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     2733 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/identify_duplicates.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    19720 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/process_multiturn_functions.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      485 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/random_name.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     6842 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/special_instructions.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3361 2024-02-22 09:52:45.000000 speechless-0.9.0/speechless/synthetic_data/augmentoolkit/generation_functions/strip_steps.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     8026 2024-04-14 18:43:51.000000 speechless-0.9.0/speechless/synthetic_data/qa_generator.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.298478 speechless-0.9.0/speechless/utils/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       45 2024-03-28 22:49:41.000000 speechless-0.9.0/speechless/utils/__init__.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     5322 2024-03-16 20:58:47.000000 speechless-0.9.0/speechless/utils/prompt_utils.py
+-rw-r--r--   0 sujiangwen   (501) staff       (20)     3967 2024-04-04 06:20:08.000000 speechless-0.9.0/speechless/utils/token_utils.py
+drwxr-xr-x   0 sujiangwen   (501) staff       (20)        0 2024-04-23 02:28:48.231386 speechless-0.9.0/speechless.egg-info/
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    34155 2024-04-23 02:28:48.000000 speechless-0.9.0/speechless.egg-info/PKG-INFO
+-rw-r--r--   0 sujiangwen   (501) staff       (20)    17644 2024-04-23 02:28:48.000000 speechless-0.9.0/speechless.egg-info/SOURCES.txt
+-rw-r--r--   0 sujiangwen   (501) staff       (20)        1 2024-04-23 02:28:48.000000 speechless-0.9.0/speechless.egg-info/dependency_links.txt
+-rw-r--r--   0 sujiangwen   (501) staff       (20)      140 2024-04-23 02:28:48.000000 speechless-0.9.0/speechless.egg-info/requires.txt
+-rw-r--r--   0 sujiangwen   (501) staff       (20)       11 2024-04-23 02:28:48.000000 speechless-0.9.0/speechless.egg-info/top_level.txt
```

### Comparing `speechless-0.8.0/LICENSE` & `speechless-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/PKG-INFO` & `speechless-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechless
-Version: 0.8.0
+Version: 0.9.0
 Summary: LLM based agents with proactive interactions, long-term memory, external tool integration, and local deployment capabilities.
 Home-page: https://github.com/uukuguy/speechless
 Author: Jiangwen Su
 Author-email: uukuguy@gmail.com
 License: Apache
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,14 +33,21 @@
 - Next, we design and implement an efficient operational framework for the intelligent entity. This framework not only supports rapid deployment and invocation of the model but also boasts features like autonomous interaction, real-time feedback adjustment, context awareness, and long-term memory.
   For instance, in customer service scenarios, the intelligent entity can provide more precise and personalized responses based on a user's historical interactions and current context. In content recommendation scenarios, it can dynamically adjust its strategies by capturing real-time shifts in user interests.
 
 - Ultimately, we integrate it with real business scenarios, ensuring that the intelligent entity seamlessly aligns with various business processes, delivering tangible value to enterprises.
 
 ## What's New
 
+
+- [2024-03-13] Release [speechless-starcoder2-15b](https://huggingface.co/uukuguy/speechless-starcoder2-15b)
+- [2024-03-10] Release [speechless-starcoder2-7b](https://huggingface.co/uukuguy/speechless-starcoder2-7b)
+- [2024-02-15] Reelase [speechless-thoughts-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b-v1.0) (Change same hyperparameters)
+- [2024-02-12] Release [speechless-thoughts-mistral-7b](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b)
+- [2024-02-10] Release [speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE), the MoE upgraded version of speechless-code-mistral-7b-v1.0. The MoE fine-tuning adopts [Parameter-Efficient Sparsity Crafting (PESC)](https://arxiv.org/abs/2401.02731), which is an efficient fine-tuning architecture that uses LoRA modules as expert models, similar to the concept of [multi-loras](https://github.com/uukuguy/multi_loras).
+- [2024-02-06] Release [speechless-mistral-hermes-code-7b](https://huggingface.co/uukuguy/speechless-mistral-hermes-code-7b) fine-tuned by speechless-thoughts-252K dataset.
 - [2024-01-23] Release [speechless-zephyr-code-functionary-7b](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b)
 - [2024-01-15] Release [speechless-nl2sql-ds-6.7b](https://huggingface.co/uukuguy/speechless-nl2sql-ds-6.7b), finetune based on [deepseek-coder-6.7b-base](https://huggingface.co/deepseek-ai/deepseek-coder-6.7b-base).
 - [2024-01-05] Release [speechless-mistral-moloras-7b](https://huggingface.co/uukuguy/speechless-mistral-moloras-7b), which is the static version of moloras ([Mixture-of-multi-LoRAs](https://github.com/uukuguy/multi_loras?tab=readme-ov-file#mixture-of-multi-loras))
 - [2023/12/30] Release [speechless-coder-ds-1.3b](https://huggingface.co/uukuguy/speechless-coder-ds-1.3b) that finetune based on [deepseek-coder-1.3b-base](https://huggingface.co/deepseek-ai/deepseek-coder-1.3b-base).
 - [2023/12/30] Release [speechless-coder-ds-6.7b](https://huggingface.co/uukuguy/speechless-coder-ds-6.7b) that finetune based on [deepseek-coder-6.7b-base](https://huggingface.co/deepseek-ai/deepseek-coder-6.7b-base).
 - [2023/12/23] Uploaded the float16 version of [prometheus-7b-v1.0-fp16](https://huggingface.co/uukuguy/prometheus-7b-v1.0-fp16) for instruction fine-tuning data quality assessment.
 - [2023/12/23] Uploaded the float16 version of [prometheus-13b-v1.0-fp16](https://huggingface.co/uukuguy/prometheus-13b-v1.0-fp16) for instruction fine-tuning data quality assessment.
@@ -79,14 +86,51 @@
 
 ## Models
 
 [Models Repositry](https://huggingface.co/uukuguy)
 
 ⭐️ My Focus 🔥🔥🔥 DL > 10k/month 🔥🔥 DL > 7K/month 🔥 DL > 3K/month
 
+### Mar. 2024
+
+- **[speechless-starcoder2-15b](https://huggingface.co/uukuguy/speechless-starcoder2-15b) 2024.03.13**
+
+- **[speechless-starcoder2-7b](https://huggingface.co/uukuguy/speechless-starcoder2-7b) 2024.03.10**
+
+### Feb. 2024
+
+- **[speechless-thoughts-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b-v1.0) 2024.02.15**
+
+    Change some hyperparameters compared to speechless-thoughts-mistral-7b.
+
+    ```json
+    learning_rate=2e-4
+    lora_r=64
+    lora_alpha=16
+    model_max_length=8192
+    ```
+
+- **[speechless-thoughts-mistral-7b](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b) 2024.02.12**
+
+    speechless-thoughts-mistral-7b is fine-tuned as a baseline of the [speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE).
+
+    **Open LLM Language Model Evaluation Harness**
+
+    | Average | ARC    | HellaSwag | MMLU   | TruthfulQA | Winogrande | GSM8K  |
+    | ------  | ------ | ------    | ------ | ------     | -------    | ------ |
+    | 59.72   | 58.96  | 87.10    | 60.11  | 49.91      | 77.82      | 30.78  |
+
+- ⭐ **[speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE) 2024.02.10**
+
+    The MoE upgraded version of speechless-code-mistral-7b-v1.0. The MoE fine-tuning adopts [Parameter-Efficient Sparsity Crafting (PESC)](https://arxiv.org/abs/2401.02731), which is an efficient fine-tuning architecture that uses LoRA modules as expert models, similar to the concept of [multi-loras](https://github.com/uukuguy/multi_loras).
+
+- ⭐ **[speechless-mistral-hermes-code-7b](https://huggingface.co/uukuguy/speechless-mistral-hermes-code-7b) 2024.02.06**
+
+    Using the speechless-thoughts-252K dataset, it was fine-tuned based on the Mistral-7B-v0.1 base model in preparation for comparison with [speechless-code-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-code-mistral-7b-v1.0).
+
 ### Jan. 2024
 
 - ⭐ **[speechless-zephyr-code-functionary-7b](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b)**
 
     [GGUF](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b/tree/main/GGUF)
 
 - **[speechless-nl2sql-ds-6.7b](https://huggingface.co/uukuguy/speechless-nl2sql-ds-6.7b)**
```

### Comparing `speechless-0.8.0/README.md` & `speechless-0.9.0/speechless.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: speechless
+Version: 0.9.0
+Summary: LLM based agents with proactive interactions, long-term memory, external tool integration, and local deployment capabilities.
+Home-page: https://github.com/uukuguy/speechless
+Author: Jiangwen Su
+Author-email: uukuguy@gmail.com
+License: Apache
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # Speechless LLM based Agents
 
 > LLM based agents with proactive interactions, long-term memory, external tool integration, and local deployment capabilities.
 
 ![Speechless.AI](imgs/speechlessai_main_3.png)
 
 [Speechless.AI](http://speechless.ai/) is committed to integrating the superior language processing and deep reasoning capabilities of large language models into practical business applications. By enhancing the model's language understanding, knowledge accumulation, and text creation abilities, and introducing long-term memory, external tool integration, and local deployment, our aim is to establish an intelligent collaborative partner that can independently interact, continuously evolve, and closely align with various business scenarios.
@@ -11,14 +33,21 @@
 - Next, we design and implement an efficient operational framework for the intelligent entity. This framework not only supports rapid deployment and invocation of the model but also boasts features like autonomous interaction, real-time feedback adjustment, context awareness, and long-term memory.
   For instance, in customer service scenarios, the intelligent entity can provide more precise and personalized responses based on a user's historical interactions and current context. In content recommendation scenarios, it can dynamically adjust its strategies by capturing real-time shifts in user interests.
 
 - Ultimately, we integrate it with real business scenarios, ensuring that the intelligent entity seamlessly aligns with various business processes, delivering tangible value to enterprises.
 
 ## What's New
 
+
+- [2024-03-13] Release [speechless-starcoder2-15b](https://huggingface.co/uukuguy/speechless-starcoder2-15b)
+- [2024-03-10] Release [speechless-starcoder2-7b](https://huggingface.co/uukuguy/speechless-starcoder2-7b)
+- [2024-02-15] Reelase [speechless-thoughts-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b-v1.0) (Change same hyperparameters)
+- [2024-02-12] Release [speechless-thoughts-mistral-7b](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b)
+- [2024-02-10] Release [speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE), the MoE upgraded version of speechless-code-mistral-7b-v1.0. The MoE fine-tuning adopts [Parameter-Efficient Sparsity Crafting (PESC)](https://arxiv.org/abs/2401.02731), which is an efficient fine-tuning architecture that uses LoRA modules as expert models, similar to the concept of [multi-loras](https://github.com/uukuguy/multi_loras).
+- [2024-02-06] Release [speechless-mistral-hermes-code-7b](https://huggingface.co/uukuguy/speechless-mistral-hermes-code-7b) fine-tuned by speechless-thoughts-252K dataset.
 - [2024-01-23] Release [speechless-zephyr-code-functionary-7b](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b)
 - [2024-01-15] Release [speechless-nl2sql-ds-6.7b](https://huggingface.co/uukuguy/speechless-nl2sql-ds-6.7b), finetune based on [deepseek-coder-6.7b-base](https://huggingface.co/deepseek-ai/deepseek-coder-6.7b-base).
 - [2024-01-05] Release [speechless-mistral-moloras-7b](https://huggingface.co/uukuguy/speechless-mistral-moloras-7b), which is the static version of moloras ([Mixture-of-multi-LoRAs](https://github.com/uukuguy/multi_loras?tab=readme-ov-file#mixture-of-multi-loras))
 - [2023/12/30] Release [speechless-coder-ds-1.3b](https://huggingface.co/uukuguy/speechless-coder-ds-1.3b) that finetune based on [deepseek-coder-1.3b-base](https://huggingface.co/deepseek-ai/deepseek-coder-1.3b-base).
 - [2023/12/30] Release [speechless-coder-ds-6.7b](https://huggingface.co/uukuguy/speechless-coder-ds-6.7b) that finetune based on [deepseek-coder-6.7b-base](https://huggingface.co/deepseek-ai/deepseek-coder-6.7b-base).
 - [2023/12/23] Uploaded the float16 version of [prometheus-7b-v1.0-fp16](https://huggingface.co/uukuguy/prometheus-7b-v1.0-fp16) for instruction fine-tuning data quality assessment.
 - [2023/12/23] Uploaded the float16 version of [prometheus-13b-v1.0-fp16](https://huggingface.co/uukuguy/prometheus-13b-v1.0-fp16) for instruction fine-tuning data quality assessment.
@@ -57,14 +86,51 @@
 
 ## Models
 
 [Models Repositry](https://huggingface.co/uukuguy)
 
 ⭐️ My Focus 🔥🔥🔥 DL > 10k/month 🔥🔥 DL > 7K/month 🔥 DL > 3K/month
 
+### Mar. 2024
+
+- **[speechless-starcoder2-15b](https://huggingface.co/uukuguy/speechless-starcoder2-15b) 2024.03.13**
+
+- **[speechless-starcoder2-7b](https://huggingface.co/uukuguy/speechless-starcoder2-7b) 2024.03.10**
+
+### Feb. 2024
+
+- **[speechless-thoughts-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b-v1.0) 2024.02.15**
+
+    Change some hyperparameters compared to speechless-thoughts-mistral-7b.
+
+    ```json
+    learning_rate=2e-4
+    lora_r=64
+    lora_alpha=16
+    model_max_length=8192
+    ```
+
+- **[speechless-thoughts-mistral-7b](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b) 2024.02.12**
+
+    speechless-thoughts-mistral-7b is fine-tuned as a baseline of the [speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE).
+
+    **Open LLM Language Model Evaluation Harness**
+
+    | Average | ARC    | HellaSwag | MMLU   | TruthfulQA | Winogrande | GSM8K  |
+    | ------  | ------ | ------    | ------ | ------     | -------    | ------ |
+    | 59.72   | 58.96  | 87.10    | 60.11  | 49.91      | 77.82      | 30.78  |
+
+- ⭐ **[speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE) 2024.02.10**
+
+    The MoE upgraded version of speechless-code-mistral-7b-v1.0. The MoE fine-tuning adopts [Parameter-Efficient Sparsity Crafting (PESC)](https://arxiv.org/abs/2401.02731), which is an efficient fine-tuning architecture that uses LoRA modules as expert models, similar to the concept of [multi-loras](https://github.com/uukuguy/multi_loras).
+
+- ⭐ **[speechless-mistral-hermes-code-7b](https://huggingface.co/uukuguy/speechless-mistral-hermes-code-7b) 2024.02.06**
+
+    Using the speechless-thoughts-252K dataset, it was fine-tuned based on the Mistral-7B-v0.1 base model in preparation for comparison with [speechless-code-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-code-mistral-7b-v1.0).
+
 ### Jan. 2024
 
 - ⭐ **[speechless-zephyr-code-functionary-7b](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b)**
 
     [GGUF](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b/tree/main/GGUF)
 
 - **[speechless-nl2sql-ds-6.7b](https://huggingface.co/uukuguy/speechless-nl2sql-ds-6.7b)**
```

### Comparing `speechless-0.8.0/setup.py` & `speechless-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/algorithms/DFS.py` & `speechless-0.9.0/speechless/agents/algorithms/DFS.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/algorithms/Tree.py` & `speechless-0.9.0/speechless/agents/algorithms/Tree.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/algorithms/base_env.py` & `speechless-0.9.0/speechless/agents/algorithms/base_env.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/algorithms/base_search.py` & `speechless-0.9.0/speechless/agents/algorithms/base_search.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/algorithms/rank_candidate.py` & `speechless-0.9.0/speechless/agents/algorithms/rank_candidate.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/algorithms/single_chain.py` & `speechless-0.9.0/speechless/agents/algorithms/single_chain.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/chatgpt_function_model.py` & `speechless-0.9.0/speechless/agents/llms/chatgpt_function_model.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/compression.py` & `speechless-0.9.0/speechless/agents/llms/compression.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/llama_model.py` & `speechless-0.9.0/speechless/agents/llms/llama_model.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/model_adapter.py` & `speechless-0.9.0/speechless/agents/llms/model_adapter.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/retriever.py` & `speechless-0.9.0/speechless/agents/llms/retriever.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/tool_llama_lora_model.py` & `speechless-0.9.0/speechless/agents/llms/tool_llama_lora_model.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/tool_llama_model.py` & `speechless-0.9.0/speechless/agents/llms/tool_llama_model.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/utils.py` & `speechless-0.9.0/speechless/agents/llms/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/llms/vllm_model.py` & `speechless-0.9.0/speechless/agents/llms/vllm_model.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/prompts/ReAct_prompts.py` & `speechless-0.9.0/speechless/agents/prompts/ReAct_prompts.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/prompts/Tree_search_prompts.py` & `speechless-0.9.0/speechless/agents/prompts/Tree_search_prompts.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/prompts/rank_prompts.py` & `speechless-0.9.0/speechless/agents/prompts/rank_prompts.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/prompts/tool_conversation.py` & `speechless-0.9.0/speechless/agents/prompts/tool_conversation.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/rapidapi/rapidapi_server.py` & `speechless-0.9.0/speechless/agents/rapidapi/rapidapi_server.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/rapidapi/run_rapidapi.py` & `speechless-0.9.0/speechless/agents/rapidapi/run_rapidapi.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/rapidapi/toolbench_cache.py` & `speechless-0.9.0/speechless/agents/rapidapi/toolbench_cache.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/automatic_eval_sample.py` & `speechless-0.9.0/speechless/agents/tooleval/automatic_eval_sample.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/convert_answers.py` & `speechless-0.9.0/speechless/agents/tooleval/convert_answers.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/convert_to_answer_format.py` & `speechless-0.9.0/speechless/agents/tooleval/convert_to_answer_format.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/eval_and_update_leaderboard.py` & `speechless-0.9.0/speechless/agents/tooleval/eval_and_update_leaderboard.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/eval_pass_rate.py` & `speechless-0.9.0/speechless/agents/tooleval/eval_pass_rate.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/eval_preference.py` & `speechless-0.9.0/speechless/agents/tooleval/eval_preference.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluation/dataclass.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluation/dataclass.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluation/methodcls.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluation/methodcls.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluation/usereval.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluation/usereval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators/__init__.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/__init__.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/base.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/base.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/rtl.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/rtl.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/tooleval.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/tooleval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators/registered_cls/utils.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators/registered_cls/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/evaluators_comparison.py` & `speechless-0.9.0/speechless/agents/tooleval/evaluators_comparison.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/tooleval/utils.py` & `speechless-0.9.0/speechless/agents/tooleval/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/agents/utils.py` & `speechless-0.9.0/speechless/agents/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/client.py` & `speechless-0.9.0/speechless/api/client.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/llms/base_llm.py` & `speechless-0.9.0/speechless/api/llms/base_llm.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/llms/exllama.py` & `speechless-0.9.0/speechless/api/llms/exllama.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/llms/huggingface.py` & `speechless-0.9.0/speechless/api/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/llms/vllm.py` & `speechless-0.9.0/speechless/api/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/protocol/openai.py` & `speechless-0.9.0/speechless/api/protocol/openai.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/protocol/sampling_params.py` & `speechless-0.9.0/speechless/api/protocol/sampling_params.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/server.py` & `speechless-0.9.0/speechless/api/server.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/api/settings.py` & `speechless-0.9.0/speechless/api/settings.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/app/app.py` & `speechless-0.9.0/speechless/chat/app/app.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/app/session_manager.py` & `speechless-0.9.0/speechless/chat/app/session_manager.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/app/session_store.py` & `speechless-0.9.0/speechless/chat/app/session_store.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/ces/common.py` & `speechless-0.9.0/speechless/chat/ces/common.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/ces/environment.py` & `speechless-0.9.0/speechless/chat/ces/environment.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/chat.py` & `speechless-0.9.0/speechless/chat/chat.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/config/config_mgt.py` & `speechless-0.9.0/speechless/chat/config/config_mgt.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/config/module_config.py` & `speechless-0.9.0/speechless/chat/config/module_config.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/logging/__init__.py` & `speechless-0.9.0/speechless/chat/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/memory/attachment.py` & `speechless-0.9.0/speechless/chat/memory/attachment.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/memory/conversation.py` & `speechless-0.9.0/speechless/chat/memory/conversation.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/memory/memory.py` & `speechless-0.9.0/speechless/chat/memory/memory.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/memory/plugin.py` & `speechless-0.9.0/speechless/chat/memory/plugin.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/memory/post.py` & `speechless-0.9.0/speechless/chat/memory/post.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/memory/round.py` & `speechless-0.9.0/speechless/chat/memory/round.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/misc/component_registry.py` & `speechless-0.9.0/speechless/chat/misc/component_registry.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/misc/example.py` & `speechless-0.9.0/speechless/chat/misc/example.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/session/session.py` & `speechless-0.9.0/speechless/chat/session/session.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/utils.py` & `speechless-0.9.0/speechless/chat/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/chat/workspace/workspace.py` & `speechless-0.9.0/speechless/chat/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/__main__.py` & `speechless-0.9.0/speechless/eval/__main__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/async_openai.py` & `speechless-0.9.0/speechless/eval/async_openai.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/arguments.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/arguments.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/base.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/base.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/evaluator.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/evaluator.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/generation.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/generation.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/__init__.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/apps.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/apps.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_code_to_text.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_code_to_text.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_text_to_text.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/codexglue_text_to_text.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/conala.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/conala.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/concode.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/concode.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/codexglue_code_to_text_bleu.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/codexglue_code_to_text_bleu.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/diff_eval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/diff_eval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/containerized_eval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/containerized_eval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cpp.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cpp.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cs.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_cs.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_dlang.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_dlang.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_go.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_go.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_java.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_java.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_javascript.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_javascript.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_julia.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_julia.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_r.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_r.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_racket.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_racket.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ruby.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ruby.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_rust.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_rust.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_scala.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_scala.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_sh.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_sh.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_swift.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_swift.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ts.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/eval_ts.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/evaluation.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/evaluation.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/generic_eval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/generic_eval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/libeval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/libeval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/__init__.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/module_test.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/safe_subprocess/module_test.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/single_experiment_pass_k.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/multiple_metrics/single_experiment_pass_k.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/pal_code_exec.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/pal_code_exec.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/python_executor.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/custom_metrics/pal_metric/python_executor.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/ds1000.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/ds1000.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/gsm.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/gsm.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/humaneval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/humaneval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack_openai.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/humanevalpack_openai.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_humaneval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_humaneval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_wizard_humaneval.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/instruct_wizard_humaneval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/mbpp.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/mbpp.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/multiple.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/multiple.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/parity.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/parity.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/python_bugs.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/python_bugs.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/quixbugs.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/quixbugs.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/tasks/recode.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/tasks/recode.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/bigcode_eval_qwen/utils.py` & `speechless-0.9.0/speechless/eval/bigcode_eval_qwen/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/data/humaneval.py` & `speechless-0.9.0/speechless/eval/evalplus/data/humaneval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/data/mbpp.py` & `speechless-0.9.0/speechless/eval/evalplus/data/mbpp.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/data/utils.py` & `speechless-0.9.0/speechless/eval/evalplus/data/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/eval/__init__.py` & `speechless-0.9.0/speechless/eval/evalplus/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/eval/_special_oracle.py` & `speechless-0.9.0/speechless/eval/evalplus/eval/_special_oracle.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/eval/utils.py` & `speechless-0.9.0/speechless/eval/evalplus/eval/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/evaluate.py` & `speechless-0.9.0/speechless/eval/evalplus/evaluate.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/gen/__init__.py` & `speechless-0.9.0/speechless/eval/evalplus/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/gen/chatgpt_gen.py` & `speechless-0.9.0/speechless/eval/evalplus/gen/chatgpt_gen.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/gen/mut_gen.py` & `speechless-0.9.0/speechless/eval/evalplus/gen/mut_gen.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/gen/type_mut.py` & `speechless-0.9.0/speechless/eval/evalplus/gen/type_mut.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/gen/util/__init__.py` & `speechless-0.9.0/speechless/eval/evalplus/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/gen/util/api_request.py` & `speechless-0.9.0/speechless/eval/evalplus/gen/util/api_request.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/evalplus/inputgen.py` & `speechless-0.9.0/speechless/eval/evalplus/inputgen.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/human_eval/data.py` & `speechless-0.9.0/speechless/eval/human_eval/data.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/human_eval/evaluate_functional_correctness.py` & `speechless-0.9.0/speechless/eval/human_eval/evaluate_functional_correctness.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/human_eval/evaluation.py` & `speechless-0.9.0/speechless/eval/human_eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/human_eval/execution.py` & `speechless-0.9.0/speechless/eval/human_eval/execution.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/humaneval.py` & `speechless-0.9.0/speechless/eval/humaneval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/llm_api.py` & `speechless-0.9.0/speechless/eval/llm_api.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/__main__.py` & `speechless-0.9.0/speechless/eval/lm_eval/__main__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/filter.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/filter.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/instance.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/instance.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/metrics.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/metrics.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/model.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/model.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/registry.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/registry.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/samplers.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/samplers.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/api/task.py` & `speechless-0.9.0/speechless/eval/lm_eval/api/task.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/decontamination/archiver.py` & `speechless-0.9.0/speechless/eval/lm_eval/decontamination/archiver.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/decontamination/decontaminate.py` & `speechless-0.9.0/speechless/eval/lm_eval/decontamination/decontaminate.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/decontamination/janitor.py` & `speechless-0.9.0/speechless/eval/lm_eval/decontamination/janitor.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/evaluator.py` & `speechless-0.9.0/speechless/eval/lm_eval/evaluator.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/filters/__init__.py` & `speechless-0.9.0/speechless/eval/lm_eval/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/filters/decontamination.py` & `speechless-0.9.0/speechless/eval/lm_eval/filters/decontamination.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/filters/extraction.py` & `speechless-0.9.0/speechless/eval/lm_eval/filters/extraction.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/filters/selection.py` & `speechless-0.9.0/speechless/eval/lm_eval/filters/selection.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/filters/transformation.py` & `speechless-0.9.0/speechless/eval/lm_eval/filters/transformation.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/anthropic_llms.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/anthropic_llms.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/dummy.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/dummy.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/gguf.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/gguf.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/huggingface.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/openai_completions.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/openai_completions.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/textsynth.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/textsynth.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/models/vllm_causallms.py` & `speechless-0.9.0/speechless/eval/lm_eval/models/vllm_causallms.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/prompts/__init__.py` & `speechless-0.9.0/speechless/eval/lm_eval/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/tasks/__init__.py` & `speechless-0.9.0/speechless/eval/lm_eval/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lm_eval/utils.py` & `speechless-0.9.0/speechless/eval/lm_eval/utils.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/lmeval.py` & `speechless-0.9.0/speechless/eval/lmeval.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/multiple.py` & `speechless-0.9.0/speechless/eval/multiple.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/eval/multiple_gen.py` & `speechless-0.9.0/speechless/eval/multiple_gen.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/finetune/__main__.py` & `speechless-0.9.0/speechless/finetune/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,26 @@
 
     if not is_speechless_task_dir(task_dir):
         raise Exception(f"{task_dir} not found or invalid")
 
     run_cmd = f"cd {task_dir} && ./run_finetune.sh"
     os.system(run_cmd)
 
+def finetune_moe(args):
+    task_name = args.task_name
+    if not task_name:
+        raise Exception("task_name is required")
+    task_dir = f"{os.curdir}/{task_name}"
+
+    if not is_speechless_task_dir(task_dir):
+        raise Exception(f"{task_dir} not found or invalid")
+
+    run_cmd = f"cd {task_dir} && ./run_moe.sh"
+    os.system(run_cmd)
+
 
 def finetune_merge(args):
     task_name = args.task_name
     if not task_name:
         raise Exception("task_name is required")
     task_dir = f"{os.curdir}/{task_name}"
 
@@ -98,14 +110,15 @@
     for speechless_task_dir in speechless_task_dirs:
         print(speechless_task_dir)
 
 
 commands = {
     "init": finetune_init,
     "run": finetune_run,
+    "moe": finetune_moe,
     "merge": finetune_merge,
     "backup": finetune_backup,
     "list": finetune_list,
 }
 
 
 def get_args():
```

### Comparing `speechless-0.8.0/speechless/finetune/finetune.py` & `speechless-0.9.0/speechless/finetune/finetune_instruction_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 import math
 import gc, ctypes
 #from rich import print
 
-# if os.environ.get('ENABLE_FLASH_ATTENTION', 'False') == 'True':
+# if os.environ.get('ENABLE_FLASH_ATTENTION', 'False') == 'True': 
 #     from flash_attn_monkey_patch import replace_llama_attn_with_flash_attn
 #     replace_llama_attn_with_flash_attn(packed=True)
 #     print(f"Enabled flash attention monkey patching.")
 
 # if os.environ.get('ENABLE_REROPE', "False") == 'True':
 #     from rerope_monkey_patch import replace_llama_attention_forword_with_rerope
 #     replace_llama_attention_forword_with_rerope(training_length=4096, window=1536)
@@ -32,16 +32,14 @@
 import logging
 import bitsandbytes as bnb
 import pandas as pd
 
 # logger = logging.getLogger(__name__)
 from loguru import logger
 
-# from speechless.patches.llama_attn_replace_sft import replace_llama_attn
-# replace_llama_attn(use_flash_attn=True, use_full=False, inference=False)
 
 import torch
 import transformers
 from torch.nn.utils.rnn import pad_sequence
 import argparse
 from transformers import (
     AutoTokenizer,
@@ -60,53 +58,14 @@
     LoraConfig,
     get_peft_model,
     PeftModel
 )
 from peft.tuners.lora import LoraLayer
 from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
 
-def qwen_prepare_model_for_kbit_training(model, use_gradient_checkpointing=True):
-    """
-    This method wraps the entire protocol for preparing a model before running a training. This includes:
-        1- Cast the layernorm in fp32 2- making output embedding layer require grads 3- Add the upcasting of the lm
-        head to fp32
-
-    Args:
-        model, (`transformers.PreTrainedModel`):
-            The loaded model from `transformers`
-    """
-    loaded_in_kbit = getattr(model, "is_loaded_in_8bit", False) or getattr(model, "is_loaded_in_4bit", False)
-    is_gptq_quantized = getattr(model, "quantization_method", None) == "gptq"
-    for name, param in model.named_parameters():
-        # freeze base model's layers
-        param.requires_grad = False
-
-    # if not is_gptq_quantized:
-    #     # cast all non INT8 parameters to fp32
-    #     for param in model.parameters():
-    #         if (param.dtype == torch.float16) or (param.dtype == torch.bfloat16):
-    #             param.data = param.data.to(torch.float32)
-
-    if (loaded_in_kbit or is_gptq_quantized) and use_gradient_checkpointing:
-        # For backward compatibility
-        if hasattr(model, "enable_input_require_grads"):
-            model.enable_input_require_grads()
-        else:
-
-            def make_inputs_require_grad(module, input, output):
-                output.requires_grad_(True)
-
-            model.get_input_embeddings().register_forward_hook(make_inputs_require_grad)
-
-        # enable gradient checkpointing for memory efficiency
-        model.gradient_checkpointing_enable()
-
-    return model
-
-
 
 torch.backends.cuda.matmul.allow_tf32 = True
 
 IGNORE_INDEX = -100
 
 def clean_memory():
     gc.collect()
@@ -115,15 +74,15 @@
 
 @dataclass
 class ModelArguments:
     model_name_or_path: Optional[str] = field(
         default="EleutherAI/pythia-12b"
     )
     trust_remote_code: Optional[bool] = field(
-        default=True,
+        default=False,
         metadata={"help": "Enable unpickling of arbitrary code in AutoModelForCausalLM#from_pretrained."}
     )
     # use_auth_token: Optional[bool] = field(
     #     default=False,
     #     metadata={"help": "Enables using Huggingface auth token from Git Credentials."}
     # )
 
@@ -132,19 +91,19 @@
     force_remove_overlength_samples: bool = field(
         default=True,
         metadata={"help": "Remove overlength samples."}
     )
     eval_dataset_size: float = field(
         default=0.02, metadata={"help": "Ratio of dataset to use for validation."}
     )
-    max_train_samples: Optional[float] = field(
+    max_train_samples: Optional[int] = field(
         default=None,
         metadata={
             "help": "For debugging purposes or quicker training, truncate the number of training examples to this "
-            "value if set. If set to a float, will truncate the number of examples to that percentage of the dataset."
+            "value if set."
         },
     )
     max_eval_samples: Optional[int] = field(
         default=None,
         metadata={
             "help": "For debugging purposes or quicker training, truncate the number of evaluation examples to this "
             "value if set."
@@ -155,40 +114,31 @@
         metadata={"help": "Maximum model length (input and output).  Sequences will be right padded (and possibly truncated)."},
     )
     dataset: str = field(
         default='alpaca',
         metadata={"help": "Which dataset to finetune on. See datamodule for options."}
     )
     dataset_format: Optional[str] = field(
-        default="conversations",
-        metadata={"help": "Which dataset format is used. [alpaca|conversations|chip2|self-instruct|hh-rlhf|mistral]"}
-    )
-    prompt_type: Optional[str] = field(
         default=None,
-        metadata={"help": "Which prompt type to use. [alpaca|chatlm|conversations|chip2|self-instruct|hh-rlhf|mistral]"}
+        metadata={"help": "Which dataset format is used. [alpaca|chip2|self-instruct|hh-rlhf|mistral]"}
     )
 
 @dataclass
 class TrainingArguments(transformers.Seq2SeqTrainingArguments):
     task_name: str = field(
         default=None,
         metadata={"help": "The name of the task to train on."},
     )
     flash_attention: bool = field(
         default=True,
         metadata={"help": "Use flash attention."}
-    )
-
-    long_lora: bool = field(
-        default=False,
-        metadata={"help": "Use long lora."}
-    )
+    ) 
 
     rerope: bool = field(
-        default=False,
+        default=False, 
         metadata={"help": "Use rerope."}
     )
     rerope_window: int = field(
         default=None,
         metadata={"help": "Rerope window size."}
     )
 
@@ -197,25 +147,14 @@
         metadata={"help": "Use neftune."}
     )
     noise_alpha: float = field(
         default=5.0,
         metadata={"help": "Neftune noise alpha."}
     )
 
-
-    sliding_window: int = field(
-        default=4096,
-        metadata={"help": "Sliding window size."}
-    )
-
-    rope_theta: float = field(
-        default=10000,
-        metadata={"help": "Rope theta."}
-    )
-
     wandb: str = field(
         default=None,
         metadata={"help": "Wandb project name."}
     )
 
     sample_packing: bool = field(
         default=False,
@@ -329,71 +268,47 @@
             lora_module_names.add(names[0] if len(names) == 1 else names[-1])
 
 
     if 'lm_head' in lora_module_names: # needed for 16-bit
         lora_module_names.remove('lm_head')
     return list(lora_module_names)
 
-class CleanMemoryCallback(transformers.TrainerCallback):
+class TrainHelperCallback(transformers.TrainerCallback):
     def on_step_end(self, args, state, control, **kwargs):
         clean_memory()
 
     def on_evaluate(self, args, state, control, **kwargs):
         clean_memory()
 
-from transformers import TrainerCallback
-class LoggingCallback(TrainerCallback):
-    def on_log(self, args, state, control, logs=None, **kwargs):
-        _ = logs.pop("total_flos", None)
-        if state.is_local_process_zero:
-            if "eval_loss" in logs:
-                logger.info(logs)
-            else:
-                logger.debug(logs)
-
-class SavePeftModelCallback(TrainerCallback):
+class SavePeftModelCallback(transformers.TrainerCallback):
     def save_model(self, args, state, kwargs):
         logger.info('Saving PEFT checkpoint...')
-        # if state.best_model_checkpoint is not None:
-        #     checkpoint_folder = os.path.join(state.best_model_checkpoint, "adapter_model")
-        # else:
-        #     checkpoint_folder = os.path.join(args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{state.global_step}")
-        checkpoint_folder = os.path.join(args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{state.global_step}")
+        if state.best_model_checkpoint is not None:
+            checkpoint_folder = os.path.join(state.best_model_checkpoint, "adapter_model")
+        else:
+            checkpoint_folder = os.path.join(args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{state.global_step}")
 
         peft_model_path = os.path.join(checkpoint_folder, "adapter_model")
         kwargs["model"].save_pretrained(peft_model_path)
 
         pytorch_model_path = os.path.join(checkpoint_folder, "pytorch_model.bin")
         if os.path.exists(pytorch_model_path):
             os.remove(pytorch_model_path)
 
-        self._symlink_latest_checkpoint(checkpoint_folder)
-
-    def _symlink_latest_checkpoint(self, checkpoint_folder):
-        # if the latest checkpoint is a symlink, remove it
-        output_dir = os.path.dirname(checkpoint_folder)
-        latest_checkpoint = os.path.join(output_dir, "latest")
-        if os.path.islink(latest_checkpoint):
-            os.remove(latest_checkpoint)
-        # symlink the latest checkpoint to the checkpoint folder
-        os.symlink(os.path.basename(checkpoint_folder), latest_checkpoint)
-
     def on_save(self, args, state, control, **kwargs):
-        if state.is_local_process_zero:
-            self.save_model(args, state, kwargs)
+        self.save_model(args, state, kwargs)
         return control
 
     def on_train_end(self, args, state, control, **kwargs):
         def touch(fname, times=None):
             with open(fname, 'a'):
                 os.utime(fname, times)
 
-        if state.is_local_process_zero:
-            touch(join(args.output_dir, 'completed'))
-            self.save_model(args, state, kwargs)
+        touch(join(args.output_dir, 'completed'))
+        self.save_model(args, state, kwargs)
 
 def get_accelerate_model(args, checkpoint_dir):
 
     n_gpus = torch.cuda.device_count()
     max_memory = f'{args.max_memory_MB}MB'
     max_memory = {i: max_memory for i in range(n_gpus)}
     device_map = "auto"
@@ -408,31 +323,20 @@
     if args.full_finetune: assert args.bits in [16, 32]
 
     logger.info(f'loading base model {args.model_name_or_path}...')
 
     config = transformers.AutoConfig.from_pretrained(
         args.model_name_or_path,
         cache_dir=args.cache_dir,
-        trust_remote_code=args.trust_remote_code,
     )
     orig_ctx_len = getattr(config, "max_position_embeddings", None)
     if orig_ctx_len and args.model_max_len > orig_ctx_len:
         scaling_factor = float(math.ceil(args.model_max_len / orig_ctx_len))
         config.rope_scaling = {"type": "linear", "factor": scaling_factor}
 
-    config.sliding_window = args.sliding_window
-    config.rope_theta = args.rope_theta
-
-
-    if "qwen" in args.model_name_or_path.lower():
-        if args.bf16:
-            config.bf16 = True
-        elif args.fp16:
-            config.fp16 = True
-
     compute_dtype = (torch.float16 if args.fp16 else (torch.bfloat16 if args.bf16 else torch.float32))
     model_kwargs = {
         "cache_dir": args.cache_dir,
         "load_in_4bit": args.bits == 4,
         "load_in_8bit": args.bits == 8,
         "device_map": device_map if not args.deepspeed else None,
         "max_memory": max_memory if not args.deepspeed else None,
@@ -441,56 +345,47 @@
             load_in_8bit=args.bits == 8,
             llm_int8_threshold=6.0,
             llm_int8_has_fp16_weight=False,
             bnb_4bit_compute_dtype=compute_dtype,
             bnb_4bit_use_double_quant=args.double_quant,
             bnb_4bit_quant_type=args.quant_type,
         ) if args.bits in (4, 8) else None,
-        "torch_dtype": (torch.float16 if args.fp16 else (torch.bfloat16 if args.bf16 else torch.float32)),
+        "torch_dtype": (torch.float32 if args.fp16 else (torch.bfloat16 if args.bf16 else torch.float32)),
         "trust_remote_code": args.trust_remote_code,
         "use_flash_attention_2": args.flash_attention,
         # "use_auth_token": args.use_auth_token
     }
-
-    # if args.mpt:
-    #     model_kwargs["attn_config"] = {"attn_impl": "triton"}
-
-    logger.info(f"{model_kwargs=}")
+    if args.mpt:
+        model_kwargs["attn_config"] = {"attn_impl": "triton"}
     # model = AutoModelForCausalLM.from_pretrained(args.model_name_or_path, **model_kwargs)
     model = AutoModelForCausalLM.from_pretrained(args.model_name_or_path, config=config, **model_kwargs)
     if compute_dtype == torch.float16 and args.bits == 4:
         major, minor = torch.cuda.get_device_capability()
         if major >= 8:
             print('='*80)
             print('Your GPU supports bfloat16, you can accelerate training with the argument --bf16')
             print('='*80)
 
     setattr(model, 'model_parallel', True)
     setattr(model, 'is_parallelizable', True)
 
-    model.config.torch_dtype=(torch.float16 if args.fp16 else (torch.bfloat16 if args.bf16 else torch.float32))
+    model.config.torch_dtype=(torch.float32 if args.fp16 else (torch.bfloat16 if args.bf16 else torch.float32))
 
     if not args.full_finetune:
-
-        if "qwen" in args.model_name_or_path.lower():
-            model = qwen_prepare_model_for_kbit_training(model, use_gradient_checkpointing=args.gradient_checkpointing)
-        else:
-            model = prepare_model_for_kbit_training(model, use_gradient_checkpointing=args.gradient_checkpointing)
-
+        model = prepare_model_for_kbit_training(model, use_gradient_checkpointing=args.gradient_checkpointing)
     if args.gradient_checkpointing:
         model.gradient_checkpointing_enable()
 
     if not args.full_finetune:
         if checkpoint_dir is not None:
             logger.info("Loading adapters from checkpoint.")
             model = PeftModel.from_pretrained(model, join(checkpoint_dir, 'adapter_model'), is_trainable=True)
         else:
             logger.info(f'adding LoRA modules...')
             modules = find_all_linear_names(args, model)
-            print(f"LoRA modules: {modules}")
             config = LoraConfig(
                 r=args.lora_r,
                 lora_alpha=args.lora_alpha,
                 target_modules=modules,
                 lora_dropout=args.lora_dropout,
                 bias="none",
                 task_type="CAUSAL_LM",
@@ -501,15 +396,15 @@
         if "norm" in name:
             module.to(compute_dtype)
         if "lm_head" in name or "embed_tokens" in name:
             if hasattr(module, "weight"):
                 module.to(compute_dtype)
 
     if args.neftune:
-        from speechless.patches.neftune_monkey_patch import NEFTune
+        from patches.neftune_monkey_patch import NEFTune
         model = NEFTune(model, noise_alpha=args.noise_alpha)
 
     return model
 
 def print_trainable_parameters(args, model):
     """
     Prints the number of trainable parameters in the model.
@@ -597,14 +492,31 @@
         data_dict = {
             'input_ids': input_ids,
             'labels': labels,
             'attention_mask':input_ids.ne(self.tokenizer.pad_token_id),
         }
         return data_dict
 
+def extract_unnatural_instructions_data(examples, extract_reformulations=False):
+    out = {
+        'input': [],
+        'output': [],
+    }
+    for example_instances in examples['instances']:
+        for instance in example_instances:
+            out['input'].append(instance['instruction_with_input'])
+            out['output'].append(instance['output'])
+    if extract_reformulations:
+        for example_reformulations in examples['reformulations']:
+            if example_reformulations is not None:
+                for instance in example_reformulations:
+                    out['input'].append(instance['instruction_with_input'])
+                    out['output'].append(instance['output'])
+    return out
+
 ALPACA_PROMPT_DICT = {
     "prompt_input": (
         "Below is an instruction that describes a task, paired with an input that provides further context. "
         "Write a response that appropriately completes the request.\n\n"
         "### Instruction:\n{instruction}\n\n### Input:\n{input}\n\n### Response: "
     ),
     "prompt_no_input": (
@@ -623,460 +535,35 @@
     "prompt_no_input": (
         "Below is an instruction that describes a task. "
         "Write a response that appropriately completes the request.\n\n"
         "### Instruction:\n{instruction}\n\n### Response:\n"
     ),
 }
 
-
-def preprocess_toolbench_dataset(
-    example,
-    model_max_len: int,
-    tokenizer: transformers.PreTrainedTokenizer,
-    template: str="tool-llama-single-round"
-) -> Dict:
-    # conv = get_conversation_template(template)
-    # if template == "tool-llama":
-    #     roles = {"human": conv.roles[0], "gpt": conv.roles[1]}
-    # elif template == "tool-llama-single-round" or template == "tool-llama-multi-rounds":
-    #     roles = {"system": conv.roles[0], "user": conv.roles[1], "function": conv.roles[2], "assistant": conv.roles[3]}
-
-    roles = {"system": "System", "user": "User", "function": "Function", "assistant": "Assistant"}
-    seps = ["\n", "</s>"]
-
-
-    # Apply prompt templates
-    conversation = ""
-    for i, round in enumerate(example['conversations']):
-        role = roles[round['from']]
-        message = round['value']
-        if i + 1 == len(example['conversations']) and message:
-            conversation += role + ": " + str(message) + seps[1]
-        elif message:
-            conversation += role + ": " + str(message) + seps[0]
-        else:
-            conversation += role + ":"
-
-
-
-    # Tokenize conversations
-    input_ids = tokenizer(
-        conversation,
-        # return_tensors="pt",
-        # padding="max_length",
-        max_length=model_max_len,
-        truncation=True,
-        # add_special_tokens=False,
-    ).input_ids
-    # input_ids begin with '<s>' and end with '</s>'
-    assert input_ids[0] == tokenizer.bos_token_id and input_ids[-1] == tokenizer.eos_token_id
-    labels = copy.deepcopy(input_ids)
-
-    input_ids = torch.tensor(input_ids)
-    labels = torch.tensor(labels)
-
-    # Mask targets. Only compute loss on the assistant outputs.
-    sep = seps[0] + roles['assistant'] + ": "
-
-    total_len = int(labels.ne(tokenizer.pad_token_id).sum())
-    turns = conversation.split(seps[1])
-    cur_len = 1
-    labels[:cur_len] = IGNORE_INDEX
-    for i, turn in enumerate(turns):
-        if turn == "":
-            continue
-        turn_len = len(tokenizer(turn).input_ids)
-
-        parts = turn.split(sep)
-
-        # only train on the last assistant reply, treat the history chat as instruction
-        prefix = parts[:-1]
-        instruction = ""
-        for part in prefix:
-            instruction += part
-            instruction += sep
-
-        # "-2" is hardcoded for the LLaMA tokenizer to make the offset correct.
-        instruction_len = len(tokenizer(instruction).input_ids) - 2
-
-        # Ignore the user instructions
-        labels[cur_len : cur_len + instruction_len] = IGNORE_INDEX
-        cur_len += turn_len
-
-    labels[cur_len:] = IGNORE_INDEX
-
-    # if False:  # Inspect and check the correctness of masking
-    #     z = labels.clone()
-    #     z = torch.where(z == IGNORE_TOKEN_ID, tokenizer.unk_token_id, z)
-    #     rank0_print(tokenizer.decode(z))
-
-    if cur_len < model_max_len:
-        if cur_len != total_len:
-            labels[:] = IGNORE_INDEX
-            logger.warning(
-                f"WARNING: tokenization mismatch: {cur_len} vs. {total_len}."
-                f" (ignored)"
-                f"{conversation=}"
-            )
-    return dict(
-        input_ids=input_ids,
-        labels=labels,
-        # attention_mask=input_ids.ne(tokenizer.pad_token_id),
-    )
-
-def preprocess_multi_rounds_dialog(
-    example,
-    model_max_len: int,
-    tokenizer: transformers.PreTrainedTokenizer,
-) -> Dict:
-    # conv = get_conversation_template(template)
-    # if template == "tool-llama":
-    #     roles = {"human": conv.roles[0], "gpt": conv.roles[1]}
-    # elif template == "tool-llama-single-round" or template == "tool-llama-multi-rounds":
-    #     roles = {"system": conv.roles[0], "user": conv.roles[1], "function": conv.roles[2], "assistant": conv.roles[3]}
-
-    roles = {"system": "System", "user": "User", "function": "Function", "assistant": "Assistant"}
-    seps = ["\n", "</s>"]
-
-    # The dialogue process is divided into multiple rounds, with each round ending when the Assistant speaks.
-    dialog = example['conversations']
-    dialog_rounds = []
-    round_messages = []
-    for i, round in enumerate(dialog):
-        who = round['from']
-        message = round['value']
-        if who != 'assistant':
-            round_messages.append((who, message))
-        else:
-            dialog_rounds.append({
-                'round_messages': round_messages,
-                'assistant': message,
-            })
-            round_messages = []
-    if len(round_messages) > 0:
-        logger.warning(f"WARNING: the last round is not ended by the assistant. IGNORE!!!. {dialog=}")
-        dialog_rounds = []
-    # print(f"{dialog_rounds=}")
-
-    example_input_ids = None
-    example_output_ids = None
-    for idx, round in enumerate(dialog_rounds):
-        round_messages = round['round_messages']
-        assistant_message = round['assistant']
-        source = ""
-        for (who, message) in round_messages:
-            source += roles[who] + ": " + str(message) + seps[0]
-        source += roles['assistant'] + ": "
-        target = assistant_message + tokenizer.eos_token
-
-        # source = f"{tokenizer.bos_token}{source}"
-        # target = f"{bot_response.strip()}\n{tokenizer.eos_token}"
-
-        tokenized_source = tokenizer(source, max_length=model_max_len, truncation=True, add_special_tokens=False)
-        tokenized_target = tokenizer(target, max_length=model_max_len, truncation=True, add_special_tokens=False)
-        tokenized_input = torch.tensor(tokenized_source['input_ids'] + tokenized_target['input_ids'])
-        tokenized_output = torch.tensor([IGNORE_INDEX for _ in range(len(tokenized_source['input_ids']))] +
-                                        copy.deepcopy(tokenized_target['input_ids']))
-        if idx == 0:
-            example_input_ids = tokenized_input
-            example_output_ids = tokenized_output
-        else:
-            example_input_ids = torch.concatenate((example_input_ids, tokenized_input), dim=0)
-            example_output_ids = torch.concatenate((example_output_ids, tokenized_output), dim=0)
-
-    input_ids = example_input_ids
-    labels = example_output_ids
-    return dict(
-        input_ids=input_ids,
-        labels=labels,
-        # attention_mask=input_ids.ne(tokenizer.pad_token_id),
-    )
-
-
-def generate_round_prompt_toolllama(
-    idx: int,
-    human_input: str,
-    bot_response: str,
-    bos_token: str,
-    eos_token: str,
-    system_prompt: str = None,
-):
-    if idx == 0:
-        if system_prompt:
-            source = f"{system_prompt} Human: {human_input} Assistant: "
-        else:
-            system_prompt = "A chat between a curious user and an artificial intelligence assistant who can use external tools and APIs to solve the user's question."
-            "The assistant gives tools and APIs calling processes or final answer to the human's question."
-            human_input = "Human: {instruction} Assistant: ".format(instruction=human_input)
-            source = f"{system_prompt} {human_input}"
-    else:
-        human_input = "Human: {instruction} Assistant: ".format(instruction=human_input)
-        source = f"{human_input}"
-    source = f"{bos_token}{source}"
-    target = f"{bot_response.strip()}\n{eos_token}"
-
-    return source, target
-
-
-def generate_round_prompt_alpaca(
-    idx: int,
-    human_input: str,
-    bot_response: str,
-    bos_token: str,
-    eos_token: str,
-    system_prompt: str = None,
-):
-    if idx == 0:
-        if system_prompt:
-            source = f"{system_prompt}\n\n### Instruction:\n{human_input}\n\n### Response:"
-        else:
-            system_prompt = "Below is an instruction that describes a task.\nWrite a response that appropriately completes the request.\n\n"
-            human_input = "### Instruction:\n{instruction}\n\n### Response:".format(instruction=human_input)
-            source = f"{system_prompt}{human_input}"
-    else:
-        human_input = "### Instruction:\n{instruction}\n\n### Response:".format(instruction=human_input)
-        source = f"{human_input}"
-
-    source = f"{bos_token}{source}"
-    target = f"{bot_response.strip()}\n{eos_token}"
-
-    return source, target
-
-def generate_round_prompt_llama2(
-    idx: int,
-    human_input: str,
-    bot_response: str,
-    bos_token: str,
-    eos_token: str,
-    system_prompt: str = None,
-):
-    if idx == 0:
-        if system_prompt:
-            source = f"{bos_token}[INST] <<SYS>>\n{system_prompt}\n<</SYS>>\n{human_input}[/INST]"
-        else:
-            source = f"{bos_token}[INST]{human_input}[/INST]"
-    else:
-        source = f"[INST]{human_input}[/INST]"
-
-    target = f"{bot_response.strip()}\n{eos_token}"
-
-    return source, target
-
-def generate_round_prompt_chatlm(
-    idx: int,
-    human_input: str,
-    bot_response: str,
-    bos_token: str,
-    eos_token: str,
-    system_prompt: str = None,
-):
-    # f"<|im_start|>system\n{system_message}<|im_end|>\n<|im_start|>user\n{user_message}<|im_end|>\n<|im_start|>assistant"
-    if idx == 0:
-        # if system_prompt:
-        #     # source = f"{system_prompt}\n\n### Instruction:\n{human_input}\n\n### Response:"
-        #     source = f"<|im_start|>system\n{system_prompt}<|im_end|>\n"
-        # else:
-        #     # system_prompt = "Below is an instruction that describes a task.\nWrite a response that appropriately completes the request.\n\n"
-        system_prompt = "You are a cautious assistant. You carefully follow instructions. You are helpful and harmless and you follow ethical guidelines and promote positive behavior."
-        human_input = f"<|im_start|>user\n{human_input}<|im_end|>\n<|im_start|>assistant"
-        source = f"<|im_start|>system\n{system_prompt}<|im_end|>\n{human_input}"
-    else:
-        human_input = f"<|im_start|>user\n{human_input}<|im_end|>\n<|im_start|>assistant"
-        source = f"{human_input}"
-
-    source = f"{bos_token}{source}"
-    target = f"{bot_response.strip()}\n{eos_token}"
-
-    return source, target
-
-@dataclass
-class DialogDataCollatorForCausalLM(object):
-    tokenizer: transformers.PreTrainedTokenizer
-    model_max_len: int
-    prompt_type: str = None
-
-    def __call__(self, instances: Sequence[Dict]) -> Dict[str, torch.Tensor]:
-        # Extract elements
-        input_ids = []
-        labels = []
-        for example in instances:
-            # system_prompt = example.get('system_prompt', 'A Bot').strip() + "\n\n"
-            if self.prompt_type is not None:
-                prompt_type = self.prompt_type
-            else:
-                prompt_type = example.get('prompt_type', None)
-            if prompt_type == "tool-llama-single-round":
-                data_dict = preprocess_toolbench_dataset(example,
-                                                   model_max_len=self.model_max_len,
-                                                   tokenizer=self.tokenizer,
-                                                   template="tool-llama-single-round")
-                example_input_ids = data_dict['input_ids']
-                example_labels = data_dict['labels']
-                if example_input_ids is not None:
-                    # print(f"{example_input_ids.shape=},{example_input_ids=}")
-                    # print(f"{example_labels.shape=},{example_labels=}")
-                    input_ids.append(example_input_ids)
-                    labels.append(example_labels)
-                continue
-
-            elif prompt_type == "tool-llama-multi-rounds":
-                data_dict = preprocess_multi_rounds_dialog(example,
-                                                   model_max_len=self.model_max_len,
-                                                   tokenizer=self.tokenizer,
-                )
-                example_input_ids = data_dict['input_ids']
-                example_labels = data_dict['labels']
-                if example_input_ids is not None:
-                    # print(f"{example_input_ids.shape=},{example_input_ids=}")
-                    # print(f"{example_labels.shape=},{example_labels=}")
-                    input_ids.append(example_input_ids)
-                    labels.append(example_labels)
-                continue
-
-            system_prompt = example.get('system_prompt', "").strip()
-            if system_prompt:
-                system_prompt += "\n\n"
-            example_input_ids = None
-            example_output_ids = None
-
-            # human_bot_dialog = example['dialog']
-            human_bot_dialog = []
-            dialog = example['conversations']
-            for _i in range(len(dialog) // 2):
-                human_input = dialog[2 * _i]['value']
-                bot_output = dialog[2 * _i + 1]['value']
-                human_bot_dialog.append((human_input, bot_output))
-            if len(human_bot_dialog) < 1:
-                continue
-            for idx, round in enumerate(human_bot_dialog):
-                human_input, bot_response = round
-                if prompt_type == 'toolllama':
-                    source, target = generate_round_prompt_toolllama(
-                        idx,
-                        human_input,
-                        bot_response,
-                        bos_token=self.tokenizer.bos_token,
-                        eos_token=self.tokenizer.eos_token,
-                        system_prompt=system_prompt,
-                    )
-                elif prompt_type == "chatlm":
-                    source, target = generate_round_prompt_chatlm(
-                        idx,
-                        human_input,
-                        bot_response,
-                        bos_token=self.tokenizer.bos_token,
-                        eos_token=self.tokenizer.eos_token,
-                        system_prompt=system_prompt,
-                    )
-                elif prompt_type == "llama2":
-                    source, target = generate_round_prompt_llama2(
-                        idx,
-                        human_input,
-                        bot_response,
-                        bos_token=self.tokenizer.bos_token,
-                        eos_token=self.tokenizer.eos_token,
-                        system_prompt=system_prompt,
-                    )
-                else: # default alpaca
-                    source, target = generate_round_prompt_alpaca(
-                        idx,
-                        human_input,
-                        bot_response,
-                        bos_token=self.tokenizer.bos_token,
-                        eos_token=self.tokenizer.eos_token,
-                        system_prompt=system_prompt,
-                    )
-
-                tokenized_source = self.tokenizer(source,
-                                                  max_length=self.model_max_len,
-                                                  truncation=True,
-                                                  add_special_tokens=False,
-                                                  )
-                tokenized_target = self.tokenizer(target,
-                                                  max_length=self.model_max_len,
-                                                  truncation=True,
-                                                  add_special_tokens=False,
-                                                  )
-                tokenized_input = torch.tensor(tokenized_source['input_ids'] + tokenized_target['input_ids'])
-                tokenized_output = torch.tensor([IGNORE_INDEX for _ in range(len(tokenized_source['input_ids']))] +
-                                                copy.deepcopy(tokenized_target['input_ids']))
-
-                # print(f"{source=}")
-                # print(f"{tokenized_input=}")
-                # print(f"{target=}")
-                # print(f"{tokenized_target=}")
-                if idx == 0:
-                    example_input_ids = tokenized_input
-                    example_output_ids = tokenized_output
-                else:
-                    example_input_ids = torch.concatenate((example_input_ids, tokenized_input), dim=0)
-                    example_output_ids = torch.concatenate((example_output_ids, tokenized_output), dim=0)
-
-            input_ids.append(example_input_ids)
-            labels.append(example_output_ids)
-
-        # print(f"{example=}")
-        # print(f"{input_ids=}")
-        # print(f"{labels=}")
-        # Apply padding
-        if self.tokenizer.padding_side == "left":
-            input_ids = [t.flip(-1) for t in input_ids]
-            labels = [t.flip(-1) for t in labels]
-        input_ids = pad_sequence(input_ids, batch_first=True, padding_value=self.tokenizer.pad_token_id)
-        labels = pad_sequence(labels, batch_first=True, padding_value=IGNORE_INDEX)
-        if self.tokenizer.padding_side == "left":
-            input_ids = input_ids.flip(-1)
-            labels = labels.flip(-1)
-
-        data_dict = {
-            'input_ids': input_ids,
-            'labels': labels,
-            'attention_mask':input_ids.ne(self.tokenizer.pad_token_id),
-        }
-        return data_dict
-
-
-def extract_unnatural_instructions_data(examples, extract_reformulations=False):
-    out = {
-        'input': [],
-        'output': [],
-    }
-    for example_instances in examples['instances']:
-        for instance in example_instances:
-            out['input'].append(instance['instruction_with_input'])
-            out['output'].append(instance['output'])
-    if extract_reformulations:
-        for example_reformulations in examples['reformulations']:
-            if example_reformulations is not None:
-                for instance in example_reformulations:
-                    out['input'].append(instance['instruction_with_input'])
-                    out['output'].append(instance['output'])
-    return out
-
 def extract_alpaca_dataset(example):
     if example.get("input", "") != "":
         prompt_format = ALPACA_PROMPT_DICT["prompt_input"]
     else:
         prompt_format = ALPACA_PROMPT_DICT["prompt_no_input"]
     return {'input': prompt_format.format(**example)}
 
-def local_dataset(dataset_name, test_size=0.02):
+def local_dataset(dataset_name):
     if dataset_name.endswith(('.json', '.jsonl')):
         full_dataset = Dataset.from_json(path_or_paths=dataset_name)
     elif dataset_name.endswith('.csv'):
         full_dataset = Dataset.from_pandas(pd.read_csv(dataset_name))
     elif dataset_name.endswith('.tsv'):
         full_dataset = Dataset.from_pandas(pd.read_csv(dataset_name, delimiter='\t'))
     else:
         raise ValueError(f"Unsupported dataset format: {dataset_name}")
 
     if 'category' in full_dataset.column_names:
         full_dataset = full_dataset.class_encode_column('category')
-        return full_dataset.train_test_split(test_size=test_size, stratify_by_column='category')
-    return full_dataset.train_test_split(test_size=test_size)
+        return full_dataset.train_test_split(test_size=0.02, stratify_by_column='category')
+    return full_dataset.train_test_split(test_size=0.02)
 
 class RepeatDataset():
     def __init__(self, ds, repeat_batch_size, repeat_steps):
         self.ds = ds
         self.batch_size = repeat_batch_size * repeat_steps
         self.in_cache = []
         self.out_cache = []
@@ -1164,92 +651,73 @@
             return load_dataset("timdettmers/openassistant-guanaco")
         elif dataset_name == 'vicuna':
             raise NotImplementedError("Vicuna data was not released.")
         else:
             if os.path.exists(dataset_name):
                 try:
                     args.dataset_format = args.dataset_format if args.dataset_format else "input-output"
-                    full_dataset = local_dataset(dataset_name, test_size=args.eval_dataset_size)
+                    full_dataset = local_dataset(dataset_name)
                     return full_dataset
                 except:
                     raise ValueError(f"Error loading dataset from {dataset_name}")
             else:
                 raise NotImplementedError(f"Dataset {dataset_name} not implemented yet.")
 
     def format_dataset(dataset, dataset_format):
         if (
             dataset_format == 'alpaca' or dataset_format == 'alpaca-clean' or
             (dataset_format is None and args.dataset in ['alpaca', 'alpaca-clean'])
         ):
             dataset = dataset.map(extract_alpaca_dataset, remove_columns=['instruction'])
-            dataset = dataset.map(lambda x: {
-                'conversations': [(x['input'], x['output'])]
-            })
-
         elif dataset_format == 'chip2' or (dataset_format is None and args.dataset == 'chip2'):
-            # dataset = dataset.map(lambda x: {
-            #     'input': x['text'].split('\n<bot>: ')[0].replace('<human>: ', ''),
-            #     'output': x['text'].split('\n<bot>: ')[1],
-            # })
             dataset = dataset.map(lambda x: {
-                'conversations': [(x['text'].split('\n<bot>: ')[0].replace('<human>: ', ''), x['text'].split('\n<bot>: ')[1])]
+                'input': x['text'].split('\n<bot>: ')[0].replace('<human>: ', ''),
+                'output': x['text'].split('\n<bot>: ')[1],
             })
         elif dataset_format == 'self-instruct' or (dataset_format is None and args.dataset == 'self-instruct'):
-            # for old, new in [["prompt", "input"], ["completion", "output"]]:
-            #     dataset = dataset.rename_column(old, new)
-            dataset = dataset.map(lambda x: {
-                'conversations': [(x['prompt'], x['completion'])]
-            })
+            for old, new in [["prompt", "input"], ["completion", "output"]]:
+                dataset = dataset.rename_column(old, new)
         elif dataset_format == 'hh-rlhf' or (dataset_format is None and args.dataset == 'hh-rlhf'):
-            # dataset = dataset.map(lambda x: {
-            #     'input': '',
-            #     'output': x['chosen']
-            # })
             dataset = dataset.map(lambda x: {
-                'conversations': [('', x['chosen'])]
+                'input': '',
+                'output': x['chosen']
             })
         elif dataset_format == 'oasst1' or (dataset_format is None and args.dataset == 'oasst1'):
-            # dataset = dataset.map(lambda x: {
-            #     'input': '',
-            #     'output': x['text'],
-            # })
             dataset = dataset.map(lambda x: {
-                'conversations': [('', x['text'])]
+                'input': '',
+                'output': x['text'],
             })
         elif dataset_format == 'airoboros':
             logger.info("---------- Formatting dataset for Airoboros. ----------")
             def _format_airoboros(instruction):
                 # FIXME - for Spider prompt
                 if "### Instructions:" in instruction["instruction"]:
                     in_ = instruction["instruction"]
                     out_ = instruction['response']
-                    # return {
-                    #     'input': in_,
-                    #     'output': out_,
-                    # }
-                    return {'conversations': [(in_, out_)]}
+                    return {
+                        'input': in_,
+                        'output': out_,
+                    }
                 else:
                     in_ = None
                     if instruction.get("skip_prompt_formatting"):
                         in_ = instruction["instruction"].strip() + "\n"
                     else:
                         in_ = "\n".join([
                             (instruction.get('system') or 'A chat.').strip(),
                             f"USER: {instruction['instruction'].strip()}",
                         ])
                         if in_.endswith("PLAINFORMAT"):
                             in_ = re.sub(r"\s+PLAINFORMAT$", "", in_, re.DOTALL)
                             in_ += " PLAINFORMAT"
                         in_ = "\n".join([in_.strip(), "ASSISTANT: "])
-                    # return {
-                    #     'input': in_,
-                    #     'output': instruction['response'].strip() + "\n",
-                    # }
-                    return {'conversations': [(in_, instruction['response'].strip() + "\n")]}
-
+                    return {
+                        'input': in_,
+                        'output': instruction['response'].strip() + "\n",
+                    }
             dataset = dataset.map(_format_airoboros)
         elif dataset_format == 'mistral':
             logger.info("---------- Formatting dataset for Mistral. ----------")
             def _format_mistral(instruction):
                 # FIXME - for Spider prompt
                 if "### Instructions:" in instruction["instruction"]:
                     in_ = instruction["instruction"]
@@ -1264,42 +732,38 @@
                             input = second_toks[0]
                             response = second_toks[1]
                             in_ = "<s>[INST] " + first + " [/INST]\n" + input + "</s> " + "[INST] " + response + " [/INST]"
 
                     out_ = instruction['response'] + "</s>"
                     # print(f"{in_=}")
                     # print(f"{out_=}")
-                    # return {
-                    #     'input': in_,
-                    #     'output': out_,
-                    # }
-                    return {'conversations': [(in_, out_)]}
+                    return {
+                        'input': in_,
+                        'output': out_,
+                    }
                 else:
                     in_ = f"<s>[INST] {instruction['instruction']} [/INST]"
                     out_ = f"{instruction['response']}</s>"
-                    # return {
-                    #     'input': in_,
-                    #     'output': out_,
-                    # }
-                    return {'conversations': [(in_, out_)]}
+                    return {
+                        'input': in_,
+                        'output': out_,
+                    }
             dataset = dataset.map(_format_mistral)
         elif dataset_format == 'llama2':
             logger.info("---------- Formatting dataset for Llama2. ----------")
             def _format_llama2(instruction):
                 sys_msg = instruction.get('system', 'A chat.')
                 user_msg = instruction['instruction']
                 mode_msg = instruction['response']
                 in_ = f"<s>[INST] <<SYS>>\n{sys_msg}\n<</SYS>>\n{user_msg}[/INST]"
                 out_ = f"{instruction['response']}</s>"
-                # return {
-                #     'input': in_,
-                #     'output': out_,
-                # }
-                return {'conversations': [(in_, out_)]}
-
+                return {
+                    'input': in_,
+                    'output': out_,
+                }
             dataset = dataset.map(_format_llama2)
 
         elif dataset_format == 'instruction-input-response':
 
             def _format_instruction_input_response(example):
                 if example.get("input", "") != "":
                     in_ = PROMPT_DICT["prompt_input"].format(instruction=example["instruction"], input=example["input"])
@@ -1307,56 +771,37 @@
                     in_ = PROMPT_DICT["prompt_no_input"].format(instruction=example["instruction"])
                 out_ = f"{example['response']}"
                 # out_lines = out_.strip().split("\n")
                 # if len(out_lines) > 1:
                 #     if out_lines[0].startswith("```"):
                 #         in_ += out_lines[0] + "\n"
                 #         out_ = "\n".join(out_lines[1:])
-
-                # return {'input': in_,
-                #         'output': out_}
-                return {'conversations': [(in_, out_)]}
+                    
+                return {'input': in_,
+                        'output': out_}
 
             dataset = dataset.map(_format_instruction_input_response)
 
         elif dataset_format == 'input-output':
             # leave as is
             pass
             def _format_input_output(instruction):
-                # return {
-                #     'input': instruction['instruction'],
-                #     'output': instruction['response'],
-                # }
-                return {'conversations': [(instruction['instruction'], instruction['response'])]}
-
+                return {
+                    'input': instruction['instruction'],
+                    'output': instruction['response'],
+                }
             dataset = dataset.map(_format_input_output)
-        elif dataset_format == 'conversations':
-            def _format_multi_turns(example):
-                human_bot_dialog = []
-                dialog = example['conversations']
-                for round in dialog:
-                    who = round['from']
-                    response = round['value']
-                    human_bot_dialog.append({
-                        "from": who,
-                        "value": response,
-                    })
-                return {'conversations': human_bot_dialog}
-
-            dataset = dataset.map(_format_multi_turns)
 
         # Remove unused columns.
         dataset = dataset.remove_columns(
-            # FIXME
-            # [col for col in dataset.column_names['train'] if col not in ['input', 'output']]
-            [col for col in dataset.column_names['train'] if col not in ['conversations', 'system_prompt', 'prompt_type']]
+            [col for col in dataset.column_names['train'] if col not in ['input', 'output']]
         )
         return dataset
 
-    # Load dataset.
+     # Load dataset.
     dataset = load_data(args.dataset)
     dataset = format_dataset(dataset, args.dataset_format)
 
     # Split train/eval, reduce size
     logger.info(f"---------- Splitting dataset into train/eval ----------")
     if args.do_eval or args.do_predict:
         if 'eval' in dataset:
@@ -1377,57 +822,48 @@
             eval_dataset = dataset['test']
         if args.max_eval_samples is not None and len(eval_dataset) > args.max_eval_samples:
             eval_dataset = eval_dataset.select(range(args.max_eval_samples))
         if args.group_by_length:
             eval_dataset = eval_dataset.map(lambda x: {'length': len(x['input']) + len(x['output'])})
     if args.do_train:
         train_dataset = dataset['train']
-        max_train_samples = args.max_train_samples
-        if max_train_samples is not None and max_train_samples > 0 and max_train_samples < 1.0:
-            max_train_samples = int(len(train_dataset) * max_train_samples)
-        else:
-            max_train_samples = 0.0
-        if max_train_samples >= 1.0 and len(train_dataset) > max_train_samples:
-            train_dataset = train_dataset.select(range(max_train_samples))
-
+        if args.max_train_samples is not None and len(train_dataset) > args.max_train_samples:
+            train_dataset = train_dataset.select(range(args.max_train_samples))
         if args.group_by_length:
             train_dataset = train_dataset.map(lambda x: {'length': len(x['input']) + len(x['output'])})
-
+            
     # Remove any training data that exceeds the max length.
     def _get_data_length(item):
         prompt = f"{tokenizer.bos_token}{item['input']}{item['output']}{tokenizer.eos_token}"
         return len(
             tokenizer(
                 prompt,
                 max_length=args.model_max_len + 1,
                 truncation=True,
                 add_special_tokens=False
             ).input_ids
         )
     if args.force_remove_overlength_samples:
-        logger.info(f"---------- Filtering out samples longer than {args.model_max_len} ----------")
+        logger.info(f"---------- Filtering out samples longer than {args.model_max_len} ----------")  
         prev_len = len(train_dataset)
         train_dataset = train_dataset.filter(
             lambda x: _get_data_length(x) < args.model_max_len - 10
         )
         logger.info(f"Filtered out {prev_len - len(train_dataset)} samples. ({len(train_dataset)}/{prev_len})")
 
-    # FIXME
-    # data_collator = DataCollatorForCausalLM(
-    data_collator = DialogDataCollatorForCausalLM(
+    data_collator = DataCollatorForCausalLM(
         tokenizer=tokenizer,
         model_max_len=args.model_max_len,
-        prompt_type=args.prompt_type,
     )
 
     # FIXME
     if args.repeat_steps > 0:
         one_batch_size = args.per_device_train_batch_size * args.gradient_accumulation_steps * torch.cuda.device_count()
         train_dataset = RepeatDataset(train_dataset, repeat_batch_size= one_batch_size, repeat_steps = args.repeat_steps)
-
+    
     return dict(
         train_dataset=train_dataset if args.do_train else None,
         eval_dataset=eval_dataset if args.do_eval else None,
         predict_dataset=eval_dataset if args.do_predict else None,
         data_collator=data_collator
     )
 
@@ -1551,46 +987,32 @@
     # training_args.generation_config = transformers.GenerationConfig(**vars(generation_args))
     args = argparse.Namespace(
         **vars(model_args), **vars(data_args), **vars(training_args)
     )
 
     if args.task_name is None:
         args.task_name = os.path.basename(os.curdir)
-
+        
     from datetime import datetime
-    logger.add(f"{args.output_dir}/logs/{args.task_name}-{datetime.now().strftime('%Y%m%d_%H%M%S')}.log", level="INFO")
+    logger.add(f"{args.output_dir}/logs/finetune_{datetime.now().strftime('%Y%m%d_%H%M%S')}.log", level="INFO")
     logger.info(f"{args=}")
 
     # setup_wandb(args)
 
     # if args.flash_attention:
-    #     from speechless.patches.flash_attn_monkey_patch import replace_llama_attn_with_flash_attn
+    #     from patches.flash_attn_monkey_patch import replace_llama_attn_with_flash_attn
     #     replace_llama_attn_with_flash_attn(packed=args.sample_packing)
     #     logger.info(f"Enabled flash attention monkey patching.")
 
-    if args.long_lora:
-        if 'mistral' in args.model_name_or_path:
-            logger.warning(f"Mistral doesn't support long alpaca now.")
-            # from speechless.patches.llama_attn_replace_sft import replace_mistral_attn
-            # replace_mistral_attn(use_flash_attn=training_args.flash_attention, use_full=False, inference=False)
-        else:
-            from speechless.patches.long_lora_monkey_patch import replace_llama_attn
-            replace_llama_attn(use_flash_attn=training_args.flash_attention, use_full=False, inference=False)
-
     if args.rerope:
-        from speechless.patches.rerope_monkey_patch import replace_llama_attention_forword_with_rerope
+        from patches.rerope_monkey_patch import replace_llama_attention_forword_with_rerope
         rerope_window = args.rerope_window or int(args.model_max_Len * 3 / 8) // 16 * 16
         replace_llama_attention_forword_with_rerope(training_length=args.model_max_len, window=rerope_window)
         logger.info(f"Enabled rerope monkey patching.")
 
-    # if args.sliding_window > 0:
-    #     if 'mistral' not in args.model_name_or_path:
-    #         from speechless.patches.sliding_window_monkey_patch import replace_llama_attn
-    #         replace_llama_attn()
-
     checkpoint_dir, completed_training = get_last_checkpoint(args.output_dir)
     if completed_training:
         logger.warning('Detected that training was already completed!')
 
     model = get_accelerate_model(args, checkpoint_dir)
 
     model.config.use_cache = False
@@ -1600,81 +1022,49 @@
     set_seed(args.seed)
 
     # Tokenizer
     tokenizer_kwargs = {
         "cache_dir": args.cache_dir,
         "padding_side": "left",
         "use_fast": False,
-        "trust_remote_code": True,
     }
     # if args.mpt:
     #     tokenizer_kwargs["padding_side"] = "left"
     #     tokenizer_kwargs.pop("use_fast")
-    print(f"---------- Original tokens----------")
     tokenizer = AutoTokenizer.from_pretrained(args.model_name_or_path, **tokenizer_kwargs)
-    print(f"{tokenizer.pad_token=},{tokenizer.pad_token_id=}")
-    print(f"{tokenizer.unk_token=},{tokenizer.unk_token_id=}")
-    print(f"{tokenizer.bos_token=},{tokenizer.bos_token_id=}")
-    print(f"{tokenizer.eos_token=},{tokenizer.eos_token_id=}")
-
-    if "qwen" in args.model_name_or_path.lower():
-        tokenizer.eos_token = "<|endoftext|>"
-        # tokenizer.unk_token = "<|extra_3|>"
-        tokenizer.bos_token = "<|extra_2|>"
-        tokenizer.pad_token = "<|extra_1|>"
-    else:
-        if tokenizer.bos_token_id is None:
-            tokenizer.bos_token_id = 1
-            tokenizer.bos_token = "<s>"
-        if tokenizer.eos_token_id is None:
-            tokenizer.eos_token_id = 2
-            tokenizer.eos_token = "</s>"
-        # if tokenizer.unk_token_id is None:
-        #     tokenizer.unk_token_id = 0
-        #     tokenizer.unk_token = "<unk>"
-        if tokenizer.pad_token_id is None:
-            tokenizer.pad_token_id = 0 # tokenizer.eos_token_id
-            tokenizer.pad_token = tokenizer._convert_id_to_token(tokenizer.pad_token_id) #tokenizer.eos_token
-    print(f"---------- Fixed tokens ----------")
-    print(f"{tokenizer.pad_token=},{tokenizer.pad_token_id=}")
-    # print(f"{tokenizer.unk_token=},{tokenizer.unk_token_id=}")
-    print(f"{tokenizer.bos_token=},{tokenizer.bos_token_id=}")
-    print(f"{tokenizer.eos_token=},{tokenizer.eos_token_id=}")
+    if tokenizer.pad_token_id is None:
+        tokenizer.pad_token_id = 0
     data_module = make_data_module(tokenizer=tokenizer, args=args)
     trainer = Seq2SeqTrainer(
     # trainer = PeftTrainer(
         model=model,
         tokenizer=tokenizer,
         args=training_args,
         **{k:v for k,v in data_module.items() if k != 'predict_dataset'},
     )
 
     # Callbacks
     if not args.full_finetune:
         trainer.add_callback(SavePeftModelCallback)
 
-    trainer.add_callback(CleanMemoryCallback)
-    trainer.add_callback(LoggingCallback)
-
+    trainer.add_callback(TrainHelperCallback)
 
     # Verifying the datatypes.
     if not args.full_finetune:
         dtypes = {}
         for _, p in model.named_parameters():
             dtype = p.dtype
             if dtype not in dtypes: dtypes[dtype] = 0
             dtypes[dtype] += p.numel()
         total = 0
         for k, v in dtypes.items(): total+= v
         for k, v in dtypes.items():
             print(k, v, v/total)
 
     all_metrics = {"run_name": args.run_name}
-
-
     # Training
     if args.do_train:
         logger.info("*** Train ***")
         # Note: `resume_from_checkpoint` not supported for adapter checkpoints by HF.
         # Currently adapter checkpoint is reloaded as expected but optimizer/scheduler states are not.
         train_result = trainer.train()
         metrics = train_result.metrics
@@ -1691,15 +1081,15 @@
         all_metrics.update(metrics)
     # Prediction
     if args.do_predict:
         logger.info("*** Predict ***")
         prediction_output = trainer.predict(test_dataset=data_module['predict_dataset'],metric_key_prefix="predict")
         prediction_metrics = prediction_output.metrics
         predictions = prediction_output.predictions
-        predictions = np.where(predictions != IGNORE_INDEX, predictions, tokenizer.pad_token_id)
+        predictions = np.where(predictions != -100, predictions, tokenizer.pad_token_id)
         predictions = tokenizer.batch_decode(
             predictions, skip_special_tokens=True, clean_up_tokenization_spaces=True
         )
         with open(os.path.join(args.output_dir, 'predictions.jsonl'), 'w') as fout:
             for i, example in enumerate(data_module['predict_dataset']):
                 example['prediction_with_input'] = predictions[i].strip()
                 example['prediction'] = predictions[i].replace(example['input'], '').strip()
```

### Comparing `speechless-0.8.0/speechless/finetune/sophia.py` & `speechless-0.9.0/speechless/finetune/sophia.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/infer/__main__.py` & `speechless-0.9.0/speechless/infer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ```
     """
     tmp_dir = os.environ.get("TMPDIR", "/tmp")
     modelfile_path = os.path.join(tmp_dir, "Modelfile." + os.path.basename(args.gguf_file))
     with open(modelfile_path, "w") as f:
         f.write(f"FROM {args.gguf_file}")
 
-    ollama_model_name = args.ollama_model_name or os.path.basename(args.gguf_file).replace('.Q', ':Q').replace('.f16', ':f16').replace('.gguf', '')
+    ollama_model_name = args.ollama_model_name or os.path.basename(args.gguf_file).replace('-Q', ':Q').replace('-f16', ':f16').replace('.Q', ':Q').replace('.f16', ':f16').replace('.gguf', '')
 
     modelfile=open(modelfile_path).read()
     ollama.create(model=ollama_model_name, modelfile=modelfile)
     # cmd = f"ollama create {ollama_model_name} -f {modelfile_path}"
     # os.system(cmd)
 
     os.remove(modelfile_path)
```

### Comparing `speechless-0.8.0/speechless/infer/infer.py` & `speechless-0.9.0/speechless/infer/infer.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/infer/openrouter.py` & `speechless-0.9.0/speechless/infer/openrouter.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/quant/__main__.py` & `speechless-0.9.0/speechless/quant/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     llamacpp_quantize = f"{llamacpp_root}/quantize"
     if not os.path.isdir(llamacpp_root) or not os.path.exists(llamacpp_convert) or not os.path.exists(llamacpp_quantize):
         raise Exception(f"llamacpp_root {llamacpp_root} not found or invalid")
 
     os.makedirs(gguf_dir, exist_ok=True)
 
     if not os.path.exists(gguf_f16_file):
-        convert_cmd = f"python {llamacpp_convert} {model_path} --padvocab --outtype f16 --outfile {gguf_f16_file}"
+        if args.skip_unknown:
+            SKIP_UNKNOWN = "--skip-unknown"
+        else:
+            SKIP_UNKNOWN = ""
+        convert_cmd = f"python {llamacpp_convert} {model_path} {SKIP_UNKNOWN} --pad-vocab --outtype f16 --outfile {gguf_f16_file}"
         print(convert_cmd)
         os.system(convert_cmd)
 
     # ./quantize ${GGML_FILE} ${Q4_K_M_FILE} q4_k_m 
     quant_file = f"{gguf_dir}/{os.path.basename(model_path)}.{args.llamacpp_quant_type.upper()}.gguf"
     quant_cmd = f"{llamacpp_quantize} {gguf_f16_file} {quant_file} {args.llamacpp_quant_type}"
     print(quant_cmd)
@@ -45,14 +49,15 @@
     parser.add_argument("cmd", type=str, choices=commands.keys(), help="command to run")
 
     parser.add_argument("--model_path", type=str, required=True)
     parser.add_argument("--gguf_dir", type=str)
     parser.add_argument("--gguf_f16_file", type=str)
     parser.add_argument("--llamacpp_quant_type", type=str, choices=llamacpp_quant_types)
     parser.add_argument("--llamacpp_root", type=str)
+    parser.add_argument("--skip-unknown", action="store_true", help="Skip unknown tokens")
 
     parser.add_argument("--litellm_port", type=int, default=18341)
 
     args = parser.parse_args()
     return args
```

### Comparing `speechless-0.8.0/speechless/rag/document/pdf.py` & `speechless-0.9.0/speechless/rag/document/pdf.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/rag/document/pdf2txt.py` & `speechless-0.9.0/speechless/rag/document/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/__main__.py` & `speechless-0.9.0/speechless/data_selection/nuggets/__main__.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/kmeans_sample.py` & `speechless-0.9.0/speechless/data_selection/nuggets/kmeans_sample.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/meta_optimizer.py` & `speechless-0.9.0/speechless/data_selection/nuggets/meta_optimizer.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/nuggets.py` & `speechless-0.9.0/speechless/data_selection/nuggets/nuggets.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/plt.py` & `speechless-0.9.0/speechless/data_selection/nuggets/plt.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/alpaca.py` & `speechless-0.9.0/speechless/data_selection/nuggets/tasks/alpaca.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/base.py` & `speechless-0.9.0/speechless/data_selection/nuggets/tasks/base.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/loader.py` & `speechless-0.9.0/speechless/data_selection/nuggets/tasks/loader.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless/synthetic_data/nuggets/tasks/rng_ctx.py` & `speechless-0.9.0/speechless/data_selection/nuggets/tasks/rng_ctx.py`

 * *Files identical despite different names*

### Comparing `speechless-0.8.0/speechless.egg-info/PKG-INFO` & `speechless-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: speechless
-Version: 0.8.0
-Summary: LLM based agents with proactive interactions, long-term memory, external tool integration, and local deployment capabilities.
-Home-page: https://github.com/uukuguy/speechless
-Author: Jiangwen Su
-Author-email: uukuguy@gmail.com
-License: Apache
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # Speechless LLM based Agents
 
 > LLM based agents with proactive interactions, long-term memory, external tool integration, and local deployment capabilities.
 
 ![Speechless.AI](imgs/speechlessai_main_3.png)
 
 [Speechless.AI](http://speechless.ai/) is committed to integrating the superior language processing and deep reasoning capabilities of large language models into practical business applications. By enhancing the model's language understanding, knowledge accumulation, and text creation abilities, and introducing long-term memory, external tool integration, and local deployment, our aim is to establish an intelligent collaborative partner that can independently interact, continuously evolve, and closely align with various business scenarios.
@@ -33,14 +11,21 @@
 - Next, we design and implement an efficient operational framework for the intelligent entity. This framework not only supports rapid deployment and invocation of the model but also boasts features like autonomous interaction, real-time feedback adjustment, context awareness, and long-term memory.
   For instance, in customer service scenarios, the intelligent entity can provide more precise and personalized responses based on a user's historical interactions and current context. In content recommendation scenarios, it can dynamically adjust its strategies by capturing real-time shifts in user interests.
 
 - Ultimately, we integrate it with real business scenarios, ensuring that the intelligent entity seamlessly aligns with various business processes, delivering tangible value to enterprises.
 
 ## What's New
 
+
+- [2024-03-13] Release [speechless-starcoder2-15b](https://huggingface.co/uukuguy/speechless-starcoder2-15b)
+- [2024-03-10] Release [speechless-starcoder2-7b](https://huggingface.co/uukuguy/speechless-starcoder2-7b)
+- [2024-02-15] Reelase [speechless-thoughts-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b-v1.0) (Change same hyperparameters)
+- [2024-02-12] Release [speechless-thoughts-mistral-7b](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b)
+- [2024-02-10] Release [speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE), the MoE upgraded version of speechless-code-mistral-7b-v1.0. The MoE fine-tuning adopts [Parameter-Efficient Sparsity Crafting (PESC)](https://arxiv.org/abs/2401.02731), which is an efficient fine-tuning architecture that uses LoRA modules as expert models, similar to the concept of [multi-loras](https://github.com/uukuguy/multi_loras).
+- [2024-02-06] Release [speechless-mistral-hermes-code-7b](https://huggingface.co/uukuguy/speechless-mistral-hermes-code-7b) fine-tuned by speechless-thoughts-252K dataset.
 - [2024-01-23] Release [speechless-zephyr-code-functionary-7b](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b)
 - [2024-01-15] Release [speechless-nl2sql-ds-6.7b](https://huggingface.co/uukuguy/speechless-nl2sql-ds-6.7b), finetune based on [deepseek-coder-6.7b-base](https://huggingface.co/deepseek-ai/deepseek-coder-6.7b-base).
 - [2024-01-05] Release [speechless-mistral-moloras-7b](https://huggingface.co/uukuguy/speechless-mistral-moloras-7b), which is the static version of moloras ([Mixture-of-multi-LoRAs](https://github.com/uukuguy/multi_loras?tab=readme-ov-file#mixture-of-multi-loras))
 - [2023/12/30] Release [speechless-coder-ds-1.3b](https://huggingface.co/uukuguy/speechless-coder-ds-1.3b) that finetune based on [deepseek-coder-1.3b-base](https://huggingface.co/deepseek-ai/deepseek-coder-1.3b-base).
 - [2023/12/30] Release [speechless-coder-ds-6.7b](https://huggingface.co/uukuguy/speechless-coder-ds-6.7b) that finetune based on [deepseek-coder-6.7b-base](https://huggingface.co/deepseek-ai/deepseek-coder-6.7b-base).
 - [2023/12/23] Uploaded the float16 version of [prometheus-7b-v1.0-fp16](https://huggingface.co/uukuguy/prometheus-7b-v1.0-fp16) for instruction fine-tuning data quality assessment.
 - [2023/12/23] Uploaded the float16 version of [prometheus-13b-v1.0-fp16](https://huggingface.co/uukuguy/prometheus-13b-v1.0-fp16) for instruction fine-tuning data quality assessment.
@@ -79,14 +64,51 @@
 
 ## Models
 
 [Models Repositry](https://huggingface.co/uukuguy)
 
 ⭐️ My Focus 🔥🔥🔥 DL > 10k/month 🔥🔥 DL > 7K/month 🔥 DL > 3K/month
 
+### Mar. 2024
+
+- **[speechless-starcoder2-15b](https://huggingface.co/uukuguy/speechless-starcoder2-15b) 2024.03.13**
+
+- **[speechless-starcoder2-7b](https://huggingface.co/uukuguy/speechless-starcoder2-7b) 2024.03.10**
+
+### Feb. 2024
+
+- **[speechless-thoughts-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b-v1.0) 2024.02.15**
+
+    Change some hyperparameters compared to speechless-thoughts-mistral-7b.
+
+    ```json
+    learning_rate=2e-4
+    lora_r=64
+    lora_alpha=16
+    model_max_length=8192
+    ```
+
+- **[speechless-thoughts-mistral-7b](https://huggingface.co/uukuguy/speechless-thoughts-mistral-7b) 2024.02.12**
+
+    speechless-thoughts-mistral-7b is fine-tuned as a baseline of the [speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE).
+
+    **Open LLM Language Model Evaluation Harness**
+
+    | Average | ARC    | HellaSwag | MMLU   | TruthfulQA | Winogrande | GSM8K  |
+    | ------  | ------ | ------    | ------ | ------     | -------    | ------ |
+    | 59.72   | 58.96  | 87.10    | 60.11  | 49.91      | 77.82      | 30.78  |
+
+- ⭐ **[speechless-sparsetral-16x7b-MoE](https://huggingface.co/uukuguy/speechless-sparsetral-16x7b-MoE) 2024.02.10**
+
+    The MoE upgraded version of speechless-code-mistral-7b-v1.0. The MoE fine-tuning adopts [Parameter-Efficient Sparsity Crafting (PESC)](https://arxiv.org/abs/2401.02731), which is an efficient fine-tuning architecture that uses LoRA modules as expert models, similar to the concept of [multi-loras](https://github.com/uukuguy/multi_loras).
+
+- ⭐ **[speechless-mistral-hermes-code-7b](https://huggingface.co/uukuguy/speechless-mistral-hermes-code-7b) 2024.02.06**
+
+    Using the speechless-thoughts-252K dataset, it was fine-tuned based on the Mistral-7B-v0.1 base model in preparation for comparison with [speechless-code-mistral-7b-v1.0](https://huggingface.co/uukuguy/speechless-code-mistral-7b-v1.0).
+
 ### Jan. 2024
 
 - ⭐ **[speechless-zephyr-code-functionary-7b](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b)**
 
     [GGUF](https://huggingface.co/uukuguy/speechless-zephyr-code-functionary-7b/tree/main/GGUF)
 
 - **[speechless-nl2sql-ds-6.7b](https://huggingface.co/uukuguy/speechless-nl2sql-ds-6.7b)**
```

