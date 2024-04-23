# Comparing `tmp/openagi-0.1.0b3.tar.gz` & `tmp/openagi-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagi-0.1.0b3.tar", max compression
+gzip compressed data, was "openagi-0.1.0b4.tar", max compression
```

## Comparing `openagi-0.1.0b3.tar` & `openagi-0.1.0b4.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     4094 2024-04-05 05:20:15.733992 openagi-0.1.0b3/README.md
--rw-r--r--   0        0        0     1053 2024-04-05 05:21:37.778721 openagi-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     1499 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/Readme.md
--rw-r--r--   0        0        0      667 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/__init__.py
--rw-r--r--   0        0        0    14360 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/agent.py
--rw-r--r--   0        0        0     3398 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/init_agent.py
--rw-r--r--   0        0        0      196 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/__init__.py
--rw-r--r--   0        0        0     2720 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/azure.py
--rw-r--r--   0        0        0     1351 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/base.py
--rw-r--r--   0        0        0      713 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/openagi_main.py
--rw-r--r--   0        0        0     1619 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/openai.py
--rw-r--r--   0        0        0     3782 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/queue/message_broker.py
--rw-r--r--   0        0        0     2750 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/queue/pq.py
--rw-r--r--   0        0        0     6433 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/queue/timer_pool.py
--rw-r--r--   0        0        0       28 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/__init__.py
--rw-r--r--   0        0        0     1979 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/base.py
--rw-r--r--   0        0        0      762 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/custom_tools/ProxyTool.py
--rw-r--r--   0        0        0      212 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/custom_tools/custom_tool_db.py
--rw-r--r--   0        0        0     1292 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/__init__.py
--rw-r--r--   0        0        0      581 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/dalle_image_generator.py
--rw-r--r--   0        0        0     2753 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/document_compare.py
--rw-r--r--   0        0        0     1047 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/duckducksearch.py
--rw-r--r--   0        0        0     1527 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/exa_search_tool.py
--rw-r--r--   0        0        0     1745 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/github.py
--rw-r--r--   0        0        0     1595 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/gmail.py
--rw-r--r--   0        0        0      270 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/google.py
--rw-r--r--   0        0        0     1433 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/google_finance_search.py
--rw-r--r--   0        0        0     1357 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/google_serper_specific.py
--rw-r--r--   0        0        0     1160 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/googlejobsearch.py
--rw-r--r--   0        0        0      841 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/googleserpersearch.py
--rw-r--r--   0        0        0     1350 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/nasa.py
--rw-r--r--   0        0        0      844 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/open_weathermap.py
--rw-r--r--   0        0        0     1743 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/polygon.py
--rw-r--r--   0        0        0     1444 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/serper_intermediate.py
--rw-r--r--   0        0        0     1357 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/sql.py
--rw-r--r--   0        0        0     1141 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/wikipedia_tool.py
--rw-r--r--   0        0        0     1256 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/xorbits.py
--rw-r--r--   0        0        0     1315 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/yahoofinancenews.py
--rw-r--r--   0        0        0      945 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/youtubesearch.py
--rw-r--r--   0        0        0     3198 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/tools_db.py
--rw-r--r--   0        0        0     3255 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/utils.py
--rw-r--r--   0        0        0      593 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/utils/extraction.py
--rw-r--r--   0        0        0    13792 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/utils/llmTasks.py
--rw-r--r--   0        0        0      730 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/utils/yamlParse.py
--rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 openagi-0.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0     6486 2024-04-23 06:32:39.825436 openagi-0.1.0b4/README.md
+-rw-r--r--   0        0        0     1159 2024-04-23 06:34:12.487295 openagi-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0     1499 2024-04-19 10:30:02.396089 openagi-0.1.0b4/src/Readme.md
+-rw-r--r--   0        0        0      667 2024-04-19 10:30:02.396089 openagi-0.1.0b4/src/openagi/__init__.py
+-rw-r--r--   0        0        0    14362 2024-04-19 11:33:11.880047 openagi-0.1.0b4/src/openagi/agent.py
+-rw-r--r--   0        0        0     3398 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/init_agent.py
+-rw-r--r--   0        0        0      196 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/llms/__init__.py
+-rw-r--r--   0        0        0     2722 2024-04-23 06:32:39.889436 openagi-0.1.0b4/src/openagi/llms/azure.py
+-rw-r--r--   0        0        0     1352 2024-04-23 06:32:39.890436 openagi-0.1.0b4/src/openagi/llms/base.py
+-rw-r--r--   0        0        0     1615 2024-04-23 06:32:39.891436 openagi-0.1.0b4/src/openagi/llms/hf.py
+-rw-r--r--   0        0        0      715 2024-04-23 06:32:39.893436 openagi-0.1.0b4/src/openagi/llms/openagi_main.py
+-rw-r--r--   0        0        0     1620 2024-04-23 06:32:39.894436 openagi-0.1.0b4/src/openagi/llms/openai.py
+-rw-r--r--   0        0        0     3782 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/queue/message_broker.py
+-rw-r--r--   0        0        0     2750 2024-04-23 06:32:39.895436 openagi-0.1.0b4/src/openagi/queue/pq.py
+-rw-r--r--   0        0        0     6433 2024-04-19 10:30:02.397089 openagi-0.1.0b4/src/openagi/queue/timer_pool.py
+-rw-r--r--   0        0        0       28 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-23 06:32:39.897436 openagi-0.1.0b4/src/openagi/tools/base.py
+-rw-r--r--   0        0        0      762 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/custom_tools/ProxyTool.py
+-rw-r--r--   0        0        0      212 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/custom_tools/custom_tool_db.py
+-rw-r--r--   0        0        0     1292 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/integrations/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-19 10:30:02.398089 openagi-0.1.0b4/src/openagi/tools/integrations/dalle_image_generator.py
+-rw-r--r--   0        0        0     2824 2024-04-23 06:32:39.898436 openagi-0.1.0b4/src/openagi/tools/integrations/document_compare.py
+-rw-r--r--   0        0        0     1045 2024-04-23 06:32:39.899436 openagi-0.1.0b4/src/openagi/tools/integrations/duckducksearch.py
+-rw-r--r--   0        0        0     1527 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/exa_search_tool.py
+-rw-r--r--   0        0        0     1745 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/github.py
+-rw-r--r--   0        0        0     1595 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/gmail.py
+-rw-r--r--   0        0        0      270 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/google.py
+-rw-r--r--   0        0        0     1433 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/google_finance_search.py
+-rw-r--r--   0        0        0     1357 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/google_serper_specific.py
+-rw-r--r--   0        0        0     1160 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/googlejobsearch.py
+-rw-r--r--   0        0        0      841 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/googleserpersearch.py
+-rw-r--r--   0        0        0     1350 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/nasa.py
+-rw-r--r--   0        0        0      844 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/open_weathermap.py
+-rw-r--r--   0        0        0     1743 2024-04-19 10:30:02.399089 openagi-0.1.0b4/src/openagi/tools/integrations/polygon.py
+-rw-r--r--   0        0        0     1444 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/serper_intermediate.py
+-rw-r--r--   0        0        0     1357 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/sql.py
+-rw-r--r--   0        0        0     1141 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/wikipedia_tool.py
+-rw-r--r--   0        0        0     1248 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/xorbits.py
+-rw-r--r--   0        0        0     1315 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/yahoofinancenews.py
+-rw-r--r--   0        0        0      945 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/integrations/youtubesearch.py
+-rw-r--r--   0        0        0     3198 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/tools_db.py
+-rw-r--r--   0        0        0     3255 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/tools/utils.py
+-rw-r--r--   0        0        0      593 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/utils/extraction.py
+-rw-r--r--   0        0        0    13792 2024-04-19 10:30:02.400089 openagi-0.1.0b4/src/openagi/utils/llmTasks.py
+-rw-r--r--   0        0        0      730 2024-04-19 10:30:02.401089 openagi-0.1.0b4/src/openagi/utils/yamlParse.py
+-rw-r--r--   0        0        0     8183 1970-01-01 00:00:00.000000 openagi-0.1.0b4/PKG-INFO
```

### Comparing `openagi-0.1.0b3/pyproject.toml` & `openagi-0.1.0b4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openagi"
-version = "0.1.0-b3"
+version = "0.1.0-b4"
 description = ""
 authors = ["AI Planet <tech@aiplanet.com>"]
 readme = "README.md"
 include = ["src/*"]
 
 [tool.poetry.dependencies]
