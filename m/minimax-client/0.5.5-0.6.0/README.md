# Comparing `tmp/minimax_client-0.5.5.tar.gz` & `tmp/minimax_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimax_client-0.5.5.tar", last modified: Sun Apr 21 12:40:45 2024, max compression
+gzip compressed data, was "minimax_client-0.6.0.tar", last modified: Tue Apr 23 06:25:27 2024, max compression
```

## Comparing `minimax_client-0.5.5.tar` & `minimax_client-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.5/LICENSE.md
--rw-r--r--   0        0        0    12307 2024-04-18 06:12:14.577504 minimax_client-0.5.5/README.md
--rw-r--r--   0        0        0     2337 2024-04-21 12:40:45.799953 minimax_client-0.5.5/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.5/src/minimax_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-21 12:40:07.030057 minimax_client-0.5.5/src/minimax_client/__version__.py
--rw-r--r--   0        0        0     6268 2024-04-19 08:40:24.666388 minimax_client-0.5.5/src/minimax_client/client.py
--rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.5/src/minimax_client/entities/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.5.5/src/minimax_client/entities/assistant.py
--rw-r--r--   0        0        0     1743 2024-04-19 09:30:46.794875 minimax_client-0.5.5/src/minimax_client/entities/audio.py
--rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.5/src/minimax_client/entities/chat_completion.py
--rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.5/src/minimax_client/entities/common.py
--rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.5/src/minimax_client/entities/embedding.py
--rw-r--r--   0        0        0     1157 2024-04-19 08:29:50.222873 minimax_client-0.5.5/src/minimax_client/entities/file.py
--rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.5/src/minimax_client/entities/fine_tuning.py
--rw-r--r--   0        0        0       28 2024-04-18 09:58:33.261586 minimax_client-0.5.5/src/minimax_client/entities/retrieval.py
--rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.5.5/src/minimax_client/entities/thread.py
--rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.5/src/minimax_client/interfaces/__init__.py
--rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.5/src/minimax_client/interfaces/assistant.py
--rw-r--r--   0        0        0    29506 2024-04-19 09:52:33.881222 minimax_client-0.5.5/src/minimax_client/interfaces/audio.py
--rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.5/src/minimax_client/interfaces/base.py
--rw-r--r--   0        0        0     8842 2024-04-18 06:15:41.712616 minimax_client-0.5.5/src/minimax_client/interfaces/chat_completion.py
--rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.5/src/minimax_client/interfaces/embedding.py
--rw-r--r--   0        0        0     8150 2024-04-19 08:40:42.905673 minimax_client-0.5.5/src/minimax_client/interfaces/file.py
--rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.5/src/minimax_client/interfaces/fine_tuning.py
--rw-r--r--   0        0        0       28 2024-04-18 09:59:03.537448 minimax_client-0.5.5/src/minimax_client/interfaces/retrieval.py
--rw-r--r--   0        0        0    35341 2024-04-18 09:36:27.802413 minimax_client-0.5.5/src/minimax_client/interfaces/thread.py
--rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.5/tests/test_client.py
--rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 minimax_client-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0    13367 2024-04-23 06:23:06.665437 minimax_client-0.6.0/README.md
+-rw-r--r--   0        0        0     2337 2024-04-23 06:25:27.923314 minimax_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.6.0/src/minimax_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-23 06:13:43.209671 minimax_client-0.6.0/src/minimax_client/__version__.py
+-rw-r--r--   0        0        0     6268 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/client.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.6.0/src/minimax_client/entities/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.6.0/src/minimax_client/entities/assistant.py
+-rw-r--r--   0        0        0     1743 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/entities/audio.py
+-rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.6.0/src/minimax_client/entities/chat_completion.py
+-rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.6.0/src/minimax_client/entities/common.py
+-rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.6.0/src/minimax_client/entities/embedding.py
+-rw-r--r--   0        0        0     1157 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/entities/file.py
+-rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.6.0/src/minimax_client/entities/fine_tuning.py
+-rw-r--r--   0        0        0       28 2024-04-18 09:58:33.261586 minimax_client-0.6.0/src/minimax_client/entities/retrieval.py
+-rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.6.0/src/minimax_client/entities/thread.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.6.0/src/minimax_client/interfaces/__init__.py
+-rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.6.0/src/minimax_client/interfaces/assistant.py
+-rw-r--r--   0        0        0    31236 2024-04-23 06:13:30.322678 minimax_client-0.6.0/src/minimax_client/interfaces/audio.py
+-rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.6.0/src/minimax_client/interfaces/base.py
+-rw-r--r--   0        0        0     8842 2024-04-18 06:15:41.712616 minimax_client-0.6.0/src/minimax_client/interfaces/chat_completion.py
+-rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.6.0/src/minimax_client/interfaces/embedding.py
+-rw-r--r--   0        0        0     8150 2024-04-19 08:40:42.905673 minimax_client-0.6.0/src/minimax_client/interfaces/file.py
+-rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.6.0/src/minimax_client/interfaces/fine_tuning.py
+-rw-r--r--   0        0        0       28 2024-04-18 09:59:03.537448 minimax_client-0.6.0/src/minimax_client/interfaces/retrieval.py
+-rw-r--r--   0        0        0    35341 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/interfaces/thread.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0    14246 1970-01-01 00:00:00.000000 minimax_client-0.6.0/PKG-INFO
```

### Comparing `minimax_client-0.5.5/LICENSE.md` & `minimax_client-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/README.md` & `minimax_client-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 - Assistants
   - Assistant
   - Assistant File
   - Thread
   - Message
   - Run
   - Run Step
