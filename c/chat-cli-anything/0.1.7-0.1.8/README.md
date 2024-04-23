# Comparing `tmp/chat_cli_anything-0.1.7.tar.gz` & `tmp/chat_cli_anything-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_cli_anything-0.1.7.tar", max compression
+gzip compressed data, was "chat_cli_anything-0.1.8.tar", max compression
```

## Comparing `chat_cli_anything-0.1.7.tar` & `chat_cli_anything-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.7/LICENSE
--rw-r--r--   0        0        0     7930 2024-04-07 09:17:05.654963 chat_cli_anything-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.7/chat_cli_anything/__init__.py
--rw-r--r--   0        0        0    32639 2024-04-15 11:33:17.045968 chat_cli_anything-0.1.7/chat_cli_anything/ask.py
--rw-r--r--   0        0        0     9641 2024-04-16 14:34:55.649939 chat_cli_anything-0.1.7/chat_cli_anything/config.py
--rw-r--r--   0        0        0     8305 2024-04-15 11:24:08.954963 chat_cli_anything-0.1.7/chat_cli_anything/db.py
--rw-r--r--   0        0        0     1583 2024-04-15 09:35:00.631353 chat_cli_anything-0.1.7/chat_cli_anything/embedding.py
--rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.7/chat_cli_anything/loader.py
--rw-r--r--   0        0        0     2695 2024-04-07 11:06:03.928644 chat_cli_anything-0.1.7/chat_cli_anything/request.py
--rw-r--r--   0        0        0      900 2024-04-15 02:15:43.665432 chat_cli_anything-0.1.7/chat_cli_anything/rerank.py
--rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.7/chat_cli_anything/service.py
--rw-r--r--   0        0        0     1067 2024-04-09 05:24:26.253738 chat_cli_anything-0.1.7/chat_cli_anything/util.py
--rw-r--r--   0        0        0     1437 2024-04-16 14:37:03.981815 chat_cli_anything-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.8/LICENSE
+-rw-r--r--   0        0        0     8280 2024-04-17 12:17:42.718698 chat_cli_anything-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.8/chat_cli_anything/__init__.py
+-rw-r--r--   0        0        0    32639 2024-04-15 11:33:17.045968 chat_cli_anything-0.1.8/chat_cli_anything/ask.py
+-rw-r--r--   0        0        0     9641 2024-04-16 14:34:55.649939 chat_cli_anything-0.1.8/chat_cli_anything/config.py
+-rw-r--r--   0        0        0     8305 2024-04-15 11:24:08.954963 chat_cli_anything-0.1.8/chat_cli_anything/db.py
+-rw-r--r--   0        0        0     1587 2024-04-23 16:40:36.018979 chat_cli_anything-0.1.8/chat_cli_anything/embedding.py
+-rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.8/chat_cli_anything/loader.py
+-rw-r--r--   0        0        0     2695 2024-04-07 11:06:03.928644 chat_cli_anything-0.1.8/chat_cli_anything/request.py
+-rw-r--r--   0        0        0      900 2024-04-15 02:15:43.665432 chat_cli_anything-0.1.8/chat_cli_anything/rerank.py
+-rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.8/chat_cli_anything/service.py
+-rw-r--r--   0        0        0     1067 2024-04-09 05:24:26.253738 chat_cli_anything-0.1.8/chat_cli_anything/util.py
+-rw-r--r--   0        0        0     1437 2024-04-23 16:48:32.493747 chat_cli_anything-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     9814 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.8/PKG-INFO
```

### Comparing `chat_cli_anything-0.1.7/LICENSE` & `chat_cli_anything-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/README.md` & `chat_cli_anything-0.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ![chat-cli-anything](./logo.png)
 
