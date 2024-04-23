# Comparing `tmp/codefuse-muagent-0.0.1.tar.gz` & `tmp/codefuse_muagent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefuse-muagent-0.0.1.tar", last modified: Mon Apr 22 03:38:13 2024, max compression
+gzip compressed data, was "codefuse_muagent-0.0.3.tar", last modified: Tue Apr 23 09:35:24 2024, max compression
```

## Comparing `codefuse-muagent-0.0.1.tar` & `codefuse_muagent-0.0.3.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.871326 codefuse-muagent-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.857327 codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/
--rw-rw-rw-   0        0        0      951 2024-04-22 03:38:12.000000 codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6215 2024-04-22 03:38:12.000000 codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 03:38:12.000000 codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2024-04-22 03:38:12.000000 codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 03:38:12.000000 codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11906 2024-03-12 06:09:58.000000 codefuse-muagent-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      951 2024-04-22 03:38:13.862327 codefuse-muagent-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4798 2024-03-22 02:31:23.000000 codefuse-muagent-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.165325 codefuse-muagent-0.0.1/muagent/
--rw-rw-rw-   0        0        0       98 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.173325 codefuse-muagent-0.0.1/muagent/base_configs/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/base_configs/__init__.py
--rw-rw-rw-   0        0        0     3547 2024-03-12 11:06:58.000000 codefuse-muagent-0.0.1/muagent/base_configs/env_config.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.208326 codefuse-muagent-0.0.1/muagent/chat/
--rw-rw-rw-   0        0        0      296 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/chat/__init__.py
--rw-rw-rw-   0        0        0    17934 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/chat/agent_chat.py
--rw-rw-rw-   0        0        0     8574 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/chat/base_chat.py
--rw-rw-rw-   0        0        0     7571 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/chat/code_chat.py
--rw-rw-rw-   0        0        0     4080 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/chat/knowledge_chat.py
--rw-rw-rw-   0        0        0     1544 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/chat/llm_chat.py
--rw-rw-rw-   0        0        0     5651 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/chat/search_chat.py
--rw-rw-rw-   0        0        0      803 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/chat/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.214327 codefuse-muagent-0.0.1/muagent/codechat/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.240324 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/__init__.py
--rw-rw-rw-   0        0        0     9385 2024-04-10 08:41:08.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_analyzer.py
--rw-rw-rw-   0        0        0      565 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_dedup.py
--rw-rw-rw-   0        0        0     9246 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_intepreter.py
--rw-rw-rw-   0        0        0      228 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_preprocess.py
--rw-rw-rw-   0        0        0      633 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_static_analysis.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.249324 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/language_static_analysis/
--rw-rw-rw-   0        0        0      198 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/language_static_analysis/__init__.py
--rw-rw-rw-   0        0        0     3783 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.261328 codefuse-muagent-0.0.1/muagent/codechat/code_crawler/
--rw-rw-rw-   0        0        0      227 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_crawler/__init__.py
--rw-rw-rw-   0        0        0     1139 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_crawler/dir_crawler.py
--rw-rw-rw-   0        0        0      682 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/codechat/code_crawler/zip_crawler.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.278326 codefuse-muagent-0.0.1/muagent/codechat/code_search/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_search/__init__.py
--rw-rw-rw-   0        0        0     9179 2024-04-10 09:14:02.000000 codefuse-muagent-0.0.1/muagent/codechat/code_search/code_search.py
--rw-rw-rw-   0        0        0     2815 2024-04-10 09:06:40.000000 codefuse-muagent-0.0.1/muagent/codechat/code_search/cypher_generator.py
--rw-rw-rw-   0        0        0      776 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/code_search/tagger.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.290326 codefuse-muagent-0.0.1/muagent/codechat/codebase_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/codechat/codebase_handler/__init__.py
--rw-rw-rw-   0        0        0    18942 2024-04-10 08:40:23.000000 codefuse-muagent-0.0.1/muagent/codechat/codebase_handler/code_importer.py
--rw-rw-rw-   0        0        0    10623 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/codechat/codebase_handler/codebase_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.309325 codefuse-muagent-0.0.1/muagent/connector/
--rw-rw-rw-   0        0        0      120 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.318325 codefuse-muagent-0.0.1/muagent/connector/actions/
--rw-rw-rw-   0        0        0       73 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/actions/__init__.py
--rw-rw-rw-   0        0        0      207 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/actions/base_action.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.340326 codefuse-muagent-0.0.1/muagent/connector/agents/
--rw-rw-rw-   0        0        0      239 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/agents/__init__.py
--rw-rw-rw-   0        0        0     9606 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/agents/base_agent.py
--rw-rw-rw-   0        0        0     8356 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/agents/executor_agent.py
--rw-rw-rw-   0        0        0     7565 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/agents/react_agent.py
--rw-rw-rw-   0        0        0     5736 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/agents/selector_agent.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.350325 codefuse-muagent-0.0.1/muagent/connector/antflow/
--rw-rw-rw-   0        0        0      114 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/antflow/__init__.py
--rw-rw-rw-   0        0        0    11507 2024-04-18 08:41:54.000000 codefuse-muagent-0.0.1/muagent/connector/antflow/flow.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.365327 codefuse-muagent-0.0.1/muagent/connector/chains/
--rw-rw-rw-   0        0        0       68 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/chains/__init__.py
--rw-rw-rw-   0        0        0     6708 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/chains/base_chain.py
--rw-rw-rw-   0        0        0      318 2024-03-13 06:55:36.000000 codefuse-muagent-0.0.1/muagent/connector/chains/chains.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.388325 codefuse-muagent-0.0.1/muagent/connector/configs/
--rw-rw-rw-   0        0        0      434 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/__init__.py
--rw-rw-rw-   0        0        0    10397 2024-03-26 07:36:32.000000 codefuse-muagent-0.0.1/muagent/connector/configs/agent_config.py
--rw-rw-rw-   0        0        0     4104 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/chain_config.py
--rw-rw-rw-   0        0        0     2274 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/phase_config.py
--rw-rw-rw-   0        0        0     5838 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompt_config.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.472325 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/
--rw-rw-rw-   0        0        0     2724 2024-03-19 12:49:14.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/__init__.py
--rw-rw-rw-   0        0        0      821 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/agent_selector_template_prompt.py
--rw-rw-rw-   0        0        0     1928 2024-03-25 09:34:34.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/checker_template_prompt.py
--rw-rw-rw-   0        0        0     3666 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/code2doc_template_prompt.py
--rw-rw-rw-   0        0        0     3928 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/code2test_template_prompt.py
--rw-rw-rw-   0        0        0     2246 2024-03-26 04:35:55.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/executor_template_prompt.py
--rw-rw-rw-   0        0        0      665 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/input_template_prompt.py
--rw-rw-rw-   0        0        0     1409 2024-03-27 08:29:05.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/intention_template_prompt.py
--rw-rw-rw-   0        0        0     7360 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/metagpt_prompt.py
--rw-rw-rw-   0        0        0     4421 2024-03-20 06:14:22.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/planner_template_prompt.py
--rw-rw-rw-   0        0        0     3032 2024-04-10 09:00:47.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/qa_template_prompt.py
--rw-rw-rw-   0        0        0     3872 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_code_prompt.py
--rw-rw-rw-   0        0        0     1639 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_template_prompt.py
--rw-rw-rw-   0        0        0     1860 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py
--rw-rw-rw-   0        0        0     8551 2024-03-25 09:34:43.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_tool_code_prompt.py
--rw-rw-rw-   0        0        0     2599 2024-03-26 02:46:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_tool_prompt.py
--rw-rw-rw-   0        0        0     1487 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/refine_template_prompt.py
--rw-rw-rw-   0        0        0     2076 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/configs/prompts/summary_template_prompt.py
--rw-rw-rw-   0        0        0    22996 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/memory_manager.py
--rw-rw-rw-   0        0        0    15420 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/message_process.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.481325 codefuse-muagent-0.0.1/muagent/connector/phase/
--rw-rw-rw-   0        0        0       60 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/phase/__init__.py
--rw-rw-rw-   0        0        0    13906 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/phase/base_phase.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.495327 codefuse-muagent-0.0.1/muagent/connector/prompt_manager/
--rw-rw-rw-   0        0        0       72 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/prompt_manager/__init__.py
--rw-rw-rw-   0        0        0     2362 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/connector/prompt_manager/extend_manager.py
--rw-rw-rw-   0        0        0    30209 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/prompt_manager/prompt_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.513327 codefuse-muagent-0.0.1/muagent/connector/schema/
--rw-rw-rw-   0        0        0      325 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/connector/schema/__init__.py
--rw-rw-rw-   0        0        0     9517 2024-03-26 07:37:47.000000 codefuse-muagent-0.0.1/muagent/connector/schema/general_schema.py
--rw-rw-rw-   0        0        0     7077 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/schema/memory.py
--rw-rw-rw-   0        0        0     4731 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/connector/schema/message.py
--rw-rw-rw-   0        0        0     5529 2024-03-27 08:28:21.000000 codefuse-muagent-0.0.1/muagent/connector/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.518326 codefuse-muagent-0.0.1/muagent/db_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/db_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.526325 codefuse-muagent-0.0.1/muagent/db_handler/graph_db_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/db_handler/graph_db_handler/__init__.py
--rw-rw-rw-   0        0        0     8783 2024-04-10 09:06:46.000000 codefuse-muagent-0.0.1/muagent/db_handler/graph_db_handler/nebula_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.537325 codefuse-muagent-0.0.1/muagent/db_handler/vector_db_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/db_handler/vector_db_handler/__init__.py
--rw-rw-rw-   0        0        0     4947 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/db_handler/vector_db_handler/chroma_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.570325 codefuse-muagent-0.0.1/muagent/embeddings/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/embeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.582325 codefuse-muagent-0.0.1/muagent/embeddings/commands/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/embeddings/commands/__init__.py
--rw-rw-rw-   0        0        0      665 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/embeddings/commands/default_vs_cds.py
--rw-rw-rw-   0        0        0    29854 2024-03-19 03:31:15.000000 codefuse-muagent-0.0.1/muagent/embeddings/faiss_m.py
--rw-rw-rw-   0        0        0     5515 2024-04-18 07:53:55.000000 codefuse-muagent-0.0.1/muagent/embeddings/get_embedding.py
--rw-rw-rw-   0        0        0     5499 2024-04-10 08:42:59.000000 codefuse-muagent-0.0.1/muagent/embeddings/huggingface_embedding.py
--rw-rw-rw-   0        0        0     1651 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/embeddings/in_memory.py
--rw-rw-rw-   0        0        0     5406 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/embeddings/openai_embedding.py
--rw-rw-rw-   0        0        0      851 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/embeddings/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.595327 codefuse-muagent-0.0.1/muagent/llm_models/
--rw-rw-rw-   0        0        0      211 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/llm_models/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-03-29 02:51:52.000000 codefuse-muagent-0.0.1/muagent/llm_models/llm_config.py
--rw-rw-rw-   0        0        0     3048 2024-03-22 07:50:16.000000 codefuse-muagent-0.0.1/muagent/llm_models/openai_model.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.607325 codefuse-muagent-0.0.1/muagent/orm/
--rw-rw-rw-   0        0        0      573 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.626327 codefuse-muagent-0.0.1/muagent/orm/commands/
--rw-rw-rw-   0        0        0      452 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/orm/commands/__init__.py
--rw-rw-rw-   0        0        0     2426 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/orm/commands/code_base_cds.py
--rw-rw-rw-   0        0        0     2793 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/orm/commands/document_base_cds.py
--rw-rw-rw-   0        0        0     3157 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/orm/commands/document_file_cds.py
--rw-rw-rw-   0        0        0     1387 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/orm/db.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.634328 codefuse-muagent-0.0.1/muagent/orm/schemas/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/orm/schemas/__init__.py
--rw-rw-rw-   0        0        0     2901 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/orm/schemas/base_schema.py
--rw-rw-rw-   0        0        0      910 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/orm/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.643325 codefuse-muagent-0.0.1/muagent/retrieval/
--rw-rw-rw-   0        0        0      139 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/retrieval/__init__.py
--rw-rw-rw-   0        0        0     2519 2024-03-21 04:10:28.000000 codefuse-muagent-0.0.1/muagent/retrieval/base_retrieval.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.658327 codefuse-muagent-0.0.1/muagent/retrieval/document_loaders/
--rw-rw-rw-   0        0        0      120 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/retrieval/document_loaders/__init__.py
--rw-rw-rw-   0        0        0     2117 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/retrieval/document_loaders/json_loader.py
--rw-rw-rw-   0        0        0     2121 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/retrieval/document_loaders/jsonl_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.675325 codefuse-muagent-0.0.1/muagent/retrieval/text_splitter/
--rw-rw-rw-   0        0        0       76 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/retrieval/text_splitter/__init__.py
--rw-rw-rw-   0        0        0     2837 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/retrieval/text_splitter/langchain_splitter.py
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/retrieval/text_splitter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.688327 codefuse-muagent-0.0.1/muagent/sandbox/
--rw-rw-rw-   0        0        0      119 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/sandbox/__init__.py
--rw-rw-rw-   0        0        0     3772 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/sandbox/basebox.py
--rw-rw-rw-   0        0        0    20458 2024-04-11 11:32:17.000000 codefuse-muagent-0.0.1/muagent/sandbox/pycodebox.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.724326 codefuse-muagent-0.0.1/muagent/service/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/service/__init__.py
--rw-rw-rw-   0        0        0     5851 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/service/base_service.py
--rw-rw-rw-   0        0        0    10063 2024-04-07 03:54:58.000000 codefuse-muagent-0.0.1/muagent/service/cb_api.py
--rw-rw-rw-   0        0        0     6887 2024-04-10 09:08:37.000000 codefuse-muagent-0.0.1/muagent/service/faiss_db_service.py
--rw-rw-rw-   0        0        0    16377 2024-03-19 05:49:11.000000 codefuse-muagent-0.0.1/muagent/service/kb_api.py
--rw-rw-rw-   0        0        0     5742 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/service/migrate.py
--rw-rw-rw-   0        0        0     5096 2024-03-19 03:31:20.000000 codefuse-muagent-0.0.1/muagent/service/service_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.790327 codefuse-muagent-0.0.1/muagent/tools/
--rw-rw-rw-   0        0        0     1108 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/abnormal_detection.py
--rw-rw-rw-   0        0        0     2332 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/base_tool.py
--rw-rw-rw-   0        0        0     2577 2024-04-10 08:46:41.000000 codefuse-muagent-0.0.1/muagent/tools/cb_query_tool.py
--rw-rw-rw-   0        0        0     4355 2024-03-27 08:14:38.000000 codefuse-muagent-0.0.1/muagent/tools/codechat_tools.py
--rw-rw-rw-   0        0        0     2070 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/tools/docs_retrieval.py
--rw-rw-rw-   0        0        0     2882 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/duckduckgo_search.py
--rw-rw-rw-   0        0        0     1110 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/metrics_query.py
--rw-rw-rw-   0        0        0     1146 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/multiplier.py
--rw-rw-rw-   0        0        0     4491 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/ocr_tool.py
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/sandbox.py
--rw-rw-rw-   0        0        0     8334 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/tools/stock_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.800326 codefuse-muagent-0.0.1/muagent/tools/tool_datas/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/tool_datas/__init__.py
--rw-rw-rw-   0        0        0   247049 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/tool_datas/stock_data.py
--rw-rw-rw-   0        0        0     4398 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/weather.py
--rw-rw-rw-   0        0        0     7788 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/tools/world_time.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.835326 codefuse-muagent-0.0.1/muagent/utils/
--rw-rw-rw-   0        0        0      209 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/utils/__init__.py
--rw-rw-rw-   0        0        0     2804 2024-04-07 04:53:53.000000 codefuse-muagent-0.0.1/muagent/utils/code2doc_util.py
--rw-rw-rw-   0        0        0     3401 2024-04-21 02:39:54.000000 codefuse-muagent-0.0.1/muagent/utils/common_utils.py
--rw-rw-rw-   0        0        0     2698 2024-03-13 06:55:37.000000 codefuse-muagent-0.0.1/muagent/utils/path_utils.py
--rw-rw-rw-   0        0        0      188 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/utils/postprocess.py
--rw-rw-rw-   0        0        0     7522 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/utils/server_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.841325 codefuse-muagent-0.0.1/muagent/utils/static/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse-muagent-0.0.1/muagent/utils/static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-22 03:38:13.872326 codefuse-muagent-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1186 2024-04-22 03:35:17.000000 codefuse-muagent-0.0.1/setup.py
--rw-rw-rw-   0        0        0     1186 2024-04-22 03:35:16.000000 codefuse-muagent-0.0.1/setup_test.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:38:13.848327 codefuse-muagent-0.0.1/tests/
--rw-rw-rw-   0        0        0     1720 2024-03-26 02:49:26.000000 codefuse-muagent-0.0.1/tests/test_config.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.375568 codefuse_muagent-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.370567 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/
+-rw-rw-rw-   0        0        0      985 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6243 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11906 2024-03-12 06:09:58.000000 codefuse_muagent-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0      985 2024-04-23 09:35:24.371569 codefuse_muagent-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5358 2024-04-23 08:48:38.000000 codefuse_muagent-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.939085 codefuse_muagent-0.0.3/muagent/
+-rw-rw-rw-   0        0        0       98 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.943085 codefuse_muagent-0.0.3/muagent/base_configs/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/base_configs/__init__.py
+-rw-rw-rw-   0        0        0     3547 2024-03-12 11:06:58.000000 codefuse_muagent-0.0.3/muagent/base_configs/env_config.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.972071 codefuse_muagent-0.0.3/muagent/chat/
+-rw-rw-rw-   0        0        0      296 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/chat/__init__.py
+-rw-rw-rw-   0        0        0    18098 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/chat/agent_chat.py
+-rw-rw-rw-   0        0        0     8574 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/base_chat.py
+-rw-rw-rw-   0        0        0     7571 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/code_chat.py
+-rw-rw-rw-   0        0        0     4080 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/knowledge_chat.py
+-rw-rw-rw-   0        0        0     1544 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/llm_chat.py
+-rw-rw-rw-   0        0        0     5651 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/search_chat.py
+-rw-rw-rw-   0        0        0      803 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/chat/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.975073 codefuse_muagent-0.0.3/muagent/codechat/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.991100 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/__init__.py
+-rw-rw-rw-   0        0        0     9385 2024-04-10 08:41:08.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_analyzer.py
+-rw-rw-rw-   0        0        0      565 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_dedup.py
+-rw-rw-rw-   0        0        0     9246 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_intepreter.py
+-rw-rw-rw-   0        0        0      228 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_preprocess.py
+-rw-rw-rw-   0        0        0      633 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_static_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.995107 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/
+-rw-rw-rw-   0        0        0      198 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/__init__.py
+-rw-rw-rw-   0        0        0     3783 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.002072 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/
+-rw-rw-rw-   0        0        0      227 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/__init__.py
+-rw-rw-rw-   0        0        0     1139 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/dir_crawler.py
+-rw-rw-rw-   0        0        0      682 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/zip_crawler.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.012071 codefuse_muagent-0.0.3/muagent/codechat/code_search/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/__init__.py
+-rw-rw-rw-   0        0        0     9179 2024-04-10 09:14:02.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/code_search.py
+-rw-rw-rw-   0        0        0     2815 2024-04-10 09:06:40.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/cypher_generator.py
+-rw-rw-rw-   0        0        0      776 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/tagger.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.019072 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/__init__.py
+-rw-rw-rw-   0        0        0    18942 2024-04-10 08:40:23.000000 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/code_importer.py
+-rw-rw-rw-   0        0        0    10625 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/codebase_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.029070 codefuse_muagent-0.0.3/muagent/connector/
+-rw-rw-rw-   0        0        0      120 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.034071 codefuse_muagent-0.0.3/muagent/connector/actions/
+-rw-rw-rw-   0        0        0       73 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/actions/__init__.py
+-rw-rw-rw-   0        0        0      207 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/actions/base_action.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.046073 codefuse_muagent-0.0.3/muagent/connector/agents/
+-rw-rw-rw-   0        0        0      239 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/agents/__init__.py
+-rw-rw-rw-   0        0        0    10500 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/base_agent.py
+-rw-rw-rw-   0        0        0     8801 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/executor_agent.py
+-rw-rw-rw-   0        0        0     7995 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/react_agent.py
+-rw-rw-rw-   0        0        0     6041 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/selector_agent.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.051072 codefuse_muagent-0.0.3/muagent/connector/antflow/
+-rw-rw-rw-   0        0        0      114 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/antflow/__init__.py
+-rw-rw-rw-   0        0        0    11507 2024-04-18 08:41:54.000000 codefuse_muagent-0.0.3/muagent/connector/antflow/flow.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.058071 codefuse_muagent-0.0.3/muagent/connector/chains/
+-rw-rw-rw-   0        0        0       68 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/chains/__init__.py
+-rw-rw-rw-   0        0        0     6960 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/chains/base_chain.py
+-rw-rw-rw-   0        0        0      318 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/connector/chains/chains.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.070113 codefuse_muagent-0.0.3/muagent/connector/configs/
+-rw-rw-rw-   0        0        0      434 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/__init__.py
+-rw-rw-rw-   0        0        0    10397 2024-03-26 07:36:32.000000 codefuse_muagent-0.0.3/muagent/connector/configs/agent_config.py
+-rw-rw-rw-   0        0        0     4104 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/chain_config.py
+-rw-rw-rw-   0        0        0     2274 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/phase_config.py
+-rw-rw-rw-   0        0        0     5838 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompt_config.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.127104 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/
+-rw-rw-rw-   0        0        0     2724 2024-03-19 12:49:14.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/__init__.py
+-rw-rw-rw-   0        0        0      829 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/agent_selector_template_prompt.py
+-rw-rw-rw-   0        0        0     1928 2024-03-25 09:34:34.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/checker_template_prompt.py
+-rw-rw-rw-   0        0        0     3666 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2doc_template_prompt.py
+-rw-rw-rw-   0        0        0     3928 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2test_template_prompt.py
+-rw-rw-rw-   0        0        0     2246 2024-03-26 04:35:55.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/executor_template_prompt.py
+-rw-rw-rw-   0        0        0      665 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/input_template_prompt.py
+-rw-rw-rw-   0        0        0     1409 2024-03-27 08:29:05.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/intention_template_prompt.py
+-rw-rw-rw-   0        0        0     7360 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/metagpt_prompt.py
+-rw-rw-rw-   0        0        0     4421 2024-03-20 06:14:22.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/planner_template_prompt.py
+-rw-rw-rw-   0        0        0     3032 2024-04-10 09:00:47.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/qa_template_prompt.py
+-rw-rw-rw-   0        0        0     3872 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_code_prompt.py
+-rw-rw-rw-   0        0        0     1639 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_template_prompt.py
+-rw-rw-rw-   0        0        0     1860 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py
+-rw-rw-rw-   0        0        0     8551 2024-03-25 09:34:43.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_prompt.py
+-rw-rw-rw-   0        0        0     2599 2024-03-26 02:46:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_prompt.py
+-rw-rw-rw-   0        0        0     1487 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/refine_template_prompt.py
+-rw-rw-rw-   0        0        0     2076 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/summary_template_prompt.py
+-rw-rw-rw-   0        0        0    37315 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/memory_manager.py
+-rw-rw-rw-   0        0        0    14713 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/message_process.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.132071 codefuse_muagent-0.0.3/muagent/connector/phase/
+-rw-rw-rw-   0        0        0       60 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/phase/__init__.py
+-rw-rw-rw-   0        0        0    14557 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/phase/base_phase.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.139071 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/
+-rw-rw-rw-   0        0        0       72 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/__init__.py
+-rw-rw-rw-   0        0        0     2362 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/extend_manager.py
+-rw-rw-rw-   0        0        0    28367 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/prompt_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.149072 codefuse_muagent-0.0.3/muagent/connector/schema/
+-rw-rw-rw-   0        0        0      325 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/schema/__init__.py
+-rw-rw-rw-   0        0        0     9517 2024-03-26 07:37:47.000000 codefuse_muagent-0.0.3/muagent/connector/schema/general_schema.py
+-rw-rw-rw-   0        0        0     7217 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/schema/memory.py
+-rw-rw-rw-   0        0        0     5953 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/schema/message.py
+-rw-rw-rw-   0        0        0     5529 2024-03-27 08:28:21.000000 codefuse_muagent-0.0.3/muagent/connector/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.152071 codefuse_muagent-0.0.3/muagent/db_handler/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.156071 codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/__init__.py
+-rw-rw-rw-   0        0        0     8783 2024-04-10 09:06:46.000000 codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/nebula_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.162071 codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/
+-rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/__init__.py
+-rw-rw-rw-   0        0        0     4947 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/chroma_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.188071 codefuse_muagent-0.0.3/muagent/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.193072 codefuse_muagent-0.0.3/muagent/embeddings/commands/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/commands/__init__.py
+-rw-rw-rw-   0        0        0      665 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/commands/default_vs_cds.py
+-rw-rw-rw-   0        0        0    29854 2024-03-19 03:31:15.000000 codefuse_muagent-0.0.3/muagent/embeddings/faiss_m.py
+-rw-rw-rw-   0        0        0     5515 2024-04-18 07:53:55.000000 codefuse_muagent-0.0.3/muagent/embeddings/get_embedding.py
+-rw-rw-rw-   0        0        0     5499 2024-04-10 08:42:59.000000 codefuse_muagent-0.0.3/muagent/embeddings/huggingface_embedding.py
+-rw-rw-rw-   0        0        0     1651 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/in_memory.py
+-rw-rw-rw-   0        0        0     5406 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/openai_embedding.py
+-rw-rw-rw-   0        0        0      851 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.200070 codefuse_muagent-0.0.3/muagent/llm_models/
+-rw-rw-rw-   0        0        0      211 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/llm_models/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-03-29 02:51:52.000000 codefuse_muagent-0.0.3/muagent/llm_models/llm_config.py
+-rw-rw-rw-   0        0        0     3048 2024-03-22 07:50:16.000000 codefuse_muagent-0.0.3/muagent/llm_models/openai_model.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.208071 codefuse_muagent-0.0.3/muagent/orm/
+-rw-rw-rw-   0        0        0      573 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.217071 codefuse_muagent-0.0.3/muagent/orm/commands/
+-rw-rw-rw-   0        0        0      452 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/orm/commands/__init__.py
+-rw-rw-rw-   0        0        0     2426 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/commands/code_base_cds.py
+-rw-rw-rw-   0        0        0     2793 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/commands/document_base_cds.py
+-rw-rw-rw-   0        0        0     3157 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/commands/document_file_cds.py
+-rw-rw-rw-   0        0        0     1387 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/db.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.222073 codefuse_muagent-0.0.3/muagent/orm/schemas/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/orm/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2901 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/schemas/base_schema.py
+-rw-rw-rw-   0        0        0      910 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.227072 codefuse_muagent-0.0.3/muagent/retrieval/
+-rw-rw-rw-   0        0        0      139 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/__init__.py
+-rw-rw-rw-   0        0        0     2519 2024-03-21 04:10:28.000000 codefuse_muagent-0.0.3/muagent/retrieval/base_retrieval.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.235071 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/
+-rw-rw-rw-   0        0        0      120 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/__init__.py
+-rw-rw-rw-   0        0        0     2117 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/json_loader.py
+-rw-rw-rw-   0        0        0     2121 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/jsonl_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.243070 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/
+-rw-rw-rw-   0        0        0       76 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/__init__.py
+-rw-rw-rw-   0        0        0     2837 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/langchain_splitter.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.249070 codefuse_muagent-0.0.3/muagent/sandbox/
+-rw-rw-rw-   0        0        0      119 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/sandbox/__init__.py
+-rw-rw-rw-   0        0        0     3772 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/sandbox/basebox.py
+-rw-rw-rw-   0        0        0    20458 2024-04-11 11:32:17.000000 codefuse_muagent-0.0.3/muagent/sandbox/pycodebox.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.276082 codefuse_muagent-0.0.3/muagent/service/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/service/__init__.py
+-rw-rw-rw-   0        0        0     5851 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/service/base_service.py
+-rw-rw-rw-   0        0        0    10063 2024-04-07 03:54:58.000000 codefuse_muagent-0.0.3/muagent/service/cb_api.py
+-rw-rw-rw-   0        0        0     6887 2024-04-10 09:08:37.000000 codefuse_muagent-0.0.3/muagent/service/faiss_db_service.py
+-rw-rw-rw-   0        0        0    16377 2024-03-19 05:49:11.000000 codefuse_muagent-0.0.3/muagent/service/kb_api.py
+-rw-rw-rw-   0        0        0     5742 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/service/migrate.py
+-rw-rw-rw-   0        0        0     5096 2024-03-19 03:31:20.000000 codefuse_muagent-0.0.3/muagent/service/service_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.313567 codefuse_muagent-0.0.3/muagent/tools/
+-rw-rw-rw-   0        0        0     1108 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/abnormal_detection.py
+-rw-rw-rw-   0        0        0     2332 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/base_tool.py
+-rw-rw-rw-   0        0        0     2577 2024-04-10 08:46:41.000000 codefuse_muagent-0.0.3/muagent/tools/cb_query_tool.py
+-rw-rw-rw-   0        0        0     4355 2024-03-27 08:14:38.000000 codefuse_muagent-0.0.3/muagent/tools/codechat_tools.py
+-rw-rw-rw-   0        0        0     2070 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/tools/docs_retrieval.py
+-rw-rw-rw-   0        0        0     2882 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/duckduckgo_search.py
+-rw-rw-rw-   0        0        0     1110 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/metrics_query.py
+-rw-rw-rw-   0        0        0     1146 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/multiplier.py
+-rw-rw-rw-   0        0        0     4491 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/ocr_tool.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/sandbox.py
+-rw-rw-rw-   0        0        0     8334 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/tools/stock_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.318567 codefuse_muagent-0.0.3/muagent/tools/tool_datas/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/tool_datas/__init__.py
+-rw-rw-rw-   0        0        0   247049 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/tool_datas/stock_data.py
+-rw-rw-rw-   0        0        0     4398 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/weather.py
+-rw-rw-rw-   0        0        0     7788 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/world_time.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.361568 codefuse_muagent-0.0.3/muagent/utils/
+-rw-rw-rw-   0        0        0      209 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/__init__.py
+-rw-rw-rw-   0        0        0     2804 2024-04-07 04:53:53.000000 codefuse_muagent-0.0.3/muagent/utils/code2doc_util.py
+-rw-rw-rw-   0        0        0     3406 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/utils/common_utils.py
+-rw-rw-rw-   0        0        0     2698 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/utils/path_utils.py
+-rw-rw-rw-   0        0        0      188 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/postprocess.py
+-rw-rw-rw-   0        0        0     7522 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/server_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.363568 codefuse_muagent-0.0.3/muagent/utils/static/
+-rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/static/__init__.py
+-rw-rw-rw-   0        0        0     5107 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/utils/tbase_util.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 09:35:24.375568 codefuse_muagent-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/setup.py
+-rw-rw-rw-   0        0        0     1203 2024-04-23 09:33:59.000000 codefuse_muagent-0.0.3/setup_test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.366567 codefuse_muagent-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1720 2024-03-26 02:49:26.000000 codefuse_muagent-0.0.3/tests/test_config.py
```

### Comparing `codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/PKG-INFO` & `codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefuse-muagent
-Version: 0.0.1
+Version: 0.0.3
 Summary: A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.
 Home-page: https://github.com/codefuse-ai/CodeFuse-muAgent
 Author: shanshi
 Author-email: wyp311395@antgroup.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,7 +21,8 @@
 Requires-Dist: psutil
 Requires-Dist: faiss-cpu
 Requires-Dist: notebook
 Requires-Dist: chromadb==0.4.17
 Requires-Dist: javalang==0.13.0
 Requires-Dist: nebula3-python==3.1.0
 Requires-Dist: redis==5.0.1
