# Comparing `tmp/termax-0.1.1.tar.gz` & `tmp/termax-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termax-0.1.1.tar", last modified: Tue Apr 16 03:36:13 2024, max compression
+gzip compressed data, was "termax-0.1.3.tar", last modified: Tue Apr 23 19:51:49 2024, max compression
```

## Comparing `termax-0.1.1.tar` & `termax-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-16 03:36:04.000000 termax-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 03:36:13.055791 termax-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 03:36:04.000000 termax-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.047791 termax-0.1.1/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 03:36:13.055791 termax-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 03:36:04.000000 termax-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.047791 termax-0.1.1/termax/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 03:36:04.000000 termax-0.1.1/termax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_qianfan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_qianwen.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/termax/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-04-16 03:36:04.000000 termax-0.1.1/termax/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-16 03:36:04.000000 termax-0.1.1/termax/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/function/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/function/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/plugin/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/fish.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/zsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/uninstall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/pricing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/termax/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/termax/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/termax/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 03:36:04.000000 termax-0.1.1/termax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/termax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 19:51:40.000000 termax-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-23 19:51:49.172725 termax-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-23 19:51:40.000000 termax-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.164724 termax-0.1.3/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-23 19:51:49.172725 termax-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-23 19:51:41.000000 termax-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.164724 termax-0.1.3/termax/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:51:41.000000 termax-0.1.3/termax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_qianfan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_qianwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/termax/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-23 19:51:41.000000 termax-0.1.3/termax/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-23 19:51:41.000000 termax-0.1.3/termax/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/function/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/function/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/win.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/plugin/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/fish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/zsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/termax/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-23 19:51:41.000000 termax-0.1.3/termax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/tests/__init__.py
```

### Comparing `termax-0.1.1/LICENSE` & `termax-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/setup.py` & `termax-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/agent/_claude.py` & `termax-0.1.3/termax/agent/_claude.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/agent/_gemini.py` & `termax-0.1.3/termax/agent/_gemini.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/agent/_mistral.py` & `termax-0.1.3/termax/agent/_mistral.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/agent/_openai.py` & `termax-0.1.3/termax/agent/_openai.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,110 @@
 import json
 import importlib.util
 
 from .types import Model
-from termax.prompt import extract_shell_commands
+from termax.prompt import extract_shell_commands, is_url
 from termax.function import get_all_function_schemas, get_all_functions
 
 
 class OpenAIModel(Model):
-    def __init__(self, api_key, version, temperature):
+    def __init__(self, api_key, version, temperature, base_url):
         """
         Initialize the OpenAI model.
         Args:
             api_key (str): The OpenAI API key.
             version (str): The model version.
             temperature (float): The temperature value.
         """
         super().__init__()
 
         dependency = "openai"
         spec = importlib.util.find_spec(dependency)
         if spec is not None:
             self.OpenAI = importlib.import_module(dependency).OpenAI
+            self.RateLimitError = importlib.import_module(dependency).RateLimitError
         else:
             raise ImportError(
                 "It seems you didn't install openai. In order to enable the OpenAI client related features, "
                 "please make sure openai Python package has been installed. "
                 "More information, please refer to: https://openai.com/product"
             )
 
         self.version = version
         self.temperature = temperature
-        self.client = self.OpenAI(api_key=api_key)
+        if is_url(base_url):
+            self.client = self.OpenAI(api_key=api_key, base_url=base_url)
+        else:
+            self.client = self.OpenAI(api_key=api_key)
 
     def guess_command(self, history, prompt):
         """
         Guess the command based on the prompt.
         Args:
             history (str): The history.
             prompt (str): The prompt.
         """