+```
 # Chat-Cli-Anything
 
-Interact with GPT-like services from the command line, supporting local RAG and pipe input.
+Interact with GPT-like services from the command line, supporting local RAG, and pipe input.
 
 Why:
-① A significant portion of a developer's time is spent interacting with the system through the terminal. When encountering issues in the terminal, they expect to resolve them without having to switch to a search engine or another application.
-② By combining the language model's excellent text capabilities and text processing abilities, it helps us achieve code generation, explanation, and translation, as well as document Q&A, beyond simple searches.
+① Developers spend a significant amount of time using the terminal to interact with the system, and when encountering issues in the terminal, they expect not to have to switch to a search engine or elsewhere.
+② By leveraging the language model's excellent text capabilities and text processing abilities, it helps us achieve code generation, explanation, and translation beyond simple searches, as well as document Q&A.
 
 ## Tutorial
 
 1. Installation
 
 ```shell
-pip install "chat-cli-anything[all]"
+pip install "chat-cli-anything"
 ```
 
 To simplify command length, you can set command aliases (optional):
 
 ```shell
 # put this in your ~/.bashrc or ~/.zshrc
 alias config="cc-config"
@@ -29,76 +30,85 @@
 
 2. Add LLM provider
 
 ```
 cc-config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
-If command aliases are already set:
+If command aliases are set:
 
 ```
 config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
 3. Start Using
 
-**Example 1**: General question
+**example 1** Normal question
 
 ```
 cc-ask "Who is the author of the science fiction novel 'Three Body'?"
 ```
 
 ```
 cc-ask "How to get the memory size occupied by a process in Linux?"
 ```
 
-**Example 2**: Using pipe
+**example 2** Using pipe
+
+```
+# Find the filename with the maximum size in the current directory
+ls -lah | cc-ask "filename with max size"
+```
 
 ```
-cat names_of_diseases.txt | cc-ask "What are the most common types of diseases among the names listed?"
+# For debugging error
+gcc -o a.out a.cpp 2>&1 | cc-ask "what is the error" -s
 ```
 
-**Example 3**: Interactive questioning
+**example 3** Interactive questioning
 
 ```
 cc-chat "What is the capital of France?"
 ```
 
-**Example 4**: Local document Q&A
+**example 4** Local document Q&A
 
 ```
 cc-ask "Which school did the candidate graduate from?" -f resume.pdf
 ```
 
-**Example 5**: Local document collection
+**example 5** Local document collection
 
 Step 1: Digest text to build a local database
 
 ```
 # d2light code
 cc-db ingest "/path/to/detectron2-light" -n d2light
 ```
 
 Step 2: Ask a question
 
 ```
-# for open question, '-a/--advance' option would be helpful
+# For open questions, the '-a/--advance' option would be helpful
 cc-ask -d d2light "DETR implementation" -a
 ```
 
-**Example 6**: Code explain
+**example 6** Code explanation
 
 ```
 # Explain line by line
 cc-code explain /path/to/your/code.py -l
 
-# If the code is lengthy, continue generating
+# If the code is lengthy, add the -l parameter to continue generating
 cc-code explain /path/to/your/code.py -l -c
 ```
 
+### Notice
+It depends on `torch` version 2.2, so it may override the current environment version.
+
 ## Command Explanation
 
 ### cc-config
 
 Configure LLM provider
 
 #### 1. Add LLM provider
@@ -120,15 +130,15 @@
 ```
 
 #### 2. Test provider
 
 ```
 cc-config ping [OPTIONS] NAME
 
-Switch to a different configuration and save the change.
+Ping provider.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 3. List all providers
 
@@ -199,15 +209,15 @@
 
 Options:
   -d, --db TEXT        Name of database.
   -f, --filename TEXT  Name of file.
   -r, --rerank         Whether to rerank the results.
   -s, --show-chunks    Whether to show the related chunks retrieved from
                        the database.
-  -a, --advance        Whether to use advanced RAG.
+  -a, --advance        Whether to use advance RAG.
   --help               Show this message and exit.
 ```
 
 ### cc-chat
 
 Interactive Q&A
 
@@ -228,20 +238,23 @@
 ### cc-code
 
 Some common commands for code based on cc-ask.
 
 #### Code Explanation
 
 ```