+Requires-Dist: pydantic<=1.10.14
```

### Comparing `codefuse-muagent-0.0.1/CodeFuse_muAgent.egg-info/SOURCES.txt` & `codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -152,9 +152,10 @@
 muagent/tools/tool_datas/stock_data.py
 muagent/utils/__init__.py
 muagent/utils/code2doc_util.py
 muagent/utils/common_utils.py
 muagent/utils/path_utils.py
 muagent/utils/postprocess.py
 muagent/utils/server_utils.py
+muagent/utils/tbase_util.py
 muagent/utils/static/__init__.py
 tests/test_config.py
```

### Comparing `codefuse-muagent-0.0.1/LICENSE.md` & `codefuse_muagent-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/PKG-INFO` & `codefuse_muagent-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefuse-muagent
-Version: 0.0.1
+Version: 0.0.3
 Summary: A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.
 Home-page: https://github.com/codefuse-ai/CodeFuse-muAgent
 Author: shanshi
 Author-email: wyp311395@antgroup.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,7 +21,8 @@
 Requires-Dist: psutil
 Requires-Dist: faiss-cpu
 Requires-Dist: notebook
 Requires-Dist: chromadb==0.4.17
 Requires-Dist: javalang==0.13.0
 Requires-Dist: nebula3-python==3.1.0
 Requires-Dist: redis==5.0.1
