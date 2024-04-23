# Comparing `tmp/python_tgpt-0.6.3.tar.gz` & `tmp/python_tgpt-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.6.3.tar", last modified: Mon Apr 15 09:54:57 2024, max compression
+gzip compressed data, was "python_tgpt-0.6.4.tar", last modified: Tue Apr 23 10:48:57 2024, max compression
```

## Comparing `python_tgpt-0.6.3.tar` & `python_tgpt-0.6.4.tar`

### file list

```diff
@@ -1,89 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.125254 python_tgpt-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-04-15 09:54:57.125254 python_tgpt-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-15 09:54:56.000000 python_tgpt-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:54:57.125254 python_tgpt-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.109254 python_tgpt-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12207 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    80577 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.113254 python_tgpt-0.6.3/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.117254 python_tgpt-0.6.3/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.121254 python_tgpt-0.6.3/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 09:54:57.000000 python_tgpt-0.6.3/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:54:57.121254 python_tgpt-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 09:54:27.000000 python_tgpt-0.6.3/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.814113 python_tgpt-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-23 10:48:57.814113 python_tgpt-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:48:57.814113 python_tgpt-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.798114 python_tgpt-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81305 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.810114 python_tgpt-0.6.4/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.810114 python_tgpt-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_webchatgpt.py
```

### Comparing `python_tgpt-0.6.3/LICENSE` & `python_tgpt-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/PKG-INFO` & `python_tgpt-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.3
+Version: 0.6.4
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: webchatgpt==0.2.9
+Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
 Requires-Dist: g4f>=0.2.6.1
 Requires-Dist: Helpingai-T2==0.3
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
@@ -140,15 +140,15 @@
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-uc.a.run.app/)
 4. [OpenAI](https://chat.openai.com) *(API key required)*
 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)*
 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session ID required)*