-cc-code explain [OPTIONS] [FILENAME] [OBJECT_NAME]
+cc-code explain [OPTIONS] [FILENAME]
 
 Explain code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -l, --line               Line by line.
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 Example 1: Specify filename
 
 ```
 cc-code explain some_complex_scripts.py
 ```
@@ -257,83 +270,81 @@
 ```
 cat some_complex_scripts.py | cc-code explain
 ```
 
 #### Fix Issues
 
 ```
-```
 cc-code fix [OPTIONS] [FILENAME]
 
-  Fix code.
+Fix code.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
-```
 
 #### Code Refactoring
 
 ```
 cc-code refactor [OPTIONS] [FILENAME]
 
-  Refactor code.
+Refactor code.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
 
 #### Code Review
 
 ```
 cc-code review [OPTIONS] [FILENAME]
 
-  Review code.
+Review code.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
 
 #### Code Translation
 
 ```
 cc-code translate [OPTIONS] LANGUAGE [FILENAME]
 
-  Translate code from one language to another. Supported languages  c++, cpp,
-  c, rust, typescript, javascript, markdown, html.
+Translate code from one language to another. Supported languages include c++, cpp,
+c, rust, typescript, javascript, markdown, html.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
 
 #### Select Code from Generated Results
 
-Used to select code snippets from the generated responses of the above commands.
+Used to select code snippets from the generated responses of the above commands
 
 ```
 cc-code select [OPTIONS] [INDEX]
 
 Select code snippet from the last output.
 
-Argument: index: code snippet index
+Argument:     index: code snippet index
 
 Options:
-  -c, --count  Get the number of code snippets
+  -c, --count  get the number of code snippets
   --help       Show this message and exit.
 ```
 
-`-c/--count` Get the number of candidate code blocks in the last response.
+`-c/--count` Get the number of candidate code blocks in the last response
 
 Example:
 
 ```
 >>> cc-code select -c
 2
 
@@ -393,35 +404,38 @@
   --help              Show this message and exit.
 ```
 
 ### cc-service
 
 Used to manage local text-to-index services.
 
+If you want to run a text-to-index service on your local machine, execute the command `"pip install chat-cli-anything[all]"`.
+
 #### start:
 
 ```
 cc-service start [OPTIONS]
 
 Options:
-  --help  Show this message and exit.
+
+--help  Show this message and exit.
 ```
 
-The process will take some time to load the model (~1min), determine if it has started with `cc-service status`.
+This process may take some time (~1min) to load the model, and you can check if it has started with `cc-service status`.
 