+Requires-Dist: pydantic<=1.10.14
```

### Comparing `codefuse-muagent-0.0.1/README.md` & `codefuse_muagent-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 <p align="left">
     <a href="README_zh.md">中文</a>&nbsp ｜ &nbsp<a>English&nbsp </a>
 </p>
 
-# <p align="center">MuAgent: A Multi-Agent FrameWork For Faster Build Agents</p>
+# <p align="center">CodeFuse-muAgent: A Multi-Agent FrameWork For Faster Build Agents</p>
 
 <p align="center">
     <a href="README.md"><img src="https://img.shields.io/badge/文档-中文版-yellow.svg" alt="ZH doc"></a>
     <a href="README_en.md"><img src="https://img.shields.io/badge/document-English-yellow.svg" alt="EN doc"></a>
-    <img src="https://img.shields.io/github/license/codefuse-ai/muagent" alt="License">
-    <a href="https://github.com/codefuse-ai/muagent/issues">
-      <img alt="Open Issues" src="https://img.shields.io/github/issues-raw/codefuse-ai/muagent" />
+    <img src="https://img.shields.io/github/license/codefuse-ai/CodeFuse-muAgent" alt="License">
+    <a href="https://github.com/codefuse-ai/CodeFuse-muAgent/issues">
+      <img alt="Open Issues" src="https://img.shields.io/github/issues-raw/codefuse-ai/CodeFuse-muAgent" />
     </a>
     <br><br>
 </p>
 
 
 
 ## 🔔 News