-python = "~3.11"
+python = "^3.9, <3.12"
 langchain = "0.1.8"
 langchain-community = "0.0.21"
 langchain-openai = "0.0.6"
-duckduckgo-search = "5.2.1"
+duckduckgo-search = "^5.3.0"
 spacy = "3.7.4"
 xorbits = "^0.7.2"
 azure-identity = "^1.15.0"
 langchain-text-splitters = "^0.0.1"
 python-dotenv = "^1.0.1"
 langchain-experimental = "^0.0.53"
 spacytextblob = "^4.0.0"
@@ -28,14 +28,19 @@
 yfinance = "^0.2.37"
 google-search-results = "^2.4.2"
 fastapi = "^0.110.0"
 uvicorn = "^0.29.0"
 pygithub = "^2.3.0"
 langchainhub = "^0.1.15"
 python-multipart = "^0.0.9"
+pandas = "^2.2.2"
+numpy = "^1.26.4"
+transformers = "^4.40.0"
+pypdf = "^4.2.0"
+faiss-cpu = "^1.8.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openagi-0.1.0b3/src/Readme.md` & `openagi-0.1.0b4/src/Readme.md`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/__init__.py` & `openagi-0.1.0b4/src/openagi/__init__.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/agent.py` & `openagi-0.1.0b4/src/openagi/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
     mapper = NameIndexMapper()
     mapper.add_mapping(agent_list[0])
     mapper.add_mapping(agent_list[1])
     mapper.add_mapping(agent_list[2])
     agent1 = Agent(agentName=agent_list[0], consumerAgent=agent_list[1])
     agent2 = Agent(agentName=agent_list[1], consumerAgent=agent_list[2])
     agent3 = Agent(agentName=agent_list[2], consumerAgent=agent_list[0])