+- Audio
+  - T2A
+  - T2A Pro
+  - T2A Large
+  - T2A Stream
+  - Voice Cloning
 
 ## Prerequisites
 
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
@@ -497,7 +503,59 @@
     thread_id=thread_id,
     assistant_id=assistant_id,
     messages=[{"type": 1, "role": "user", "content": "1 + 1 equals:"}],
 ):
     print(part.data.model_dump())
     print("\n-----\n")
 ```
+
+#### 2.17 Sync T2A
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.audio.speech(
+    text="One apple a day keeps the doctor away",
+    model="speech-02",
+    timber_weights=[
+        {
+            "voice_id": "male-qn-qingse",
+            "weight": 1,
+        },
+        {
+            "voice_id": "presenter_female",
+            "weight": 1,
+        },
+    ],
+    vol=1,
+    pitch=2,
+)
+
+if isinstance(resp, bytes):
+    with open("speech.mp3", "wb") as f:
+        f.write(resp)
+else:
+    print(resp.model_dump())
+```
+
+#### 2.18 Sync Voice Cloning
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.files.create(filepath="original_voice.mp3", purpose="voice_clone")
+
+file_id = resp.file.file_id
+
+resp = client.audio.voice_cloning(
+    file_id=file_id,
+    voice_id="cloned12345678",
+)
+
+print(resp.model_dump())
+```
```