-- [2024.04.01] muagent is now open source, featuring functionalities such as knowledge base, code library, tool usage, code interpreter, and more
+- [2024.04.01] codefuse-muagent is now open source, featuring functionalities such as knowledge base, code library, tool usage, code interpreter, and more
 
 ## 📜 Contents
 - [🤝 Introduction](#-Introduction)
 - [🚀 QuickStart](#-QuickStart)
 - [🧭 Key Technologies](#-Key-Technologies)
 - [🗂 Miscellaneous](#-Miscellaneous)
   - [📱 Contact Us](#-Contact-Us)
 
 
 ## 🤝 Introduction
-Developed by the Ant CodeFuse Team, muagent is a Multi-Agent framework whose primary goal is to streamline the Standard Operating Procedure (SOP) orchestration for agents. muagent integrates a rich collection of toolkits, code libraries, knowledge bases, and sandbox environments, enabling users to rapidly construct complex Multi-Agent interactive applications in any field. This framework allows for the efficient execution and handling of multi-layered and multi-dimensional complex tasks.
+Developed by the Ant CodeFuse Team, CodeFuse-muAgent is a Multi-Agent framework whose primary goal is to streamline the Standard Operating Procedure (SOP) orchestration for agents. muagent integrates a rich collection of toolkits, code libraries, knowledge bases, and sandbox environments, enabling users to rapidly construct complex Multi-Agent interactive applications in any field. This framework allows for the efficient execution and handling of multi-layered and multi-dimensional complex tasks.
 
 ![](docs/resources/agent_runtime.png)
 
 ## 🚀 快速使用
-For complete documentation, see: [muagent](docs/overview/o1.muagent.md)
+For complete documentation, see: [CodeFuse-muAgent](docs/overview/o1.muagent.md)
 For more [demos](docs/overview/o3.quick-start.md)
 
 1. Installation
 ```
-pip install muagent
+pip install codefuse-muagent
 ```
 
 2. Code answer Prepare related llm and embedding model configurations
 ```
 import os
 
 # set your config
@@ -66,14 +66,15 @@
 )
 ```
 
 <br>
 
 Initialize the codebase
 ```
+from muagent.base_configs.env_config import CB_ROOT_PATH
 codebase_name = 'client_local'
 code_path = "D://chromeDownloads/devopschat-bot/client_v2/client"
 
 cbh = CodeBaseHandler(
     codebase_name, code_path, crawl_type='dir', use_nh=use_nh,local_graph_path=CB_ROOT_PATH,
     llm_config=llm_config, embed_config=embed_config
 )
@@ -85,14 +86,23 @@
 Start codebase Q&A
 ```
 # 
 phase_name = "codeChatPhase"
 phase = BasePhase(
     phase_name, embed_config=embed_config, llm_config=llm_config,
 )
+# 
+query_content = "what does the remove' function?"
+query = Message(
+    role_name="user", role_type="human", input_query=query_content,
+    code_engine_name=codebase_name, score_threshold=1.0, top_k=3, cb_search_type="tag",
+    local_graph_path=CB_ROOT_PATH, use_nh=False
+    )
+output_message3, output_memory3 = phase.step(query)
+print(output_memory3.to_str_messages(return_all=True, content_key="parsed_output_list"))
 ```
 
 ## Key Technologies
 
 ● Agent Base：Four fundamental Agent types are constructed – BaseAgent, ReactAgent, ExecutorAgent, SelectorAgent, supporting basic activities across various scenarios 
 ● Communication: Information transmission between Agents is accomplished through Message and Parse Message entities, interacting with Memory Manager and managing memories in the Memory Pool 
 ● Prompt Manager: Customized Agent Prompts are automatically assembled with the aid of Role Handler, Doc/Tool Handler, Session Handler, and Customized Handler
```

#### html2text {}

```diff
@@ -1,58 +1,67 @@
 _ä_¸_­_æ__  ï½  English 
 #
-           MuAgent: A Multi-Agent FrameWork For Faster Build Agents
+       CodeFuse-muAgent: A Multi-Agent FrameWork For Faster Build Agents
                     _[_Z_H_ _d_o_c_]_[_E_N_ _d_o_c_][License]_[_O_p_e_n_ _I_s_s_u_e_s_]
 
-## ð News - [2024.04.01] muagent is now open source, featuring
+## ð News - [2024.04.01] codefuse-muagent is now open source, featuring
 functionalities such as knowledge base, code library, tool usage, code
 interpreter, and more ## ð Contents - [ð¤ Introduction](#-Introduction) -
 [ð QuickStart](#-QuickStart) - [ð§­ Key Technologies](#-Key-Technologies) -
 [ð Miscellaneous](#-Miscellaneous) - [ð± Contact Us](#-Contact-Us) ## ð¤
-Introduction Developed by the Ant CodeFuse Team, muagent is a Multi-Agent
-framework whose primary goal is to streamline the Standard Operating Procedure
-(SOP) orchestration for agents. muagent integrates a rich collection of
-toolkits, code libraries, knowledge bases, and sandbox environments, enabling
-users to rapidly construct complex Multi-Agent interactive applications in any
-field. This framework allows for the efficient execution and handling of multi-
-layered and multi-dimensional complex tasks. ![](docs/resources/
-agent_runtime.png) ## ð å¿«éä½¿ç¨ For complete documentation, see:
-[muagent](docs/overview/o1.muagent.md) For more [demos](docs/overview/o3.quick-
-start.md) 1. Installation ``` pip install muagent ``` 2. Code answer Prepare
-related llm and embedding model configurations ``` import os # set your config
-api_key = "" api_base_url= "" model_name = "" embed_model = "" embed_model_path
-= "" from muagent.llm_models.llm_config import EmbedConfig, LLMConfig from
-muagent.connector.phase import BasePhase from muagent.connector.schema import
-Message, Memory from muagent.codechat.codebase_handler.codebase_handler import
-CodeBaseHandler llm_config = LLMConfig( model_name=model_name, api_key=api_key,
+Introduction Developed by the Ant CodeFuse Team, CodeFuse-muAgent is a Multi-
+Agent framework whose primary goal is to streamline the Standard Operating
+Procedure (SOP) orchestration for agents. muagent integrates a rich collection
+of toolkits, code libraries, knowledge bases, and sandbox environments,
+enabling users to rapidly construct complex Multi-Agent interactive
+applications in any field. This framework allows for the efficient execution
+and handling of multi-layered and multi-dimensional complex tasks. ![](docs/
+resources/agent_runtime.png) ## ð å¿«éä½¿ç¨ For complete documentation,
+see: [CodeFuse-muAgent](docs/overview/o1.muagent.md) For more [demos](docs/
+overview/o3.quick-start.md) 1. Installation ``` pip install codefuse-muagent
+``` 2. Code answer Prepare related llm and embedding model configurations ```
+import os # set your config api_key = "" api_base_url= "" model_name = ""
+embed_model = "" embed_model_path = "" from muagent.llm_models.llm_config
+import EmbedConfig, LLMConfig from muagent.connector.phase import BasePhase
+from muagent.connector.schema import Message, Memory from
+muagent.codechat.codebase_handler.codebase_handler import CodeBaseHandler
+llm_config = LLMConfig( model_name=model_name, api_key=api_key,
 api_base_url=api_base_url, temperature=0.3 ) embed_config = EmbedConfig
 ( embed_engine="model", embed_model=embed_model,
 embed_model_path=embed_model_path ) ```
-Initialize the codebase ``` codebase_name = 'client_local' code_path = "D://
-chromeDownloads/devopschat-bot/client_v2/client" cbh = CodeBaseHandler
-( codebase_name, code_path, crawl_type='dir',
-use_nh=use_nh,local_graph_path=CB_ROOT_PATH, llm_config=llm_config,
-embed_config=embed_config ) cbh.import_code(do_interpret=do_interpret) ```
+Initialize the codebase ``` from muagent.base_configs.env_config import
+CB_ROOT_PATH codebase_name = 'client_local' code_path = "D://chromeDownloads/
+devopschat-bot/client_v2/client" cbh = CodeBaseHandler( codebase_name,
+code_path, crawl_type='dir', use_nh=use_nh,local_graph_path=CB_ROOT_PATH,
+llm_config=llm_config, embed_config=embed_config ) cbh.import_code
+(do_interpret=do_interpret) ```
 Start codebase Q&A ``` # phase_name = "codeChatPhase" phase = BasePhase
-( phase_name, embed_config=embed_config, llm_config=llm_config, ) ``` ## Key
-Technologies â Agent Baseï¼Four fundamental Agent types are constructed â
-BaseAgent, ReactAgent, ExecutorAgent, SelectorAgent, supporting basic
-activities across various scenarios â Communication: Information transmission
-between Agents is accomplished through Message and Parse Message entities,
-interacting with Memory Manager and managing memories in the Memory Pool â
-Prompt Manager: Customized Agent Prompts are automatically assembled with the
-aid of Role Handler, Doc/Tool Handler, Session Handler, and Customized Handler
-â Memory Manager: Facilitates the management of chat history storage,
-information compression, and memory retrieval, culminating in storage within
-databases, local systems, and vector databases via the Memory Pool â
-Component: Auxiliary ecosystem components to construct Agents, including
-Retrieval, Tool, Action, Sandbox, etc. â Customized Model: Supports the
-integration of private LLM and Embedding models ## Contribution We are deeply
-grateful for your interest in the Codefuse project and warmly welcome any
-suggestions, opinions (including criticism), comments, and contributions. Feel
-free to raise your suggestions, opinions, and comments directly through GitHub
-Issues. There are numerous ways to participate in and contribute to the
-Codefuse project: code implementation, writing tests, process tool
-improvements, documentation enhancements, etc. We welcome any contribution and
-will add you to the list of contributors. See [Contribution Guide...](docs/
-contribution/contribute_guide.md) ## ð Miscellaneous ### ð± Contact Us
+( phase_name, embed_config=embed_config, llm_config=llm_config, ) #
+query_content = "what does the remove' function?" query = Message
+( role_name="user", role_type="human", input_query=query_content,
+code_engine_name=codebase_name, score_threshold=1.0, top_k=3,
+cb_search_type="tag", local_graph_path=CB_ROOT_PATH, use_nh=False )
+output_message3, output_memory3 = phase.step(query) print
+(output_memory3.to_str_messages(return_all=True,
+content_key="parsed_output_list")) ``` ## Key Technologies â Agent
+Baseï¼Four fundamental Agent types are constructed â BaseAgent, ReactAgent,
+ExecutorAgent, SelectorAgent, supporting basic activities across various
+scenarios â Communication: Information transmission between Agents is
+accomplished through Message and Parse Message entities, interacting with
+Memory Manager and managing memories in the Memory Pool â Prompt Manager:
+Customized Agent Prompts are automatically assembled with the aid of Role
+Handler, Doc/Tool Handler, Session Handler, and Customized Handler â Memory
+Manager: Facilitates the management of chat history storage, information
+compression, and memory retrieval, culminating in storage within databases,
+local systems, and vector databases via the Memory Pool â Component:
+Auxiliary ecosystem components to construct Agents, including Retrieval, Tool,
+Action, Sandbox, etc. â Customized Model: Supports the integration of private
+LLM and Embedding models ## Contribution We are deeply grateful for your
+interest in the Codefuse project and warmly welcome any suggestions, opinions
+(including criticism), comments, and contributions. Feel free to raise your
+suggestions, opinions, and comments directly through GitHub Issues. There are
+numerous ways to participate in and contribute to the Codefuse project: code
+implementation, writing tests, process tool improvements, documentation
+enhancements, etc. We welcome any contribution and will add you to the list of
+contributors. See [Contribution Guide...](docs/contribution/
+contribute_guide.md) ## ð Miscellaneous ### ð± Contact Us
                                  width="360">
```

### Comparing `codefuse-muagent-0.0.1/muagent/base_configs/env_config.py` & `codefuse_muagent-0.0.3/muagent/base_configs/env_config.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/chat/agent_chat.py` & `codefuse_muagent-0.0.3/muagent/chat/agent_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             api_base_url: str = Body(os.environ.get("API_BASE_URL"),),
             embed_model: str = Body("", description="向量模型"),
             embed_model_path: str = Body("", description="向量模型路径"),
             model_device: str = Body("", description="模型加载设备"),
             embed_engine: str = Body("", description="向量模型类型"),
             model_name: str = Body("", description="llm模型名称"),
             temperature: float = Body(0.2, description=""),
+            chat_index: str = "",
             **kargs
             ) -> Message:
         
         # update configs
         phase_configs, chain_configs, agent_configs = self.update_configs(
             custom_phase_configs, custom_chain_configs, custom_role_configs)
         params = locals()
@@ -102,14 +103,15 @@
             upload_file_name = upload_file if upload_file and isinstance(upload_file, str) else upload_file.name
             for _filename_idx in range(len(upload_file_name), 0, -1):
                 if upload_file_name[:_filename_idx] in query:
                     query = query.replace(upload_file_name[:_filename_idx], upload_file_name)
                     break
 
         input_message = Message(
+            chat_index=chat_index,
             role_content=query,
             role_type="user",
             role_name="human",
             input_query=query,
             phase_name=phase_name,
             chain_name=chain_name,
             do_search=do_search,
@@ -120,15 +122,15 @@
             code_engine_name=code_engine_name,
             score_threshold=score_threshold, top_k=top_k,
             history_node_list=history_node_list,
             tools=tools
         )
         # history memory mangemant
         history = Memory(messages=[
-            Message(role_name=i["role"], role_type=i["role"], role_content=i["content"]) 
+            Message(chat_index=chat_index,role_name=i["role"], role_type=i["role"], role_content=i["content"]) 
             for i in history
             ])
         # start to execute
         phase_class = getattr(PHASE_MODULE, phase_configs[input_message.phase_name]["phase_type"])
         # TODO 需要把相关信息补充上去
         phase = phase_class(input_message.phase_name,
             task = input_message.task,
@@ -216,14 +218,15 @@
             api_base_url: str = Body(os.environ.get("API_BASE_URL"),),
             embed_model: str = Body("", description="向量模型"),
             embed_model_path: str = Body("", description="向量模型路径"),
             model_device: str = Body("", description="模型加载设备"),
             embed_engine: str = Body("", description="向量模型类型"),
             model_name: str = Body("", description="llm模型名称"),
             temperature: float = Body(0.2, description=""),
+            chat_index: str = "",
             **kargs
             ) -> Message:
         
         # update configs
         phase_configs, chain_configs, agent_configs = self.update_configs(
             custom_phase_configs, custom_chain_configs, custom_role_configs)
         
@@ -240,14 +243,15 @@
             upload_file_name = upload_file if upload_file and isinstance(upload_file, str) else upload_file.name
             for _filename_idx in range(len(upload_file_name), 0, -1):
                 if upload_file_name[:_filename_idx] in query:
                     query = query.replace(upload_file_name[:_filename_idx], upload_file_name)
                     break
 
         input_message = Message(
+            chat_index=chat_index,
             role_content=query,
             role_type="user",
             role_name="human",
             input_query=query,
             phase_name=phase_name,
             chain_name=chain_name,
             do_search=do_search,
```

### Comparing `codefuse-muagent-0.0.1/muagent/chat/base_chat.py` & `codefuse_muagent-0.0.3/muagent/chat/base_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/chat/code_chat.py` & `codefuse_muagent-0.0.3/muagent/chat/code_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/chat/knowledge_chat.py` & `codefuse_muagent-0.0.3/muagent/chat/knowledge_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/chat/llm_chat.py` & `codefuse_muagent-0.0.3/muagent/chat/llm_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/chat/search_chat.py` & `codefuse_muagent-0.0.3/muagent/chat/search_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/chat/utils.py` & `codefuse_muagent-0.0.3/muagent/chat/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_analyzer.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_analyzer.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_dedup.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_dedup.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_intepreter.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_intepreter.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/code_static_analysis.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_static_analysis.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_crawler/dir_crawler.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_crawler/dir_crawler.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_crawler/zip_crawler.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_crawler/zip_crawler.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_search/code_search.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_search/code_search.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_search/cypher_generator.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_search/cypher_generator.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/code_search/tagger.py` & `codefuse_muagent-0.0.3/muagent/codechat/code_search/tagger.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/codebase_handler/code_importer.py` & `codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/code_importer.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/codechat/codebase_handler/codebase_handler.py` & `codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/codebase_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if use_nh:
             try:
                 self.nh = NebulaHandler(host=NEBULA_HOST, port=NEBULA_PORT, username=NEBULA_USER,
                                         password=NEBULA_PASSWORD, space_name=codebase_name)
                 self.nh.add_host(NEBULA_HOST, NEBULA_STORAGED_PORT)
                 time.sleep(1)
             except Exception as e:
-                logger.exception(e)
+                # logger.exception(e)
                 self.nh = None
                 try:
                     with open(self.local_graph_file_path, 'r') as f:
                         self.graph = json.load(f)
                 except:
                     pass
         elif local_graph_path:
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/agents/base_agent.py` & `codefuse_muagent-0.0.3/muagent/connector/agents/base_agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List, Union
 import importlib
 import re, os
 import copy
+import uuid
 from loguru import logger
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.schema import (
     Memory, Task, Role, Message, PromptField, LogVerboseEnum
 )
-from muagent.connector.memory_manager import BaseMemoryManager
 from muagent.connector.message_process import MessageUtils
 from muagent.llm_models import getExtraModel, LLMConfig, getChatModelFromConfig, EmbedConfig
 from muagent.connector.prompt_manager.prompt_manager import PromptManager
-from muagent.connector.memory_manager import LocalMemoryManager
+from muagent.connector.memory_manager import BaseMemoryManager, LocalMemoryManager, TbaseMemoryManager
 from muagent.base_configs.env_config import JUPYTER_WORK_PATH, KB_ROOT_PATH
-
+from muagent.utils.tbase_util import TbaseHandler
 
 class BaseAgent:
 
     def __init__(
             self, 
             role: Role,
             prompt_config: List[PromptField] = None,
@@ -34,15 +34,16 @@
             embed_config: EmbedConfig = None,
             sandbox_server: dict = {},
             jupyter_work_path: str = JUPYTER_WORK_PATH,
             kb_root_path: str = KB_ROOT_PATH,
             doc_retrieval: Union[BaseRetriever] = None,
             code_retrieval = None,
             search_retrieval = None,
-            log_verbose: str = "0"
+            log_verbose: str = "0",
+            tbase_handler: TbaseHandler = None,
             ):
         
         self.task = task
         self.role = role
         self.sandbox_server = sandbox_server
         self.jupyter_work_path = jupyter_work_path
         self.kb_root_path = kb_root_path
@@ -56,43 +57,47 @@
         self.focus_agents = focus_agents
         self.focus_message_keys = focus_message_keys
         # 
         prompt_manager_module = importlib.import_module("muagent.connector.prompt_manager")
         prompt_manager = getattr(prompt_manager_module, prompt_manager_type)
         self.prompt_manager: PromptManager = prompt_manager(role=role, role_prompt=role.role_prompt, prompt_config=prompt_config)
         self.log_verbose = max(os.environ.get("log_verbose", "0"), log_verbose)
+        self.tbase_handler = tbase_handler
 
-    def step(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None) -> Message:
+    def step(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str = "") -> Message:
         '''agent reponse from multi-message'''
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         message = None
-        for message in self.astep(query, history, background, memory_manager):
+        for message in self.astep(query, history, background, memory_manager, chat_index=chat_index):
             pass
         return message
     
-    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None) -> Message:
+    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str = "") -> Message:
         '''agent reponse from multi-message'''
         # insert query into memory
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         query_c = copy.deepcopy(query)
         query_c = self.start_action_step(query_c)
 
         memory_manager = self.init_memory_manager(memory_manager)
         memory_manager.append(query)
-        memory_pool = memory_manager.get_memory_pool(query_c.user_name)
+        memory_pool = memory_manager.get_memory_pool(chat_index)
 
         prompt = self.prompt_manager.generate_full_prompt(
             previous_agent_message=query_c, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, memory_pool=memory_pool)
         content = self.llm.predict(prompt)
 
         if LogVerboseEnum.ge(LogVerboseEnum.Log2Level, self.log_verbose):
             logger.debug(f"{self.role.role_name} prompt: {prompt}")
 
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
             logger.info(f"{self.role.role_name} content: {content}")
 
         output_message = Message(
+            chat_index=chat_index,
             user_name=query.user_name,
             role_name=self.role.role_name,
             role_type="assistant", #self.role.role_type,
             role_content=content,
             step_content=content,
             input_query=query_c.input_query,
             tools=query_c.tools,
@@ -100,15 +105,15 @@
             customed_kargs=query_c.customed_kargs
             )
         
         # common parse llm' content to message
         output_message = self.message_utils.parser(output_message)
 
         # action step
-        output_message, observation_message = self.message_utils.step_router(output_message, history, background, memory_manager=memory_manager)
+        output_message, observation_message = self.message_utils.step_router(output_message, history, background, memory_manager=memory_manager, chat_index=chat_index)
         output_message.parsed_output_list.append(output_message.parsed_output)
         if observation_message:
             output_message.parsed_output_list.append(observation_message.parsed_output)
 
         # update self_memory
         self.append_history(query_c)
         self.append_history(output_message)
@@ -118,18 +123,20 @@
         output_message = self.message_utils.inherit_extrainfo(query, output_message)
         output_message = self.end_action_step(output_message)
 
         # update memory pool
         memory_manager.append(output_message)
         yield output_message
     
-    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None):
+    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str = ""):
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
+
         memory_manager = self.init_memory_manager(memory_manager)
         memory_manager.append(query)
-        memory_pool = memory_manager.get_memory_pool(query.user_name)
+        memory_pool = memory_manager.get_memory_pool(chat_index)
 
         prompt = self.prompt_manager.pre_print(
             previous_agent_message=query, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, memory_pool=memory_pool)
         title = f"<<<<{self.role.role_name}'s prompt>>>>"
         print("#"*len(title) + f"\n{title}\n"+ "#"*len(title)+ f"\n\n{prompt}\n\n")
 
     def init_history(self, memory: Memory = None) -> Memory:
@@ -143,21 +150,28 @@
         
     def clear_history(self, ):
         self.memory.clear()
         self.memory = self.init_history()
     
     def init_memory_manager(self, memory_manager):
         if memory_manager is None:
-            memory_manager = LocalMemoryManager(
-                unique_name=self.role.role_name, 
-                do_init=True, 
-                kb_root_path = self.kb_root_path, 
-                embed_config=self.embed_config, 
-                llm_config=self.llm_config
-            )
+            if self.tbase_handler:
+                memory_manager = TbaseMemoryManager(
+                unique_name=self.role.role_name, use_vector=True, 
+                tbase_handler=self.tbase_handler, 
+                embed_config=self.embed_config, llm_config=self.llm_config,
+                )
+            else:
+                memory_manager = LocalMemoryManager(
+                    unique_name=self.role.role_name, 
+                    do_init=True, 
+                    kb_root_path = self.kb_root_path, 
+                    embed_config=self.embed_config, 
+                    llm_config=self.llm_config
+                )
         return memory_manager
 
     def create_llm_engine(self, llm_config: LLMConfig = None, temperature=0.2, stop=None):
         return getChatModelFromConfig(llm_config=llm_config)
     
     def registry_actions(self, actions):
         '''registry llm's actions'''
@@ -175,43 +189,43 @@
         # message["customed_kargs"]["xx"] = action_json
         return message
     
     def token_usage(self, ):
         '''calculate the usage of token'''
         pass
 
-    def select_memory_by_key(self, memory: Memory) -> Memory:
-        return Memory(
-            messages=[self.select_message_by_key(message) for message in memory.messages 
-                      if self.select_message_by_key(message) is not None]
-                      )
-
-    def select_memory_by_agent_key(self, memory: Memory) -> Memory:
-        return Memory(
-            messages=[self.select_message_by_agent_key(message) for message in memory.messages 
-                      if self.select_message_by_agent_key(message) is not None]
-                      )
-
-    def select_message_by_agent_key(self, message: Message) -> Message:
-        # assume we focus all agents
-        if self.focus_agents == []:
-            return message
-        return None if message is None or message.role_name not in self.focus_agents else self.select_message_by_key(message)
-    
-    def select_message_by_key(self, message: Message) -> Message:
-        # assume we focus all key contents
-        if message is None:
-            return message
+    # def select_memory_by_key(self, memory: Memory) -> Memory:
+    #     return Memory(
+    #         messages=[self.select_message_by_key(message) for message in memory.messages 
+    #                   if self.select_message_by_key(message) is not None]
+    #                   )
+
+    # def select_memory_by_agent_key(self, memory: Memory) -> Memory:
+    #     return Memory(
+    #         messages=[self.select_message_by_agent_key(message) for message in memory.messages 
+    #                   if self.select_message_by_agent_key(message) is not None]
+    #                   )
+
+    # def select_message_by_agent_key(self, message: Message) -> Message:
+    #     # assume we focus all agents
+    #     if self.focus_agents == []:
+    #         return message
+    #     return None if message is None or message.role_name not in self.focus_agents else self.select_message_by_key(message)
+    
+    # def select_message_by_key(self, message: Message) -> Message:
+    #     # assume we focus all key contents
+    #     if message is None:
+    #         return message
         
-        if self.focus_message_keys == []:
-            return message
+    #     if self.focus_message_keys == []:
+    #         return message
         
-        message_c = copy.deepcopy(message)
-        message_c.parsed_output = {k: v for k,v in message_c.parsed_output.items() if k in self.focus_message_keys}
-        message_c.parsed_output_list = [{k: v for k,v in parsed_output.items() if k in self.focus_message_keys} for parsed_output in message_c.parsed_output_list]
-        return message_c
+    #     message_c = copy.deepcopy(message)
+    #     message_c.parsed_output = {k: v for k,v in message_c.parsed_output.items() if k in self.focus_message_keys}
+    #     message_c.parsed_output_list = [{k: v for k,v in parsed_output.items() if k in self.focus_message_keys} for parsed_output in message_c.parsed_output_list]
+    #     return message_c
     
     def get_memory(self, content_key="role_content"):
         return self.memory.to_tuple_messages(content_key="step_content")
     
     def get_memory_str(self, content_key="role_content"):
         return "\n".join([": ".join(i) for i in self.memory.to_tuple_messages(content_key="step_content")])
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/agents/executor_agent.py` & `codefuse_muagent-0.0.3/muagent/connector/agents/executor_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import List, Union
 import copy
+import uuid
 from loguru import logger
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.schema import (
     Memory, Task, Env, Role, Message, ActionStatus, PromptField, LogVerboseEnum
 )
 from muagent.connector.memory_manager import BaseMemoryManager
 from muagent.llm_models import LLMConfig, EmbedConfig
-from muagent.connector.memory_manager import LocalMemoryManager
 from muagent.connector.configs.prompts import PLAN_EXECUTOR_PROMPT
 from muagent.base_configs.env_config import JUPYTER_WORK_PATH, KB_ROOT_PATH
+from muagent.utils.tbase_util import TbaseHandler
 
 from .base_agent import BaseAgent
 
 executor_output_template = '''#### RESPONSE OUTPUT FORMAT
 **Thoughts:** Considering the session records and task records, decide whether the current step requires the use of a tool or code_executing. 
 Solve the problem  only displaying the thought process necessary for the current step of solving the problem. 
 
@@ -43,99 +44,105 @@
             embed_config: EmbedConfig = None,
             sandbox_server: dict = {},
             jupyter_work_path: str = JUPYTER_WORK_PATH,
             kb_root_path: str = KB_ROOT_PATH,
             doc_retrieval: Union[BaseRetriever] = None,
             code_retrieval = None,
             search_retrieval = None,
-            log_verbose: str = "0"
+            log_verbose: str = "0",
+            tbase_handler: TbaseHandler = None
             ):
         role.task_context_level = 1
         role.output_template = executor_output_template
 
         super().__init__(role, prompt_config, prompt_manager_type, task, memory, chat_turn,
                          focus_agents, focus_message_keys, llm_config, embed_config, sandbox_server,
-                         jupyter_work_path, kb_root_path, doc_retrieval, code_retrieval, search_retrieval, log_verbose
+                         jupyter_work_path, kb_root_path, doc_retrieval, code_retrieval, search_retrieval, 
+                         log_verbose, tbase_handler
                          )
         self.do_all_task = True # run all tasks
 
-    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None) -> Message:
+    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str = "") -> Message:
         '''agent reponse from multi-message'''
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         # insert query into memory
         task_executor_memory = Memory(messages=[])
         # insert query
         output_message = Message(
+                chat_index=chat_index,
                 user_name=query.user_name,
                 role_name=self.role.role_name,
                 role_type="assistant", #self.role.role_type,
                 role_content="",
                 step_content="",
                 input_query=query.input_query,
                 tools=query.tools,
                 # parsed_output_list=[query.parsed_output],
                 customed_kargs=query.customed_kargs
             )
         
         memory_manager = self.init_memory_manager(memory_manager)
         memory_manager.append(query)
-        memory_pool = memory_manager.get_memory_pool(query.user_name)
+        memory_pool = memory_manager.get_memory_pool(chat_index)
         # acquire the input_query
         input_query = query.role_content or query.input_query
         prompt = PLAN_EXECUTOR_PROMPT.format(**{"content": input_query.replace("*", "")})
         content = self.llm.predict(prompt)
         # logger.debug(f"prompt={prompt}")
         # logger.debug(f"content={content}")
         plan_message = Message(
+                chat_index=chat_index,
                 user_name=query.user_name,
                 role_name="plan_extracter",
                 role_type="assistant", #self.role.role_type,
                 role_content=content,
                 customed_kargs=query.customed_kargs
             )
 
         plan_message = self.message_utils.parser(plan_message)
         # process input_quert to plans and plan_step
         plan_step = int(plan_message.parsed_output.get("PLAN_STEP", 0))
         plans = plan_message.parsed_output.get("PLAN", [input_query])
         # logger.debug(f"plans={plans}, plan_step={plan_step}")
 
-        def _execute_line(task_content, output_message, task_executor_memory, plan_step):
+        def _execute_line(task_content, output_message, task_executor_memory, plan_step, chat_index):
             '''task execute line'''
             query_c = copy.deepcopy(query)
             query_c.parsed_output = {"CURRENT_STEP": task_content}
             query_c = self.start_action_step(query_c)
             task_executor_memory.append(query_c)
-            for output_message, task_executor_memory in self._arun_step(output_message, query_c, self.memory, history, background, memory_pool, task_executor_memory):
+            for output_message, task_executor_memory in self._arun_step(
+                        output_message, query_c, self.memory, history, background, memory_pool, task_executor_memory, chat_index):
                 pass
             output_message.parsed_output.update({"PLAN_STEP": plan_step})
 
         if self.do_all_task:
             # run all tasks step by step
             for idx, task_content in enumerate(plans[plan_step:]):
                 # create your llm prompt
-                _execute_line(task_content, output_message, task_executor_memory, plan_step+idx)
+                _execute_line(task_content, output_message, task_executor_memory, plan_step+idx, chat_index)
                 yield output_message
         else:
             task_content = plans[plan_step]
-            _execute_line(task_content, output_message, task_executor_memory, plan_step)
+            _execute_line(task_content, output_message, task_executor_memory, plan_step, chat_index)
 
         # update self_memory
         self.append_history(query)
         self.append_history(output_message)
         # output_message.input_query = output_message.role_content
 
         # end_action_step
         output_message = self.end_action_step(output_message)
         # update memory pool
         memory_manager.append(output_message)
         yield output_message
 
     def _arun_step(self, output_message: Message, query: Message, self_memory: Memory, 
             history: Memory, background: Memory, memory_pool: BaseMemoryManager, 
-            task_memory: Memory) -> Union[Message, Memory]:
+            task_memory: Memory, chat_index: str) -> Union[Message, Memory]:
         '''execute the llm predict by created prompt'''
         prompt = self.prompt_manager.generate_full_prompt(
             previous_agent_message=query, agent_long_term_memory=self_memory, ui_history=history, chain_summary_messages=background, memory_pool=memory_pool,
             task_memory=task_memory)
         content = self.llm.predict(prompt)
 
         if LogVerboseEnum.ge(LogVerboseEnum.Log2Level, self.log_verbose):
@@ -144,26 +151,27 @@
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
             logger.info(f"{self.role.role_name} content: {content}")
 
         output_message.role_content = content
         output_message.step_content += "\n"+output_message.role_content
         output_message = self.message_utils.parser(output_message)
         # according the output to choose one action for code_content or tool_content
-        output_message, observation_message = self.message_utils.step_router(output_message)
+        output_message, observation_message = self.message_utils.step_router(output_message, chat_index=chat_index)
         # update parserd_output_list
         output_message.parsed_output_list.append(output_message.parsed_output)
 
         react_message = copy.deepcopy(output_message)
         task_memory.append(react_message)
         if observation_message:
             task_memory.append(observation_message)
             output_message.parsed_output_list.append(observation_message.parsed_output)
             # logger.debug(f"{observation_message.role_name} content: {observation_message.role_content}")
         yield output_message, task_memory
 
-    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None):
+    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None, chat_index: str = ""):
         task_memory = Memory(messages=[])
+        memory_pool = memory_manager.get_memory_pool(chat_index)
         prompt = self.prompt_manager.pre_print(
                 previous_agent_message=query, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, react_memory=None, 
-                memory_pool=memory_manager.current_memory, task_memory=task_memory)
+                memory_pool=memory_pool, task_memory=task_memory)
         title = f"<<<<{self.role.role_name}'s prompt>>>>"
         print("#"*len(title) + f"\n{title}\n"+ "#"*len(title)+ f"\n\n{prompt}\n\n")
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/agents/react_agent.py` & `codefuse_muagent-0.0.3/muagent/connector/agents/react_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import List, Union
 import traceback
 import copy
+import uuid
 from loguru import logger
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.schema import (
     Memory, Task, Env, Role, Message, ActionStatus, PromptField, LogVerboseEnum
 )
 from muagent.connector.memory_manager import BaseMemoryManager
 from muagent.llm_models import LLMConfig, EmbedConfig
+from muagent.utils.tbase_util import TbaseHandler
+
 from .base_agent import BaseAgent
-from muagent.connector.memory_manager import LocalMemoryManager
 from muagent.base_configs.env_config import JUPYTER_WORK_PATH, KB_ROOT_PATH
 
 react_output_template = '''#### RESPONSE OUTPUT FORMAT
 **Thoughts:** According the previous observations, plan the approach for using the tool effectively.
 
 **Action Status:** Set to either 'stopped' or 'tool_using'. If 'stopped', provide the final response to the original question. If 'tool_using', proceed with using the specified tool.
 
@@ -62,37 +64,42 @@
             embed_config: EmbedConfig = None,
             sandbox_server: dict = {},
             jupyter_work_path: str = JUPYTER_WORK_PATH,
             kb_root_path: str = KB_ROOT_PATH,
             doc_retrieval: Union[BaseRetriever] = None,
             code_retrieval = None,
             search_retrieval = None,
-            log_verbose: str = "0"
+            log_verbose: str = "0",
+            tbase_handler: TbaseHandler = None
             ):
         
         role.react_context_level = 1
         role.output_template = react_output_template
         # role.session_context_level = 0
         super().__init__(role, prompt_config, prompt_manager_type, task, memory, chat_turn, 
                          focus_agents, focus_message_keys, llm_config, embed_config, sandbox_server,
-                         jupyter_work_path, kb_root_path, doc_retrieval, code_retrieval, search_retrieval, log_verbose
+                         jupyter_work_path, kb_root_path, doc_retrieval, code_retrieval, search_retrieval,
+                         log_verbose, tbase_handler
                          )
 
-    def step(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None) -> Message:
+    def step(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None, chat_index: str = "") -> Message:
         '''agent reponse from multi-message'''
-        for message in self.astep(query, history, background, memory_manager):
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
+        for message in self.astep(query, history, background, memory_manager, chat_index=chat_index):
             pass
         return message
 
-    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None) -> Message:
+    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None, chat_index: str = "") -> Message:
         '''agent reponse from multi-message'''
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         step_nums = copy.deepcopy(self.chat_turn)
         react_memory = Memory(messages=[])
         # insert query
         output_message = Message(
+                chat_index=chat_index,
                 user_name=query.user_name,
                 role_name=self.role.role_name,
                 role_type="assistant", #self.role.role_type,
                 role_content=query.input_query,
                 step_content="",
                 input_query=query.input_query,
                 tools=query.tools,
@@ -100,15 +107,15 @@
                 customed_kargs=query.customed_kargs
                 )
         query_c = copy.deepcopy(query)
         query_c = self.start_action_step(query_c)
 
         memory_manager = self.init_memory_manager(memory_manager)
         memory_manager.append(query)
