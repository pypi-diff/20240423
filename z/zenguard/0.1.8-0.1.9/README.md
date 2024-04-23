# Comparing `tmp/zenguard-0.1.8.tar.gz` & `tmp/zenguard-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenguard-0.1.8.tar", max compression
+gzip compressed data, was "zenguard-0.1.9.tar", max compression
```

## Comparing `zenguard-0.1.8.tar` & `zenguard-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1068 2024-03-27 23:17:17.162445 zenguard-0.1.8/LICENSE
--rw-r--r--   0        0        0     4717 2024-04-21 18:48:37.634036 zenguard-0.1.8/README.md
--rw-r--r--   0        0        0      444 2024-04-21 18:48:37.634235 zenguard-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      103 2024-03-25 18:32:49.933079 zenguard-0.1.8/zenguard/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 16:56:11.876514 zenguard-0.1.8/zenguard/pentest/__init__.py
--rw-r--r--   0        0        0      107 2024-03-25 16:56:11.876674 zenguard-0.1.8/zenguard/pentest/prompt_injections/__init__.py
--rw-r--r--   0        0        0      614 2024-03-25 16:56:11.876786 zenguard-0.1.8/zenguard/pentest/prompt_injections/_utils.py
--rw-r--r--   0        0        0      959 2024-03-25 16:56:11.876906 zenguard-0.1.8/zenguard/pentest/prompt_injections/config.py
--rw-r--r--   0        0        0    27037 2024-03-25 16:56:11.877082 zenguard-0.1.8/zenguard/pentest/prompt_injections/prompt_data.py
--rw-r--r--   0        0        0    10014 2024-03-25 16:56:11.877333 zenguard-0.1.8/zenguard/pentest/prompt_injections/prompting.py
--rw-r--r--   0        0        0     1965 2024-03-25 18:32:49.933251 zenguard-0.1.8/zenguard/pentest/prompt_injections/run.py
--rw-r--r--   0        0        0     2369 2024-03-25 16:56:11.877590 zenguard-0.1.8/zenguard/pentest/prompt_injections/scoring.py
--rw-r--r--   0        0        0     1342 2024-03-25 16:56:11.877728 zenguard-0.1.8/zenguard/pentest/prompt_injections/visualization.py
--rw-r--r--   0        0        0     3524 2024-04-21 18:29:18.545646 zenguard-0.1.8/zenguard/zenguard.py
--rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 zenguard-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-27 23:17:17.162445 zenguard-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4717 2024-04-21 18:48:37.634036 zenguard-0.1.9/README.md
+-rw-r--r--   0        0        0      501 2024-04-22 16:30:53.187134 zenguard-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-03-25 18:32:49.933079 zenguard-0.1.9/zenguard/__init__.py
+-rw-r--r--   0        0        0     5253 2024-04-22 16:25:29.747047 zenguard-0.1.9/zenguard/ai_clients/openai.py
+-rw-r--r--   0        0        0        0 2024-03-25 16:56:11.876514 zenguard-0.1.9/zenguard/pentest/__init__.py
+-rw-r--r--   0        0        0      107 2024-03-25 16:56:11.876674 zenguard-0.1.9/zenguard/pentest/prompt_injections/__init__.py
+-rw-r--r--   0        0        0      614 2024-03-25 16:56:11.876786 zenguard-0.1.9/zenguard/pentest/prompt_injections/_utils.py
+-rw-r--r--   0        0        0      959 2024-03-25 16:56:11.876906 zenguard-0.1.9/zenguard/pentest/prompt_injections/config.py
+-rw-r--r--   0        0        0    27037 2024-03-25 16:56:11.877082 zenguard-0.1.9/zenguard/pentest/prompt_injections/prompt_data.py
+-rw-r--r--   0        0        0    10014 2024-03-25 16:56:11.877333 zenguard-0.1.9/zenguard/pentest/prompt_injections/prompting.py
+-rw-r--r--   0        0        0     1965 2024-03-25 18:32:49.933251 zenguard-0.1.9/zenguard/pentest/prompt_injections/run.py
+-rw-r--r--   0        0        0     2369 2024-03-25 16:56:11.877590 zenguard-0.1.9/zenguard/pentest/prompt_injections/scoring.py
+-rw-r--r--   0        0        0     1342 2024-03-25 16:56:11.877728 zenguard-0.1.9/zenguard/pentest/prompt_injections/visualization.py
+-rw-r--r--   0        0        0     3641 2024-04-22 16:25:29.747224 zenguard-0.1.9/zenguard/zenguard.py
+-rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 zenguard-0.1.9/PKG-INFO
```

### Comparing `zenguard-0.1.8/LICENSE` & `zenguard-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/README.md` & `zenguard-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/_utils.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/_utils.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/config.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/config.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/prompt_data.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/prompt_data.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/prompting.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/prompting.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/run.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/run.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/scoring.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/scoring.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/pentest/prompt_injections/visualization.py` & `zenguard-0.1.9/zenguard/pentest/prompt_injections/visualization.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.8/zenguard/zenguard.py` & `zenguard-0.1.9/zenguard/zenguard.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from enum import Enum
 from typing import Optional
 
 import httpx
 from openai import OpenAI
 from tqdm import tqdm
 
