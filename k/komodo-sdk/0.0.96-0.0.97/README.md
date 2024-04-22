# Comparing `tmp/komodo_sdk-0.0.96.tar.gz` & `tmp/komodo_sdk-0.0.97.tar.gz`

## Comparing `komodo_sdk-0.0.96.tar` & `komodo_sdk-0.0.97.tar`

### file list

```diff
@@ -1,264 +1,264 @@
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/.dockerignore
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/requirements.txt
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/.github/workflows/deploy-all.yml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/.github/workflows/publish-container.yml
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/.github/workflows/publish-private-pypi.yml
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/README.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/config.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/chatdoc_agent.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/collection_builder.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/coordinator_agent.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/default.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/difference_agent.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/echo_agent.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/elastic_agent.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/groot_agent.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/librarian_agent.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/mongo_agent.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/pdf_generator.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/sample_agent.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/summarizer_agent.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/translator_agent.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/agents/widget_builder_agent.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/sources/filesystem.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/sources/s3bucketkey.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/sources/webpages.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/sources/website_crawler.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_connect.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_count.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_get.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_search.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/files/collection_builder.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/files/collection_lister.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/files/collection_reader.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/files/directory_reader.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/files/file_reader.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/files/file_writer.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/markets/polygon_search.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_connect.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_databases.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_query.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_schema.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_unique.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/search/vector_search.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/search/vector_search_runtime.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/utils/agent_tool.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/utils/sample_tool.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/utils/thought_tool.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/utils/workflow_tool.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/web/data_fetcher.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/web/serpapi_search.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/web/tavily_search.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/tools/web/web_scraper.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/utils/agent_helper.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/utils/indexer.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/utils/play.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/utils/rag_context.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/vector_stores/pinecone_store.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/vector_stores/qdrant_store.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/vector_stores/vector_store_helper.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/core/workflows/sample_workflow.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/data/agents/planner/personal_finance_profile.yml
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/data/appliances/citibank/personal_finance_profile.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/data/appliances/komodo/dir1/hello.txt
--rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/data/workflows/analyzer/personal_finance_profile.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/checker/agent.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/checker/context.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/checker/dictionary.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/checker/instructions.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/agent.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/context.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/instructions.txt
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/role.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/tools/income_calculator.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/tools/income_contributions.yml
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/appliances/citibank/appliance.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/appliances/komodo/appliance.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/appliances/sample/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/appliances/sample/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/appliances/sample/instructions.txt
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/workflows/analyzer/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/workflows/analyzer/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/workflows/analyzer/instructions.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/definitions/workflows/analyzer/workflow.yml
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_agent.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_app.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_collection.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_config.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_context.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_datasource.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_features.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_locations.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_runnable.py
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_runtime.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_tool.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_tool_registry.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_user.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_vector.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_vectorstore.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/framework/komodo_workflow.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/database/agent_loader.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/database/appliance_loader.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/database/tool_loader.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/database/user_loader.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/filesystem/agent_loader.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/filesystem/appliance_loader.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/filesystem/loader_helper.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/filesystem/loader_locations.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/loaders/filesystem/workflow_loader.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/azure/azure.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/azure/azure_openai.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/bedrock/bedrock.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_claude.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_cohere.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_model.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_titan.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/agent_runner.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/appliance_utils.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/chat_message.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/chat_metadata.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/model_request.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/model_response.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/models.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/responder.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/workflow_executor.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/workflow_runner.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/framework/workflow_selector.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/openai/openai_api.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/openai/openai_api_streamed.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/openai/openai_api_streamed_tool_call.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/openai/openai_completion.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/openai/openai_debug.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/models/openai/openai_process_actions.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/collection.proto
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/data.proto
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/model.proto
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/report.proto
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/sample.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/collection_pb2.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/collection_pb2.pyi
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/data_pb2.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/data_pb2.pyi
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/model_pb2.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/model_pb2.pyi
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/report_pb2.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/proto/generated/report_pb2.pyi
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_agent_runner.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_agent_runner_2.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_difference_agent.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_librarian_agent.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_sample_agent.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_streaming_test.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/scripts/run_widget_builder.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/agent_router.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/appliance_router.py
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/ask_request.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/audio_router.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/collections_router.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/conversation_router.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/fast.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/globals.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/logo_router.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/report_router.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/server/user_router.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/directory/assistants_helpers.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/documents/file_writer_helper.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/documents/text_convert_helper.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/documents/text_extract.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/documents/text_extract_helper.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/documents/text_html.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/embeddings/faiss_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/embeddings/openai.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/embeddings/pinecone_store.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/mssql/mssql.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/api_query.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/digest.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/filestats.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/globber.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/hidden_prints.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/lambda_entry.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/lambda_utils.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/logconfig.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/pathutils.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/s3_file_utils.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/sentry_utils.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/switchdir.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/tags.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/term_colors.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/timebox.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/shared/utils/watcher.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/agent_store.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/appliance_store.py
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/collection_store.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/conversations_store.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/logo_store.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/proto_utils.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/redis_database.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/tool_store.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/store/user_store.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_elastic_agent.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_elastic_sample.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_elastic_tools.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_groot_agent.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_mongo_agent.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_mongo_sample.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_mongo_tools.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/core/test_serpapi_search.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/models/test_azure.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/models/test_bedrock.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/models/test_model_request.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/models/test_openai.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/models/test_workflow_runner.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/shared/test_mssql.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/komodo/tests/store/test_conversation_store.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/pdf2html/Dockerfile
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/pdf2html/docker-compose.yml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/pdf2html/server.py
--rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/pdf2html/data/sample.html
--rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/pdf2html/data/sample.pdf
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/Dockerfile
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/README.md
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/docker-compose.yml
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/docker-production.yml
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/appliance/appliance.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/appliance/config.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/appliance/seed.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/appliance/server.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/appliance/workflow.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/definitions/agents/dasher_v1/agent.yml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/definitions/agents/dasher_v1/instructions.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/definitions/agents/dasher_v2/agent.yml
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/definitions/agents/dasher_v2/instructions.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/app.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/globals.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/server.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/themes.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/assets/custom.css
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/agent.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/analytics.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/appliance.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/archive.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/charter.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/dasher_v1.py
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/dasher_v2.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/department.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/home.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/not_found_404.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/present.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/report.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/side_bar.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/topic_1.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/reports/bar_chart.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/reports/line_chart.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/sample/widgets/pages/reports/pie_chart.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/.gitignore
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/README.md
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/pyproject.toml
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 komodo_sdk-0.0.96/PKG-INFO
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/.dockerignore
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/requirements.txt
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/.github/workflows/deploy-all.yml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/.github/workflows/publish-container.yml
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/.github/workflows/publish-private-pypi.yml
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/README.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/config.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/chatdoc_agent.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/collection_builder.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/coordinator_agent.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/default.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/difference_agent.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/echo_agent.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/elastic_agent.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/groot_agent.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/librarian_agent.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/mongo_agent.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/pdf_generator.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/sample_agent.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/summarizer_agent.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/translator_agent.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/agents/widget_builder_agent.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/sources/filesystem.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/sources/s3bucketkey.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/sources/webpages.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/sources/website_crawler.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_connect.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_count.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_get.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_search.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/files/collection_builder.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/files/collection_lister.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/files/collection_reader.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/files/directory_reader.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/files/file_reader.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/files/file_writer.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/markets/polygon_search.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_connect.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_databases.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_query.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_schema.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_unique.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/search/vector_search.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/search/vector_search_runtime.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/utils/agent_tool.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/utils/sample_tool.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/utils/thought_tool.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/utils/workflow_tool.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/web/data_fetcher.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/web/serpapi_search.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/web/tavily_search.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/tools/web/web_scraper.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/utils/agent_helper.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/utils/indexer.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/utils/play.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/utils/rag_context.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/vector_stores/pinecone_store.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/vector_stores/qdrant_store.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/vector_stores/vector_store_helper.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/core/workflows/sample_workflow.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/data/agents/planner/personal_finance_profile.yml
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/data/appliances/citibank/personal_finance_profile.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/data/appliances/komodo/dir1/hello.txt
+-rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/data/workflows/analyzer/personal_finance_profile.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/checker/agent.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/checker/context.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/checker/dictionary.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/checker/instructions.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/agent.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/context.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/instructions.txt
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/role.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/tools/income_calculator.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/tools/income_contributions.yml
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/appliances/citibank/appliance.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/appliances/komodo/appliance.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/appliances/sample/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/appliances/sample/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/appliances/sample/instructions.txt
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/workflows/analyzer/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/workflows/analyzer/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/workflows/analyzer/instructions.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/definitions/workflows/analyzer/workflow.yml
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_agent.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_app.py
+-rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_collection.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_config.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_context.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_datasource.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_features.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_locations.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_runnable.py
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_runtime.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_tool.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_tool_registry.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_user.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_vector.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_vectorstore.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/framework/komodo_workflow.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/database/agent_loader.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/database/appliance_loader.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/database/tool_loader.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/database/user_loader.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/filesystem/agent_loader.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/filesystem/appliance_loader.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/filesystem/loader_helper.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/filesystem/loader_locations.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/loaders/filesystem/workflow_loader.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/azure/azure.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/azure/azure_openai.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/bedrock/bedrock.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_claude.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_cohere.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_model.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_titan.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/agent_runner.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/appliance_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/chat_message.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/chat_metadata.py
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/model_request.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/model_response.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/models.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/responder.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/workflow_executor.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/workflow_runner.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/framework/workflow_selector.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/openai/openai_api.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/openai/openai_api_streamed.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/openai/openai_api_streamed_tool_call.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/openai/openai_completion.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/openai/openai_debug.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/models/openai/openai_process_actions.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/collection.proto
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/data.proto
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/model.proto
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/report.proto
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/sample.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/collection_pb2.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/collection_pb2.pyi
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/data_pb2.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/data_pb2.pyi
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/model_pb2.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/model_pb2.pyi
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/report_pb2.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/proto/generated/report_pb2.pyi
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_agent_runner.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_agent_runner_2.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_difference_agent.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_librarian_agent.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_sample_agent.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_streaming_test.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/scripts/run_widget_builder.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/agent_router.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/appliance_router.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/ask_request.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/audio_router.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/collections_router.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/conversation_router.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/fast.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/globals.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/logo_router.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/report_router.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/server/user_router.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/directory/assistants_helpers.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/documents/file_writer_helper.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/documents/text_convert_helper.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/documents/text_extract.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/documents/text_extract_helper.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/documents/text_html.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/embeddings/faiss_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/embeddings/openai.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/embeddings/pinecone_store.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/mssql/mssql.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/api_query.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/digest.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/filestats.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/globber.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/hidden_prints.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/lambda_entry.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/lambda_utils.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/logconfig.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/pathutils.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/s3_file_utils.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/sentry_utils.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/switchdir.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/tags.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/term_colors.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/timebox.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/shared/utils/watcher.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/agent_store.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/appliance_store.py
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/collection_store.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/conversations_store.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/logo_store.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/proto_utils.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/redis_database.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/tool_store.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/store/user_store.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_elastic_agent.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_elastic_sample.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_elastic_tools.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_groot_agent.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_mongo_agent.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_mongo_sample.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_mongo_tools.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/core/test_serpapi_search.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/models/test_azure.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/models/test_bedrock.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/models/test_model_request.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/models/test_openai.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/models/test_workflow_runner.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/shared/test_mssql.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/komodo/tests/store/test_conversation_store.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/pdf2html/Dockerfile
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/pdf2html/docker-compose.yml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/pdf2html/server.py
+-rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/pdf2html/data/sample.html
+-rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/pdf2html/data/sample.pdf
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/Dockerfile
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/README.md
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/docker-compose.yml
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/docker-production.yml
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/appliance/appliance.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/appliance/config.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/appliance/seed.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/appliance/server.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/appliance/workflow.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/definitions/agents/dasher_v1/agent.yml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/definitions/agents/dasher_v1/instructions.txt
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/definitions/agents/dasher_v2/agent.yml
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/definitions/agents/dasher_v2/instructions.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/app.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/globals.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/server.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/themes.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/assets/custom.css
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/agent.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/analytics.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/appliance.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/archive.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/charter.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/dasher_v1.py
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/dasher_v2.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/department.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/home.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/not_found_404.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/present.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/report.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/side_bar.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/topic_1.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/reports/bar_chart.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/reports/line_chart.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/sample/widgets/pages/reports/pie_chart.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/.gitignore
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/README.md
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/pyproject.toml
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 komodo_sdk-0.0.97/PKG-INFO
```