-        memory_pool = memory_manager.get_memory_pool(query_c.user_name)
+        memory_pool = memory_manager.get_memory_pool(chat_index)
         
         idx = 0
         # start to react
         while step_nums > 0:
             output_message.role_content = output_message.step_content
             prompt = self.prompt_manager.generate_full_prompt(
                 previous_agent_message=query_c, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, react_memory=react_memory, 
@@ -131,15 +138,15 @@
 
             output_message = self.message_utils.parser(output_message)
             # when get finished signal can stop early
             if output_message.action_status == ActionStatus.FINISHED or output_message.action_status == ActionStatus.STOPPED: 
                 output_message.parsed_output_list.append(output_message.parsed_output)
                 break
             # according the output to choose one action for code_content or tool_content
-            output_message, observation_message = self.message_utils.step_router(output_message)
+            output_message, observation_message = self.message_utils.step_router(output_message, chat_index=chat_index)
             output_message.parsed_output_list.append(output_message.parsed_output)
             
             react_message = copy.deepcopy(output_message)
             react_memory.append(react_message)
             if observation_message:
                 react_memory.append(observation_message)
                 output_message.parsed_output_list.append(observation_message.parsed_output)
@@ -152,16 +159,17 @@
         output_message.input_query = query.input_query
         # end_action_step, BUG:it may cause slack some information
         output_message = self.end_action_step(output_message)
         # update memory pool
         memory_manager.append(output_message)
         yield output_message
         
-    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None):
+    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str=""):
         react_memory = Memory(messages=[])
+        memory_pool = memory_manager.get_memory_pool(chat_index)
         prompt = self.prompt_manager.pre_print(
                 previous_agent_message=query, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, react_memory=react_memory, 
-                memory_pool=memory_manager.current_memory)
+                memory_pool=memory_pool)
         title = f"<<<<{self.role.role_name}'s prompt>>>>"
         print("#"*len(title) + f"\n{title}\n"+ "#"*len(title)+ f"\n\n{prompt}\n\n")
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/agents/selector_agent.py` & `codefuse_muagent-0.0.3/muagent/connector/agents/selector_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import List, Union
 import copy
 import random