-        completion = self.client.chat.completions.create(
-            model=self.version,
-            messages=[
-                {
-                    "role": "system",
-                    "content": prompt
-                },
-                {
-                    "role": "user",
-                    "content": history,
-                }
-            ],
-            temperature=self.temperature
-        )
-        response = completion.choices[0].message.content
-        return extract_shell_commands(response)
+        try:
+            completion = self.client.chat.completions.create(
+                model=self.version,
+                messages=[
+                    {
+                        "role": "system",
+                        "content": prompt
+                    },
+                    {
+                        "role": "user",
+                        "content": history,
+                    }
+                ],
+                temperature=self.temperature
+            )
+            response = completion.choices[0].message.content
+            return extract_shell_commands(response)
+        except self.RateLimitError as e:
+            print("Rate limit exceeded. Please try again later.")
+            print(f"Error message: {e}")
+        except Exception as e:
+            print("OpenAI error occurred.")
+            print(f"Error message: {e}")
 
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
-        chat_history = [
-            {"role": "system", "content": prompt},
-            {"role": "user", "content": text}
-        ]
-
-        completion = self.client.chat.completions.create(
-            model=self.version,
-            messages=chat_history,
-            temperature=self.temperature,
-            functions=get_all_function_schemas()
-        )
-
-        function = completion.choices[0].message.function_call
-        if function:
-            for f in get_all_functions():
-                if f.openai_schema["name"] == function.name:
-                    return f.execute(**json.loads(function.arguments))
-        else:
-            response = completion.choices[0].message.content
-            return extract_shell_commands(response)
+        try:
+            chat_history = [
+                {"role": "system", "content": prompt},
+                {"role": "user", "content": text}
+            ]
+
+            completion = self.client.chat.completions.create(
+                model=self.version,
+                messages=chat_history,
+                temperature=self.temperature,
+                functions=get_all_function_schemas()
+            )
+
+            function = completion.choices[0].message.function_call
+            if function:
+                for f in get_all_functions():
+                    if f.openai_schema["name"] == function.name:
+                        return f.execute(**json.loads(function.arguments))
+            else:
+                response = completion.choices[0].message.content
+                return extract_shell_commands(response)
+        except self.RateLimitError as e:
+            print("Rate limit exceeded. Please try again later.")
+            print(f"Error message: {e}")
+        except Exception as e:
+            print("OpenAI error occurred.")
+            print(f"Error message: {e}")
 
     def to_description(self, prompt, command):
         """
         Generate a description based on the prompt and command.
         Args:
             prompt (str): The prompt.
             command (str): The command.
```

### Comparing `termax-0.1.1/termax/agent/_qianfan.py` & `termax-0.1.3/termax/agent/_qianfan.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/agent/_qianwen.py` & `termax-0.1.3/termax/agent/_qianwen.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/cli/cli.py` & `termax-0.1.3/termax/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from rich.console import Console
 
 import termax
 from .utils import *
 from termax.utils.const import *
 from termax.prompt import Prompt, Memory
 from termax.plugin import install_plugin, uninstall_plugin
-from termax.utils.metadata import get_command_history
 from termax.utils import Config, CONFIG_PATH, qa_confirm
 
 memory = Memory()
 # avoid the tokenizers parallelism issue
 os.environ['TOKENIZERS_PARALLELISM'] = 'false'
 
 
@@ -76,46 +75,39 @@
 
     platform = config_dict['general']['platform']
     if not configuration.config.has_section(platform):
         click.echo(f"Platform {platform} section not found. Running config setup...")
         build_config()
         config_dict = configuration.read()
 
-    model = load_model()
+    model, platform = load_model()
     # generate the commands from the model, and execute if auto_execute is True
     with console.status(f"[cyan]Guessing..."):
-        def filter_and_format_history(command_history, filter_condition, max_count):
-            """Filter and format command history based on a condition and maximum count."""
-            filtered_history = [f"Command: {entry['command']}\nExecution Date: {entry['time']}\n" for entry in
-                                command_history if filter_condition(entry)][:max_count]
-
-            return "Command History: \n" + "\n".join(filtered_history)
-
-        command_history = get_command_history()['shell_command_history']
-
         # Filter and format history excluding certain commands
         initial_history = filter_and_format_history(
-            command_history,
+            prompt.command_history["shell_command_history"],
             lambda entry: entry['command'] not in ("t guess", "termax guess"),
             COMMAND_HISTORY_COUNT
         )
         # Guess the intent based on the initial history
         prompt_intent = prompt.intent_detect()
         intent = model.guess_command(initial_history, prompt_intent)
+        if not intent: return
 
         # Filter and format history including commands related to the guessed intent
         related_history = filter_and_format_history(
-            command_history,
+            prompt.command_history["shell_command_history"],
             lambda entry: intent in entry['command'],
             COMMAND_HISTORY_COUNT // 3
         )
 
         # Generate suggestions and guess the final command
         prompt_guess = prompt.gen_suggestions(intent)
         command = model.guess_command(related_history, prompt_guess)
+        if not command: return
 
     if config_dict['general']['show_command'] == "True":
         console.log(command, style="purple")
 
     try:
         if config_dict['general']['auto_execute'] == "True":
             execute_command(command)
@@ -160,26 +152,30 @@
     platform = config_dict['general']['platform']
     if not configuration.config.has_section(platform):
         click.echo(f"Platform {platform} section not found. Running config setup...")
         build_config()
         config_dict = configuration.read()
 
     # load the LLM model
-    model = load_model()
-
+    model, platform = load_model()
     # generate the commands from the model, and execute if auto_execute is True
     with console.status(f"[cyan]Generating..."):
         # loop until the generated command is not ''.
-        while True:
-            command = model.to_command(prompt.gen_commands(text), text)
-            if command != '':
+        for i in range(3):
+            command = model.to_command(prompt.gen_commands(text, platform), text)
+            if command == None:
+                return
+            elif command != '':
                 if not command.startswith('t ') and not command.startswith('termax '):
                     break
                 else:
                     text = text + ", do not use command t or termax."
+            if i == 2:
+                console.log("Unable to generate the command, please try again.")
+                return
 
     if print_cmd:
         print(command)
         # TODO: improve the RAG compatibility using the shell plugin.
         # the command generate using the shell plugin will not be saved in the memory.
         # save_command(command, text, config_dict, memory)
     else:
```

### Comparing `termax-0.1.1/termax/cli/utils.py` & `termax-0.1.3/termax/cli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import platform
 import subprocess
 
 from termax.prompt import Memory
-from termax.agent import OpenAIModel, GeminiModel, ClaudeModel, QianFanModel, MistralModel, QianWenModel
+from termax.agent import OpenAIModel, OllamaModel, GeminiModel, ClaudeModel, QianFanModel, MistralModel, QianWenModel
 from termax.utils import Config, qa_general, qa_platform
 from termax.utils.const import *
 
 
 def build_config(general: bool = False):
     """
     build_config: build the configuration for Termax.