-9. [Phind](https://www.phind.com) - *default*
+9. [Phind](https://www.phind.com)
 10. [Llama2](https://www.llama2.ai)
 11. [Blackboxai](https://www.blackbox.ai)
 12. [gpt4all](https://gpt4all.io) *(Offline)*
 13. [Poe](https://poe.com) - Poe|Quora *(Session ID required)*
 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai)
 
@@ -296,68 +296,68 @@
 {'completion': "I'm so excited to share with you the incredible experiences...", 'stop_reason': None, 'truncated': False, 'stop': None, 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 """
 ```
 
 <details>
 
 <summary>
-Openai
+Auto - *(selects any working provider)*
 
 </summary>
 
 ```python
-import pytgpt.openai as openai
-bot = openai.OPENAI("<OPENAI-API-KEY>")
+import pytgpt.auto import auto
+bot = auto.AUTO()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
-
 <details>
 
 <summary>
-Koboldai
+Openai
 
 </summary>
 
 ```python
-import pytgpt.koboldai as koboldai
-bot = koboldai.KOBOLDAI()
+import pytgpt.openai as openai
+bot = openai.OPENAI("<OPENAI-API-KEY>")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 
 <details>
 
 <summary>
-Opengpt
+Koboldai
 
 </summary>
 
 ```python
-import pytgpt.opengpt as opengpt
-bot = opengpt.OPENGPT()
+import pytgpt.koboldai as koboldai
+bot = koboldai.KOBOLDAI()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
+
 <details>
 
 <summary>
-Bard
+Opengpt
 
 </summary>
 
 ```python
-import pytgpt.bard as bard
-bot = bard.BARD('<Path-to-bard.google.com.cookies.json>')
+import pytgpt.opengpt as opengpt
+bot = opengpt.OPENGPT()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 <details>
 
@@ -379,15 +379,15 @@
 <summary>
 Gpt4free providers
 
 </summary>
 
 ```python
 import pytgpt.gpt4free as gpt4free
-bot = gpt4free.GPT4FREE(provider="Aura")
+bot = gpt4free.GPT4FREE(provider="Koala")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.3 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.4 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -17,15 +17,15 @@
 Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist:
-pyyaml==6.0.1 Requires-Dist: webchatgpt==0.2.9 Requires-Dist:
+pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
 brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3
 Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
 rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
 extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
 python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
@@ -65,17 +65,17 @@
 [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 ## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
 (https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
 tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
 uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
 [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
 required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
-//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
-//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
+ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
+www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
+gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
 required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
 [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
 run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
 (https://python.org) *(Optional)* ## Installation and Usage ### Installation
 Download binaries for your system from [here.](https://github.com/Simatwa/
 python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
@@ -112,47 +112,48 @@
 chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 {'completion': "I'm so excited to share with you the incredible ",
 'stop_reason': None, 'truncated': False, 'stop': None, 'model': 'llama-2-13b-
 chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx',
-'exception': None} """ ``` Openai ```python import pytgpt.openai as openai bot
-= openai.OPENAI("") print(bot.chat("")) ``` Koboldai ```python import
-pytgpt.koboldai as koboldai bot = koboldai.KOBOLDAI() print(bot.chat("")) ```
-Opengpt ```python import pytgpt.opengpt as opengpt bot = opengpt.OPENGPT()
-print(bot.chat("")) ``` Bard ```python import pytgpt.bard as bard bot =
-bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgpt.phind as
-phind bot = phind.PHIND() print(bot.chat("")) ``` Gpt4free providers ```python
-import pytgpt.gpt4free as gpt4free bot = gpt4free.GPT4FREE(provider="Aura")
-print(bot.chat("")) ``` To obtain more tailored responses, consider utilizing
-[optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can
-be set to either `code` or `system_command`. ```python from pytgpt.leo import
-LEO bot = LEO() resp = bot.ask('', optimizer='code') print(resp) ``` >
-[!IMPORTANT] > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/
-releases/), the default mode of interaction is conversational. This mode
-enhances the interactive experience, offering better control over the chat
-history. By associating previous prompts and responses, it tailors
-conversations for a more engaging experience. You can still disable the mode:
-```python bot = koboldai.KOBOLDAI(is_conversation=False) ``` Utilize the `--
-disable-conversation` flag in the console to achieve the same functionality. >
-[!CAUTION] > **Bard** autohandles context due to the obvious reason; the
-`is_conversation` parameter is not necessary at all hence not required when
-initializing the class. Also be informed that majority of providers offered by
-*gpt4free* requires *Google Chrome* inorder to function. ### Image Generation
-This has been made possible by [pollinations.ai](https://pollination.ai). ```sh
-$ pytgpt imager "" # e.g pytgpt imager "Coding bot" ``` Developers ```python
-from pytgpt.imager import Imager img = Imager() generated_img = img.generate
-('Coding bot') # [bytes] img.save(generated_img) ``` Download Multiple Images
-```python from pytgpt.imager import Imager img = Imager() img_generator =
-img.generate('Coding bot', amount=3, stream=True) img.save(img_generator) # RAM
-friendly ``` ### Advanced Usage of Placeholders The `generate` functionality
-has been enhanced starting from *v0.3.0* to enable comprehensive utilization of
-the `--with-copied` option and support for accepting piped inputs. This
-improvement introduces placeholders, offering dynamic values for more versatile
+'exception': None} """ ``` Auto - *(selects any working provider)* ```python
+import pytgpt.auto import auto bot = auto.AUTO() print(bot.chat("")) ``` Openai
+```python import pytgpt.openai as openai bot = openai.OPENAI("") print(bot.chat
+("")) ``` Koboldai ```python import pytgpt.koboldai as koboldai bot =
+koboldai.KOBOLDAI() print(bot.chat("")) ``` Opengpt ```python import
+pytgpt.opengpt as opengpt bot = opengpt.OPENGPT() print(bot.chat("")) ``` phind
+```python import pytgpt.phind as phind bot = phind.PHIND() print(bot.chat(""))
+``` Gpt4free providers ```python import pytgpt.gpt4free as gpt4free bot =
+gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` To obtain more
+tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the
+`optimizer` parameter. Its values can be set to either `code` or
+`system_command`. ```python from pytgpt.leo import LEO bot = LEO() resp =
+bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] > Commencing from
+[v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of
+interaction is conversational. This mode enhances the interactive experience,
+offering better control over the chat history. By associating previous prompts
+and responses, it tailors conversations for a more engaging experience. You can
+still disable the mode: ```python bot = koboldai.KOBOLDAI
+(is_conversation=False) ``` Utilize the `--disable-conversation` flag in the
+console to achieve the same functionality. > [!CAUTION] > **Bard** autohandles
+context due to the obvious reason; the `is_conversation` parameter is not
+necessary at all hence not required when initializing the class. Also be
+informed that majority of providers offered by *gpt4free* requires *Google
+Chrome* inorder to function. ### Image Generation This has been made possible
+by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
+pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
+Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
+img.save(generated_img) ``` Download Multiple Images ```python from
+pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
+bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ###
+Advanced Usage of Placeholders The `generate` functionality has been enhanced
+starting from *v0.3.0* to enable comprehensive utilization of the `--with-
+copied` option and support for accepting piped inputs. This improvement
+introduces placeholders, offering dynamic values for more versatile
 interactions. | Placeholder | Represents | | ------------ | ----------- | | `{
 {stream}}` | The piped input | | `{{copied}}` | The last copied text | This
 feature is particularly beneficial for intricate operations. For example:
 ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a
 concise commit message from it, aligning with my commit message history: {
 {copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
 result of the `$ git diff` operation, while `{{copied}}` signifies the content
```

### Comparing `python_tgpt-0.6.3/README.md` & `python_tgpt-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-uc.a.run.app/)
 4. [OpenAI](https://chat.openai.com) *(API key required)*
 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)*
 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session ID required)*
-9. [Phind](https://www.phind.com) - *default*
+9. [Phind](https://www.phind.com)
 10. [Llama2](https://www.llama2.ai)
 11. [Blackboxai](https://www.blackbox.ai)
 12. [gpt4all](https://gpt4all.io) *(Offline)*
 13. [Poe](https://poe.com) - Poe|Quora *(Session ID required)*
 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai)
 
@@ -231,68 +231,68 @@
 {'completion': "I'm so excited to share with you the incredible experiences...", 'stop_reason': None, 'truncated': False, 'stop': None, 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 """
 ```
 
 <details>
 
 <summary>
-Openai
+Auto - *(selects any working provider)*
 
 </summary>
 
 ```python
-import pytgpt.openai as openai
-bot = openai.OPENAI("<OPENAI-API-KEY>")
+import pytgpt.auto import auto
+bot = auto.AUTO()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
-
 <details>
 
 <summary>
-Koboldai
+Openai
 
 </summary>
 
 ```python
-import pytgpt.koboldai as koboldai
-bot = koboldai.KOBOLDAI()
+import pytgpt.openai as openai
+bot = openai.OPENAI("<OPENAI-API-KEY>")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 
 <details>
 
 <summary>
-Opengpt
+Koboldai
 
 </summary>
 
 ```python
-import pytgpt.opengpt as opengpt
-bot = opengpt.OPENGPT()
+import pytgpt.koboldai as koboldai
+bot = koboldai.KOBOLDAI()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
+
 <details>
 
 <summary>
-Bard
+Opengpt
 
 </summary>
 
 ```python
-import pytgpt.bard as bard
-bot = bard.BARD('<Path-to-bard.google.com.cookies.json>')
+import pytgpt.opengpt as opengpt
+bot = opengpt.OPENGPT()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 <details>
 
@@ -314,15 +314,15 @@
 <summary>
 Gpt4free providers
 
 </summary>
 
 ```python
 import pytgpt.gpt4free as gpt4free
-bot = gpt4free.GPT4FREE(provider="Aura")
+bot = gpt4free.GPT4FREE(provider="Koala")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 </details>
```

#### html2text {}

```diff
@@ -26,17 +26,17 @@
 [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 ## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
 (https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
 tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
 uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
 [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
 required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
-//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
-//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
+ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
+www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
+gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
 required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
 [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
 run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
 (https://python.org) *(Optional)* ## Installation and Usage ### Installation
 Download binaries for your system from [here.](https://github.com/Simatwa/
 python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
@@ -73,47 +73,48 @@
 chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 {'completion': "I'm so excited to share with you the incredible ",
 'stop_reason': None, 'truncated': False, 'stop': None, 'model': 'llama-2-13b-
 chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx',
-'exception': None} """ ``` Openai ```python import pytgpt.openai as openai bot
-= openai.OPENAI("") print(bot.chat("")) ``` Koboldai ```python import
-pytgpt.koboldai as koboldai bot = koboldai.KOBOLDAI() print(bot.chat("")) ```
-Opengpt ```python import pytgpt.opengpt as opengpt bot = opengpt.OPENGPT()
-print(bot.chat("")) ``` Bard ```python import pytgpt.bard as bard bot =
-bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgpt.phind as
-phind bot = phind.PHIND() print(bot.chat("")) ``` Gpt4free providers ```python
-import pytgpt.gpt4free as gpt4free bot = gpt4free.GPT4FREE(provider="Aura")
-print(bot.chat("")) ``` To obtain more tailored responses, consider utilizing
-[optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can
-be set to either `code` or `system_command`. ```python from pytgpt.leo import
-LEO bot = LEO() resp = bot.ask('', optimizer='code') print(resp) ``` >
-[!IMPORTANT] > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/
-releases/), the default mode of interaction is conversational. This mode
-enhances the interactive experience, offering better control over the chat
-history. By associating previous prompts and responses, it tailors
-conversations for a more engaging experience. You can still disable the mode:
-```python bot = koboldai.KOBOLDAI(is_conversation=False) ``` Utilize the `--
-disable-conversation` flag in the console to achieve the same functionality. >
-[!CAUTION] > **Bard** autohandles context due to the obvious reason; the
-`is_conversation` parameter is not necessary at all hence not required when
-initializing the class. Also be informed that majority of providers offered by
-*gpt4free* requires *Google Chrome* inorder to function. ### Image Generation
-This has been made possible by [pollinations.ai](https://pollination.ai). ```sh
-$ pytgpt imager "" # e.g pytgpt imager "Coding bot" ``` Developers ```python
-from pytgpt.imager import Imager img = Imager() generated_img = img.generate
-('Coding bot') # [bytes] img.save(generated_img) ``` Download Multiple Images
-```python from pytgpt.imager import Imager img = Imager() img_generator =
-img.generate('Coding bot', amount=3, stream=True) img.save(img_generator) # RAM
-friendly ``` ### Advanced Usage of Placeholders The `generate` functionality
-has been enhanced starting from *v0.3.0* to enable comprehensive utilization of
-the `--with-copied` option and support for accepting piped inputs. This
-improvement introduces placeholders, offering dynamic values for more versatile
+'exception': None} """ ``` Auto - *(selects any working provider)* ```python
+import pytgpt.auto import auto bot = auto.AUTO() print(bot.chat("")) ``` Openai
+```python import pytgpt.openai as openai bot = openai.OPENAI("") print(bot.chat
+("")) ``` Koboldai ```python import pytgpt.koboldai as koboldai bot =
+koboldai.KOBOLDAI() print(bot.chat("")) ``` Opengpt ```python import
+pytgpt.opengpt as opengpt bot = opengpt.OPENGPT() print(bot.chat("")) ``` phind
+```python import pytgpt.phind as phind bot = phind.PHIND() print(bot.chat(""))
+``` Gpt4free providers ```python import pytgpt.gpt4free as gpt4free bot =
+gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` To obtain more
+tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the
+`optimizer` parameter. Its values can be set to either `code` or
+`system_command`. ```python from pytgpt.leo import LEO bot = LEO() resp =
+bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] > Commencing from
+[v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of
+interaction is conversational. This mode enhances the interactive experience,
+offering better control over the chat history. By associating previous prompts
+and responses, it tailors conversations for a more engaging experience. You can
+still disable the mode: ```python bot = koboldai.KOBOLDAI
+(is_conversation=False) ``` Utilize the `--disable-conversation` flag in the
+console to achieve the same functionality. > [!CAUTION] > **Bard** autohandles
+context due to the obvious reason; the `is_conversation` parameter is not
+necessary at all hence not required when initializing the class. Also be
+informed that majority of providers offered by *gpt4free* requires *Google
+Chrome* inorder to function. ### Image Generation This has been made possible
+by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
+pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
+Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
+img.save(generated_img) ``` Download Multiple Images ```python from
+pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
+bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ###
+Advanced Usage of Placeholders The `generate` functionality has been enhanced
+starting from *v0.3.0* to enable comprehensive utilization of the `--with-
+copied` option and support for accepting piped inputs. This improvement
+introduces placeholders, offering dynamic values for more versatile
 interactions. | Placeholder | Represents | | ------------ | ----------- | | `{
 {stream}}` | The piped input | | `{{copied}}` | The last copied text | This
 feature is particularly beneficial for intricate operations. For example:
 ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a
 concise commit message from it, aligning with my commit message history: {
 {copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
 result of the `$ git diff` operation, while `{{copied}}` signifies the content
```

### Comparing `python_tgpt-0.6.3/setup.py` & `python_tgpt-0.6.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages
 
 
 INSTALL_REQUIRE = [
     "requests[socks]==2.31.0",
     "appdirs==1.4.4",
     "pyyaml==6.0.1",
-    "webchatgpt==0.2.9",
+    "webchatgpt==0.3.0",
     "GoogleBard1>=2.1.4",
     "poe-api-wrapper==1.3.6",
     "brotli==1.1.0",
     "g4f>=0.2.6.1",
     "Helpingai-T2==0.3",
 ]
 
@@ -42,15 +42,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.3",
+    version="0.6.4",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.6.3/src/pytgpt/__init__.py` & `python_tgpt-0.6.4/src/pytgpt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 except metadata.PackageNotFoundError:
     __version__ = "0.0.0"
 
 __author__ = "Smartwa"
 __repo__ = "https://github.com/Simatwa/python-tgpt"
 
 tgpt_providers = [
+    "auto",
     "leo",
     "openai",
     "opengpt",
     "koboldai",
     "gemini",
     "phind",
     "llama2",
```

### Comparing `python_tgpt-0.6.3/src/pytgpt/api/__init__.py` & `python_tgpt-0.6.4/src/pytgpt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/api/utils.py` & `python_tgpt-0.6.4/src/pytgpt/api/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/api/v1.py` & `python_tgpt-0.6.4/src/pytgpt/api/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 from pytgpt.opengpt import OPENGPT
 from pytgpt.koboldai import KOBOLDAI
 from pytgpt.phind import PHIND
 from pytgpt.llama2 import LLAMA2
 from pytgpt.blackboxai import BLACKBOXAI
 from pytgpt.perplexity import PERPLEXITY
 from pytgpt.gpt4free import GPT4FREE
+from pytgpt.auto import AUTO
 from pytgpt.imager import Imager
 from pytgpt.utils import api_static_image_dir
 
 provider_map = {
     "leo": LEO,
     "opengpt": OPENGPT,
     "koboldai": KOBOLDAI,
     "phind": PHIND,
     "llama2": LLAMA2,
     "blackboxai": BLACKBOXAI,
     "perplexity": PERPLEXITY,
+    "auto": AUTO,
 }
 
 supported_providers = list(provider_map.keys()) + gpt4free_providers
 
 app = APIRouter()
 
 
@@ -53,27 +55,27 @@
             ]
         }
     }
 
 
 class UserPayload(BaseModel):
     prompt: str
-    provider: str = "phind"
+    provider: str = "auto"
     # is_conversation: bool = False
     whole: bool = False
     max_tokens: PositiveInt = 600
     timeout: PositiveInt = 30
     proxy: Union[dict[str, str], None] = None
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
                     "prompt": "Hello there",
-                    "provider": "phind",
+                    "provider": "auto",
                     "whole": False,
                     "max_tokens": 600,
                     "timeout": 30,
                     "proxy": {
                         "http": "socks4://38.54.6.39:4000",
                         "https": "socks4://38.54.6.39:4000",
                     },
@@ -258,27 +260,35 @@
     *Ensure `proxy` value is correct otherwise make it `null`*
 
     **NOTE** : Example values are modified for illustration purposes.
     """
     provider_obj: LEO = init_provider(payload)
     ai_generated_text: str = provider_obj.chat(payload.prompt)
     return ProviderResponse(
-        provider=payload.provider,
-        text=None if payload.whole else ai_generated_text,
+        provider=(
+            provider_obj.provider_name
+            if payload.provider == "auto"
+            else payload.provider
+        ),
+        text=ai_generated_text,
         body=provider_obj.last_response if payload.whole else None,
     )
 
 
 def generate_streaming_response(payload: UserPayload) -> Generator:
     provider_obj: LEO = init_provider(payload)
 
     for text in provider_obj.chat(payload.prompt, stream=True):
         response = ProviderResponse(
-            provider=payload.provider,
-            text=None if payload.whole else text,
+            provider=(
+                provider_obj.provider_name
+                if payload.provider == "auto"
+                else payload.provider
+            ),
+            text=text,
             body=provider_obj.last_response if payload.whole else None,
         )
         yield dumps(jsonable_encoder(response)) + "\n"
 
 
 @app.post("/chat/stream", name="stream", response_model=ProviderResponse)
 @api_exception_handler
```

### Comparing `python_tgpt-0.6.3/src/pytgpt/base.py` & `python_tgpt-0.6.4/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.6.4/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/console.py` & `python_tgpt-0.6.4/src/pytgpt/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 class this:
     """Console's common variables"""
 
     rich_code_themes = ["monokai", "paraiso-dark", "igor", "vs", "fruity", "xcode"]
 
-    default_provider = "phind"
+    default_provider = "auto"
 
     getExc = lambda e: e.args[1] if len(e.args) > 1 else str(e)
 
     context_settings = dict(auto_envvar_prefix="PYTGPT")
 
     """Console utils"""
 
@@ -378,21 +378,36 @@
                     confirm_script=confirm_script,
                     interpreter=interpreter,
                     prettify=True,
                 )
                 intro = self.RawDog.intro_prompt
                 getpass.getuser = lambda: "RawDog"
 
-            if provider == "g4fauto":
+            if provider == "auto":
+                from pytgpt.auto import AUTO
+
+                self.bot = AUTO(
+                    is_conversation=disable_conversation,
+                    max_tokens=max_tokens,
+                    timeout=timeout,
+                    intro=intro,
+                    filepath=filepath,
+                    update_file=update_file,
+                    proxies=proxies,
+                    history_offset=history_offset,
+                    act=awesome_prompt,
+                )
+
+            elif provider == "g4fauto":
                 from pytgpt.gpt4free.utils import TestProviders
 
                 test = TestProviders(quiet=quiet, timeout=timeout)
                 g4fauto = test.best if ignore_working else test.auto
                 if isinstance(g4fauto, str):
-                    provider = "g4fauto+" + g4fauto
+                    provider = "g4f-" + g4fauto
                     from pytgpt.gpt4free import GPT4FREE
 
                     self.bot = GPT4FREE(
                         provider=g4fauto,
                         auth=auth,
                         max_tokens=max_tokens,
                         model=model,
@@ -707,42 +722,49 @@
         self.interpreter = interpreter
         self.rawdog = rawdog
         self.__init_time = time.time()
         self.__start_time = time.time()
         self.__end_time = time.time()
 
     @property
+    def get_provider(self):
+        if self.provider == "auto" and self.bot.provider_name is not None:
+            return self.bot.provider_name
+        else:
+            return self.provider
+
+    @property
     def prompt(self):
         current_time = datetime.datetime.now().strftime("%H:%M:%S")
 
         def find_range(start, end, hms: bool = False):
             in_seconds = round(end - start, 1)
             return (
                 str(datetime.timedelta(seconds=in_seconds)).split(".")[0].zfill(8)
                 if hms
                 else in_seconds
             )
 
         if not self.disable_coloring:
             cmd_prompt = (
                 f"╭─[`{Fore.CYAN}{getpass.getuser().capitalize()}@pyTGPT]`"
-                f"(`{Fore.MAGENTA}{self.provider})`"
+                f"(`{Fore.MAGENTA}{self.get_provider})`"
                 f"~[`{Fore.LIGHTWHITE_EX}🕒{Fore.BLUE}{current_time}-`"
                 f"{Fore.LIGHTWHITE_EX}💻{Fore.RED}{find_range(self.__init_time, time.time(), True)}-`"
                 f"{Fore.LIGHTWHITE_EX}⚡{Fore.YELLOW}{find_range(self.__start_time, self.__end_time)}s]`"
                 f"\n╰─>"
             )
             whitelist = ["[", "]", "~", "-", "(", ")"]
             for character in whitelist:
                 cmd_prompt = cmd_prompt.replace(character + "`", Fore.RESET + character)
             return cmd_prompt
 
         else:
             return (
-                f"╭─[{getpass.getuser().capitalize()}@pyTGPT]({self.provider})"
+                f"╭─[{getpass.getuser().capitalize()}@pyTGPT]({self.get_provider})"
                 f"~[🕒{current_time}"
                 f"-💻{find_range(self.__init_time, time.time(), True)}"
                 f"-⚡{find_range(self.__start_time, self.__end_time)}s]"
                 "\n╰─>"
             )
 
     def output_bond(
```

### Comparing `python_tgpt-0.6.3/src/pytgpt/gemini/main.py` & `python_tgpt-0.6.4/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.6.4/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.6.4/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.6.4/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/groq/main.py` & `python_tgpt-0.6.4/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/imager/imager.py` & `python_tgpt-0.6.4/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/koboldai/main.py` & `python_tgpt-0.6.4/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/leo/main.py` & `python_tgpt-0.6.4/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/llama2/main.py` & `python_tgpt-0.6.4/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/openai/main.py` & `python_tgpt-0.6.4/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/opengpt/main.py` & `python_tgpt-0.6.4/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/perplexity/main.py` & `python_tgpt-0.6.4/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/phind/main.py` & `python_tgpt-0.6.4/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/poe/main.py` & `python_tgpt-0.6.4/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/utils.py` & `python_tgpt-0.6.4/src/pytgpt/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.6.4/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.6.4/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.3
+Version: 0.6.4
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: webchatgpt==0.2.9
+Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
 Requires-Dist: g4f>=0.2.6.1
 Requires-Dist: Helpingai-T2==0.3
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
@@ -140,15 +140,15 @@
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-uc.a.run.app/)
 4. [OpenAI](https://chat.openai.com) *(API key required)*
 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)*
 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session ID required)*
-9. [Phind](https://www.phind.com) - *default*
+9. [Phind](https://www.phind.com)
 10. [Llama2](https://www.llama2.ai)
 11. [Blackboxai](https://www.blackbox.ai)
 12. [gpt4all](https://gpt4all.io) *(Offline)*
 13. [Poe](https://poe.com) - Poe|Quora *(Session ID required)*
 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai)
 
@@ -296,68 +296,68 @@
 {'completion': "I'm so excited to share with you the incredible experiences...", 'stop_reason': None, 'truncated': False, 'stop': None, 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 """
 ```
 
 <details>
 
 <summary>
-Openai
+Auto - *(selects any working provider)*
 
 </summary>
 
 ```python
-import pytgpt.openai as openai
-bot = openai.OPENAI("<OPENAI-API-KEY>")
+import pytgpt.auto import auto
+bot = auto.AUTO()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
-
 <details>
 
 <summary>
-Koboldai
+Openai
 
 </summary>
 
 ```python
-import pytgpt.koboldai as koboldai
-bot = koboldai.KOBOLDAI()
+import pytgpt.openai as openai
+bot = openai.OPENAI("<OPENAI-API-KEY>")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 
 <details>
 
 <summary>
-Opengpt
+Koboldai
 
 </summary>
 
 ```python
-import pytgpt.opengpt as opengpt
-bot = opengpt.OPENGPT()
+import pytgpt.koboldai as koboldai
+bot = koboldai.KOBOLDAI()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
+
 <details>
 
 <summary>
-Bard
+Opengpt
 
 </summary>
 
 ```python
-import pytgpt.bard as bard
-bot = bard.BARD('<Path-to-bard.google.com.cookies.json>')
+import pytgpt.opengpt as opengpt
+bot = opengpt.OPENGPT()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 <details>
 
@@ -379,15 +379,15 @@
 <summary>
 Gpt4free providers
 
 </summary>
 
 ```python
 import pytgpt.gpt4free as gpt4free
-bot = gpt4free.GPT4FREE(provider="Aura")
+bot = gpt4free.GPT4FREE(provider="Koala")
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.3 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.4 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -17,15 +17,15 @@
 Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist:
-pyyaml==6.0.1 Requires-Dist: webchatgpt==0.2.9 Requires-Dist:
+pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
 brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3
 Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
 rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
 extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
 python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
@@ -65,17 +65,17 @@
 [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 ## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
 (https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
 tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
 uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
 [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
 required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
-//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
-//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
+ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
+www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
+gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
 required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
 [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
 run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
 (https://python.org) *(Optional)* ## Installation and Usage ### Installation
 Download binaries for your system from [here.](https://github.com/Simatwa/
 python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
@@ -112,47 +112,48 @@
 chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 {'completion': "I'm so excited to share with you the incredible ",
 'stop_reason': None, 'truncated': False, 'stop': None, 'model': 'llama-2-13b-
 chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx', 'exception': None}
 {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx',
-'exception': None} """ ``` Openai ```python import pytgpt.openai as openai bot
-= openai.OPENAI("") print(bot.chat("")) ``` Koboldai ```python import
-pytgpt.koboldai as koboldai bot = koboldai.KOBOLDAI() print(bot.chat("")) ```
-Opengpt ```python import pytgpt.opengpt as opengpt bot = opengpt.OPENGPT()
-print(bot.chat("")) ``` Bard ```python import pytgpt.bard as bard bot =
-bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgpt.phind as
-phind bot = phind.PHIND() print(bot.chat("")) ``` Gpt4free providers ```python
-import pytgpt.gpt4free as gpt4free bot = gpt4free.GPT4FREE(provider="Aura")
-print(bot.chat("")) ``` To obtain more tailored responses, consider utilizing
-[optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can
-be set to either `code` or `system_command`. ```python from pytgpt.leo import
-LEO bot = LEO() resp = bot.ask('', optimizer='code') print(resp) ``` >
-[!IMPORTANT] > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/
-releases/), the default mode of interaction is conversational. This mode
-enhances the interactive experience, offering better control over the chat
-history. By associating previous prompts and responses, it tailors
-conversations for a more engaging experience. You can still disable the mode:
-```python bot = koboldai.KOBOLDAI(is_conversation=False) ``` Utilize the `--
-disable-conversation` flag in the console to achieve the same functionality. >
-[!CAUTION] > **Bard** autohandles context due to the obvious reason; the
-`is_conversation` parameter is not necessary at all hence not required when
-initializing the class. Also be informed that majority of providers offered by
-*gpt4free* requires *Google Chrome* inorder to function. ### Image Generation
-This has been made possible by [pollinations.ai](https://pollination.ai). ```sh
-$ pytgpt imager "" # e.g pytgpt imager "Coding bot" ``` Developers ```python
-from pytgpt.imager import Imager img = Imager() generated_img = img.generate
-('Coding bot') # [bytes] img.save(generated_img) ``` Download Multiple Images
-```python from pytgpt.imager import Imager img = Imager() img_generator =
-img.generate('Coding bot', amount=3, stream=True) img.save(img_generator) # RAM
-friendly ``` ### Advanced Usage of Placeholders The `generate` functionality
-has been enhanced starting from *v0.3.0* to enable comprehensive utilization of
-the `--with-copied` option and support for accepting piped inputs. This
-improvement introduces placeholders, offering dynamic values for more versatile
+'exception': None} """ ``` Auto - *(selects any working provider)* ```python
+import pytgpt.auto import auto bot = auto.AUTO() print(bot.chat("")) ``` Openai
+```python import pytgpt.openai as openai bot = openai.OPENAI("") print(bot.chat
+("")) ``` Koboldai ```python import pytgpt.koboldai as koboldai bot =
+koboldai.KOBOLDAI() print(bot.chat("")) ``` Opengpt ```python import
+pytgpt.opengpt as opengpt bot = opengpt.OPENGPT() print(bot.chat("")) ``` phind
+```python import pytgpt.phind as phind bot = phind.PHIND() print(bot.chat(""))
+``` Gpt4free providers ```python import pytgpt.gpt4free as gpt4free bot =
+gpt4free.GPT4FREE(provider="Koala") print(bot.chat("")) ``` To obtain more
+tailored responses, consider utilizing [optimizers](pytgpt/utils.py) using the
+`optimizer` parameter. Its values can be set to either `code` or
+`system_command`. ```python from pytgpt.leo import LEO bot = LEO() resp =
+bot.ask('', optimizer='code') print(resp) ``` > [!IMPORTANT] > Commencing from
+[v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of
+interaction is conversational. This mode enhances the interactive experience,
+offering better control over the chat history. By associating previous prompts
+and responses, it tailors conversations for a more engaging experience. You can
+still disable the mode: ```python bot = koboldai.KOBOLDAI
+(is_conversation=False) ``` Utilize the `--disable-conversation` flag in the
+console to achieve the same functionality. > [!CAUTION] > **Bard** autohandles
+context due to the obvious reason; the `is_conversation` parameter is not
+necessary at all hence not required when initializing the class. Also be
+informed that majority of providers offered by *gpt4free* requires *Google
+Chrome* inorder to function. ### Image Generation This has been made possible
+by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
+pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
+Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
+img.save(generated_img) ``` Download Multiple Images ```python from
+pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
+bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ###
+Advanced Usage of Placeholders The `generate` functionality has been enhanced
+starting from *v0.3.0* to enable comprehensive utilization of the `--with-
+copied` option and support for accepting piped inputs. This improvement
+introduces placeholders, offering dynamic values for more versatile
 interactions. | Placeholder | Represents | | ------------ | ----------- | | `{
 {stream}}` | The piped input | | `{{copied}}` | The last copied text | This
 feature is particularly beneficial for intricate operations. For example:
 ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a
 concise commit message from it, aligning with my commit message history: {
 {copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
 result of the `$ git diff` operation, while `{{copied}}` signifies the content
```

### Comparing `python_tgpt-0.6.3/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.6.4/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 src/pytgpt/base.py
 src/pytgpt/console.py
 src/pytgpt/utils.py
 src/pytgpt/api/__init__.py
 src/pytgpt/api/__main__.py
 src/pytgpt/api/utils.py
 src/pytgpt/api/v1.py
+src/pytgpt/auto/__init__.py
+src/pytgpt/auto/errors.py
+src/pytgpt/auto/main.py
 src/pytgpt/blackboxai/__init__.py
 src/pytgpt/blackboxai/main.py
 src/pytgpt/gemini/__init__.py
 src/pytgpt/gemini/main.py
 src/pytgpt/gpt4all/__init__.py
 src/pytgpt/gpt4all/main.py
 src/pytgpt/gpt4free/__init__.py
@@ -44,14 +47,15 @@
 src/python_tgpt.egg-info/PKG-INFO
 src/python_tgpt.egg-info/SOURCES.txt
 src/python_tgpt.egg-info/dependency_links.txt
 src/python_tgpt.egg-info/entry_points.txt
 src/python_tgpt.egg-info/requires.txt
 src/python_tgpt.egg-info/top_level.txt
 tests/test_api.py
+tests/test_auto.py
 tests/test_blackboxai.py
 tests/test_gemini.py
 tests/test_gpt4all.py
 tests/test_gpt4free.py
 tests/test_groq.py
 tests/test_imager.py
 tests/test_koboldai.py
```

### Comparing `python_tgpt-0.6.3/tests/test_api.py` & `python_tgpt-0.6.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/tests/test_imager.py` & `python_tgpt-0.6.4/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.3/tests/test_utils.py` & `python_tgpt-0.6.4/tests/test_utils.py`

 * *Files identical despite different names*