+import uuid
 from loguru import logger
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.schema import (
     Memory, Task, Role, Message, PromptField, LogVerboseEnum
 )
 from muagent.connector.memory_manager import BaseMemoryManager
-from muagent.connector.memory_manager import LocalMemoryManager
 from muagent.llm_models import LLMConfig, EmbedConfig
+from muagent.utils.tbase_util import TbaseHandler
+
 from muagent.base_configs.env_config import JUPYTER_WORK_PATH, KB_ROOT_PATH
 from .base_agent import BaseAgent
 
 
 class SelectorAgent(BaseAgent):
 
     def __init__(
@@ -33,46 +35,50 @@
             embed_config: EmbedConfig = None,
             sandbox_server: dict = {},
             jupyter_work_path: str = JUPYTER_WORK_PATH,
             kb_root_path: str = KB_ROOT_PATH,
             doc_retrieval: Union[BaseRetriever] = None,
             code_retrieval = None,
             search_retrieval = None,
-            log_verbose: str = "0"
+            log_verbose: str = "0",
+            tbase_handler: TbaseHandler = None
             ):
         
         super().__init__(role, prompt_config, prompt_manager_type, task, memory, chat_turn, 
                          focus_agents, focus_message_keys, llm_config, embed_config, sandbox_server,
-                         jupyter_work_path, kb_root_path, doc_retrieval, code_retrieval, search_retrieval, log_verbose
+                         jupyter_work_path, kb_root_path, doc_retrieval, code_retrieval, search_retrieval, 
+                         log_verbose, tbase_handler
                          )
         self.group_agents = group_agents
 
-    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None) -> Message:
+    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str="") -> Message:
         '''agent reponse from multi-message'''
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         # insert query into memory
         query_c = copy.deepcopy(query)
         query_c = self.start_action_step(query_c)
         # memory_manager init
         memory_manager = self.init_memory_manager(memory_manager)
         memory_manager.append(query)
-        memory_pool = memory_manager.get_memory_pool(query_c.user_name)
+        memory_pool = memory_manager.get_memory_pool(chat_index)
 
         prompt = self.prompt_manager.generate_full_prompt(
                 previous_agent_message=query_c, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, react_memory=None, 
                 memory_pool=memory_pool, agents=self.group_agents)
         content = self.llm.predict(prompt)
 
         if LogVerboseEnum.ge(LogVerboseEnum.Log2Level, self.log_verbose):
             logger.debug(f"{self.role.role_name} prompt: {prompt}")
 
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
             logger.info(f"{self.role.role_name} content: {content}")
 
         # select agent
         select_message = Message(
+            chat_index=chat_index,
             role_name=self.role.role_name,
             role_type="assistant", #self.role.role_type,
             role_content=content,
             step_content=content,
             input_query=query_c.input_query,
             tools=query_c.tools,
             # parsed_output_list=[query_c.parsed_output]
@@ -86,15 +92,15 @@
         if select_message.parsed_output.get("Role", "") in [agent.role.role_name for agent in self.group_agents]:
             for agent in self.group_agents:
                 if agent.role.role_name == select_message.parsed_output.get("Role", ""):
                     break
             
             # 把除了role以外的信息传给下一个agent
             query_c.parsed_output.update({k:v for k,v in select_message.parsed_output.items() if k!="Role"})
-            for output_message in agent.astep(query_c, history, background=background, memory_manager=memory_manager):
+            for output_message in agent.astep(query_c, history, background=background, memory_manager=memory_manager, chat_index=chat_index):
                 yield output_message or select_message
             # update self_memory
             self.append_history(query_c)
             self.append_history(output_message)
             output_message.input_query = output_message.role_content
             # output_message.parsed_output_list.append(output_message.parsed_output)
             # 
@@ -103,16 +109,17 @@
             memory_manager.append(output_message)
 
             select_message.parsed_output = output_message.parsed_output
             select_message.spec_parsed_output.update(output_message.spec_parsed_output)
             select_message.parsed_output_list.extend(output_message.parsed_output_list)
         yield select_message
 
-    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None):
+    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index:str=""):
+        memory_pool = memory_manager.get_memory_pool(chat_index)
         prompt = self.prompt_manager.pre_print(
                 previous_agent_message=query, agent_long_term_memory=self.memory, ui_history=history, chain_summary_messages=background, react_memory=None, 
-                memory_pool=memory_manager.current_memory, agents=self.group_agents)
+                memory_pool=memory_pool, agents=self.group_agents)
         title = f"<<<<{self.role.role_name}'s prompt>>>>"
         print("#"*len(title) + f"\n{title}\n"+ "#"*len(title)+ f"\n\n{prompt}\n\n")
 
         for agent in self.group_agents:
             agent.pre_print(query=query, history=history, background=background, memory_manager=memory_manager)
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/antflow/flow.py` & `codefuse_muagent-0.0.3/muagent/connector/antflow/flow.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/chains/base_chain.py` & `codefuse_muagent-0.0.3/muagent/connector/chains/base_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Tuple, Union
 from loguru import logger
 import copy, os
+import uuid
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.agents import BaseAgent
 from muagent.connector.schema import (
     Memory, Role, Message, ActionStatus, ChainConfig,
     load_role_configs
@@ -51,40 +52,40 @@
             doc_retrieval=doc_retrieval, code_retrieval=code_retrieval,
             search_retrieval=search_retrieval
             )
         self.messageUtils = MessageUtils(None, sandbox_server, self.jupyter_work_path, embed_config, llm_config, kb_root_path, doc_retrieval, code_retrieval, search_retrieval, log_verbose)
         # all memory created by agent until instance deleted
         self.global_memory = Memory(messages=[])
 
-    def step(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None) -> Tuple[Message, Memory]:
+    def step(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None, chat_index: str = "") -> Tuple[Message, Memory]:
         '''execute chain'''
-        for output_message, local_memory in self.astep(query, history, background, memory_manager):
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
+        for output_message, local_memory in self.astep(query, history, background, memory_manager, chat_index):
             pass
         return output_message, local_memory
 
-    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None) -> Message:
+    def pre_print(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None, chat_index: str="") -> Message:
         '''execute chain'''
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         for agent in self.agents:
             agent.pre_print(query, history, background=background, memory_manager=memory_manager)
     
-    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None) -> Tuple[Message, Memory]:
+    def astep(self, query: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager = None, chat_index: str = "") -> Tuple[Message, Memory]:
         '''execute chain'''
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
         local_memory = Memory(messages=[])
         input_message = copy.deepcopy(query)
         step_nums = copy.deepcopy(self.chat_turn)
         check_message = None
 
-        # if input_message not in memory_manager:
-        #     memory_manager.append(input_message)
-
         self.global_memory.append(input_message)
         # local_memory.append(input_message)
         while step_nums > 0:
             for agent in self.agents:
-                for output_message in agent.astep(input_message, history, background=background, memory_manager=memory_manager):
+                for output_message in agent.astep(input_message, history, background=background, memory_manager=memory_manager, chat_index=chat_index):
                     # logger.debug(f"local_memory {local_memory + output_message}")
                     yield output_message, local_memory + output_message
                 output_message = self.messageUtils.inherit_extrainfo(input_message, output_message)
                 # according the output to choose one action for code_content or tool_content
                 # output_message = self.messageUtils.parser(output_message)
                 yield output_message, local_memory + output_message
                 # output_message = self.step_router(output_message)
@@ -96,15 +97,15 @@
                 if output_message.action_status == ActionStatus.FINISHED or output_message.action_status == ActionStatus.STOPPED:
                     action_status = False
                     break
             if output_message.action_status == ActionStatus.FINISHED:
                 break
 
             if self.do_checker and self.chat_turn > 1:
-                for check_message in self.checker.astep(query, background=local_memory, memory_manager=memory_manager):
+                for check_message in self.checker.astep(query, background=local_memory, memory_manager=memory_manager, chat_index=chat_index):
                     pass
                 check_message = self.messageUtils.parser(check_message)
                 check_message = self.messageUtils.inherit_extrainfo(output_message, check_message)
                 # logger.debug(f"{self.checker.role.role_name}: {check_message.role_content}")
 
                 if check_message.action_status == ActionStatus.FINISHED: 
                     self.global_memory.append(check_message)
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/agent_config.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/agent_config.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/chain_config.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/chain_config.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/phase_config.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/phase_config.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompt_config.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompt_config.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/__init__.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/agent_selector_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/agent_selector_template_prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 Your goal is to response according the Context Data's information with the role that will best facilitate a solution, taking into account all relevant context (Context) provided.
 
 When you need to select the appropriate role for handling a user's query, carefully read the provided role names, role descriptions and tool list.
 
 ATTENTION: response carefully referenced "Response Output Format" in format.
 
-#### Input Format
-
-**Origin Query:** the initial question or objective that the user wanted to achieve
-
-**Context:** the context history to determine if Origin Query has been achieved.
-
 #### Response Output Format
 
 **Thoughts:** think the reason step by step about why you selecte one role
 
 **Role:** Select the role from agent names.
 
-"""
+"""
+
+
+# #### Input Format
+
+# **Origin Query:** the initial question or objective that the user wanted to achieve
+
+# **Context:** the context history to determine if Origin Query has been achieved.
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/checker_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/checker_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/code2doc_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2doc_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/code2test_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2test_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/executor_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/executor_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/input_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/input_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/intention_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/intention_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/metagpt_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/metagpt_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/planner_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/planner_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/qa_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/qa_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_code_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_code_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_tool_code_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/react_tool_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/refine_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/refine_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/configs/prompts/summary_template_prompt.py` & `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/summary_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/message_process.py` & `codefuse_muagent-0.0.3/muagent/connector/message_process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re, traceback, uuid, copy, json, os
-from typing import Union
+from typing import Union, Tuple
 from loguru import logger
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.schema import (
     Memory, Role, Message, ActionStatus, CodeDoc, Doc, LogVerboseEnum
 )
@@ -158,114 +158,103 @@
             )
         else:
             code_docs = CodeRetrieval.run(code_engine_name, query, code_limit=message.top_k, history_node_list=history_node_list, search_type=message.cb_search_type,
                                       llm_config=self.llm_config, embed_config=self.embed_config,
                                       use_nh=use_nh, local_graph_path=local_graph_path)
         
         message.code_docs = [CodeDoc(**doc) for doc in code_docs] 
-
-        # related_nodes = [doc.get_related_node() for idx, doc in enumerate(message.code_docs) if idx==0],
-        # history_node_list.extend([node[0] for node in related_nodes]) 
         return message
     
     def get_tool_retrieval(self, message: Message) -> Message:
         return message
     
-    def step_router(self, message: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None) -> tuple[Message, ...]:
+    def step_router(self, message: Message, history: Memory = None, background: Memory = None, memory_manager: BaseMemoryManager=None, chat_index: str = "") -> Tuple[Message, ...]:
         ''''''
+        chat_index = message.chat_index or chat_index or str(uuid.uuid4())
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
             logger.info(f"message.action_status: {message.action_status}")
             
         observation_message = None
         if message.action_status == ActionStatus.CODE_EXECUTING:
-            message, observation_message = self.code_step(message)
+            message, observation_message = self.code_step(message, chat_index)
         elif message.action_status == ActionStatus.TOOL_USING:
-            message, observation_message = self.tool_step(message)
+            message, observation_message = self.tool_step(message, chat_index)
         elif message.action_status == ActionStatus.CODING2FILE:
             self.save_code2file(message, self.jupyter_work_path)
         elif message.action_status == ActionStatus.CODE_RETRIEVAL:
             pass
         elif message.action_status == ActionStatus.CODING:
             pass
         
         return message, observation_message
 
-    def code_step(self, message: Message) -> Message:
+    def code_step(self, message: Message, chat_index: str) -> Message:
         '''execute code'''
-        # logger.debug(f"message.role_content: {message.role_content}, message.code_content: {message.code_content}")
-        code_answer = self.codebox.chat('```python\n{}```'.format(message.code_content))
+        # code_answer = self.codebox.chat('```python\n{}```'.format(message.code_content))
+        code_answer = self.codebox.chat('```python\n{}```'.format(message.customed_kargs.get("code_content", "")))
         code_prompt = f"The return error after executing the above code is {code_answer.code_exe_response}，need to recover.\n" \
                     if code_answer.code_exe_type == "error" else f"The return information after executing the above code is {code_answer.code_exe_response}.\n"
         
         observation_message = Message(
+                chat_index=chat_index,
                 user_name=message.user_name,
                 role_name="observation",
                 role_type="function", #self.role.role_type,
                 role_content="",
                 step_content="",
-                input_query=message.code_content,
+                # input_query=message.code_content,
+                input_query=message.customed_kargs.get("code_content", ""),
                 )
         uid = str(uuid.uuid1())
         if code_answer.code_exe_type == "image/png":
             message.figures[uid] = code_answer.code_exe_response
-            message.code_answer = f"\n**Observation:**: The return figure name is {uid} after executing the above code.\n"
-            message.observation = f"\n**Observation:**: The return figure name is {uid} after executing the above code.\n"
             message.step_content += f"\n**Observation:**: The return figure name is {uid} after executing the above code.\n"
-            # message.role_content += f"\n**Observation:**:执行上述代码后生成一张图片, 图片名为{uid}\n"
             observation_message.role_content = f"\n**Observation:**: The return figure name is {uid} after executing the above code.\n"
             observation_message.parsed_output = {"Observation": f"The return figure name is {uid} after executing the above code.\n"}
         else:
-            message.code_answer = code_answer.code_exe_response
-            message.observation = code_answer.code_exe_response
             message.step_content += f"\n**Observation:**: {code_prompt}\n"
-            # message.role_content += f"\n**Observation:**: {code_prompt}\n"
             observation_message.role_content = f"\n**Observation:**: {code_prompt}\n"
             observation_message.parsed_output = {"Observation": f"{code_prompt}\n"}
         
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
-            logger.info(f"**Observation:** {message.action_status}, {message.observation}")
+            logger.info(f"**Observation:** {message.action_status}, {observation_message.role_content}")
         return message, observation_message
 
-    def tool_step(self, message: Message) -> Message:
+    def tool_step(self, message: Message, chat_index: str) -> Message:
         '''execute tool'''
         observation_message = Message(
+                chat_index=chat_index,
                 user_name=message.user_name,
                 role_name="observation",
                 role_type="function", #self.role.role_type,
                 role_content="\n**Observation:** there is no tool can execute\n",
                 step_content="",
-                input_query=str(message.tool_params),
+                input_query=str(message.customed_kargs.get("tool_params", {})),
                 tools=message.tools,
                 )
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
-            logger.info(f"message: {message.action_status}, {message.tool_params}")
+            logger.info(f"message: {message.action_status}, {message.customed_kargs.get('tool_params', '')}")
 
         tool_names = [tool.name for tool in message.tools]