### Comparing `komodo_sdk-0.0.96/.dockerignore` & `komodo_sdk-0.0.97/.dockerignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/requirements.txt` & `komodo_sdk-0.0.97/requirements.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/.github/workflows/publish-container.yml` & `komodo_sdk-0.0.97/.github/workflows/publish-container.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/.github/workflows/publish-private-pypi.yml` & `komodo_sdk-0.0.97/.github/workflows/publish-private-pypi.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/.github/workflows/publish-pypi.yml` & `komodo_sdk-0.0.97/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/README.md` & `komodo_sdk-0.0.97/komodo/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/config.py` & `komodo_sdk-0.0.97/komodo/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/chatdoc_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/chatdoc_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/collection_builder.py` & `komodo_sdk-0.0.97/komodo/core/agents/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/coordinator_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/coordinator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/default.py` & `komodo_sdk-0.0.97/komodo/core/agents/default.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/difference_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/elastic_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/groot_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/groot_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/librarian_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/mongo_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/mongo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/pdf_generator.py` & `komodo_sdk-0.0.97/komodo/core/agents/pdf_generator.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/sample_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/sample_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/summarizer_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/summarizer_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/translator_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/translator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/agents/widget_builder_agent.py` & `komodo_sdk-0.0.97/komodo/core/agents/widget_builder_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/sources/filesystem.py` & `komodo_sdk-0.0.97/komodo/core/sources/filesystem.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/sources/s3bucketkey.py` & `komodo_sdk-0.0.97/komodo/core/sources/s3bucketkey.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/sources/webpages.py` & `komodo_sdk-0.0.97/komodo/core/sources/webpages.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/sources/website_crawler.py` & `komodo_sdk-0.0.97/komodo/core/sources/website_crawler.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_count.py` & `komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_count.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_get.py` & `komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_get.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/elastic/elastic_search.py` & `komodo_sdk-0.0.97/komodo/core/tools/elastic/elastic_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/files/collection_builder.py` & `komodo_sdk-0.0.97/komodo/core/tools/files/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/files/collection_lister.py` & `komodo_sdk-0.0.97/komodo/core/tools/files/collection_lister.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/files/collection_reader.py` & `komodo_sdk-0.0.97/komodo/core/tools/files/collection_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/files/directory_reader.py` & `komodo_sdk-0.0.97/komodo/core/tools/files/directory_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,18 +38,18 @@
         shortcode = self.shortcode
         super().__init__(shortcode=shortcode,
                          name=self.name,
                          definition=self.definition(shortcode),
                          action=self.action)
 
     def action(self, args, runtime=None):