-    # , role="RESEARCHER", goal="search for latest trends in Carona treatment", capability="INTERNET_SEARCHER", agent_type="STATIC",
+    # , role="RESEARCHER", goal="search for latest trends in COVID-19 treatment", capability="INTERNET_SEARCHER", agent_type="STATIC",
     #                multiplicity=3, task="search internet for the goal", output_consumer_agent=agent_list[1],
     #               llm_api="gpt4", go_d_timer=10000, llm_resp_timer=20, tools_list=["Google", "Bing","DuckduckGo-search" ])
     agent1.start_agent(mapper)
     agent2.start_agent(mapper)
     agent3.start_agent(mapper)
     time.sleep(5)  # Simulating data availability after 5 seconds
     msg1 = "message for agent RESEARCHER from ENVIRONMENT "
```

### Comparing `openagi-0.1.0b3/src/openagi/init_agent.py` & `openagi-0.1.0b4/src/openagi/init_agent.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/llms/azure.py` & `openagi-0.1.0b4/src/openagi/llms/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if not self.llm:
             raise ValueError("`llm` attribute not set.")
         message = HumanMessage(content=input_text)
         resp = self.llm([message])
         return resp.content
 
     @staticmethod
-    def load_from_yml_config() -> AzureChatConfigModel:
+    def load_from_yaml_config() -> AzureChatConfigModel:
         """Loads the AzureChatOpenAI configurations from a YAML file.
 
         Returns:
             An instance of AzureChatConfigModel with loaded configurations.
         """
         return AzureChatConfigModel(
             base_url=read_yaml_config("BASE_URL", raise_exception=True),
@@ -67,15 +67,15 @@
             api_key=read_yaml_config("AZURE_OPENAI_API_KEY", raise_exception=True),
         )
 
 
 """
 def main():
     # Demonstrates the use of AzureChatOpenAIModel.
-    config = AzureChatOpenAIModel.load_from_yml_config()
+    config = AzureChatOpenAIModel.load_from_yaml_config()
     azure_chat_model = AzureChatOpenAIModel(config=config)
     response = azure_chat_model.run("Hello, how can I help you today?")
     print(response)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openagi-0.1.0b3/src/openagi/llms/base.py` & `openagi-0.1.0b4/src/openagi/llms/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,10 +44,10 @@
         Returns:
             The result from processing the input data through the LLM.
         """
         pass
 
     @staticmethod
     @abstractmethod
-    def load_from_yml_config():
+    def load_from_yaml_config():
         """Loads configuration values from a YAML file."""
         pass
```

### Comparing `openagi-0.1.0b3/src/openagi/llms/openagi_main.py` & `openagi-0.1.0b4/src/openagi/llms/openagi_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from openagi.llms.azure import AzureChatOpenAIModel
 from openagi.llms.openai import OpenAIModel
 
 
 def loadLLM(llm="openai"):
     if llm == "openai":
-        config = OpenAIModel.load_from_yml_config()
+        config = OpenAIModel.load_from_yaml_config()
         llm = OpenAIModel(config=config)
         return llm
     else:
-        config = AzureChatOpenAIModel.load_from_yml_config()
+        config = AzureChatOpenAIModel.load_from_yaml_config()
         llm = AzureChatOpenAIModel(config=config)
     return llm
 
 
 def getLLM(sys):
     # total arguments
     n = len(sys.argv)
```

### Comparing `openagi-0.1.0b3/src/openagi/llms/openai.py` & `openagi-0.1.0b4/src/openagi/llms/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         if not self.llm:
             raise ValueError("`llm` attribute not set.")
         message = HumanMessage(content=input_text)
         resp = self.llm([message])
         return resp.content
 
     @staticmethod