-        if message.tool_name not in tool_names:
-            message.tool_answer = "\n**Observation:** there is no tool can execute.\n"    
-            message.observation = "\n**Observation:** there is no tool can execute.\n"    
-            # message.role_content += f"\n**Observation:**: 不存在可以执行的tool\n"
+        if message.customed_kargs.get("tool_name", "") not in tool_names:
             message.step_content += f"\n**Observation:** there is no tool can execute.\n"
             observation_message.role_content = f"\n**Observation:** there is no tool can execute.\n"
             observation_message.parsed_output = {"Observation": "there is no tool can execute.\n"}
         
         # logger.debug(message.tool_params)
         for tool in message.tools:
-            if tool.name == message.tool_params.get("tool_name", ""):
-                tool_res = tool.func(**message.tool_params.get("tool_params", {}))
-                message.tool_answer = tool_res    
-                message.observation = tool_res
-                # message.role_content += f"\n**Observation:**: {tool_res}\n"
+            if tool.name == message.customed_kargs.get("tool_params", {}).get("tool_name", ""):
+                tool_res = tool.func(**message.customed_kargs.get("tool_params", {}).get("tool_params", {}))
                 message.step_content += f"\n**Observation:** {tool_res}.\n"
                 observation_message.role_content = f"\n**Observation:** {tool_res}.\n"
                 observation_message.parsed_output = {"Observation": f"{tool_res}.\n"}
                 break
 
         if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
-            logger.info(f"**Observation:** {message.action_status}, {message.observation}")
+            logger.info(f"**Observation:** {message.action_status}, {observation_message.role_content}")
         return message, observation_message
 
     def parser(self, message: Message) -> Message:
         '''parse llm output into dict'''
         content = message.role_content
         # parse start
         parsed_dict = parse_text_to_dict(content)
@@ -275,20 +264,20 @@
         if action_value:
             action_value = action_value.lower()
 
         code_content_value = spec_parsed_dict.get('code')
         if action_value == 'tool_using':
             tool_params_value = spec_parsed_dict.get('json')
         else:
-            tool_params_value = None
+            tool_params_value = {}
 
         # add parse value to message
         message.action_status = action_value or "default"
-        message.code_content = code_content_value
-        message.tool_params = tool_params_value
+        message.customed_kargs["code_content"] = code_content_value
+        message.customed_kargs["tool_params"] = tool_params_value
         message.parsed_output = parsed_dict
         message.spec_parsed_output = spec_parsed_dict
         return message
 
     def save_code2file(self, message: Message, project_dir="./"):
         filename = message.parsed_output.get("SaveFileName")
         code = message.spec_parsed_output.get("code")
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/phase/base_phase.py` & `codefuse_muagent-0.0.3/muagent/connector/phase/base_phase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from typing import List, Union, Dict, Tuple
 import os
 import json
 import importlib
 import copy
+import uuid
 from loguru import logger
 
 from langchain.schema import BaseRetriever
 
 from muagent.connector.agents import BaseAgent
 from muagent.connector.chains import BaseChain
 from muagent.connector.schema import (
     Memory, Task, Message, AgentConfig, ChainConfig, PhaseConfig, LogVerboseEnum,
     CompletePhaseConfig,
     load_chain_configs, load_phase_configs, load_role_configs
 )
-from muagent.connector.memory_manager import BaseMemoryManager, LocalMemoryManager
+from muagent.connector.memory_manager import BaseMemoryManager, LocalMemoryManager, TbaseMemoryManager
 from muagent.connector.configs import AGETN_CONFIGS, CHAIN_CONFIGS, PHASE_CONFIGS
 from muagent.connector.message_process import MessageUtils
 from muagent.llm_models.llm_config import EmbedConfig, LLMConfig
 from muagent.base_configs.env_config import JUPYTER_WORK_PATH, KB_ROOT_PATH
+from muagent.utils.tbase_util import TbaseHandler
 
 
 role_configs = load_role_configs(AGETN_CONFIGS)
 chain_configs = load_chain_configs(CHAIN_CONFIGS)
 phase_configs = load_phase_configs(PHASE_CONFIGS)
 
 
@@ -44,15 +46,16 @@
             base_phase_config: Union[dict, str] = PHASE_CONFIGS,
             base_chain_config: Union[dict, str] = CHAIN_CONFIGS,
             base_role_config: Union[dict, str] = AGETN_CONFIGS,
             chains: List[BaseChain] = [],
             doc_retrieval: Union[BaseRetriever] = None,
             code_retrieval = None,
             search_retrieval = None,
-            log_verbose: str = "0"
+            log_verbose: str = "0",
+            tbase_handler: TbaseHandler = None,
             ) -> None:
         # 
         self.phase_name = phase_name
         self.do_summary = False
         self.do_search = search_retrieval is not None
         self.do_code_retrieval = code_retrieval is not None
         self.do_doc_retrieval = doc_retrieval is not None
@@ -77,62 +80,70 @@
             phase_name,
             phase_config,
             task=task, 
             memory=None,
             base_phase_config = base_phase_config,
             base_chain_config = base_chain_config,
             base_role_config = base_role_config,
+            tbase_handler=tbase_handler
             )
-        self.memory_manager: BaseMemoryManager = LocalMemoryManager(
-            unique_name=phase_name, do_init=True, kb_root_path = kb_root_path, embed_config=embed_config, llm_config=llm_config
+        if tbase_handler:
+            self.memory_manager: BaseMemoryManager = TbaseMemoryManager(
+                unique_name=phase_name, use_vector=True, tbase_handler=tbase_handler, embed_config=embed_config, llm_config=llm_config,
             )
+        else:
+            self.memory_manager: BaseMemoryManager = LocalMemoryManager(
+                unique_name=phase_name, do_init=True, kb_root_path = kb_root_path, embed_config=embed_config, llm_config=llm_config
+                )
         self.conv_summary_agent = BaseAgent(
             role=role_configs["conv_summary"].role,
             prompt_config=role_configs["conv_summary"].prompt_config,
             task = None, memory = None,
             llm_config=self.llm_config,
             embed_config=self.embed_config,
             sandbox_server=sandbox_server,
             jupyter_work_path=jupyter_work_path,
             kb_root_path=kb_root_path
             )
 
-    def astep(self, query: Message, history: Memory = None, reinit_memory=False) -> Tuple[Message, Memory]:
+    def astep(self, query: Message, history: Memory = None, chat_index: str = "", reinit_memory=False) -> Tuple[Message, Memory]:
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
+
         if reinit_memory:
             self.memory_manager.re_init(reinit_memory)
         self.memory_manager.append(query)
         summary_message = None
         chain_message = Memory(messages=[])
         local_phase_memory = Memory(messages=[])
         # do_search、do_doc_search、do_code_search
         query = self.message_utils.get_extrainfo_step(query, self.do_search, self.do_doc_retrieval, self.do_code_retrieval, self.do_tool_retrieval)
-        # query.parsed_output = query.parsed_output if query.parsed_output else {"origin_query": query.input_query}
-        # query.parsed_output_list = query.parsed_output_list if query.parsed_output_list else [{"origin_query": query.input_query}]
         input_message = copy.deepcopy(query)
         
         self.global_memory.append(input_message)
         local_phase_memory.append(input_message)
         for chain in self.chains:
             # chain can supply background and query to next chain
-            for output_message, local_chain_memory in chain.astep(input_message, history, background=chain_message, memory_manager=self.memory_manager):
+            for output_message, local_chain_memory in chain.astep(
+                        input_message, history, background=chain_message, memory_manager=self.memory_manager, chat_index=chat_index):
                 # logger.debug(f"local_memory: {local_phase_memory + local_chain_memory}")
                 yield output_message, local_phase_memory + local_chain_memory
 
             output_message = self.message_utils.inherit_extrainfo(input_message, output_message)
             input_message = output_message
             # logger.info(f"{chain.chainConfig.chain_name} phase_step: {output_message.role_content}")
             # 这一段也有问题
             self.global_memory.extend(local_chain_memory)
             local_phase_memory.extend(local_chain_memory)
 
             # whether to use summary_llm
             if self.do_summary:
                 if LogVerboseEnum.ge(LogVerboseEnum.Log1Level, self.log_verbose):
                     logger.info(f"{self.conv_summary_agent.role.role_name} input global memory: {local_phase_memory.to_str_messages(content_key='step_content')}")
-                for summary_message in self.conv_summary_agent.astep(query, background=local_phase_memory, memory_manager=self.memory_manager):
+                for summary_message in self.conv_summary_agent.astep(
+                            query, background=local_phase_memory, memory_manager=self.memory_manager, chat_index=chat_index):
                     pass
                 # summary_message = Message(**summary_message)
                 summary_message.role_name = chain.chainConfig.chain_name
                 summary_message = self.conv_summary_agent.message_utils.parser(summary_message)
                 summary_message = self.message_utils.inherit_extrainfo(output_message, summary_message)
                 chain_message.append(summary_message)
 
@@ -143,26 +154,27 @@
         for chain in self.chains:
             self.phase_memory.append(chain.global_memory)
         # TODO：local_memory缺少添加summary的过程
         message = summary_message or output_message
         message.role_name = self.phase_name
         yield message, local_phase_memory
 
-    def step(self, query: Message, history: Memory = None, reinit_memory=False) -> Tuple[Message, Memory]:
-        for message, local_phase_memory in self.astep(query, history=history, reinit_memory=reinit_memory):
+    def step(self, query: Message, history: Memory = None, chat_index: str = "", reinit_memory=False) -> Tuple[Message, Memory]:
+        chat_index = query.chat_index or chat_index or str(uuid.uuid4())
+        for message, local_phase_memory in self.astep(query, history=history, chat_index=chat_index, reinit_memory=reinit_memory):
             pass
         return message, local_phase_memory
 
     def pre_print(self, query, history: Memory = None) -> List[str]:
         chain_message = Memory(messages=[])
         for chain in self.chains:
             chain.pre_print(query, history, background=chain_message, memory_manager=self.memory_manager)
 
     def init_chains(self, phase_name: str, phase_config: CompletePhaseConfig, base_phase_config, base_chain_config,
-            base_role_config, task=None, memory=None) -> List[BaseChain]:
+            base_role_config, task=None, memory=None, tbase_handler=None) -> List[BaseChain]:
         # load config
         role_configs = load_role_configs(base_role_config)
         chain_configs = load_chain_configs(base_chain_config)
         phase_configs = load_phase_configs(base_phase_config)
 
         chains = []
         self.chain_module = importlib.import_module("muagent.connector.chains")
@@ -201,15 +213,16 @@
                     embed_config=self.embed_config,
                     sandbox_server=self.sandbox_server,
                     jupyter_work_path=self.jupyter_work_path,
                     kb_root_path=self.kb_root_path,
                     doc_retrieval=self.doc_retrieval,
                     code_retrieval=self.code_retrieval,
                     search_retrieval=self.search_retrieval,
-                    log_verbose=self.log_verbose
+                    log_verbose=self.log_verbose,
+                    tbase_handler=tbase_handler
                 ) 
                 if agent_config.role.agent_type == "SelectorAgent":
                     for group_agent_name in agent_config.group_agents:
                         group_agent_config = role_configs[group_agent_name]
                         llm_config = copy.deepcopy(self.llm_config)
                         llm_config.stop = group_agent_config.stop
                         baseAgent: BaseAgent = getattr(self.agent_module, group_agent_config.role.agent_type)
@@ -226,15 +239,16 @@
                             embed_config=self.embed_config,
                             sandbox_server=self.sandbox_server,
                             jupyter_work_path=self.jupyter_work_path,
                             kb_root_path=self.kb_root_path,
                             doc_retrieval=self.doc_retrieval,
                             code_retrieval=self.code_retrieval,
                             search_retrieval=self.search_retrieval,