-        try:
-            pattern = args.get("pattern", "*")
-            path = args.get("folder")
+        pattern = args.get("pattern", "*")
+        path = args.get("folder")
 
+        try:
             if not path and runtime:
                 path = str(runtime.get_working_directory())
 
             if not path:
                 return "Please provide a folder path."
 
             files = self.get_files_recursively_pathlib(path, pattern)
```

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/files/file_reader.py` & `komodo_sdk-0.0.97/komodo/core/tools/files/file_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,33 +42,21 @@
                          name=self.name,
                          definition=self.definition(shortcode),
                          action=self.action)
 
     def action(self, args, runtime: KomodoRuntime):
         folder = args.get('folder', None)
         filename = args.get("filename", None)
-        collection = runtime.selected_collection or runtime.home_folder
-        path = None
 
         if folder is None or filename is None:
             return "Please provide folder and filename."
 
-        folder = Path(folder)
-        if not folder.exists():
-            return f"Could not find folder: {str(folder)}"
-
-        filename = Path(filename).name
-
-        if folder.is_absolute():
-            path = Path(folder) / filename
-        elif folder.name == collection.path.name:
-            path = collection.path / filename
-
+        path = runtime.resolve_file(folder, filename)
         if not path or not path.exists():
-            return f"Could not find folder or filename. folder: {str(folder)}, filename: {str(filename)}"
+            return f"Could not find folder or filename. folder: {folder}, filename: {filename}"
 
         try:
             page = args.get("page", 1)
             page_size = min(args.get("page_size", 2000), 100000)
             raw = args.get("raw", False)
 
             if not raw:
```

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/files/file_writer.py` & `komodo_sdk-0.0.97/komodo/core/tools/files/file_writer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/markets/polygon_search.py` & `komodo_sdk-0.0.97/komodo/core/tools/markets/polygon_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_databases.py` & `komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_databases.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_query.py` & `komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_schema.py` & `komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_schema.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/mongo/mongo_unique.py` & `komodo_sdk-0.0.97/komodo/core/tools/mongo/mongo_unique.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/search/vector_search.py` & `komodo_sdk-0.0.97/komodo/core/tools/search/vector_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/search/vector_search_runtime.py` & `komodo_sdk-0.0.97/komodo/core/tools/search/vector_search_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                          action=self.action)
 
     def action(self, args, runtime: KomodoRuntime = None):
         # prepare the index for searching
         recache = args.get('recache', False)
         reindex = args.get('reindex', False)
 