+from zenguard.ai_clients.openai import ChatWithZenguard
 from zenguard.pentest.prompt_injections import (
     config,
     prompting,
     run,
     scoring,
     visualization,
 )
@@ -28,14 +29,15 @@
     api_key: str
     llm_api_key: Optional[str] = None
 
 
 @dataclass
 class ZenGuardConfig:
     credentials: Credentials
+    ai_client: Optional[OpenAI] = None
     llm: Optional[SupportedLLMs] = None
 
 
 class Detector(Enum):
     PROMPT_INJECTION = "v1/detect/prompt_injection"
     PII = "v1/detect/pii"
     ALLOWED_TOPICS = "v1/detect/topics/allowed"
@@ -50,36 +52,33 @@
 
 class ZenGuard:
     """
     ZenGuard is a class that represents the ZenGuard object.
     It is used to connect to ZenGuard AI API and its services.
     """
 
-    def __init__(
-        self,
-        config: ZenGuardConfig,
-    ):
+    def __init__(self, config: ZenGuardConfig):
         api_key = config.credentials.api_key
         if type(api_key) != str or api_key == '':
             raise ValueError("The API key must be a string type and not empty.")
         self._api_key = api_key
         self._backend = "https://api.zenguard.ai/"
 
-        self._llm_client = None
         if config.llm == SupportedLLMs.CHATGPT:
-            self._llm_client = OpenAI(
-                api_key=config.credentials.llm_api_key,
+            self.chat = ChatWithZenguard(
+                client=config.ai_client,
+                zenguard=self,
+                openai_key=config.credentials.llm_api_key
             )
         elif config.llm is not None:
             raise ValueError(f"LLM {config.llm} is not supported")
 
     def detect(self, detectors: list[Detector], prompt: str):
         if len(detectors) == 0:
             return {"error": "No detectors were provided"}
-
         try:
             response = httpx.post(
                 self._backend + detectors[0].value,
                 json={"message": prompt},
                 headers={"x-api-key": self._api_key},
                 timeout=3,
             )
@@ -106,12 +105,12 @@
             print("\nRunning attack on ZenGuard endpoint:")
             assert (
                 detector == Detector.PROMPT_INJECTION
             ), "Only prompt injection pentesting is currently supported"
             self._attack_zenguard(Detector.PROMPT_INJECTION, attack_prompts)
         elif endpoint == Endpoint.OPENAI:
             print("\nRunning attack on OpenAI endpoint:")
-            run.run_prompts_api(attack_prompts, self._llm_client)
+            run.run_prompts_api(attack_prompts, self.chat._client)
 
         scoring.score_attacks(attack_prompts)
         df = visualization.build_dataframe(attack_prompts)
         print(scoring.get_metrics(df, "Attack Instruction"))
```

### Comparing `zenguard-0.1.8/PKG-INFO` & `zenguard-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenguard
-Version: 0.1.8
+Version: 0.1.9
 Summary: Plug-and-play production grade security for GenAI applications
 License: MIT
 Author: ZenGuard Team
 Author-email: hello@zenguard.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

