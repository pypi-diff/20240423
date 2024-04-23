# Comparing `tmp/gtsystem-0.1.8.tar.gz` & `tmp/gtsystem-0.2.1.tar.gz`

## Comparing `gtsystem-0.1.8.tar` & `gtsystem-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/anthropic.py
--rw-r--r--   0        0        0    10303 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/bedrock.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/benchmark.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/chat.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/groq.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/instrument.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/leaderboard.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/ollama.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/openai.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/render.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 gtsystem-0.1.8/gtsystem/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.8/LICENSE
--rw-r--r--   0        0        0     9306 2020-02-02 00:00:00.000000 gtsystem-0.1.8/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 gtsystem-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/__init__.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/anthropic.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/bedrock.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/chat.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/groq.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/leaderboard.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/ollama.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/openai.py
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/render.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 gtsystem-0.2.1/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 gtsystem-0.2.1/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 gtsystem-0.2.1/PKG-INFO
```

### Comparing `gtsystem-0.1.8/gtsystem/anthropic.py` & `gtsystem-0.2.1/gtsystem/anthropic.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,7 +96,22 @@
             return opus_text(prompt, system, temperature, topP, tokens)
         case 'sonnet':
             return sonnet_text(prompt, system, temperature, topP, tokens)
         case 'haiku':
             return haiku_text(prompt, system, temperature, topP, tokens)
         case _:
             return 'Please specify a valid model name'
+
+def chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, cache=False,
+         image_url="", model="opus"):
+    match model:
+        case 'opus':
+            return opus_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url)
+        case 'sonnet':
+            return sonnet_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url)
+        case 'haiku':
+            return haiku_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url)
+        case _:
+            return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.1.8/gtsystem/bedrock.py` & `gtsystem-0.2.1/gtsystem/bedrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,7 +289,19 @@
             return claude2_text(prompt, system, temperature, topP, tokens)
         case 'instant':
             return instant_text(prompt, system, temperature, topP, tokens)
         case 'llama2':
             return llama2_text(prompt, system, temperature, topP, tokens)
         case _:
             return 'Please specify a valid model name'
+
+def chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, cache=False,
+         image_url="", model="sonnet"):
+    match model:
+        case 'sonnet':
+            return sonnet_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url)
+        case 'haiku':
+            return haiku_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url)
+        case _:
+            return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.1.8/gtsystem/benchmark.py` & `gtsystem-0.2.1/gtsystem/benchmark.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/gtsystem/chat.py` & `gtsystem-0.2.1/gtsystem/chat.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/gtsystem/groq.py` & `gtsystem-0.2.1/gtsystem/groq.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/gtsystem/instrument.py` & `gtsystem-0.2.1/gtsystem/instrument.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/gtsystem/leaderboard.py` & `gtsystem-0.2.1/gtsystem/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/gtsystem/ollama.py` & `gtsystem-0.2.1/gtsystem/ollama.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/gtsystem/openai.py` & `gtsystem-0.2.1/gtsystem/openai.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,71 +7,66 @@
 
 def init():
     global OPENAI
     OPENAI = OpenAI()
 
 CHAT = GptChat()
 
-def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, stream=False, cache=False, model=""):
+def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", 
+              reset=False, cache=False, model=""):
     if OPENAI is None:
         init()
 
     if cache:
         cache_match = CHAT.match(prompt)
         if cache_match:
             CHAT.load(cache_match)
-            return next(msg['content'] for msg in CHAT.messages if msg['role'] == 'assistant')
-
-    if reset:
-        CHAT.reset_context()
-    
-    if system != "":
-        CHAT.add_message("system", system)
-    
-    if image_url != "":
-        CHAT.add_image_message(prompt=prompt, image_url=image_url)
+            yield next(msg['content'] for msg in CHAT.messages if msg['role'] == 'assistant')
     else:
-        CHAT.add_message("user", prompt)
-
-    response = OPENAI.chat.completions.create(
-        model=model,
-        messages=CHAT.get_messages(),
-        temperature=temperature,
-        top_p=topP,
-        max_tokens=tokens,
-        stream=stream
-    )
-    if stream:
+        if reset:
+            CHAT.reset_context()
+        
+        if system != "":
+            CHAT.add_message("system", system)
+        
+        if image_url != "":
+            CHAT.add_image_message(prompt=prompt, image_url=image_url)
+        else:
+            CHAT.add_message("user", prompt)
+
+        response = OPENAI.chat.completions.create(
+            model=model,
+            messages=CHAT.get_messages(),
+            temperature=temperature,
+            top_p=topP,
+            max_tokens=tokens,
+            stream=True
+        )
         all_chunks = ""
         for chunk in response:
             part = chunk.choices[0].delta.content
             if part:
-                print(part, end='')
+                yield part
                 all_chunks += part
         response_text = all_chunks
-    else:
-        response_text = response.choices[0].message.content.strip()
-    CHAT.add_message("assistant", response_text)
-    clear_output()
-    return response_text
+        CHAT.add_message("assistant", response_text)
 
 @metrics.track
-def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, 
-              stream=False, cache=False):
-    return _gpt_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, image_url=image_url, reset=reset,
-                stream=stream, cache=cache, model="gpt-4-turbo")
+def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, cache=False):
+    for chunk in _gpt_chat(prompt, system=system, temperature=temperature, topP=topP, tokens=tokens, 
+                           image_url=image_url, reset=reset, cache=cache, model="gpt-4-turbo"):
+        yield chunk
 
 @metrics.track