-        collection = runtime.selected_collection or runtime.home_folder
+        collection = runtime.get_working_collection()
         rag_context = RagContext(collection.path, cache_path=runtime.config.cache(), recache=recache)
         indexer = Indexer(rag_context)
         indexer.run(reindex=reindex)
 
         # do the search
         text = args.get('query')
         if not text:
```

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/utils/agent_tool.py` & `komodo_sdk-0.0.97/komodo/core/tools/utils/agent_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/utils/sample_tool.py` & `komodo_sdk-0.0.97/komodo/core/tools/utils/sample_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/utils/thought_tool.py` & `komodo_sdk-0.0.97/komodo/core/tools/utils/thought_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/utils/workflow_tool.py` & `komodo_sdk-0.0.97/komodo/core/tools/utils/workflow_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/web/data_fetcher.py` & `komodo_sdk-0.0.97/komodo/core/tools/web/data_fetcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/web/serpapi_search.py` & `komodo_sdk-0.0.97/komodo/core/tools/web/serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/web/tavily_search.py` & `komodo_sdk-0.0.97/komodo/core/tools/web/tavily_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/tools/web/web_scraper.py` & `komodo_sdk-0.0.97/komodo/core/tools/web/web_scraper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/utils/agent_helper.py` & `komodo_sdk-0.0.97/komodo/core/utils/agent_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/utils/indexer.py` & `komodo_sdk-0.0.97/komodo/core/utils/indexer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/utils/play.py` & `komodo_sdk-0.0.97/komodo/core/utils/play.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/utils/rag_context.py` & `komodo_sdk-0.0.97/komodo/core/utils/rag_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/vector_stores/pinecone_store.py` & `komodo_sdk-0.0.97/komodo/core/vector_stores/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/vector_stores/qdrant_store.py` & `komodo_sdk-0.0.97/komodo/core/vector_stores/qdrant_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/vector_stores/vector_store_helper.py` & `komodo_sdk-0.0.97/komodo/core/vector_stores/vector_store_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/core/workflows/sample_workflow.py` & `komodo_sdk-0.0.97/komodo/core/workflows/sample_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/data/agents/planner/personal_finance_profile.yml` & `komodo_sdk-0.0.97/komodo/data/agents/planner/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/data/appliances/citibank/personal_finance_profile.yml` & `komodo_sdk-0.0.97/komodo/data/appliances/citibank/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf` & `komodo_sdk-0.0.97/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/data/workflows/analyzer/personal_finance_profile.yml` & `komodo_sdk-0.0.97/komodo/data/workflows/analyzer/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/definitions/agents/planner/context.yml` & `komodo_sdk-0.0.97/komodo/definitions/agents/planner/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/definitions/agents/planner/role.yml` & `komodo_sdk-0.0.97/komodo/definitions/agents/planner/role.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml` & `komodo_sdk-0.0.97/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/definitions/appliances/sample/context.yml` & `komodo_sdk-0.0.97/komodo/definitions/appliances/sample/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/definitions/workflows/analyzer/context.yml` & `komodo_sdk-0.0.97/komodo/definitions/workflows/analyzer/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_agent.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         self.context = kwargs.get("context", KomodoContext())
         self.role = kwargs.get("role")
         self.data = kwargs.get("data", {})
         self.dictionary = kwargs.get("dictionary", {})
         self.folders = kwargs.get("folders", [])
 
         self.autoload_collection = kwargs.get("autoload_collection", True)
-        self.max_files_per_request = kwargs.get("max_files_per_request", 10)
-        self.max_tokens_per_file = kwargs.get("max_tokens_per_file", 4096)
-        self.max_total_tokens = kwargs.get("max_total_tokens", 4096 * 10)
+        self.max_files_per_request = kwargs.get("max_files_per_request", 5)
+        self.max_tokens_per_file = kwargs.get("max_tokens_per_file", 1024)
+        self.max_total_tokens = kwargs.get("max_total_tokens", 1024 * 5)
 
         self.kwargs = kwargs
 
     def __str__(self):
         return f"KomodoAgent: {self.name} ({self.shortcode}), {self.purpose}"
 
     def __hash__(self) -> int:
```

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_app.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_app.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_collection.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_collection.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_config.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_context.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_datasource.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_datasource.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_locations.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_runnable.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_runnable.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_runtime.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import copy
 from pathlib import Path
 