@@ -28,81 +28,85 @@
 
 def load_model():
     """
     load_model: load the model based on the configuration.
     """
     configuration = Config()
     config_dict = configuration.read()
-    platform = config_dict['general']['platform']
+    plat = config_dict['general']['platform']
 
-    if platform == CONFIG_SEC_OPENAI:
+    if plat == CONFIG_SEC_OPENAI:
         model = OpenAIModel(
             api_key=config_dict['openai'][CONFIG_SEC_API_KEY], version=config_dict['openai']['model'],
-            temperature=float(config_dict['openai']['temperature'])
+            temperature=float(config_dict['openai']['temperature']), base_url=config_dict['openai']['base_url']
         )
-    elif platform == CONFIG_SEC_GEMINI:
+    elif plat == CONFIG_SEC_OLLAMA:
+        model = OllamaModel(
+            host_url=config_dict['ollama']['host_url'], version=config_dict['ollama']['model'],
+        )
+    elif plat == CONFIG_SEC_GEMINI:
         model = GeminiModel(
             api_key=config_dict['gemini'][CONFIG_SEC_API_KEY], version=config_dict['gemini']['model'],
             generation_config={
                 'stop_sequences': config_dict['gemini']['stop_sequences']
                 if config_dict['gemini']['stop_sequences'] != 'None' else None,
                 'temperature': config_dict['gemini']['temperature'],
                 'top_p': config_dict['gemini']['top_p'],
                 'top_k': config_dict['gemini']['top_k'],
                 'candidate_count': config_dict['gemini']['candidate_count'],
                 'max_output_tokens': config_dict['gemini']['max_tokens']
             }
         )
-    elif platform == CONFIG_SEC_CLAUDE:
+    elif plat == CONFIG_SEC_CLAUDE:
         model = ClaudeModel(
             api_key=config_dict['claude'][CONFIG_SEC_API_KEY], version=config_dict['claude']['model'],
             generation_config={
                 'stop_sequences': config_dict['claude']['stop_sequences']
                 if config_dict['claude']['stop_sequences'] != 'None' else None,
                 'temperature': config_dict['claude']['temperature'],
                 'top_p': config_dict['claude']['top_p'],
                 'top_k': config_dict['claude']['top_k'],
                 'max_tokens': config_dict['claude']['max_tokens']
             }
         )