-#### stop:
+#### stop
 
 ```
 cc-service stop [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
 
-#### status:
+#### status
 
 ```
 cc-service status [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
```

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/ask.py` & `chat_cli_anything-0.1.8/chat_cli_anything/ask.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/config.py` & `chat_cli_anything-0.1.8/chat_cli_anything/config.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/db.py` & `chat_cli_anything-0.1.8/chat_cli_anything/db.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/embedding.py` & `chat_cli_anything-0.1.8/chat_cli_anything/embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 class LocalEmbeddings(Embeddings):
     def __init__(self, url: str) -> None:
         self.url = url
         super().__init__()
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         response = requests.post(
-            f'{self.url}/embed_documents',
+            f'{self.url}/embedding_documents',
             timeout=10 * len(texts) + 10,
             json=[{'text': text} for text in texts]
         )
         return [r['embedding'] for r in response.json()]
 
     def embed_query(self, text: str) -> List[float]:
         response = requests.post(
```

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/loader.py` & `chat_cli_anything-0.1.8/chat_cli_anything/loader.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/request.py` & `chat_cli_anything-0.1.8/chat_cli_anything/request.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/rerank.py` & `chat_cli_anything-0.1.8/chat_cli_anything/rerank.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/service.py` & `chat_cli_anything-0.1.8/chat_cli_anything/service.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/chat_cli_anything/util.py` & `chat_cli_anything-0.1.8/chat_cli_anything/util.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.7/pyproject.toml` & `chat_cli_anything-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-cli-anything"
-version = "0.1.7"
+version = "0.1.8"
 description = "Chat with anything on cli."
 authors = ["liuping <liuping@shukun.net>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["chatgpt", "cli", "chat"]
 packages = [{ include = "chat_cli_anything" }]
```

### Comparing `chat_cli_anything-0.1.7/PKG-INFO` & `chat_cli_anything-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-cli-anything
-Version: 0.1.7
+Version: 0.1.8
 Summary: Chat with anything on cli.
 License: Apache
 Keywords: chatgpt,cli,chat
 Author: liuping
 Author-email: liuping@shukun.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -34,28 +34,29 @@
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Requires-Dist: xonsh (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 ![chat-cli-anything](./logo.png)
 
+```
 # Chat-Cli-Anything
 
-Interact with GPT-like services from the command line, supporting local RAG and pipe input.
+Interact with GPT-like services from the command line, supporting local RAG, and pipe input.
 
 Why:
-① A significant portion of a developer's time is spent interacting with the system through the terminal. When encountering issues in the terminal, they expect to resolve them without having to switch to a search engine or another application.
-② By combining the language model's excellent text capabilities and text processing abilities, it helps us achieve code generation, explanation, and translation, as well as document Q&A, beyond simple searches.
+① Developers spend a significant amount of time using the terminal to interact with the system, and when encountering issues in the terminal, they expect not to have to switch to a search engine or elsewhere.
+② By leveraging the language model's excellent text capabilities and text processing abilities, it helps us achieve code generation, explanation, and translation beyond simple searches, as well as document Q&A.
 
 ## Tutorial
 
 1. Installation
 
 ```shell
-pip install "chat-cli-anything[all]"
+pip install "chat-cli-anything"
 ```
 
 To simplify command length, you can set command aliases (optional):
 
 ```shell
 # put this in your ~/.bashrc or ~/.zshrc
 alias config="cc-config"
@@ -67,76 +68,85 @@
 
 2. Add LLM provider
 
 ```
 cc-config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
-If command aliases are already set:
+If command aliases are set:
 
 ```
 config add "openai" "https://api.openai.com/v1"  --api-key "your-api-key"
 ```
 
 3. Start Using
 
-**Example 1**: General question
+**example 1** Normal question
 
 ```
 cc-ask "Who is the author of the science fiction novel 'Three Body'?"
 ```
 
 ```
 cc-ask "How to get the memory size occupied by a process in Linux?"
 ```
 
-**Example 2**: Using pipe
+**example 2** Using pipe
+
+```
+# Find the filename with the maximum size in the current directory
+ls -lah | cc-ask "filename with max size"
+```
 
 ```
-cat names_of_diseases.txt | cc-ask "What are the most common types of diseases among the names listed?"
+# For debugging error
+gcc -o a.out a.cpp 2>&1 | cc-ask "what is the error" -s
 ```
 
-**Example 3**: Interactive questioning
+**example 3** Interactive questioning
 
 ```
 cc-chat "What is the capital of France?"
 ```
 
-**Example 4**: Local document Q&A
+**example 4** Local document Q&A
 
 ```
 cc-ask "Which school did the candidate graduate from?" -f resume.pdf
 ```
 
-**Example 5**: Local document collection
+**example 5** Local document collection
 
 Step 1: Digest text to build a local database
 
 ```
 # d2light code
 cc-db ingest "/path/to/detectron2-light" -n d2light
 ```
 
 Step 2: Ask a question
 
 ```
-# for open question, '-a/--advance' option would be helpful
+# For open questions, the '-a/--advance' option would be helpful
 cc-ask -d d2light "DETR implementation" -a
 ```
 
-**Example 6**: Code explain
+**example 6** Code explanation
 
 ```
 # Explain line by line
 cc-code explain /path/to/your/code.py -l
 
-# If the code is lengthy, continue generating
+# If the code is lengthy, add the -l parameter to continue generating
 cc-code explain /path/to/your/code.py -l -c
 ```
 
+### Notice
+It depends on `torch` version 2.2, so it may override the current environment version.
+
 ## Command Explanation
 
 ### cc-config
 
 Configure LLM provider
 
 #### 1. Add LLM provider
@@ -158,15 +168,15 @@
 ```
 
 #### 2. Test provider
 
 ```
 cc-config ping [OPTIONS] NAME
 
-Switch to a different configuration and save the change.
+Ping provider.
 
 Options:
   --help  Show this message and exit.
 ```
 
 #### 3. List all providers
 
@@ -237,15 +247,15 @@
 
 Options:
   -d, --db TEXT        Name of database.
   -f, --filename TEXT  Name of file.
   -r, --rerank         Whether to rerank the results.
   -s, --show-chunks    Whether to show the related chunks retrieved from
                        the database.
-  -a, --advance        Whether to use advanced RAG.
+  -a, --advance        Whether to use advance RAG.
   --help               Show this message and exit.
 ```
 
 ### cc-chat
 
 Interactive Q&A
 
@@ -266,20 +276,23 @@
 ### cc-code
 
 Some common commands for code based on cc-ask.
 
 #### Code Explanation
 
 ```
-cc-code explain [OPTIONS] [FILENAME] [OBJECT_NAME]
+cc-code explain [OPTIONS] [FILENAME]
 
 Explain code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -l, --line               Line by line.
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 Example 1: Specify filename
 
 ```
 cc-code explain some_complex_scripts.py
 ```
@@ -295,83 +308,81 @@
 ```
 cat some_complex_scripts.py | cc-code explain
 ```
 
 #### Fix Issues
 
 ```
-```
 cc-code fix [OPTIONS] [FILENAME]
 
-  Fix code.
+Fix code.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
-```
 
 #### Code Refactoring
 
 ```
 cc-code refactor [OPTIONS] [FILENAME]
 
-  Refactor code.
+Refactor code.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
 
 #### Code Review
 
 ```
 cc-code review [OPTIONS] [FILENAME]
 
-  Review code.
+Review code.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
 
 #### Code Translation
 
 ```
 cc-code translate [OPTIONS] LANGUAGE [FILENAME]
 
-  Translate code from one language to another. Supported languages  c++, cpp,
-  c, rust, typescript, javascript, markdown, html.
+Translate code from one language to another. Supported languages include c++, cpp,
+c, rust, typescript, javascript, markdown, html.
 
 Options:
   -o, --object-name TEXT
   -c, --continue-generate
   --help                   Show this message and exit.
 ```
 
 #### Select Code from Generated Results
 
-Used to select code snippets from the generated responses of the above commands.
+Used to select code snippets from the generated responses of the above commands
 
 ```
 cc-code select [OPTIONS] [INDEX]
 
 Select code snippet from the last output.
 
-Argument: index: code snippet index
+Argument:     index: code snippet index
 
 Options:
-  -c, --count  Get the number of code snippets
+  -c, --count  get the number of code snippets
   --help       Show this message and exit.
 ```
 
-`-c/--count` Get the number of candidate code blocks in the last response.
+`-c/--count` Get the number of candidate code blocks in the last response
 
 Example:
 
 ```
 >>> cc-code select -c
 2
 
@@ -431,35 +442,38 @@
   --help              Show this message and exit.
 ```
 
 ### cc-service
 
 Used to manage local text-to-index services.
 
+If you want to run a text-to-index service on your local machine, execute the command `"pip install chat-cli-anything[all]"`.
+
 #### start:
 
 ```
 cc-service start [OPTIONS]
 
 Options:
-  --help  Show this message and exit.
+
+--help  Show this message and exit.
 ```
 
-The process will take some time to load the model (~1min), determine if it has started with `cc-service status`.
+This process may take some time (~1min) to load the model, and you can check if it has started with `cc-service status`.
 
-#### stop:
+#### stop
 
 ```
 cc-service stop [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
 
-#### status:
+#### status
 
 ```
 cc-service status [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
```