-def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False, cache=False):
-    return _gpt_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, reset=reset, 
-                stream=stream, cache=cache, model="gpt-3.5-turbo")
+def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, cache=False):
+    for chunk in _gpt_chat(prompt, system=system, temperature=temperature, topP=topP, tokens=tokens, 
+                           reset=reset, cache=cache, model="gpt-3.5-turbo"):
+        yield chunk
 
-def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False, model=""):
+def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model=""):
     if OPENAI is None:
         init()
 
     response = OPENAI.chat.completions.create(
         model=model,
         messages=[
             {
@@ -82,54 +77,50 @@
             "role": "user",
             "content": prompt
             }
         ],
         temperature=temperature,
         top_p=topP,
         max_tokens=tokens,
-        stream=stream
+        stream=True
     )
-    if stream:
-        all_chunks = ""
-        for chunk in response:
-            part = chunk.choices[0].delta.content
-            if part:
-                print(part, end='')
-                all_chunks += part
-        response_text = all_chunks
-    else:
-        response_text = response.choices[0].message.content.strip()
-    clear_output()
-    return response_text
+    for chunk in response:
+        part = chunk.choices[0].delta.content
+        if part:
+            yield part
 
 @metrics.track
-def gpt3_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False):
-    return _gpt_text(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, stream=stream, model="gpt-3.5-turbo")
+def gpt3_text(prompt, system='', temperature=0.0, topP=1, tokens=512):
+    for chunk in _gpt_text(prompt, system=system, temperature=temperature, topP=topP, 
+                           tokens=tokens, model="gpt-3.5-turbo"):
+        yield chunk
 
 @metrics.track
-def gpt4_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False):
-    return _gpt_text(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, stream=stream, model="gpt-4-turbo-preview")
+def gpt4_text(prompt, system='', temperature=0.0, topP=1, tokens=512):
+    for chunk in _gpt_text(prompt, system=system, temperature=temperature, topP=topP, 
+                     tokens=tokens, model="gpt-4-turbo-preview"):
+        yield chunk
 
-def text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False, model="gpt4"):
+def text(prompt, system='', temperature=0.0, topP=1, tokens=512, model="gpt4"):
     match model:
-        case 'gpt3':
-            return gpt3_text(prompt, system, temperature, topP, tokens, stream)
         case 'gpt4':
-            return gpt4_text(prompt, system, temperature, topP, tokens, stream)
+            for chunk in gpt4_text(prompt, system, temperature, topP, tokens):
+                yield chunk
+        case 'gpt3.5':
+            for chunk in gpt3_text(prompt, system, temperature, topP, tokens):
+                yield chunk
         case _:
             return 'Please specify a valid model name'
 
 def chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False, cache=False,
          image_url="", model="gpt4"):
     match model:
-        case 'gpt3':
-            return gpt3_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, reset=reset, cache=cache,
-                stream=stream)
         case 'gpt4':
-            return gpt4_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url,
-                stream=stream)
+            for chunk in gpt4_chat(prompt, system=system, temperature=temperature, topP=topP, 
+                                   tokens=tokens, reset=reset, cache=cache, image_url=image_url):
+                yield chunk
+        case 'gpt3.5':
+            for chunk in gpt3_chat(prompt, system=system, temperature=temperature, topP=topP, 
+                                   tokens=tokens, reset=reset, cache=cache):
+                yield chunk
         case _:
             return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.1.8/gtsystem/render.py` & `gtsystem-0.2.1/gtsystem/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import pandas as pd
-from IPython.display import display, Markdown, Image
+from IPython.display import display, Markdown, Image, clear_output
 import base64
 import re
 
 def md(text):
-    display(Markdown(text))
+    if isinstance(text, str):
+        display(Markdown(text))
+    else:
+        full_text = ""
+        for chunk in text:
+            if chunk:
+                full_text += chunk
+                print(chunk, end='')
+        clear_output(wait=True)
+        display(Markdown(full_text))
 
 def img(url):
     return Image(url=url)
 
 def _display_base64_image(base64_string):
     image_data = base64.b64decode(base64_string)
     display(Image(data=image_data))
```

### Comparing `gtsystem-0.1.8/gtsystem/tasks.py` & `gtsystem-0.2.1/gtsystem/tasks.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/.gitignore` & `gtsystem-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/LICENSE` & `gtsystem-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.8/README.md` & `gtsystem-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,19 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-21 (Release 0.2.1)
+
+- Streamlit app with streaming chat playgroud for OpenAI models with configurable system message, temperature, tokens
+- New methods for bedrock.chat and anthropic.chat
+
 ### 2024-04-21 (Release 0.1.8)
 
 - Improve configurable quality benchmark criteria
 - Ability to merge instrumentation and benchmarking stats in one table
 - Quality evaluation tasks dataset
 - Configurable GPT4 or Opus model for automated self/other benchmarking
```

### Comparing `gtsystem-0.1.8/pyproject.toml` & `gtsystem-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.1.8"
+version = "0.2.1"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.1.8/PKG-INFO` & `gtsystem-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtsystem
-Version: 0.1.8
+Version: 0.2.1
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -87,14 +87,19 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-21 (Release 0.2.1)
+
+- Streamlit app with streaming chat playgroud for OpenAI models with configurable system message, temperature, tokens
+- New methods for bedrock.chat and anthropic.chat
+
 ### 2024-04-21 (Release 0.1.8)
 
 - Improve configurable quality benchmark criteria
 - Ability to merge instrumentation and benchmarking stats in one table
 - Quality evaluation tasks dataset
 - Configurable GPT4 or Opus model for automated self/other benchmarking
```