### Comparing `minimax_client-0.5.5/pyproject.toml` & `minimax_client-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.5.5"
+version = "0.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=8.1.1,<9",
```

### Comparing `minimax_client-0.5.5/src/minimax_client/client.py` & `minimax_client-0.6.0/src/minimax_client/client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/assistant.py` & `minimax_client-0.6.0/src/minimax_client/entities/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/audio.py` & `minimax_client-0.6.0/src/minimax_client/entities/audio.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/chat_completion.py` & `minimax_client-0.6.0/src/minimax_client/entities/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/common.py` & `minimax_client-0.6.0/src/minimax_client/entities/common.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/file.py` & `minimax_client-0.6.0/src/minimax_client/entities/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/fine_tuning.py` & `minimax_client-0.6.0/src/minimax_client/entities/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/entities/thread.py` & `minimax_client-0.6.0/src/minimax_client/entities/thread.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/assistant.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/audio.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,32 +34,36 @@
         char_to_pitch: Optional[List[str]] = None,
     ) -> Union[AudioSpeechErrorResponse, bytes]:
         """
         Text to Speech. Maximum characters to synthesize: 500
 
         Args:
             text (str): The text to synthesize. Should be < 500 characters.
-            model (Literal["speech-01", "speech-02"]): The model to use.
+            model (Literal["speech-01", "speech-02"]):
+                The model to use.
+                "speech-01" is suited in Chinese cases;
+                "speech-02" supports Chinese, English, CN/EN mix, Japanese and Korean.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             timber_weights (Optional[List[Dict[str, Union[str, int]]]], optional):
                 Weights info of mixture of voices.
-                If specified, `voice_id` will be ignored.
+                If `timber_weights` is specified, `voice_id` will be ignored.
                 Defaults to None.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             output_format (Literal["mp3", "wav", "pcm", "flac", "aac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
                 Defaults to None.
 
         Returns:
             Union[AudioSpeechErrorResponse, bytes]: The response from the API
@@ -104,32 +108,36 @@
         char_to_pitch: Optional[List[str]] = None,
     ) -> AudioSpeechProResponse:
         """
         Text to Speech Pro. Maximum characters to synthesize: 50,000
 
         Args:
             text (str): The text to synthesize. Should be < 50,000 characters.
-            model (Literal["speech-01", "speech-02"]): The model to use.
+            model (Literal["speech-01", "speech-02"]):
+                The model to use.
+                "speech-01" is suited in Chinese cases;
+                "speech-02" supports Chinese, English, CN/EN mix, Japanese and Korean.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             timber_weights (Optional[List[Dict[str, Union[str, int]]]], optional):
                 Weights info of mixture of voices.