-    elif platform == CONFIG_SEC_QIANFAN:
+    elif plat == CONFIG_SEC_QIANFAN:
         model = QianFanModel(
             api_key=config_dict['qianfan'][CONFIG_SEC_API_KEY], secret_key=config_dict['qianfan']['secret_key'],
             version=config_dict['qianfan']['model'],
             generation_config={
                 'temperature': config_dict['qianfan']['temperature'],
                 'top_p': config_dict['qianfan']['top_p'],
                 'max_output_tokens': config_dict['qianfan']['max_tokens']
             }
         )
-    elif platform == CONFIG_SEC_MISTRAL:
+    elif plat == CONFIG_SEC_MISTRAL:
         model = MistralModel(
             api_key=config_dict['mistral'][CONFIG_SEC_API_KEY], version=config_dict['mistral']['model'],
             generation_config={
                 'temperature': config_dict['mistral']['temperature'],
                 'top_p': config_dict['mistral']['top_p'],
                 'max_tokens': config_dict['mistral']['max_tokens']
             }
         )
-    elif platform == CONFIG_SEC_QIANWEN:
+    elif plat == CONFIG_SEC_QIANWEN:
         model = QianWenModel(
             api_key=config_dict['qianwen'][CONFIG_SEC_API_KEY], version=config_dict['qianwen']['model'],
             generation_config={
                 'temperature': config_dict['qianwen']['temperature'],
                 'top_p': config_dict['qianwen']['top_p'],
                 'top_k': config_dict['qianwen']['top_k'],
                 'stop': config_dict['qianwen']['stop_sequences']
                 if config_dict['qianwen']['stop_sequences'] != 'None' else None,
                 'max_tokens': config_dict['qianwen']['max_tokens']
             }
         )
     else:
-        raise ValueError(f"Platform {platform} not supported.")
+        raise ValueError(f"Platform {plat} not supported.")
 
-    return model
+    return model, plat
 
 
 def execute_command(command: str) -> bool:
     """
     Execute a command and return whether it was successful.
 
     Args:
@@ -147,7 +151,15 @@
         storage_size = int(config_dict[CONFIG_SEC_GENERAL]['storage_size'])
 
     if memory.count() > storage_size:
         memory.delete()
 
     if command != '':
         memory.add_query(queries=[{"query": text, "response": command}])
+
+
+def filter_and_format_history(command_history, filter_condition, max_count):
+    """Filter and format command history based on a condition and maximum count."""
+    filtered_history = [f"Command: {entry['command']}\nExecution Date: {entry['time']}\n" for entry in
+                        command_history if filter_condition(entry)][:max_count]
+
+    return "Command History: \n" + "\n".join(filtered_history)
```

### Comparing `termax-0.1.1/termax/function/openai/git.py` & `termax-0.1.3/termax/function/openai/git.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/function/openai/macos.py` & `termax-0.1.3/termax/function/openai/macos.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/plugin/install.py` & `termax-0.1.3/termax/plugin/install.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/plugin/shell/bash.py` & `termax-0.1.3/termax/plugin/shell/bash.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         set +m
         local _termax_prev_line="$READLINE_LINE"
         { spin 5 & } 2>/dev/null
         SPIN_PID=$!
 
         READLINE_LINE=$(t termax -p "$_termax_prev_line")
         kill "$SPIN_PID"
-        printf "\r%s" "DONE.         "
+        printf "\r%s" "                 "
         echo " "
         READLINE_POINT=${#READLINE_LINE}
     fi
 }
 spin() {
     local -a marks=('⠋ Generating.' '⠙ Generating..' '⠹ Generating...' '⠸ Generating.' '⠼ Generating..' '⠴ Generating...' '⠦ Generating.' '⠧ Generating..' '⠇ Generating...' '⠏ Generating...')
     local i=0
```

### Comparing `termax-0.1.1/termax/plugin/shell/fish.py` & `termax-0.1.3/termax/plugin/shell/fish.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/plugin/shell/zsh.py` & `termax-0.1.3/termax/plugin/shell/zsh.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/plugin/uninstall.py` & `termax-0.1.3/termax/plugin/uninstall.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/prompt/memory.py` & `termax-0.1.3/termax/prompt/memory.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.1/termax/prompt/prompt.py` & `termax-0.1.3/termax/prompt/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             primary_data = 'None'
 
         files = get_file_metadata()
         if model == CONFIG_SEC_OPENAI:
             return textwrap.dedent(
                 f"""\
                 You are an shell expert, you need to infer the next command based on the provided list