-                            log_verbose=self.log_verbose
+                            log_verbose=self.log_verbose,
+                            tbase_handler=tbase_handler
                         ) 
                         base_agent.group_agents.append(group_base_agent)
 
                 agents.append(base_agent)
             
             chain_instance = BaseChain(
                 chain_config,
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/prompt_manager/extend_manager.py` & `codefuse_muagent-0.0.3/muagent/connector/prompt_manager/extend_manager.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/prompt_manager/prompt_manager.py` & `codefuse_muagent-0.0.3/muagent/connector/prompt_manager/prompt_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,15 +206,14 @@
     def generate_full_prompt(self, **kwargs):
         full_prompt = []
         context_prompts = []  # 用于收集上下文内容
         is_pre_print = kwargs.get("is_pre_print", False) # 用于强制打印所有prompt 字段信息，不管有没有空
 
         # update all title's description and function_value
         title_values = {}
-        # logger.debug(f"{self.star_output_titles}")
         for forth_title, forth_value in self.forth_titles.items():
             handler = getattr(self, forth_value["function"])
             kwargs.update({"title_key": forth_title})
             function_value = handler(**kwargs)
             title_values[forth_title] = {
                 "description": forth_value["description"],
                 "function_value": function_value,
@@ -247,53 +246,25 @@
         # logger.debug(f"{title_values}")
         prompt_values = []
         prompt_values = self._process_title_values(title_values, prompt_values, 
                                                    title_type="description", is_pre_print=is_pre_print)
         prompt_values.append("## BEGIN!!!")
         prompt_values = self._process_title_values(title_values, prompt_values, 
                                                    title_type="function_value", is_pre_print=is_pre_print)
-        # 返回完整的提示，移除尾部的空行
-        # logger.debug('\n'.join(prompt_values).rstrip('\n'))
+
         # logger.debug(prompt_values)
         if not any([i=="#### RESPONSE OUTPUT" for i in prompt_values]):
             prompt_values.append("#### RESPONSE OUTPUT")
-
-        return '\n'.join(prompt_values).rstrip('\n')
-        
-        # 先处理上下文字段
-        for field_name in self.context_order:
-            handler = self.context_handlers[field_name]
-            processed_prompt = handler(**kwargs)
-            # Check if the field should be omitted when empty
-            if self.omit_if_empty_flags.get(field_name, False) and not processed_prompt and not is_pre_print:
-                continue  # Skip this field
-            title_or_description = self.field_descriptions.get(field_name, f"#### {field_name.replace('_', ' ').title()}\n\n")
-            context_prompts.append(title_or_description + processed_prompt + '\n\n')
-
-        # 处理普通字段，同时查找 context_placeholder 的位置
-        for field_name in self.field_order:
-            if field_name == 'context_placeholder':
-                # 在 context_placeholder 的位置插入上下文数据
-                full_prompt.append(self.context_title)  # 添加上下文部分的大标题
-                full_prompt.extend(context_prompts)  # 添加收集的上下文内容
-            else:
-                handler = self.field_handlers[field_name]
-                processed_prompt = handler(**kwargs)
-                # Check if the field should be omitted when empty
-                if self.omit_if_empty_flags.get(field_name, False) and not processed_prompt and not is_pre_print:
-                    continue  # Skip this field
-                title_or_description = self.field_descriptions.get(field_name, f"### {field_name.replace('_', ' ').title()}\n\n")
-                full_prompt.append(title_or_description + processed_prompt + '\n\n')
-
         # 返回完整的提示，移除尾部的空行
-        return ''.join(full_prompt).rstrip('\n')
+        return '\n'.join(prompt_values).rstrip('\n')
 
     def _process_title_values(self, title_values, prompt_values, title_type="description", is_pre_print=False):
         '''process title values to prompt'''
         response_omit_flag = False
+        key_placeholder = {}
         for forth_title in title_values.keys():
             forth_title_value = title_values[forth_title]
             func_values = {k: [i["function_value"] for i in forth_title_value[k]] 
                            for k in ['agent_values', 'info_values', 'context_values', 'star_output_values', 'star_input_values'] }
             
             star_values = {k: forth_title_value[k] for k in ['star_output_values', 'star_input_values'] }
             
@@ -310,15 +281,14 @@
             # #### title
             if title_type == "description":
                 prompt_values.append(f"#### {forth_title}\n{forth_title_value['description'] or forth_title_value['function_value'] }")
             elif title_type == "function_value" and forth_title not in ["AGENT PROFILE", "AGENT INFORMATION", "TOOL INFORMATION"]:
                 prompt_values.append(f"#### {forth_title.replace(' FORMAT', '')}\n{ forth_title_value['function_value'] }")
 
             # ### title
-            key_placeholder = {}
             for key in ['agent_values', 'info_values', 'context_values', 'star_output_values', 'star_input_values']:
                 values = forth_title_value[key]
                 str_template = '### {}\n{}' if key not in ['star_output_values', 'star_input_values'] else "**{}:** {}"
 
                 for value in values:
                     title = value["title"]
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/schema/general_schema.py` & `codefuse_muagent-0.0.3/muagent/connector/schema/general_schema.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/connector/schema/memory.py` & `codefuse_muagent-0.0.3/muagent/connector/schema/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
     def extend(self, memory: 'Memory'):
         self.messages.extend(memory.messages)
 
     def update(self, role_name: str, role_type: str, role_content: str):
         self.messages.append(Message(role_name, role_type, role_content, role_content))
 
+    def sort_by_key(self, key: str):
+        self.messages = sorted(self.messages, key=lambda x: getattr(x, key, f"No this {key}"))
+
     def clear(self, ):
         self.messages = []
 
     def delete(self, ):
         pass
 
     def get_messages(self, k=0) -> List[Message]:
@@ -132,15 +135,15 @@
         # return [parsed_output for message in self.messages for parsed_output in message.parsed_output_list[1:]]
         return [parsed_output for message in self.messages for parsed_output in message.parsed_output_list]
 
     def get_spec_parserd_output(self, ):
         return [message.spec_parsed_output for message in self.messages]
     
     def get_datetimes(self, ):
-        return [m.datetime for m in self.messages]
+        return [m.end_datetime for m in self.messages]
     
     def get_contents(self, ):
         return [m.role_content or m.input_query for m in self.messages]
     
     def get_rolenames(self, ):
         ''''''
         return [message.role_name for message in self.messages]
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/schema/message.py` & `codefuse_muagent-0.0.3/muagent/connector/schema/message.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from pydantic import BaseModel, root_validator
 from loguru import logger
-
+import uuid
 from muagent.utils.common_utils import getCurrentDatetime
 from .general_schema import *
 
 
 class Message(BaseModel):
-    chat_index: str = None
+    chat_index: str = "" # 会话ID，某一轮会话
+    message_index: str = "" # 会话消息ID，某轮会话里第几个会话记录
     user_name: str = "default"
     role_name: str
     role_type: str
-    role_prompt: str = None
-    input_query: str = None
-    # origin_query: str = None
-    datetime: str = getCurrentDatetime()
+    role_prompt: str = ""
+    input_query: str = ""
+    start_datetime: str = None
+    end_datetime: str = None
 
     # llm output
-    role_content: str = None
-    step_content: str = None
+    role_content: str = ""
+    step_content: str = ""
 
     # llm parsed information
-    plans: List[str] = None
-    code_content: str = None
-    code_filename: str = None
-    tool_params: str = None
-    tool_name: str = None
+    # code_content: str = None
+    # tool_params: str = None
+    # tool_name: str = None
     parsed_output: dict = {}
     spec_parsed_output: dict = {}
     parsed_output_list: List[Dict] = []
 
     # llm\tool\code executre information
     action_status: str = "default"
-    agent_index: int = None
-    code_answer: str = None
-    tool_answer: str = None
-    observation: str = None
+    # code_answer: str = None
+    # tool_answer: str = None
+    # observation: str = None
     figures: Dict[str, str] = {}
 
     # prompt support information
-    tools: List[BaseTool] = []
     task: Task = None
     db_docs: List['Doc'] = []
     code_docs: List['CodeDoc'] = []
     search_docs: List['Doc'] = []
-    agents: List = []
+    # user's customed kargs for init or end action
+    customed_kargs: dict = {}
 
     # phase input
+    agents: List = []
+    tools: List[BaseTool] = []
     phase_name: str = None
     chain_name: str = None
     do_search: bool = False
     doc_engine_name: str = None
     code_engine_name: str = None
     cb_search_type: str = None
     search_engine_name: str = None 
@@ -57,28 +57,58 @@
     use_nh: bool = True
     local_graph_path: str = ''
     score_threshold: float = 1.0
     do_doc_retrieval: bool = False
     do_code_retrieval: bool = False
     do_tool_retrieval: bool = False
     history_node_list: List[str] = []
-    # user's customed kargs for init or end action
-    customed_kargs: dict = {}
 
 
     @root_validator(pre=True)
     def check_card_number_omitted(cls, values):
         input_query = values.get("input_query")
         role_content = values.get("role_content")
         if input_query is None:
             values["input_query"] = role_content
         if role_content is None:
             values["role_content"] = input_query
         return values
     
+    @root_validator(pre=True)
+    def check_datetime(cls, values):
+        start_datetime = values.get("start_datetime")
+        end_datetime = values.get("end_datetime")
+        if start_datetime is None:
+            values["start_datetime"] = getCurrentDatetime()
+        if end_datetime is None:
+            values["end_datetime"] = getCurrentDatetime()
+        return values
+
+    @root_validator(pre=True)
+    def check_message_index(cls, values):
+        message_index = values.get("message_index")
+        chat_index = values.get("chat_index")
+        if message_index is None or message_index == "":
+            values["message_index"] = str(uuid.uuid4())
+
+        if chat_index is None or chat_index == "":
+            values["chat_index"] = str(uuid.uuid4())
+        return values
+    
+
+    def update_attribute(self, key: str, value):
+        if hasattr(self, key):
+            setattr(self, key, value)
+            self.end_datetime = getCurrentDatetime()
+        else:
+            raise AttributeError(f"{key} is not a valid property of {self.__class__.__name__}")
+
+    def get_attribute_type(self, key):
+        return type(getattr(self, key, None))
+
     # @root_validator(pre=True)
     # def check_card_number_omitted(cls, values):
     #     input_query = values.get("input_query")
     #     origin_query = values.get("origin_query")
     #     role_content = values.get("role_content")
     #     if input_query is None:
     #         values["input_query"] = origin_query or role_content
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codefuse-muagent-0.0.1/muagent/connector/utils.py` & `codefuse_muagent-0.0.3/muagent/connector/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/db_handler/graph_db_handler/nebula_handler.py` & `codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/nebula_handler.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/db_handler/vector_db_handler/chroma_handler.py` & `codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/chroma_handler.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/commands/default_vs_cds.py` & `codefuse_muagent-0.0.3/muagent/embeddings/commands/default_vs_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/faiss_m.py` & `codefuse_muagent-0.0.3/muagent/embeddings/faiss_m.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/get_embedding.py` & `codefuse_muagent-0.0.3/muagent/embeddings/get_embedding.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/huggingface_embedding.py` & `codefuse_muagent-0.0.3/muagent/embeddings/huggingface_embedding.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/in_memory.py` & `codefuse_muagent-0.0.3/muagent/embeddings/in_memory.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/openai_embedding.py` & `codefuse_muagent-0.0.3/muagent/embeddings/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/embeddings/utils.py` & `codefuse_muagent-0.0.3/muagent/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/llm_models/llm_config.py` & `codefuse_muagent-0.0.3/muagent/llm_models/llm_config.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/llm_models/openai_model.py` & `codefuse_muagent-0.0.3/muagent/llm_models/openai_model.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/__init__.py` & `codefuse_muagent-0.0.3/muagent/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/commands/code_base_cds.py` & `codefuse_muagent-0.0.3/muagent/orm/commands/code_base_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/commands/document_base_cds.py` & `codefuse_muagent-0.0.3/muagent/orm/commands/document_base_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/commands/document_file_cds.py` & `codefuse_muagent-0.0.3/muagent/orm/commands/document_file_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/db.py` & `codefuse_muagent-0.0.3/muagent/orm/db.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/schemas/base_schema.py` & `codefuse_muagent-0.0.3/muagent/orm/schemas/base_schema.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/orm/utils.py` & `codefuse_muagent-0.0.3/muagent/orm/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/retrieval/base_retrieval.py` & `codefuse_muagent-0.0.3/muagent/retrieval/base_retrieval.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/retrieval/document_loaders/json_loader.py` & `codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/retrieval/document_loaders/jsonl_loader.py` & `codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/jsonl_loader.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/retrieval/text_splitter/langchain_splitter.py` & `codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/langchain_splitter.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/sandbox/basebox.py` & `codefuse_muagent-0.0.3/muagent/sandbox/basebox.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/sandbox/pycodebox.py` & `codefuse_muagent-0.0.3/muagent/sandbox/pycodebox.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/service/base_service.py` & `codefuse_muagent-0.0.3/muagent/service/base_service.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/service/cb_api.py` & `codefuse_muagent-0.0.3/muagent/service/cb_api.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/service/faiss_db_service.py` & `codefuse_muagent-0.0.3/muagent/service/faiss_db_service.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/service/kb_api.py` & `codefuse_muagent-0.0.3/muagent/service/kb_api.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/service/migrate.py` & `codefuse_muagent-0.0.3/muagent/service/migrate.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/service/service_factory.py` & `codefuse_muagent-0.0.3/muagent/service/service_factory.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/__init__.py` & `codefuse_muagent-0.0.3/muagent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/abnormal_detection.py` & `codefuse_muagent-0.0.3/muagent/tools/abnormal_detection.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/base_tool.py` & `codefuse_muagent-0.0.3/muagent/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/cb_query_tool.py` & `codefuse_muagent-0.0.3/muagent/tools/cb_query_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/codechat_tools.py` & `codefuse_muagent-0.0.3/muagent/tools/codechat_tools.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/docs_retrieval.py` & `codefuse_muagent-0.0.3/muagent/tools/docs_retrieval.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/duckduckgo_search.py` & `codefuse_muagent-0.0.3/muagent/tools/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/metrics_query.py` & `codefuse_muagent-0.0.3/muagent/tools/metrics_query.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/multiplier.py` & `codefuse_muagent-0.0.3/muagent/tools/multiplier.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/ocr_tool.py` & `codefuse_muagent-0.0.3/muagent/tools/ocr_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/stock_tool.py` & `codefuse_muagent-0.0.3/muagent/tools/stock_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/tool_datas/stock_data.py` & `codefuse_muagent-0.0.3/muagent/tools/tool_datas/stock_data.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/weather.py` & `codefuse_muagent-0.0.3/muagent/tools/weather.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/tools/world_time.py` & `codefuse_muagent-0.0.3/muagent/tools/world_time.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/utils/code2doc_util.py` & `codefuse_muagent-0.0.3/muagent/utils/code2doc_util.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/utils/common_utils.py` & `codefuse_muagent-0.0.3/muagent/utils/common_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def timestampToDateformat(ts, interval=1000, dateformat=DATE_FORMAT):
     '''将标准时间戳转换标准指定时间格式'''
     return datetime.fromtimestamp(ts//interval).strftime(dateformat)
 
 
 def datefromatToTimestamp(dt, interval=1000, dateformat=DATE_FORMAT):
     '''将标准时间格式转换未标准时间戳'''
-    return datetime.strptime(dt, dateformat).timestamp()*interval
+    return int(datetime.strptime(dt, dateformat).timestamp()*interval)
 
 
 def func_timer():
     '''
     用装饰器实现函数计时
     :param function: 需要计时的函数
     :return: None
```

### Comparing `codefuse-muagent-0.0.1/muagent/utils/path_utils.py` & `codefuse_muagent-0.0.3/muagent/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/muagent/utils/server_utils.py` & `codefuse_muagent-0.0.3/muagent/utils/server_utils.py`

 * *Files identical despite different names*

### Comparing `codefuse-muagent-0.0.1/setup.py` & `codefuse_muagent-0.0.3/setup_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="codefuse-muagent",
-    version="0.0.1",
+    version="0.0.3",
     author="shanshi",
     author_email="wyp311395@antgroup.com",
     description="A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.",
     # long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/codefuse-ai/CodeFuse-muAgent",
     packages=setuptools.find_packages(),
@@ -30,11 +30,11 @@
         "psutil",
         "faiss-cpu",
         "notebook",
         # 
         "chromadb==0.4.17",
         "javalang==0.13.0",
         "nebula3-python==3.1.0",
-        # 
         "redis==5.0.1",
+        "pydantic<=1.10.14"
     ],
 )
```

### Comparing `codefuse-muagent-0.0.1/setup_test.py` & `codefuse_muagent-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
-    name="codefuse-muagent",
-    version="0.0.1",
+    name="muagent",
+    version="0.0.3",
     author="shanshi",
     author_email="wyp311395@antgroup.com",
     description="A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.",
     # long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/codefuse-ai/CodeFuse-muAgent",
     packages=setuptools.find_packages(),
@@ -30,11 +30,11 @@
         "psutil",
         "faiss-cpu",
         "notebook",
         # 
         "chromadb==0.4.17",
         "javalang==0.13.0",
         "nebula3-python==3.1.0",
-        # 
         "redis==5.0.1",
+        "pydantic<=1.10.14"
     ],
 )
```

### Comparing `codefuse-muagent-0.0.1/tests/test_config.py` & `codefuse_muagent-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