-    def load_from_yml_config() -> OpenAIConfigModel:
+    def load_from_yaml_config() -> OpenAIConfigModel:
         """Loads the OpenAI configurations from a YAML file.
 
         Returns:
             An instance of OpenAIConfigModel with loaded configurations.
         """
         return OpenAIConfigModel(
             openai_api_key=read_yaml_config("OPENAI_API_KEY", raise_exception=True),
```

### Comparing `openagi-0.1.0b3/src/openagi/queue/message_broker.py` & `openagi-0.1.0b4/src/openagi/queue/message_broker.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/queue/pq.py` & `openagi-0.1.0b4/src/openagi/queue/pq.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/queue/timer_pool.py` & `openagi-0.1.0b4/src/openagi/queue/timer_pool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/base.py` & `openagi-0.1.0b4/src/openagi/tools/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Callable, Type
 
 from pydantic import BaseModel, Field
-
+import asyncio
 from openagi.llms.base import LLMBaseModel
 
 
 def tool(args_schema: Type[BaseModel], output_schema: Type[BaseModel] = None) -> Callable:
     def decorator(func: Callable) -> Callable:
         # Ensure we're accessing the correct attribute for Pydantic fields
         func.description = func.__doc__
@@ -15,14 +15,16 @@
         }
         func.output_schema = {
             field_name: field.description
             for field_name, field in output_schema.model_fields.items()
         }
 
         def wrapper(self, *args, **kwargs) -> Any:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
             return func(self, *args, **kwargs)
 
         # Attach metadata to the wrapper function to ensure it's accessible
         wrapper.args = func.args
         wrapper.output_schema = func.output_schema
         return wrapper
```

### Comparing `openagi-0.1.0b3/src/openagi/tools/custom_tools/ProxyTool.py` & `openagi-0.1.0b4/src/openagi/tools/custom_tools/ProxyTool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/__init__.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/dalle_image_generator.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/document_compare.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/document_compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,31 @@
             files.append(file_info)
     for file in files:
         loader = PyPDFLoader(file["path"])
         pages = loader.load_and_split()
         text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
         docs = text_splitter.split_documents(pages)
         embeddings = AzureOpenAIEmbeddings(
+            api_key = read_yaml_config("AZURE_OPENAI_API_KEY"),
             azure_deployment=deployment_name,
             openai_api_version=read_yaml_config("OPENAI_API_VERSION"),
         )
         retriever = FAISS.from_documents(docs, embeddings).as_retriever()
         tools.append(
             Tool(
                 name=file["name"],
                 description=f"useful when you want to answer questions about {file['name']}",
                 func=RetrievalQA.from_chain_type(llm=llm, retriever=retriever),
             )
         )
     agent = initialize_agent(
-        agent=AgentType.OPENAI_FUNCTIONS,
+        agent=AgentType.OPENAI_MULTI_FUNCTIONS,
         tools=tools,
         llm=llm,
-        verbose=True,
+        verbose=False,
     )
     result = agent({"input": searchString})
     logging.debug(result)
     return result
 
 
 class DocumentCompareInputSchema(BaseModel):
```

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/duckducksearch.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/duckducksearch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
-
 from duckduckgo_search import DDGS
 from pydantic import BaseModel, Field
-
 from openagi.tools.base import BaseTool, tool
 
 
 def getDuckduckgoSearchResults(query):
     results = DDGS().text(query, max_results=5)
     logging.debug(f"Results from DUCKDUCKGO --- {results}")
     return results
```

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/exa_search_tool.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/exa_search_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/github.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/github.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/gmail.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/gmail.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/google_finance_search.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/google_finance_search.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/google_serper_specific.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/google_serper_specific.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/googlejobsearch.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/googlejobsearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/googleserpersearch.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/googleserpersearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/nasa.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/nasa.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/open_weathermap.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/open_weathermap.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/polygon.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/polygon.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/serper_intermediate.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/serper_intermediate.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/sql.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/sql.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/wikipedia_tool.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/xorbits.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/xorbits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-import xorbits.pandas as pd
+import pandas as pd
 from langchain_experimental.agents.agent_toolkits import create_xorbits_agent
 from pydantic import BaseModel, Field
 
 from openagi.tools.base import BaseTool, tool
 from openagi.utils.yamlParse import read_yaml_config
```

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/yahoofinancenews.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/yahoofinancenews.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/integrations/youtubesearch.py` & `openagi-0.1.0b4/src/openagi/tools/integrations/youtubesearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/tools_db.py` & `openagi-0.1.0b4/src/openagi/tools/tools_db.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/tools/utils.py` & `openagi-0.1.0b4/src/openagi/tools/utils.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/utils/extraction.py` & `openagi-0.1.0b4/src/openagi/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/utils/llmTasks.py` & `openagi-0.1.0b4/src/openagi/utils/llmTasks.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b3/src/openagi/utils/yamlParse.py` & `openagi-0.1.0b4/src/openagi/utils/yamlParse.py`

 * *Files identical despite different names*