-                 of command history entries.
+                of command history entries.
                 
                 [INFORMATION] The user's current system information:
                 
                 1. OS: {self.system_metadata['platform']}
                 2. OS Version: {self.system_metadata['platform_version']}
                 3. Architecture: {self.system_metadata['architecture']}
                 
@@ -220,15 +220,15 @@
             User Input: {documents[i]}
             Generated Commands: {metadatas[i]['response']}
             Distance Score: {distances[i]}
             Date: {metadatas[i]['created_at']}\n
             """
 
         # refresh the metadata
-        self.command_history = get_command_history()
+        files = get_file_metadata()
         if model == CONFIG_SEC_OPENAI:
             return textwrap.dedent(
                 f"""\
                 You are an shell expert, you can convert natural language text from user to shell commands.
                 
                 1. Please provide only shell commands for os without any description.
                 2. Ensure the output is a valid shell command.
@@ -238,51 +238,67 @@
 
                 1. The commands should be able to run on the current system according to the system information.
                 2. The files in the commands should be available in the path, according to the path information.
                 3. The CLI application should be installed in the system (check the path information).
 
                 Here are some information you may need to know:
                 
-                Current system information (in dict format): {self.system_metadata}
-                
-                The user's system PATH information (in dict format): {self.path_metadata}
-                
-                The user's command history: {self.command_history["shell_command_history"][:15]}
+                [INFORMATION] The user's current system information:
+                1. OS: {self.system_metadata['platform']}
+                2. OS Version: {self.system_metadata['platform_version']}
+                3. Architecture: {self.system_metadata['architecture']}
                 
+                [INFORMATION] The user's current PATH information:
+                1. User: {self.path_metadata['user']}
+                2. Current PATH: {self.path_metadata['current_directory']}
+                3. Files under the current directory: {files['files']}
+                4. Directories under the current directory: {files['directory']}
+                5. Invisible files under the current directory: {files['invisible_files']}
+                6. Invisible directories under the current directory: {files['invisible_directory']}
+    
                 Here are some similar commands generated before:
-                
                 {sample_string}
+
+                The output shell commands is (please replace the `{{commands}}` with the actual commands):
+
+                Commands: ${{commands}}
                 """
             )
         else:
             # TODO: add more models specific prompt
             return textwrap.dedent(
                 f"""\
-                You are an shell expert, you can convert this text to shell commands.
+                You are an shell expert, you can convert natural language text from user to shell commands.
                 
-                1. Please provide only shell commands for os without any description.
+                1. Please provide only shell commands for os without any extra description.
                 2. Ensure the output is a valid shell command.
                 3. If multiple steps required try to combine them together.
                 
                 Here are some rules you need to follow:
-                
+
                 1. The commands should be able to run on the current system according to the system information.
                 2. The files in the commands should be available in the path, according to the path information.
                 3. The CLI application should be installed in the system (check the path information).
-                
-                Here are some information you may need to know:
 
-                Current system information (in dict format): {self.system_metadata}
+                Here are some information you may need to know:
                 
-                The user's system PATH information (in dict format): {self.path_metadata}
+                [INFORMATION] The user's current system information:
+                1. OS: {self.system_metadata['platform']}
+                2. OS Version: {self.system_metadata['platform_version']}
+                3. Architecture: {self.system_metadata['architecture']}
                 
-                The user's command history: {self.command_history["shell_command_history"][:15]}
+                [INFORMATION] The user's current PATH information:
+                1. User: {self.path_metadata['user']}
+                2. Current PATH: {self.path_metadata['current_directory']}
+                3. Files under the current directory: {files['files']}
+                4. Directories under the current directory: {files['directory']}
+                5. Invisible files under the current directory: {files['invisible_files']}
+                6. Invisible directories under the current directory: {files['invisible_directory']}
                 
                 Here are some similar commands generated before:
-
                 {sample_string}
                 
                 The output shell commands is (please replace the `{{commands}}` with the actual commands):
 
                 Commands: ${{commands}}
                 """
             )
```

### Comparing `termax-0.1.1/termax/prompt/utils.py` & `termax-0.1.3/termax/prompt/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from urllib.parse import urlparse
 
 
 def extract_code_from_markdown(markdown_text, separator="\n\n"):
     """
     Extracts code blocks from a markdown text.
     :param markdown_text:  the markdown text.
     :param separator: the separator to join the code blocks.
