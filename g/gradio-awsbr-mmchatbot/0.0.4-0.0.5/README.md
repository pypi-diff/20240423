# Comparing `tmp/gradio_awsbr_mmchatbot-0.0.4.tar.gz` & `tmp/gradio_awsbr_mmchatbot-0.0.5.tar.gz`

## Comparing `gradio_awsbr_mmchatbot-0.0.4.tar` & `gradio_awsbr_mmchatbot-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/__init__.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/multimodalchatbot.py
--rw-r--r--   0        0        0    26428 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/multimodalchatbot.pyi
--rw-r--r--   0        0        0   766349 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/templates/component/index.js
--rw-r--r--   0        0        0  1483905 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/templates/component/style.css
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/templates/component/assets/worker-43d19264.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/demo/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/demo/app.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/demo/bedrock_utils.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/demo/css.css
--rw-r--r--   0        0        0    15592 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/demo/space.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/Index.svelte
--rw-r--r--   0        0        0    59659 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/package-lock.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/package.json
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/shared/ChatBot.svelte
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/shared/Copy.svelte
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/shared/LikeDislike.svelte
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/shared/Pending.svelte
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/shared/autorender.d.ts
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/frontend/shared/utils.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/.gitignore
--rw-r--r--   0        0        0    14370 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/README.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/__init__.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/multimodalchatbot.py
+-rw-r--r--   0        0        0    26428 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/multimodalchatbot.pyi
+-rw-r--r--   0        0        0   766349 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/templates/component/index.js
+-rw-r--r--   0        0        0  1483905 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/templates/component/style.css
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/templates/component/assets/worker-43d19264.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/demo/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/demo/app.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/demo/bedrock_utils.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/demo/css.css
+-rw-r--r--   0        0        0    15592 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/demo/space.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/Index.svelte
+-rw-r--r--   0        0        0    59659 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/package-lock.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/package.json
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/shared/ChatBot.svelte
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/shared/Copy.svelte
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/shared/LikeDislike.svelte
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/shared/Pending.svelte
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/shared/autorender.d.ts
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/frontend/shared/utils.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/.gitignore
+-rw-r--r--   0        0        0    14370 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/README.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 gradio_awsbr_mmchatbot-0.0.5/PKG-INFO
```

### Comparing `gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/multimodalchatbot.py` & `gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/multimodalchatbot.py`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/multimodalchatbot.pyi` & `gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/multimodalchatbot.pyi`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/templates/component/index.js` & `gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/templates/component/style.css` & `gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/backend/gradio_awsbr_mmchatbot/templates/component/assets/worker-43d19264.js` & `gradio_awsbr_mmchatbot-0.0.5/backend/gradio_awsbr_mmchatbot/templates/component/assets/worker-43d19264.js`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/demo/app.py` & `gradio_awsbr_mmchatbot-0.0.5/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/demo/bedrock_utils.py` & `gradio_awsbr_mmchatbot-0.0.5/demo/bedrock_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 formatType = "image/webp"
 
             # Encode the image as base64
             b64EncodedImage = base64.b64encode(open(self.image, "rb").read())
 
             # Send the image and text to the Anthropic API
             with self.client.messages.stream(
-                model="anthropic.claude-3-sonnet-20240229-v1:0",
+                model="anthropic.claude-3-opus-20240229-v1:0",
                 max_tokens=5000,
                 messages=[{
                     'role': 'user',
                     'content': [
                         {
                             "type": "image",
                             "source": {
```

### Comparing `gradio_awsbr_mmchatbot-0.0.4/demo/css.css` & `gradio_awsbr_mmchatbot-0.0.5/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/demo/space.py` & `gradio_awsbr_mmchatbot-0.0.5/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/Index.svelte` & `gradio_awsbr_mmchatbot-0.0.5/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/package-lock.json` & `gradio_awsbr_mmchatbot-0.0.5/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/package.json` & `gradio_awsbr_mmchatbot-0.0.5/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/shared/ChatBot.svelte` & `gradio_awsbr_mmchatbot-0.0.5/frontend/shared/ChatBot.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/shared/Copy.svelte` & `gradio_awsbr_mmchatbot-0.0.5/frontend/shared/Copy.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/shared/LikeDislike.svelte` & `gradio_awsbr_mmchatbot-0.0.5/frontend/shared/LikeDislike.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/shared/Pending.svelte` & `gradio_awsbr_mmchatbot-0.0.5/frontend/shared/Pending.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/frontend/shared/utils.ts` & `gradio_awsbr_mmchatbot-0.0.5/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/README.md` & `gradio_awsbr_mmchatbot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gradio_awsbr_mmchatbot-0.0.4/pyproject.toml` & `gradio_awsbr_mmchatbot-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_awsbr_mmchatbot"
-version = "0.0.4"
+version = "0.0.5"
 description = "This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Jedijamez", email = "" }]
 keywords = ["gradio-custom-component", "gradio-template-Chatbot", "AWS", "Bedrock", "Amazon Bedrock", "Anthropic", "LLM", "Chatbot", "Multimodal", "Claude", "Claude v3"]
 # Add dependencies here
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_awsbr_mmchatbot/templates", "*.pyi", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates"]
+artifacts = ["/backend/gradio_awsbr_mmchatbot/templates", "*.pyi", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates", "backend/gradio_awsbr_mmchatbot/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_awsbr_mmchatbot"]
```

### Comparing `gradio_awsbr_mmchatbot-0.0.4/PKG-INFO` & `gradio_awsbr_mmchatbot-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_awsbr_mmchatbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock
 Author: Jedijamez
 License-Expression: MIT
 Keywords: AWS,Amazon Bedrock,Anthropic,Bedrock,Chatbot,Claude,Claude v3,LLM,Multimodal,gradio-custom-component,gradio-template-Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