-                If specified, `voice_id` will be ignored.
+                If `timber_weights` is specified, `voice_id` will be ignored.
                 Defaults to None.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             output_format (Literal["mp3", "wav", "pcm", "flac", "aac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             audio_sample_rate (Literal[16_000, 24_000, 32_000]):
                 The sample rate of the synthesized voice. Defaults to 32,000.
             bitrate (Literal[32_000, 64_000, 128_000]):
                 The bitrate of the synthesized voice. Defaults to 128,000.
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
@@ -184,25 +192,26 @@
                 The path to a single (local) zip file containing the text to synthesize.
                 The zip file should only contain txt or json files.
                 The text inside should be < 10,000,000 characters.
             model (Literal["speech-01"]):
                 The model to use. Only `speech-01` is supported.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             output_format (Literal["mp3", "wav", "pcm", "flac", "aac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             audio_sample_rate (Literal[16_000, 24_000]):
                 The sample rate of the synthesized voice. Defaults to 24,000.
             bitrate (Literal[32_900, 64_900, 128_900]):
                 The bitrate of the synthesized voice. Defaults to 64,900.
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
@@ -237,15 +246,15 @@
         return AudioSpeechLargeResponse(**resp.json())
 
     def speech_large_status(self, task_id: int) -> AudioSpeechLargeStatusResponse:
         """
         Retrieve the status of a Text to Speech Large request.
 
         Args:
-            task_id (int): The task_id from the response when creating the request
+            task_id (int): The task_id from the response which creates the request.
 
         Returns:
             AudioSpeechLargeStatusResponse: The response from the API
         """
         resp = self.client.get(
             url="https://api.minimax.chat/query/t2a_async_query",
             params={"task_id": task_id},
@@ -273,29 +282,30 @@
 
         Args:
             text (str): The text to synthesize.
             model (Literal["speech-01"]):
                 The model to use. Only `speech-01` is supported.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             timber_weights (Optional[List[Dict[str, Union[str, int]]]], optional):
                 Weights info of mixture of voices.
-                If specified, `voice_id` will be ignored.
+                If `timber_weights` is specified, `voice_id` will be ignored.
                 Defaults to None.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             format (Literal["mp3", "pcm", "flac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             audio_sample_rate (Literal[16_000, 24_000, 32_000]):
                 The sample rate of the synthesized voice. Defaults to 32,000.
             bitrate (Literal[32_000, 64_000, 128_000]):
                 The bitrate of the synthesized voice. Defaults to 128,000.
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
@@ -384,32 +394,36 @@
         char_to_pitch: Optional[List[str]] = None,
     ) -> Union[AudioSpeechErrorResponse, bytes]:
         """
         Text to Speech. Maximum characters to synthesize: 500
 
         Args:
             text (str): The text to synthesize. Should be < 500 characters.
-            model (Literal["speech-01", "speech-02"]): The model to use.
+            model (Literal["speech-01", "speech-02"]):
+                The model to use.
+                "speech-01" is suited in Chinese cases;
+                "speech-02" supports Chinese, English, CN/EN mix, Japanese and Korean.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             timber_weights (Optional[List[Dict[str, Union[str, int]]]], optional):
                 Weights info of mixture of voices.
-                If specified, `voice_id` will be ignored.
+                If `timber_weights` is specified, `voice_id` will be ignored.
                 Defaults to None.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             output_format (Literal["mp3", "wav", "pcm", "flac", "aac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
                 Defaults to None.
 
         Returns:
             Union[AudioSpeechErrorResponse, bytes]: The response from the API
@@ -454,32 +468,36 @@
         char_to_pitch: Optional[List[str]] = None,
     ) -> AudioSpeechProResponse:
         """
         Text to Speech Pro. Maximum characters to synthesize: 50,000
 
         Args:
             text (str): The text to synthesize. Should be < 50,000 characters.
-            model (Literal["speech-01", "speech-02"]): The model to use.
+            model (Literal["speech-01", "speech-02"]):
+                The model to use.
+                "speech-01" is suited in Chinese cases;
+                "speech-02" supports Chinese, English, CN/EN mix, Japanese and Korean.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             timber_weights (Optional[List[Dict[str, Union[str, int]]]], optional):
                 Weights info of mixture of voices.
-                If specified, `voice_id` will be ignored.
+                If `timber_weights` is specified, `voice_id` will be ignored.
                 Defaults to None.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             output_format (Literal["mp3", "wav", "pcm", "flac", "aac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             audio_sample_rate (Literal[16_000, 24_000, 32_000]):
                 The sample rate of the synthesized voice. Defaults to 32,000.
             bitrate (Literal[32_000, 64_000, 128_000]):
                 The bitrate of the synthesized voice. Defaults to 128,000.
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
@@ -534,25 +552,26 @@
                 The path to a single (local) zip file containing the text to synthesize.
                 The zip file should only contain txt or json files.
                 The text inside should be < 10,000,000 characters.
             model (Literal["speech-01"]):
                 The model to use. Only `speech-01` is supported.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             output_format (Literal["mp3", "wav", "pcm", "flac", "aac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             audio_sample_rate (Literal[16_000, 24_000]):
                 The sample rate of the synthesized voice. Defaults to 24,000.
             bitrate (Literal[32_900, 64_900, 128_900]):
                 The bitrate of the synthesized voice. Defaults to 64,900.
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
@@ -589,15 +608,15 @@
         return AudioSpeechLargeResponse(**resp.json())
 
     async def speech_large_status(self, task_id: int) -> AudioSpeechLargeStatusResponse:
         """
         Retrieve the status of a Text to Speech Large request.
 
         Args:
-            task_id (int): The task_id from the response when creating the request
+            task_id (int): The task_id from the response which creates the request.
 
         Returns:
             AudioSpeechLargeStatusResponse: The response from the API
         """
         resp = await self.client.get(
             url="https://api.minimax.chat/query/t2a_async_query",
             params={"task_id": task_id},
@@ -625,29 +644,30 @@
 
         Args:
             text (str): The text to synthesize.
             model (Literal["speech-01"]):
                 The model to use. Only `speech-01` is supported.
             voice_id (Optional[str], optional):
                 The ID of the voice to use. eg. "male-qn-qingse", "female-shaonv"
+                Could be one of preset IDs from MiniMax, or one out of voice cloning.
             timber_weights (Optional[List[Dict[str, Union[str, int]]]], optional):
                 Weights info of mixture of voices.
-                If specified, `voice_id` will be ignored.
+                If `timber_weights` is specified, `voice_id` will be ignored.
                 Defaults to None.
             speed (float):
                 The speed of the synthesized voice. Should be in range [0.5, 2].
                 Defaults to 1.0.
             vol (float):
                 The volume of the synthesized voice. Should be in range (0, 10].
                 Defaults to 1.0.
             format (Literal["mp3", "pcm", "flac"]):
                 The output format of the synthesized voice. Defaults to "mp3".
             pitch (int):
                 The pitch of the synthesized voice. Should be in range [-12, 12].
-                Defaults to 0.
+                Defaults to 0 (which means the original pitch).
             audio_sample_rate (Literal[16_000, 24_000, 32_000]):
                 The sample rate of the synthesized voice. Defaults to 32,000.
             bitrate (Literal[32_000, 64_000, 128_000]):
                 The bitrate of the synthesized voice. Defaults to 128,000.
             char_to_pitch (Optional[List[str]], optional):
                 List of rules to replace tones/symbols. One string per rule.
                 eg. "燕少飞/(yan4)(shao3)(fei1)", "omg/oh my god", "=/等于"
```

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/base.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/chat_completion.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/embedding.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/embedding.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/file.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/fine_tuning.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/src/minimax_client/interfaces/thread.py` & `minimax_client-0.6.0/src/minimax_client/interfaces/thread.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/tests/test_client.py` & `minimax_client-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.5/PKG-INFO` & `minimax_client-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimax-client
-Version: 0.5.5
+Version: 0.6.0
 Summary: An (unofficial) python native client for easy interaction with MiniMax Open Platform
 Keywords: web,api,llm
 Author-Email: Zeyang Lin <4020306+linzeyang@users.noreply.github.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -53,14 +53,20 @@
 - Assistants
   - Assistant
   - Assistant File
   - Thread
   - Message
   - Run
   - Run Step
+- Audio
+  - T2A
+  - T2A Pro
+  - T2A Large
+  - T2A Stream
+  - Voice Cloning
 
 ## Prerequisites
 
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
@@ -531,7 +537,59 @@
     thread_id=thread_id,
     assistant_id=assistant_id,
     messages=[{"type": 1, "role": "user", "content": "1 + 1 equals:"}],
 ):
     print(part.data.model_dump())
     print("\n-----\n")
 ```
+
+#### 2.17 Sync T2A
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.audio.speech(
+    text="One apple a day keeps the doctor away",
+    model="speech-02",
+    timber_weights=[
+        {
+            "voice_id": "male-qn-qingse",
+            "weight": 1,
+        },
+        {
+            "voice_id": "presenter_female",
+            "weight": 1,
+        },
+    ],
+    vol=1,
+    pitch=2,
+)
+
+if isinstance(resp, bytes):
+    with open("speech.mp3", "wb") as f:
+        f.write(resp)
+else:
+    print(resp.model_dump())
+```
+
+#### 2.18 Sync Voice Cloning
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.files.create(filepath="original_voice.mp3", purpose="voice_clone")
+
+file_id = resp.file.file_id
+
+resp = client.audio.voice_cloning(
+    file_id=file_id,
+    voice_id="cloned12345678",
+)
+
+print(resp.model_dump())
+```
```