@@ -44,21 +45,57 @@
     """
     processed_text = re.sub(r'^\s*osascript -e\s*', '', text)
     if (processed_text.startswith('"') and processed_text.endswith('"')) or (processed_text.startswith("'") and processed_text.endswith("'")):
         processed_text = remove_quotes(processed_text)
     return f"'{processed_text}'"
 
 
+def process_powershell_script(text):
+    """
+    Process a PowerShell script string to remove extra quotes and ensure it's wrapped within a single pair of double quotes.
+
+    Args:
+    - text (str): The input text potentially containing multiple quotes.
+
+    Returns:
+    - str: The processed text wrapped within double quotes.
+    """
+    processed_text = re.sub(r'^\s*powershell -Command\s*', '', text)
+    if (text.startswith('"') and text.endswith('"')) or (text.startswith("'") and text.endswith("'")):
+        processed_text = remove_quotes(text)
+    else:
+        processed_text = text
+    return f'"{processed_text}"'
+
+
 def remove_quotes(input_string):
     """
     Remove all single and double quotes from the beginning and end of the input string.
 
     Args:
     - input_string (str): The string from which to remove leading and trailing quotes.
 
     Returns:
     - str: The modified string with leading and trailing quotes removed.
     """
     # Use a regular expression to remove leading and trailing quotes
     # The pattern looks for quotes at the start (^["']+) and end (["']+$) of the string and removes them
     modified_string = re.sub(r'^["\']+|["\']+$', '', input_string)
     return modified_string
+
+
+def is_url(string):
+    """
+    Check if a string is a valid URL.
+
+    Args:
+    - string (str): The string to check.
+
+    Returns:
+    - bool: True if the string is a valid URL, False otherwise.
+    """
+    try:
+        result = urlparse(string)
+        # Check if the parsing succeeded and scheme and netloc are present
+        return all([result.scheme, result.netloc])
+    except ValueError:
+        return False
```

### Comparing `termax-0.1.1/termax/utils/config.py` & `termax-0.1.3/termax/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         """
         write_platform: indicate and generate the platform related configuration.
 
         @param config_dict: the configuration dictionary.
         @param platform: the platform to configure.
 
         """
+        del config_dict['platform']
         # create the configuration to connect with OpenAI.
         if not self.config.has_section(platform):
             self.config.add_section(platform)
 
         self.config[platform] = config_dict
 
         # save the new configuration and reload.
```

### Comparing `termax-0.1.1/termax/utils/const.py` & `termax-0.1.3/termax/utils/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 CONFIG_SEC_GENERAL = 'general'
 CONFIG_SEC_API_KEY = 'api_key'
 CONFIG_LLM_LIST = {  # with the default model.
     'OpenAI': 'gpt-3.5-turbo',
+    'Ollama': 'llama2',
     'Gemini': 'gemini-pro',
     'Claude': 'claude-3-opus-20240229',
     'Mistral': 'mistral-small-latest',
     'Qianfan': 'ERNIE-3.5-8K',
     'Qianwen': 'qwen-turbo'
 }
 
 COMMAND_HISTORY_COUNT = 15
 DB_PATH = 'database'
 DB_COMMAND_HISTORY = 'history'
 DB_SYS_METRICS = 'system'
 
 # LLMs
 CONFIG_SEC_OPENAI = 'openai'
+CONFIG_SEC_OLLAMA = 'ollama'
 CONFIG_SEC_GEMINI = 'gemini'
 CONFIG_SEC_CLAUDE = 'claude'
 CONFIG_SEC_MISTRAL = 'mistral'
 CONFIG_SEC_QIANFAN = 'qianfan'
 CONFIG_SEC_QIANWEN = 'qianwen'
 
 # Plugins
```

### Comparing `termax-0.1.1/termax/utils/metadata.py` & `termax-0.1.3/termax/utils/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 import os
 import sys
-import pwd
 import psutil
 import socket
 import shutil
 import getpass
 import platform
 import subprocess
 from datetime import datetime
@@ -302,14 +301,15 @@
     """
     get_command_history: Get the command history of the current user including command times for zsh.
 
     :return: A list of dictionaries with 'command' and optionally 'time' keys, where 'time' is in datetime format.
     """
     if sys.platform.startswith('linux') or sys.platform == 'darwin':
         # Attempt to detect the default shell from the $SHELL environment variable or /etc/passwd
+        import pwd
         shell = os.environ.get('SHELL', pwd.getpwnam(getpass.getuser()).pw_shell)
 
         if 'bash' in shell:
             shell_type = 'bash'
             history_file = os.path.join(os.environ['HOME'], '.bash_history')
             history_format = 'plain'
         elif 'zsh' in shell:
```

### Comparing `termax-0.1.1/termax/utils/qa.py` & `termax-0.1.3/termax/utils/qa.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,45 +6,71 @@
     """
     qa_platform: ask the user to input the platform related configuration.
 
     Args:
         model_list: the list of models.
     """
     try:
-        first_questions = [
+        # Prompt for platform selection
+        platform_question = [
             inquirer.List(
                 "platform",
-                message="What LLM (platform) are you setting?",
+                message="What LLM (platform) are you setting",
                 choices=model_list.keys()
             )
         ]
-        answers_1 = inquirer.prompt(first_questions)
-        selected_platform = answers_1['platform']
+        platform_answer = inquirer.prompt(platform_question)
+        if not platform_answer:
+            return None
+
+        selected_platform = platform_answer['platform']
 
-        second_questions = [
+        # Setup questions based on the selected platform
+        other_questions = [
             inquirer.Text(
-                CONFIG_SEC_API_KEY,
-                message=f"What is your {selected_platform} API key?",
+                'host_url' if selected_platform == 'Ollama' else CONFIG_SEC_API_KEY,
+                message=f"[OPTIONAL] What is your {selected_platform} HOST url"
+                if selected_platform == 'Ollama' else f"What is your {selected_platform} API key"
+            ),
+            inquirer.Text(
+                'model',
+                message=f"Which model are you using for {selected_platform}",
+                default=model_list[selected_platform]
             )
         ]
-        answers_2 = inquirer.prompt(second_questions)
-        if answers_2:
-            return {
-                "model": model_list[selected_platform],
-                "platform": selected_platform.lower(),
-                "api_key": answers_2[CONFIG_SEC_API_KEY],
-                'temperature': 0.7,
-                'max_tokens': 1500,
-                'top_p': 1.0,
-                'top_k': 32,
-                'stop_sequences': 'None',
-                'candidate_count': 1
-            }
-        else:
+
+        if selected_platform == 'OpenAI':
+            other_questions.append(
+                inquirer.Text(
+                    'base_url',
+                    message=f"[OPTIONAL] What is the base url for {selected_platform}"
+                )
+            )
+
+        # Gather responses to other questions
+        answers = inquirer.prompt(other_questions)
+        if not answers:
             return None
+
+        # Configuration dictionary
+        config_dict = {
+            'platform': selected_platform.lower(),
+            'model': answers['model'],
+            'temperature': 0.7,
+            'max_tokens': 1500,
+            'top_p': 1.0,
+            'top_k': 32,
+            'stop_sequences': 'None',
+            'candidate_count': 1,
+            'api_key': answers.get(CONFIG_SEC_API_KEY) if selected_platform != 'Ollama' else 'None',
+            'host_url': answers.get('host_url') if selected_platform == 'Ollama' else 'None',
+            'base_url': answers.get('base_url') if selected_platform == 'OpenAI' else 'None'
+        }
+
+        return config_dict
     except TypeError:
         return None
 
 
 def qa_general(model_list: dict = CONFIG_LLM_LIST):
     """
     qa_general: ask the user to input the general configuration.
```

### Comparing `termax-0.1.1/termax.egg-info/SOURCES.txt` & `termax-0.1.3/termax.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 termax.egg-info/entry_points.txt
 termax.egg-info/requires.txt
 termax.egg-info/top_level.txt
 termax/agent/__init__.py
 termax/agent/_claude.py
 termax/agent/_gemini.py
 termax/agent/_mistral.py
+termax/agent/_ollama.py
 termax/agent/_openai.py
 termax/agent/_qianfan.py
 termax/agent/_qianwen.py
 termax/agent/types.py
 termax/cli/__init__.py
 termax/cli/cli.py
 termax/cli/utils.py
 termax/function/__init__.py
 termax/function/base.py
 termax/function/openai/__init__.py
 termax/function/openai/git.py
 termax/function/openai/macos.py
 termax/function/openai/shell.py
+termax/function/openai/win.py
 termax/plugin/__init__.py
 termax/plugin/install.py
 termax/plugin/uninstall.py
 termax/plugin/shell/__init__.py
 termax/plugin/shell/bash.py
 termax/plugin/shell/fish.py
 termax/plugin/shell/zsh.py
```

