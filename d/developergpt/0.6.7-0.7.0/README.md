# Comparing `tmp/developergpt-0.6.7.tar.gz` & `tmp/developergpt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.6.7.tar", last modified: Wed Apr  3 02:30:49 2024, max compression
+gzip compressed data, was "developergpt-0.7.0.tar", last modified: Tue Apr 23 03:07:48 2024, max compression
```

## Comparing `developergpt-0.6.7.tar` & `developergpt-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.043264 developergpt-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 02:30:40.000000 developergpt-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:30:40.000000 developergpt-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-04-03 02:30:49.043264 developergpt-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-03 02:30:40.000000 developergpt-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.039264 developergpt-0.6.7/developergpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/gemini_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.039264 developergpt-0.6.7/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 02:30:49.000000 developergpt-0.6.7/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:30:49.043264 developergpt-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-03 02:30:40.000000 developergpt-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.039264 developergpt-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:40.000000 developergpt-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-03 02:30:40.000000 developergpt-0.6.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 02:30:40.000000 developergpt-0.6.7/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.912621 developergpt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 03:07:40.000000 developergpt-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 03:07:40.000000 developergpt-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-23 03:07:48.912621 developergpt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-23 03:07:40.000000 developergpt-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.908621 developergpt-0.7.0/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/gemini_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-23 03:07:40.000000 developergpt-0.7.0/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.908621 developergpt-0.7.0/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 03:07:48.000000 developergpt-0.7.0/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:07:48.912621 developergpt-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 03:07:40.000000 developergpt-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:48.908621 developergpt-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:07:40.000000 developergpt-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-23 03:07:40.000000 developergpt-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 03:07:40.000000 developergpt-0.7.0/tests/test_cli.py
```

### Comparing `developergpt-0.6.7/LICENSE` & `developergpt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.6.7/PKG-INFO` & `developergpt-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.6.7
+Version: 0.7.0
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -15,15 +15,16 @@
 Requires-Dist: tiktoken
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: prompt_toolkit
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: llama-cpp-python
-Requires-Dist: huggingface-hub>=0.20.0
+Requires-Dist: huggingface-hub>=0.22.2
+Requires-Dist: minijinja
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -31,35 +32,33 @@
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
-[![OpenAI GPTs](https://img.shields.io/badge/OpenAI%20GPTs-Try%20the%20online%20DeveloperGPT-8A2BE2)](https://chat.openai.com/g/g-mfPPe6MKC-developergpt)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs from Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
 As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                   | Source                                                                                                            | Details                                                  |
-| -------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                        | Free (up to 15 requests/min), Google AI API Key Required |
-| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                  | Free, Open-Source, Hugging Face Inference API            |
-| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                 | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Zephyr**                 | [Zephyr (7B-Beta)](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                           | Free, Open-Source, Hugging Face Inference API            |
-| **OpenChat**               | [OpenChat (3.5-0106)](https://huggingface.co/openchat/openchat-3.5-0106)                                          | Free, Open-Source, Hugging Face Inference API            |
-| **Gemma, Gemma-Base**      | [Gemma-Instruct](https://huggingface.co/google/gemma-7b), [Gemma-Base](https://huggingface.co/google/gemma-7b-it) | Free, Open-Source, Hugging Face Inference API            |
-| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)               | Free, Open-Source, OFFLINE, ON-DEVICE                    |
+| Model(s)                          | Source                                                                                                                       | Details                                                  |
+| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)              | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                   | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                        | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open-Source, Hugging Face Inference API            |
+| **Gemma, Gemma-Base**             | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open-Source, Hugging Face Inference API            |
+| **Mistral-Q6, Mistral-Q4**        | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open-Source, OFFLINE, ON-DEVICE                    |
+| **Mistral** [current not working] | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open-Source, Hugging Face Inference API            |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
@@ -79,15 +78,15 @@
 
 Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
 # Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
 $ developergpt --offline cmd [your natural language command request]
 ```
 
-Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini (used by default).  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Pro (used by default).  
 ```bash
 # Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
@@ -121,15 +120,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 60 queries per minute).
+By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -152,16 +151,17 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Open-Source Hugging-Face Inference API LLMs
-To use open-source LLMs such as Zephyr or OpenChat hosted on Hugging Face, you can optionally set up a [Hugging Face](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token as an environment variable using the steps below. Setting up a token is **not required**, but it will allow you to make more requests without being rate limited. 
+#### Using Open-Source Hugging Face Inference API LLMs
+To use open-source LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+See https://huggingface.co/docs/api-inference/index for more details. 
 
 ```bash
 # [OPTIONAL] set Hugging Face token (using zsh for example)
 # You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
@@ -174,16 +174,17 @@
 
 #### Google Gemini
 As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
-#### Hugging-Face Open-Source LLMs 
-As of December 2023, using Hugging Face LLMs does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
+#### Hugging Face Hosted Open LLMs 
+As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
-- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, tools, quantization, and other resources! 
+- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, generous free hosted inference API, tools, quantization, and other resources! 
+- Thanks to Google for the generous Gemini Pro API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.6.7/README.md` & `developergpt-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
-[![OpenAI GPTs](https://img.shields.io/badge/OpenAI%20GPTs-Try%20the%20online%20DeveloperGPT-8A2BE2)](https://chat.openai.com/g/g-mfPPe6MKC-developergpt)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs from Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
 As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                   | Source                                                                                                            | Details                                                  |
-| -------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                        | Free (up to 15 requests/min), Google AI API Key Required |
-| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                  | Free, Open-Source, Hugging Face Inference API            |
-| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                 | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Zephyr**                 | [Zephyr (7B-Beta)](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                           | Free, Open-Source, Hugging Face Inference API            |
-| **OpenChat**               | [OpenChat (3.5-0106)](https://huggingface.co/openchat/openchat-3.5-0106)                                          | Free, Open-Source, Hugging Face Inference API            |
-| **Gemma, Gemma-Base**      | [Gemma-Instruct](https://huggingface.co/google/gemma-7b), [Gemma-Base](https://huggingface.co/google/gemma-7b-it) | Free, Open-Source, Hugging Face Inference API            |
-| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)               | Free, Open-Source, OFFLINE, ON-DEVICE                    |
+| Model(s)                          | Source                                                                                                                       | Details                                                  |
+| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)              | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                   | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                        | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open-Source, Hugging Face Inference API            |
+| **Gemma, Gemma-Base**             | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open-Source, Hugging Face Inference API            |
+| **Mistral-Q6, Mistral-Q4**        | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open-Source, OFFLINE, ON-DEVICE                    |
+| **Mistral** [current not working] | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open-Source, Hugging Face Inference API            |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
@@ -44,15 +42,15 @@
 
 Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
 # Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
 $ developergpt --offline cmd [your natural language command request]
 ```
 
-Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini (used by default).  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Pro (used by default).  
 ```bash
 # Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
@@ -86,15 +84,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 60 queries per minute).
+By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -117,16 +115,17 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Open-Source Hugging-Face Inference API LLMs
-To use open-source LLMs such as Zephyr or OpenChat hosted on Hugging Face, you can optionally set up a [Hugging Face](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token as an environment variable using the steps below. Setting up a token is **not required**, but it will allow you to make more requests without being rate limited. 
+#### Using Open-Source Hugging Face Inference API LLMs
+To use open-source LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+See https://huggingface.co/docs/api-inference/index for more details. 
 
 ```bash
 # [OPTIONAL] set Hugging Face token (using zsh for example)
 # You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
@@ -139,16 +138,17 @@
 
 #### Google Gemini
 As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
-#### Hugging-Face Open-Source LLMs 
-As of December 2023, using Hugging Face LLMs does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
+#### Hugging Face Hosted Open LLMs 
+As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
-- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, tools, quantization, and other resources! 
+- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, generous free hosted inference API, tools, quantization, and other resources! 
+- Thanks to Google for the generous Gemini Pro API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.6.7/developergpt/cli.py` & `developergpt-0.7.0/developergpt/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         openai_adapter.check_open_ai_key(console, client)
         console.print(f"[bold yellow]Using OpenAI {config.OPENAI_MODEL_MAP[model]}.")
     elif model in config.HF_MODEL_MAP:
         ctx.obj["api_key"] = config.get_environ_key_optional(
             config.HUGGING_FACE_API_KEY, console
         )
         console.print(
-            f"[bold yellow]Using {config.HF_MODEL_MAP[model]} via HF: some features may have unexpected behavior and results may not be as accurate."
+            f"[bold yellow]Using {config.HF_MODEL_MAP[model]} via Hugging Face Inference API."
         )
     elif model in config.GOOGLE_MODEL_MAP:
         api_key = config.get_environ_key(config.GOOGLE_API_KEY, console)
         genai.configure(api_key=api_key)
 
     ctx.obj["temperature"] = temperature
     ctx.obj["model"] = model
@@ -123,14 +123,17 @@
     ctx.obj["client"] = client
 
 
 @main.command(help="Chat with DeveloperGPT")
 @click.pass_context
 @click.argument("user_input", nargs=-1)
 def chat(ctx, user_input):
+    """
+    Chat with LLMs in Terminal
+    """
     if user_input:
         user_input = str(" ".join(user_input))
         session.history.append_string(user_input)
 
     model = ctx.obj["model"]
     input_messages = []
 
@@ -196,14 +199,17 @@
     "--fast",
     is_flag=True,
     default=False,
     help="Get commands without command or argument explanations (less accurate)",
 )
 @click.pass_context
 def cmd(ctx, user_input, fast):
+    """
+    Natural Language to Terminal Commands
+    """
     input_request = "\nDesired Command Request: "
 
     if user_input:
         user_input = str(" ".join(user_input))
         session.history.append_string(user_input)
 
     model = ctx.obj["model"]
@@ -251,15 +257,15 @@
                 console=console,
                 fast_mode=fast,
                 model=model,
             )
 
         user_input = None  # clear input for next iteration
 
-        commands = utils.print_command_response(model_output, console, fast, model)
+        commands = utils.print_command_response(model_output, console, fast)
         if not commands:
             continue
 
         # Give user options to revise query, execute command(s), or quit
         options = [
             "Revise Query",
             "Execute Command(s)",
```

### Comparing `developergpt-0.6.7/developergpt/config.py` & `developergpt-0.7.0/developergpt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,41 +9,39 @@
 
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.styles import Style
 from rich.console import Console
 
-# appearance constants
+### Appearance Constants ###
 DEFAULT_COLUMN_WIDTH = 100
 
 INPUT_STYLE = Style.from_dict(
     {
         "prompt": "bold ansigreen",
     }
 )
 
-# supported models
+### Supported LLMs and Configuration ###
 GPT35 = "gpt35"
 GPT4 = "gpt4"
-OPENCHAT = "openchat"
 ZEPHYR = "zephyr"
 GEMMA = "gemma"
 GEMMA_BASE = "gemma-base"
 GEMINI = "gemini"
 MISTRAL_Q6 = "mistral-q6"
 MISTRAL_Q4 = "mistral-q4"
 MISTRAL_HF = "mistral"
 BLOOM = "bloom"  # not supported due to poor performance
 SUPPORTED_MODELS = set(
     [
         GPT35,
         GPT4,
         GEMINI,
-        OPENCHAT,
         ZEPHYR,
         MISTRAL_Q6,
         MISTRAL_Q4,
         MISTRAL_HF,
         GEMMA,
         GEMMA_BASE,
     ]
@@ -67,32 +65,38 @@
 
 OPENAI_MODEL_MAP = {
     GPT35: "gpt-3.5-turbo",
     GPT4: "gpt-4-turbo-preview",
 }
 
 HF_MODEL_MAP = {
-    OPENCHAT: "openchat/openchat-3.5-0106",
     ZEPHYR: "HuggingFaceH4/zephyr-7b-beta",
-    GEMMA: "google/gemma-7b-it",
+    GEMMA: "google/gemma-1.1-7b-it",
     GEMMA_BASE: "google/gemma-7b",
     MISTRAL_HF: "mistralai/Mistral-7B-Instruct-v0.2",
     BLOOM: "bigscience/bloom",
 }
 
-HF_INSTRUCT_MODELS = set([GEMMA, ZEPHYR, OPENCHAT, MISTRAL_HF])
+HF_INSTRUCT_MODELS = set([GEMMA, ZEPHYR, MISTRAL_HF])
+
+# set of models that support the new chat completion endpoint
+HF_CHAT_COMPLETION_MODELS = set([ZEPHYR])
 
 GOOGLE_MODEL_MAP = {
     GEMINI: "gemini-1.0-pro",
 }
 
+### API Key Constants ###
+
 GOOGLE_API_KEY = "GOOGLE_API_KEY"
 OPEN_AI_API_KEY = "OPENAI_API_KEY"
 HUGGING_FACE_API_KEY = "HUGGING_FACE_API_KEY"
 
+### General Configuration ###
+
 USER_PLATFORM = platform.platform()
 CMD_TEMP = 0.01
 
 
 def get_environ_key(keyname: str, console: Console) -> str:
     key = os.environ.get(keyname, None)
     if not key:
```

### Comparing `developergpt-0.6.7/developergpt/few_shot_prompts.py` & `developergpt-0.7.0/developergpt/few_shot_prompts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from datetime import datetime
 
-from developergpt import config
-
 JSON_CMD_FORMAT = """
-    {
-        "input": "<user input>",
-        "error": 0,
-        "commands": [
-            {
-                "seq": <Order of Command>,
-                "cmd_to_execute": "<commands and arguments to execute>",
-                "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
-                "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
-            },
-            {
-                "seq": <Order of Command>,
-                "cmd_to_execute": "<commands and arguments to execute>",
-                "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
-                "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
-            }
-        ]
-    }
-    """
+{
+    "input": "<user input>",
+    "error": 0,
+    "commands": [
+        {
+            "seq": <Order of Command>,
+            "cmd_to_execute": "<commands and arguments to execute>",
+            "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
+            "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
+        },
+        {
+            "seq": <Order of Command>,
+            "cmd_to_execute": "<commands and arguments to execute>",
+            "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
+            "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
+        }
+    ]
+}
+"""
 
 JSON_CMD_FORMAT_FAST = """
-    {
-        "commands": ["<commands and arguments to execute>", "<commands and arguments to execute>", ...]
-    }
-    """
+{
+    "commands": ["<commands and arguments to execute>", "<commands and arguments to execute>", ...]
+}
+"""
 
 JSON_INVALID_FORMAT = """{"input": "<user input>", "error": 1}"""
 
 JSON_INVALID_FORMAT_FAST = """{"error": 1}"""
 
 
 def format_initial_cmd_msg(cmd_format: str, invalid_format: str) -> str:
@@ -88,56 +86,50 @@
     """
 
 CONDA_OUTPUT_EXAMPLE_MARKDOWN = """
 `curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh`\n
 `bash Miniconda3-latest-MacOSX-x86_64.sh`\n
 """
 
-SEARCH_REQUEST = "search ~/Documents directory for any .py file that begins with 'test'"
+SEARCH_REQUEST = (
+    "search ~/Documents directory for any python file that begins with 'test'"
+)
 
 SEARCH_OUTPUT_EXAMPLE = """
     {
-        "input": "search the ~/Documents/ directory for any .py file that begins with 'test'",
+        "input": "search the ~/Documents/ directory for any python file that begins with 'test'",
         "error" : 0,
         "commands": [
             {
                 "seq": 1,
                 "cmd_to_execute": "find ~/Documents/ -name 'test*.py'",
                 "cmd_explanations": ["`find` is used to list files."],
                 "arg_explanations": {
                                         "~/Documents": "specifies the folder to search in.",
-                                        "-name 'test*.py'": "specifies that we want to search for files starting with `test` and ending with `.py`."
+                                        "-name 'test*.py'": "specifies that we want to search for files starting with `test` that are python files."
                                     }
             }
         ]
     }
     """
 
 SEARCH_OUTPUT_EXAMPLE_FAST = """
     {
         "commands": ["find ~/Documents/ -name 'test*.py'"]
     }
     """
 
-SEARCH_OUTPUT_EXAMPLE_MARKDOWN = """
-`find ~/Documents/ -name 'test*.py'`\n
-"""
-
 PROCESS_REQUEST = "list all processes using more than 50 MB of memory"
 
 PROCESS_OUTPUT_EXAMPLE_FAST = """
 {
 "commands": ["ps -axm -o %mem,rss,comm | awk '$1 > 0.5 { printf(\\"%.0fMB\\\\t%s\\\\n\\", $2/1024, $3); }'"]
 }
 """
 
-PROCESS_OUTPUT_EXAMPLE_MARKDOWN = """
-`ps -axm -o %mem,rss,comm | awk '$1 > 0.5 { printf(\\"%.0fMB\\\\t%s\\\\n\\", $2/1024, $3); }'`\n
-"""
-
 UNKNOWN_REQUEST = "the quick brown fox jumped over"
 
 UNKNOWN_QUERY_OUTPUT_EXAMPLE_ONE = (
     """{"input": "the quick brown fox jumped over", "error": 1}"""
 )
 
 UNKNOWN_QUERY_OUTPUT_EXAMPLE_ONE_FAST = """{"error": 1}"""
```

### Comparing `developergpt-0.6.7/developergpt/gemini_adapter.py` & `developergpt-0.7.0/developergpt/gemini_adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -115,15 +115,26 @@
 def get_model_chat_response(
     *,
     user_input: str,
     console: Console,
     chat_session: "ChatSession",
     temperature: float,
 ) -> None:
-    """Get the response from the model."""
+    """
+    Get the chat response from Gemini model.
+
+    Args:
+        user_input (str): The user's input message.
+        console (Console): The console object for displaying the output.
+        chat_session (ChatSession): The chat session object.
+        temperature (float): The temperature value for generating the response.
+
+    Returns:
+        None
+    """
     response = chat_session.send_message(
         user_input,
         stream=True,
         generation_config=genai.types.GenerationConfig(temperature=temperature),
     )
     collected_messages = []
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
@@ -141,15 +152,27 @@
                 output_panel.renderable = Markdown(
                     "".join(collected_messages), inline_code_theme="monokai"
                 )
 
 
 def model_command(
     *, user_input: str, console: Console, fast_mode: bool, model: str
-) -> Optional[str]:
+) -> str:
+    """
+    Get model command suggestion.
+
+    Args:
+        user_input (str): The user natural language command request.
+        console (Console): The console object for displaying status messages.
+        fast_mode (bool): Flag indicating whether to use fast mode or not.
+        model (str): The model to use for generating the response.
+
+    Returns:
+        str: The generated response as a string, or None if no response is generated.
+    """
     gemini_model = GenerativeModel(config.GOOGLE_MODEL_MAP[model])
 
     if fast_mode:
         input_messages = list(BASE_INPUT_CMD_MSGS_FAST)
     else:
         input_messages = list(BASE_INPUT_CMD_MSGS)
```

### Comparing `developergpt-0.6.7/developergpt/openai_adapter.py` & `developergpt-0.7.0/developergpt/openai_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,14 +110,28 @@
     user_input: str,
     console: Console,
     input_messages: list,
     temperature: float,
     model: str,
     client: OpenAI | Llama,
 ) -> list:
+    """
+    Get the chat response from the model.
+
+    Args:
+        user_input (str): The user's input message.
+        console (Console): The console object for printing messages.
+        input_messages (list): The list of input messages exchanged between the user and the model.
+        temperature (float): The temperature parameter for controlling the randomness of the model's output.
+        model (str): The name of the model to use for generating the response.
+        client (OpenAI | Llama): The client object for making API requests to the model.
+
+    Returns:
+        list: The updated list of input messages, including the generated response.
+    """
     MAX_TOKENS = 4000
     RESERVED_OUTPUT_TOKENS = 1024
     MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
     # Note: llama.cpp models use OpenAI token counts as rough estimate
     if model in config.OFFLINE_MODELS:
         model_name = "gpt-3.5-turbo"
     else:
@@ -159,34 +173,48 @@
             for chunk in response:
                 msg = chunk.choices[0].delta.content
                 if msg:
                     collected_messages.append(msg)
                     output_panel.renderable = Markdown(
                         "".join(collected_messages), inline_code_theme="monokai"
                     )
+
+        full_response = "".join(collected_messages)
+        input_messages.append(format_assistant_response(full_response))
+        return input_messages
+
     except openai.RateLimitError:
         console.print("[bold red] Rate limit exceeded. Try again later.[/bold red]")
-        sys.exit(-1)
     except openai.BadRequestError as e:
         console.log(f"[bold red] Bad Request: {e}[/bold red]")
-        sys.exit(-1)
 
-    full_response = "".join(collected_messages)
-    input_messages.append(format_assistant_response(full_response))
-    return input_messages
+    sys.exit(-1)
 
 
 def model_command(
     *,
     user_input: str,
     console: Console,
     fast_mode: bool,
     model: str,
     client: OpenAI | Llama,
 ) -> Optional[str]:
+    """
+    Get command suggestion from model.
+
+    Args:
+        user_input (str): The user's natural language terminal command request.
+        console (Console): The console object for displaying status messages.
+        fast_mode (bool): Flag indicating whether to use fast mode.
+        model (str): The model to use for generating the response.
+        client (OpenAI | Llama): The client object for making API requests.
+
+    Returns:
+        Optional[str]: The model's response as a string, or None if there is no response.
+    """
     n_output_tokens = 4000
 
     if fast_mode:
         input_messages = list(BASE_INPUT_CMD_MSGS_FAST)
     else:
         input_messages = list(BASE_INPUT_CMD_MSGS)
 
@@ -221,27 +249,26 @@
         console.log(f"[bold red] Bad Request: {e}[/bold red]")
         sys.exit(-1)
     except openai.APIError as e:
         console.log(f"[bold red] OpenAI API Error: {e}[/bold red]")
         sys.exit(-1)
 
     raw_output = response.choices[0].message.content
-    return utils.clean_model_output(raw_output)
+    return utils.clean_model_output(raw_output) if raw_output else None
 
 
 def check_open_ai_key(console: "Console", client: "OpenAI") -> None:
     """Check if the OpenAI API key is valid."""
     try:
         _ = client.models.list()
+        return
     except openai.AuthenticationError:
         console.print(
             f"[bold red]Error: Invalid OpenAI API key. Check your {config.OPEN_AI_API_KEY} environment variable.[/bold red]"
         )
-        sys.exit(-1)
     except openai.PermissionDeniedError:
         console.print(
             "[bold red]Error: OpenAI API Permission Denied. Your location may not be supported by OpenAI.[/bold red]"
         )
-        sys.exit(-1)
     except openai.APIError as e:
         console.print(f"[bold red]Error: OpenAI API error: {e}.[/bold red]")
-        sys.exit(-1)
+    sys.exit(-1)
```

### Comparing `developergpt-0.6.7/developergpt/utils.py` & `developergpt-0.7.0/developergpt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,31 @@
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config
 
 
 def clean_model_output(raw_output: str) -> str:
-    # clean up the output - some models like to put ``` and ```or other text around the output JSON { }
+    """
+    Clean up the model output to remove any extraneous text.
+    Some models like to put ``` and ```or other text around the output JSON { }
+    """
+    raw_output = raw_output.strip()
     startPos = raw_output.find("{")
     if startPos != -1:
         raw_output = raw_output[startPos:]
     endPos = raw_output.rfind("}")
     if endPos != -1:
         raw_output = raw_output[: endPos + 1]
     model_output = raw_output.strip()
     return model_output
 
 
 def pretty_print_commands(commands: list, console: Console, panel_width: int) -> None:
-    # print all the commands in a panel
+    """Pretty print the commands in a panel"""
     commands_format = "\n\n".join([f"""- `{c}`""" for c in commands])
 
     cmd_out = Markdown(
         commands_format,
         inline_code_lexer="bash",
     )
 
@@ -47,16 +51,17 @@
             title_align="left",
             width=panel_width,
         )
     )
 
 
 def print_command_response(
-    model_output: Optional[str], console: Console, fast_mode: bool, model: str
+    model_output: Optional[str], console: Console, fast_mode: bool
 ) -> list:
+    """Print the commands and explanations from the model output in terminal GUI."""
     if not model_output:
         return []
 
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
 
     try:
         output_data = json.loads(model_output)
@@ -114,14 +119,15 @@
     session: PromptSession,
     console: Console,
     completer=None,
     complete_style=None,
     auto_suggest=None,
     key_bindings=None,
 ) -> str:
+    """Prompt the user for input and handle exit if requested."""
     user_input = session.prompt(
         input_request,
         style=config.INPUT_STYLE,
         completer=completer,
         complete_style=complete_style,
         auto_suggest=auto_suggest,
         key_bindings=key_bindings,
@@ -204,48 +210,42 @@
         n_removed = count_msg_tokens([removed_ctx], model)
         n_tokens -= n_removed
 
     return messages, n_tokens
 
 
 class PathCompleter(Completer):
-    """A completer for file paths."""
+    """A completer for file paths for terminal input."""
 
     def get_completions(self, document, complete_event):
         if complete_event.completion_requested:
             # only display completions when the user presses tab
             cwd = os.getcwd()
 
             text = document.text_before_cursor.lstrip().lower().split(" ")[-1]
-            # print(f"text={text}")
-
             auto_completion = []
 
             if text.startswith("~/"):
                 f_path = os.path.expanduser(text)
             elif text.startswith("/"):
                 f_path = text
             else:
                 f_path = os.path.join(cwd, text)
 
             curr_dir = os.path.dirname(f_path)
             fname = os.path.basename(f_path) if len(text) > 0 else ""
 
-            # print(f"f_path={f_path}, fname={fname}, curr_dir={dir}")
-
             if os.path.isdir(curr_dir):
                 # Generate a list of matching file names in the current directory
-                # TODO: possibly change to glob + re to handle regular expressions
                 auto_completion = [
                     os.path.join(curr_dir, f)
                     for f in os.listdir(curr_dir)
                     if fname in f.lower()
                 ]
 
-            # Yield the completions
             for completion in auto_completion:
                 # simplify the completion substitution if possible
                 if text.startswith("~/"):
                     completion = completion.replace(os.path.expanduser("~/"), "~/")
                 elif cwd in completion:
                     completion = os.path.relpath(completion, cwd)
```

### Comparing `developergpt-0.6.7/developergpt.egg-info/PKG-INFO` & `developergpt-0.7.0/developergpt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.6.7
+Version: 0.7.0
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -15,15 +15,16 @@
 Requires-Dist: tiktoken
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: prompt_toolkit
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: llama-cpp-python
-Requires-Dist: huggingface-hub>=0.20.0
+Requires-Dist: huggingface-hub>=0.22.2
+Requires-Dist: minijinja
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -31,35 +32,33 @@
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
-[![OpenAI GPTs](https://img.shields.io/badge/OpenAI%20GPTs-Try%20the%20online%20DeveloperGPT-8A2BE2)](https://chat.openai.com/g/g-mfPPe6MKC-developergpt)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs from Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
 As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                   | Source                                                                                                            | Details                                                  |
-| -------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                        | Free (up to 15 requests/min), Google AI API Key Required |
-| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                  | Free, Open-Source, Hugging Face Inference API            |
-| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                 | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Zephyr**                 | [Zephyr (7B-Beta)](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                           | Free, Open-Source, Hugging Face Inference API            |
-| **OpenChat**               | [OpenChat (3.5-0106)](https://huggingface.co/openchat/openchat-3.5-0106)                                          | Free, Open-Source, Hugging Face Inference API            |
-| **Gemma, Gemma-Base**      | [Gemma-Instruct](https://huggingface.co/google/gemma-7b), [Gemma-Base](https://huggingface.co/google/gemma-7b-it) | Free, Open-Source, Hugging Face Inference API            |
-| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)               | Free, Open-Source, OFFLINE, ON-DEVICE                    |
+| Model(s)                          | Source                                                                                                                       | Details                                                  |
+| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)              | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                   | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                        | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open-Source, Hugging Face Inference API            |
+| **Gemma, Gemma-Base**             | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open-Source, Hugging Face Inference API            |
+| **Mistral-Q6, Mistral-Q4**        | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open-Source, OFFLINE, ON-DEVICE                    |
+| **Mistral** [current not working] | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open-Source, Hugging Face Inference API            |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
@@ -79,15 +78,15 @@
 
 Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
 # Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
 $ developergpt --offline cmd [your natural language command request]
 ```
 
-Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini (used by default).  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Pro (used by default).  
 ```bash
 # Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
@@ -121,15 +120,15 @@
 ```bash
 # see available commands
 $ developergpt 
 ```
 
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 60 queries per minute).
+By default, DeveloperGPT uses Google Gemini Pro. To use Gemini Pro, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
 2. Set your Google API Key as an environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
@@ -152,16 +151,17 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Open-Source Hugging-Face Inference API LLMs
-To use open-source LLMs such as Zephyr or OpenChat hosted on Hugging Face, you can optionally set up a [Hugging Face](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token as an environment variable using the steps below. Setting up a token is **not required**, but it will allow you to make more requests without being rate limited. 
+#### Using Open-Source Hugging Face Inference API LLMs
+To use open-source LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+See https://huggingface.co/docs/api-inference/index for more details. 
 
 ```bash
 # [OPTIONAL] set Hugging Face token (using zsh for example)
 # You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
@@ -174,16 +174,17 @@
 
 #### Google Gemini
 As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
-#### Hugging-Face Open-Source LLMs 
-As of December 2023, using Hugging Face LLMs does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
+#### Hugging Face Hosted Open LLMs 
+As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
-- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, tools, quantization, and other resources! 
+- Thanks to Hugging Face and the NLP/LLM community for open-source LLMs, generous free hosted inference API, tools, quantization, and other resources! 
+- Thanks to Google for the generous Gemini Pro API free tier. 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.6.7/developergpt.egg-info/SOURCES.txt` & `developergpt-0.7.0/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.6.7/setup.py` & `developergpt-0.7.0/setup.py`

 * *Files identical despite different names*