+from werkzeug.utils import secure_filename
+
 from komodo.framework.komodo_agent import KomodoAgent
 from komodo.framework.komodo_app import KomodoApp
 from komodo.framework.komodo_collection import KomodoCollection
 from komodo.framework.komodo_config import KomodoConfig
 from komodo.framework.komodo_user import KomodoUser
 from komodo.framework.komodo_workflow import KomodoWorkflow
 
@@ -87,17 +89,33 @@
             self.get_shared_collections()) + list(self.get_user_collections())
 
     def get_collection(self, shortcode):
         for collection in self.get_available_collections():
             if collection.shortcode == shortcode:
                 return collection
 
-    def get_working_directory(self):
-        collection = self.selected_collection or self.home_folder
-        return collection.path
+
+    def get_working_collection(self):
+        return self.selected_collection or self.home_folder
+
+
+    def get_working_directory(self) -> Path:
+        return self.get_working_collection().path
+
+    def resolve_folder(self, folder) ->  Path:
+        cwd = self.get_working_directory()
+        if folder is None or folder == "." or folder == cwd.name:
+            return cwd
+
+        name = secure_filename(Path(folder).name)
+        return Path(cwd) / name
+
+    def resolve_file(self, folder, filename) -> Path:
+        folder = self.resolve_folder(folder)
+        return folder / secure_filename(Path(filename).name)
 
     def __str__(self):
         template = "From: {} To: {} Name: {} (provider: {}, model: {})"
         return template.format(self.user.email if self.user else "Anon",
                                self.agent.email,
                                self.agent.name,
                                self.agent.provider,
```

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_tool.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_tool_registry.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_tool_registry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_user.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_user.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_vector.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_vector.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_vectorstore.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_vectorstore.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/framework/komodo_workflow.py` & `komodo_sdk-0.0.97/komodo/framework/komodo_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/database/agent_loader.py` & `komodo_sdk-0.0.97/komodo/loaders/database/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/database/appliance_loader.py` & `komodo_sdk-0.0.97/komodo/loaders/database/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/database/user_loader.py` & `komodo_sdk-0.0.97/komodo/loaders/database/user_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/filesystem/agent_loader.py` & `komodo_sdk-0.0.97/komodo/loaders/filesystem/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/filesystem/appliance_loader.py` & `komodo_sdk-0.0.97/komodo/loaders/filesystem/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/filesystem/loader_helper.py` & `komodo_sdk-0.0.97/komodo/loaders/filesystem/loader_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/filesystem/loader_locations.py` & `komodo_sdk-0.0.97/komodo/loaders/filesystem/loader_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/loaders/filesystem/workflow_loader.py` & `komodo_sdk-0.0.97/komodo/loaders/filesystem/workflow_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/azure/azure.py` & `komodo_sdk-0.0.97/komodo/models/azure/azure.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/azure/azure_openai.py` & `komodo_sdk-0.0.97/komodo/models/azure/azure_openai.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/bedrock/bedrock.py` & `komodo_sdk-0.0.97/komodo/models/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_claude.py` & `komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_claude.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_cohere.py` & `komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_cohere.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_model.py` & `komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_model.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/bedrock/bedrock_titan.py` & `komodo_sdk-0.0.97/komodo/models/bedrock/bedrock_titan.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/agent_runner.py` & `komodo_sdk-0.0.97/komodo/models/framework/agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/appliance_utils.py` & `komodo_sdk-0.0.97/komodo/models/framework/appliance_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/chat_message.py` & `komodo_sdk-0.0.97/komodo/models/framework/chat_message.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/model_request.py` & `komodo_sdk-0.0.97/komodo/models/framework/model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         conversation.append("Prompt: " + self.prompt)
         return "\n".join(conversation)
 
     def prepare_messages(self):
         agent = self.runtime.agent
         messages = self.prepare_agent_messages(agent)
 
-        if collection := self.runtime.selected_collection:
+        if collection := self.runtime.get_working_collection():
             if agent.autoload_collection:
                 messages += self.prepare_file_messages(agent, collection)
 
         workflow_context = self.kwargs.get('workflow_context', KomodoContext())
         workflow_messages = ChatMessage.convert_from_context(workflow_context)
         messages += [m.add_tag('Workflow') for m in workflow_messages]
```

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/model_response.py` & `komodo_sdk-0.0.97/komodo/models/framework/model_response.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/responder.py` & `komodo_sdk-0.0.97/komodo/models/framework/responder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/workflow_executor.py` & `komodo_sdk-0.0.97/komodo/models/framework/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/framework/workflow_runner.py` & `komodo_sdk-0.0.97/komodo/models/framework/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/openai/openai_api.py` & `komodo_sdk-0.0.97/komodo/models/openai/openai_api.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/openai/openai_api_streamed.py` & `komodo_sdk-0.0.97/komodo/models/openai/openai_api_streamed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/openai/openai_api_streamed_tool_call.py` & `komodo_sdk-0.0.97/komodo/models/openai/openai_api_streamed_tool_call.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/openai/openai_debug.py` & `komodo_sdk-0.0.97/komodo/models/openai/openai_debug.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/models/openai/openai_process_actions.py` & `komodo_sdk-0.0.97/komodo/models/openai/openai_process_actions.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/collection.proto` & `komodo_sdk-0.0.97/komodo/proto/collection.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/data.proto` & `komodo_sdk-0.0.97/komodo/proto/data.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/model.proto` & `komodo_sdk-0.0.97/komodo/proto/model.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/report.proto` & `komodo_sdk-0.0.97/komodo/proto/report.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/sample.py` & `komodo_sdk-0.0.97/komodo/proto/sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/collection_pb2.py` & `komodo_sdk-0.0.97/komodo/proto/generated/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/collection_pb2.pyi` & `komodo_sdk-0.0.97/komodo/proto/generated/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/data_pb2.py` & `komodo_sdk-0.0.97/komodo/proto/generated/data_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/data_pb2.pyi` & `komodo_sdk-0.0.97/komodo/proto/generated/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/model_pb2.py` & `komodo_sdk-0.0.97/komodo/proto/generated/model_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/model_pb2.pyi` & `komodo_sdk-0.0.97/komodo/proto/generated/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/report_pb2.py` & `komodo_sdk-0.0.97/komodo/proto/generated/report_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/proto/generated/report_pb2.pyi` & `komodo_sdk-0.0.97/komodo/proto/generated/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/scripts/run_agent_runner.py` & `komodo_sdk-0.0.97/komodo/scripts/run_agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/scripts/run_agent_runner_2.py` & `komodo_sdk-0.0.97/komodo/scripts/run_agent_runner_2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/scripts/run_difference_agent.py` & `komodo_sdk-0.0.97/komodo/scripts/run_difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/scripts/run_librarian_agent.py` & `komodo_sdk-0.0.97/komodo/scripts/run_librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/scripts/run_streaming_test.py` & `komodo_sdk-0.0.97/komodo/scripts/run_streaming_test.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/scripts/run_widget_builder.py` & `komodo_sdk-0.0.97/komodo/scripts/run_widget_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/agent_router.py` & `komodo_sdk-0.0.97/komodo/server/agent_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/appliance_router.py` & `komodo_sdk-0.0.97/komodo/server/appliance_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/ask_request.py` & `komodo_sdk-0.0.97/komodo/server/ask_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/audio_router.py` & `komodo_sdk-0.0.97/komodo/server/audio_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/collections_router.py` & `komodo_sdk-0.0.97/komodo/server/collections_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/conversation_router.py` & `komodo_sdk-0.0.97/komodo/server/conversation_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/fast.py` & `komodo_sdk-0.0.97/komodo/server/fast.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/globals.py` & `komodo_sdk-0.0.97/komodo/server/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/logo_router.py` & `komodo_sdk-0.0.97/komodo/server/logo_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/report_router.py` & `komodo_sdk-0.0.97/komodo/server/report_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/server/user_router.py` & `komodo_sdk-0.0.97/komodo/server/user_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/directory/assistants_helpers.py` & `komodo_sdk-0.0.97/komodo/shared/directory/assistants_helpers.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/documents/file_writer_helper.py` & `komodo_sdk-0.0.97/komodo/shared/documents/file_writer_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/documents/text_convert_helper.py` & `komodo_sdk-0.0.97/komodo/shared/documents/text_convert_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/documents/text_extract.py` & `komodo_sdk-0.0.97/komodo/shared/documents/text_extract.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/documents/text_extract_helper.py` & `komodo_sdk-0.0.97/komodo/shared/documents/text_extract_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/documents/text_html.py` & `komodo_sdk-0.0.97/komodo/shared/documents/text_html.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/embeddings/faiss_store.py` & `komodo_sdk-0.0.97/komodo/shared/embeddings/faiss_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/embeddings/pinecone_store.py` & `komodo_sdk-0.0.97/komodo/shared/embeddings/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/mssql/mssql.py` & `komodo_sdk-0.0.97/komodo/shared/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/api_query.py` & `komodo_sdk-0.0.97/komodo/shared/utils/api_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/digest.py` & `komodo_sdk-0.0.97/komodo/shared/utils/digest.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/filestats.py` & `komodo_sdk-0.0.97/komodo/shared/utils/filestats.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/globber.py` & `komodo_sdk-0.0.97/komodo/shared/utils/globber.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/lambda_entry.py` & `komodo_sdk-0.0.97/komodo/shared/utils/lambda_entry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/lambda_utils.py` & `komodo_sdk-0.0.97/komodo/shared/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/logconfig.py` & `komodo_sdk-0.0.97/komodo/shared/utils/logconfig.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/s3_file_utils.py` & `komodo_sdk-0.0.97/komodo/shared/utils/s3_file_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/tags.py` & `komodo_sdk-0.0.97/komodo/shared/utils/tags.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/term_colors.py` & `komodo_sdk-0.0.97/komodo/shared/utils/term_colors.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/timebox.py` & `komodo_sdk-0.0.97/komodo/shared/utils/timebox.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/shared/utils/watcher.py` & `komodo_sdk-0.0.97/komodo/shared/utils/watcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/agent_store.py` & `komodo_sdk-0.0.97/komodo/store/agent_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/appliance_store.py` & `komodo_sdk-0.0.97/komodo/store/appliance_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/collection_store.py` & `komodo_sdk-0.0.97/komodo/store/collection_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/conversations_store.py` & `komodo_sdk-0.0.97/komodo/store/conversations_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/logo_store.py` & `komodo_sdk-0.0.97/komodo/store/logo_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/redis_database.py` & `komodo_sdk-0.0.97/komodo/store/redis_database.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/tool_store.py` & `komodo_sdk-0.0.97/komodo/store/tool_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/store/user_store.py` & `komodo_sdk-0.0.97/komodo/store/user_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/core/test_elastic_agent.py` & `komodo_sdk-0.0.97/komodo/tests/core/test_elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/core/test_elastic_sample.py` & `komodo_sdk-0.0.97/komodo/tests/core/test_elastic_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/core/test_elastic_tools.py` & `komodo_sdk-0.0.97/komodo/tests/core/test_elastic_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/core/test_mongo_sample.py` & `komodo_sdk-0.0.97/komodo/tests/core/test_mongo_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/core/test_mongo_tools.py` & `komodo_sdk-0.0.97/komodo/tests/core/test_mongo_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/core/test_serpapi_search.py` & `komodo_sdk-0.0.97/komodo/tests/core/test_serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/models/test_bedrock.py` & `komodo_sdk-0.0.97/komodo/tests/models/test_bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/models/test_model_request.py` & `komodo_sdk-0.0.97/komodo/tests/models/test_model_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/models/test_workflow_runner.py` & `komodo_sdk-0.0.97/komodo/tests/models/test_workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/shared/test_mssql.py` & `komodo_sdk-0.0.97/komodo/tests/shared/test_mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/komodo/tests/store/test_conversation_store.py` & `komodo_sdk-0.0.97/komodo/tests/store/test_conversation_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/pdf2html/Dockerfile` & `komodo_sdk-0.0.97/pdf2html/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/pdf2html/server.py` & `komodo_sdk-0.0.97/pdf2html/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/pdf2html/data/sample.html` & `komodo_sdk-0.0.97/pdf2html/data/sample.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/pdf2html/data/sample.pdf` & `komodo_sdk-0.0.97/pdf2html/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/Dockerfile` & `komodo_sdk-0.0.97/sample/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/docker-compose.yml` & `komodo_sdk-0.0.97/sample/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/docker-production.yml` & `komodo_sdk-0.0.97/sample/docker-production.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/appliance/appliance.py` & `komodo_sdk-0.0.97/sample/appliance/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/appliance/config.py` & `komodo_sdk-0.0.97/sample/appliance/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/appliance/seed.py` & `komodo_sdk-0.0.97/sample/appliance/seed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/appliance/server.py` & `komodo_sdk-0.0.97/sample/appliance/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/appliance/workflow.py` & `komodo_sdk-0.0.97/sample/appliance/workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/definitions/agents/dasher_v1/instructions.txt` & `komodo_sdk-0.0.97/sample/definitions/agents/dasher_v1/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/definitions/agents/dasher_v2/instructions.txt` & `komodo_sdk-0.0.97/sample/definitions/agents/dasher_v2/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/app.py` & `komodo_sdk-0.0.97/sample/widgets/app.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/globals.py` & `komodo_sdk-0.0.97/sample/widgets/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/themes.py` & `komodo_sdk-0.0.97/sample/widgets/themes.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/assets/custom.css` & `komodo_sdk-0.0.97/sample/widgets/assets/custom.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/agent.py` & `komodo_sdk-0.0.97/sample/widgets/pages/agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/analytics.py` & `komodo_sdk-0.0.97/sample/widgets/pages/analytics.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/appliance.py` & `komodo_sdk-0.0.97/sample/widgets/pages/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/charter.py` & `komodo_sdk-0.0.97/sample/widgets/pages/charter.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/dasher_v1.py` & `komodo_sdk-0.0.97/sample/widgets/pages/dasher_v1.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/dasher_v2.py` & `komodo_sdk-0.0.97/sample/widgets/pages/dasher_v2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/department.py` & `komodo_sdk-0.0.97/sample/widgets/pages/department.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/present.py` & `komodo_sdk-0.0.97/sample/widgets/pages/present.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/report.py` & `komodo_sdk-0.0.97/sample/widgets/pages/report.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/side_bar.py` & `komodo_sdk-0.0.97/sample/widgets/pages/side_bar.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/reports/bar_chart.py` & `komodo_sdk-0.0.97/sample/widgets/pages/reports/bar_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/reports/line_chart.py` & `komodo_sdk-0.0.97/sample/widgets/pages/reports/line_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/sample/widgets/pages/reports/pie_chart.py` & `komodo_sdk-0.0.97/sample/widgets/pages/reports/pie_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/.gitignore` & `komodo_sdk-0.0.97/.gitignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.96/pyproject.toml` & `komodo_sdk-0.0.97/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "komodo-sdk"
-version = "0.0.96"
+version = "0.0.97"
 authors = [
     { name = "Ryan Oberoi", email = "ryan.oberoi@komodoapp.ai" },
 ]
 description = "Komodo SDK"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `komodo_sdk-0.0.96/PKG-INFO` & `komodo_sdk-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: komodo-sdk
-Version: 0.0.96
+Version: 0.0.97
 Summary: Komodo SDK
 Project-URL: Homepage, https://github.com/Komodo-AI/komodo-sdk.git
 Author-email: Ryan Oberoi <ryan.oberoi@komodoapp.ai>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: aiofiles~=23.2.1
```

