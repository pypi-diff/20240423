# Comparing `tmp/hume-0.5.0rc2.tar.gz` & `tmp/hume-0.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.5.0rc2.tar", max compression
+gzip compressed data, was "hume-0.5.0rc3.tar", max compression
```

## Comparing `hume-0.5.0rc2.tar` & `hume-0.5.0rc3.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.0rc2/LICENSE
--rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.0rc2/README.md
--rw-r--r--   0        0        0      824 2024-04-18 07:05:31.675321 hume-0.5.0rc2/hume/__init__.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.0rc2/hume/_common/__init__.py
--rw-r--r--   0        0        0     4853 2024-04-09 05:23:34.092782 hume-0.5.0rc2/hume/_common/client_base.py
--rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.0rc2/hume/_common/config_base.py
--rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.0rc2/hume/_common/protocol.py
--rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.0rc2/hume/_common/utilities/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.0rc2/hume/_common/utilities/config_utilities.py
--rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.0rc2/hume/_common/utilities/model_utilities.py
--rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.0rc2/hume/_common/utilities/paging_utilities.py
--rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.0rc2/hume/_common/utilities/retry_utilities.py
--rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.0rc2/hume/_common/utilities/typing_utilities.py
--rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.0rc2/hume/_measurement/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.0rc2/hume/_measurement/batch/__init__.py
--rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.0rc2/hume/_measurement/batch/batch_job.py
--rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.0rc2/hume/_measurement/batch/batch_job_details.py
--rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.0rc2/hume/_measurement/batch/batch_job_state.py
--rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.0rc2/hume/_measurement/batch/batch_job_status.py
--rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.0rc2/hume/_measurement/batch/hume_batch_client.py
--rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.0rc2/hume/_measurement/batch/transcription_config.py
--rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.0rc2/hume/_measurement/stream/__init__.py
--rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.0rc2/hume/_measurement/stream/hume_stream_client.py
--rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.0rc2/hume/_measurement/stream/stream_socket.py
--rw-r--r--   0        0        0      435 2024-04-18 07:05:31.675469 hume-0.5.0rc2/hume/_voice/__init__.py
--rw-r--r--   0        0        0      363 2024-04-18 10:40:32.709085 hume-0.5.0rc2/hume/_voice/hume_voice_client.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.675674 hume-0.5.0rc2/hume/_voice/microphone/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-18 10:40:32.750347 hume-0.5.0rc2/hume/_voice/microphone/asyncio_utilities.py
--rw-r--r--   0        0        0      728 2024-04-18 10:40:32.750572 hume-0.5.0rc2/hume/_voice/microphone/audio_utilities.py
--rw-r--r--   0        0        0     3350 2024-04-18 17:50:18.091852 hume-0.5.0rc2/hume/_voice/microphone/microphone.py
--rw-r--r--   0        0        0     6008 2024-04-18 16:59:18.126023 hume-0.5.0rc2/hume/_voice/microphone/microphone_interface.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676175 hume-0.5.0rc2/hume/_voice/mixins/__init__.py
--rw-r--r--   0        0        0     2166 2024-04-18 10:40:33.207487 hume-0.5.0rc2/hume/_voice/mixins/chat_mixin.py
--rw-r--r--   0        0        0     2841 2024-04-18 10:40:32.751582 hume-0.5.0rc2/hume/_voice/mixins/chats_mixin.py
--rw-r--r--   0        0        0     4744 2024-04-18 10:40:32.751861 hume-0.5.0rc2/hume/_voice/mixins/configs_mixin.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676663 hume-0.5.0rc2/hume/_voice/models/__init__.py
--rw-r--r--   0        0        0     2608 2024-04-18 10:40:32.752076 hume-0.5.0rc2/hume/_voice/models/chats_models.py
--rw-r--r--   0        0        0     1723 2024-04-18 10:40:32.752282 hume-0.5.0rc2/hume/_voice/models/configs_models.py
--rw-r--r--   0        0        0     2407 2024-04-18 10:40:33.239201 hume-0.5.0rc2/hume/_voice/voice_socket.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.0rc2/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.0rc2/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.0rc2/hume/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.0rc2/hume/models/config/__init__.py
--rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.0rc2/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.0rc2/hume/models/config/face_config.py
--rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.0rc2/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.0rc2/hume/models/config/language_config.py
--rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.0rc2/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.0rc2/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.0rc2/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.0rc2/hume/models/model_type.py
--rw-r--r--   0        0        0     2783 2024-04-18 17:55:01.519277 hume-0.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.0rc3/LICENSE
+-rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.0rc3/README.md
+-rw-r--r--   0        0        0      824 2024-04-19 22:11:56.728457 hume-0.5.0rc3/hume/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.0rc3/hume/_common/__init__.py
+-rw-r--r--   0        0        0     4853 2024-04-23 08:07:03.239984 hume-0.5.0rc3/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.0rc3/hume/_common/config_base.py
+-rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.0rc3/hume/_common/protocol.py
+-rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.0rc3/hume/_common/utilities/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.0rc3/hume/_common/utilities/config_utilities.py
+-rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.0rc3/hume/_common/utilities/model_utilities.py
+-rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.0rc3/hume/_common/utilities/paging_utilities.py
+-rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.0rc3/hume/_common/utilities/retry_utilities.py
+-rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.0rc3/hume/_common/utilities/typing_utilities.py
+-rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.0rc3/hume/_measurement/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.0rc3/hume/_measurement/batch/__init__.py
+-rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.0rc3/hume/_measurement/batch/batch_job.py
+-rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.0rc3/hume/_measurement/batch/batch_job_details.py
+-rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.0rc3/hume/_measurement/batch/batch_job_state.py
+-rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.0rc3/hume/_measurement/batch/batch_job_status.py
+-rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.0rc3/hume/_measurement/batch/hume_batch_client.py
+-rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.0rc3/hume/_measurement/batch/transcription_config.py
+-rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.0rc3/hume/_measurement/stream/__init__.py
+-rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.0rc3/hume/_measurement/stream/hume_stream_client.py
+-rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.0rc3/hume/_measurement/stream/stream_socket.py
+-rw-r--r--   0        0        0      435 2024-04-23 08:23:37.608105 hume-0.5.0rc3/hume/_voice/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-19 22:11:56.729003 hume-0.5.0rc3/hume/_voice/hume_voice_client.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.675674 hume-0.5.0rc3/hume/_voice/microphone/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-19 22:11:56.729569 hume-0.5.0rc3/hume/_voice/microphone/asyncio_utilities.py
+-rw-r--r--   0        0        0      728 2024-04-19 22:11:56.729947 hume-0.5.0rc3/hume/_voice/microphone/audio_utilities.py
+-rw-r--r--   0        0        0     2976 2024-04-23 07:40:24.964687 hume-0.5.0rc3/hume/_voice/microphone/chat_client.py
+-rw-r--r--   0        0        0     3350 2024-04-23 07:48:39.289465 hume-0.5.0rc3/hume/_voice/microphone/microphone.py
+-rw-r--r--   0        0        0     1667 2024-04-23 07:50:17.115703 hume-0.5.0rc3/hume/_voice/microphone/microphone_interface.py
+-rw-r--r--   0        0        0     2001 2024-04-23 07:52:43.076236 hume-0.5.0rc3/hume/_voice/microphone/microphone_sender.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676175 hume-0.5.0rc3/hume/_voice/mixins/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-23 08:27:51.769384 hume-0.5.0rc3/hume/_voice/mixins/chat_mixin.py
+-rw-r--r--   0        0        0     2841 2024-04-19 22:11:56.731387 hume-0.5.0rc3/hume/_voice/mixins/chats_mixin.py
+-rw-r--r--   0        0        0     4960 2024-04-23 08:24:48.860089 hume-0.5.0rc3/hume/_voice/mixins/configs_mixin.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676663 hume-0.5.0rc3/hume/_voice/models/__init__.py
+-rw-r--r--   0        0        0     2608 2024-04-19 22:11:56.732113 hume-0.5.0rc3/hume/_voice/models/chats_models.py
+-rw-r--r--   0        0        0     1860 2024-04-23 08:15:31.863465 hume-0.5.0rc3/hume/_voice/models/configs_models.py
+-rw-r--r--   0        0        0      459 2024-04-23 07:39:58.261758 hume-0.5.0rc3/hume/_voice/session_settings.py
+-rw-r--r--   0        0        0     2815 2024-04-23 08:33:34.069026 hume-0.5.0rc3/hume/_voice/voice_socket.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.0rc3/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.0rc3/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.0rc3/hume/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.0rc3/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.0rc3/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.0rc3/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.0rc3/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.0rc3/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.0rc3/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.0rc3/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.0rc3/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.0rc3/hume/models/model_type.py
+-rw-r--r--   0        0        0     2783 2024-04-23 08:41:21.680464 hume-0.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.0rc3/PKG-INFO
```

### Comparing `hume-0.5.0rc2/LICENSE` & `hume-0.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/README.md` & `hume-0.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/__init__.py` & `hume-0.5.0rc3/hume/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_common/client_base.py` & `hume-0.5.0rc3/hume/_common/client_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_common/config_base.py` & `hume-0.5.0rc3/hume/_common/config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_common/utilities/config_utilities.py` & `hume-0.5.0rc3/hume/_common/utilities/config_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_common/utilities/retry_utilities.py` & `hume-0.5.0rc3/hume/_common/utilities/retry_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/__init__.py` & `hume-0.5.0rc3/hume/_measurement/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/batch_job.py` & `hume-0.5.0rc3/hume/_measurement/batch/batch_job.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/batch_job_details.py` & `hume-0.5.0rc3/hume/_measurement/batch/batch_job_details.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/batch_job_state.py` & `hume-0.5.0rc3/hume/_measurement/batch/batch_job_state.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/batch_job_status.py` & `hume-0.5.0rc3/hume/_measurement/batch/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/hume_batch_client.py` & `hume-0.5.0rc3/hume/_measurement/batch/hume_batch_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/batch/transcription_config.py` & `hume-0.5.0rc3/hume/_measurement/batch/transcription_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/stream/hume_stream_client.py` & `hume-0.5.0rc3/hume/_measurement/stream/hume_stream_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_measurement/stream/stream_socket.py` & `hume-0.5.0rc3/hume/_measurement/stream/stream_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_voice/microphone/asyncio_utilities.py` & `hume-0.5.0rc3/hume/_voice/microphone/asyncio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_voice/microphone/audio_utilities.py` & `hume-0.5.0rc3/hume/_voice/microphone/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_voice/microphone/microphone.py` & `hume-0.5.0rc3/hume/_voice/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_voice/mixins/chat_mixin.py` & `hume-0.5.0rc3/hume/_voice/mixins/chat_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import urllib.parse
 from contextlib import asynccontextmanager
-from typing import AsyncIterator, ClassVar, Optional
+from typing import Any, AsyncIterator, ClassVar, Dict, Optional
 
 import websockets
 import websockets.client
 
 from hume._common.client_base import ClientBase
 from hume._common.protocol import Protocol
 from hume._voice.voice_socket import VoiceSocket
@@ -24,26 +24,22 @@
         """Connect to the EVI API.
 
         Args:
             config_id (Optional[str]): Config ID.
         """
         uri_base = self._build_endpoint("evi", "chat", Protocol.WS)
 
-        params = {
-            "cut_ms": VoiceSocket.DEFAULT_CUT_MS,
-            "encoding": VoiceSocket.DEFAULT_ENCODING,
-            "channels": VoiceSocket.DEFAULT_NUM_CHANNELS,
-            "sample_rate": VoiceSocket.DEFAULT_SAMPLE_RATE,
-        }
+        params: Dict[str, Any] = {}
+        if config_id is not None:
+            params["config_id"] = config_id
 
         encoded_params = urllib.parse.urlencode(params)
         uri = f"{uri_base}?{encoded_params}"
 
-        if config_id is not None:
-            uri += f"&config_id={config_id}"
+        logger.info("Connecting to EVI API at %s", uri)
 
         max_size = self.DEFAULT_MAX_PAYLOAD_SIZE_BYTES
         try:
             # pylint: disable=no-member
             async with websockets.connect(  # type: ignore[attr-defined]
                 uri,
                 extra_headers=self._get_client_headers(),
```

### Comparing `hume-0.5.0rc2/hume/_voice/mixins/chats_mixin.py` & `hume-0.5.0rc3/hume/_voice/mixins/chats_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_voice/mixins/configs_mixin.py` & `hume-0.5.0rc3/hume/_voice/mixins/configs_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,30 +9,34 @@
     ConfigResponse,
     ConfigsResponse,
     PostConfigRequest,
     PostPromptRequest,
     PromptMeta,
     PromptResponse,
     VoiceConfig,
+    VoiceIdentityConfig,
 )
 from hume.error.hume_client_exception import HumeClientException
 
 logger = logging.getLogger(__name__)
 
 
 # pylint: disable=redefined-builtin
 class ConfigsMixin(ClientBase):
     """Client operations for managing EVI configurations."""
 
+    DEFAULT_VOICE_NAME = "ITO"
+
     def create_config(
         self,
         *,
         name: str,
         prompt: str,
         description: Optional[str] = None,
+        voice_name: Optional[str] = DEFAULT_VOICE_NAME,
     ) -> VoiceConfig:
         """Create a new EVI config.
 
         Args:
             name (str): Config name.
             prompt (str): System prompt text.
             description (Optional[str]): Config description.
@@ -40,15 +44,20 @@
         post_prompt_request = PostPromptRequest(name=name, version_description=description, text=prompt)
         post_prompt_body = post_prompt_request.to_json_str()
         endpoint = self._build_endpoint("evi", "prompts")
         response = self._request(endpoint, method="POST", body_json_str=post_prompt_body)
         prompt_response = PromptResponse.model_validate_json(response.text)
         prompt_meta = PromptMeta(id=prompt_response.id, version=prompt_response.version)
 
-        post_config_request = PostConfigRequest(name=name, version_description=description, prompt=prompt_meta)
+        post_config_request = PostConfigRequest(
+            name=name,
+            version_description=description,
+            prompt=prompt_meta,
+            voice=VoiceIdentityConfig(name=voice_name),
+        )
         post_config_body = post_config_request.to_json_str()
         endpoint = self._build_endpoint("evi", "configs")
         response = self._request(endpoint, method="POST", body_json_str=post_config_body)
         config_response = ConfigResponse.model_validate_json(response.text)
 
         return self._config_from_response(config_response)
```

### Comparing `hume-0.5.0rc2/hume/_voice/models/chats_models.py` & `hume-0.5.0rc3/hume/_voice/models/chats_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/_voice/models/configs_models.py` & `hume-0.5.0rc3/hume/_voice/models/configs_models.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,20 +56,26 @@
     """Response model for a page of EVI configurations."""
 
     page_number: int
     page_size: int
     configs_page: List[ConfigResponse]
 
 
+class VoiceIdentityConfig(BaseModel):
+    provider: Optional[str] = None
+    name: Optional[str] = None
+
+
 class PostConfigRequest(BaseModel):
     """Post request model for creating a new EVI configuration."""
 
     name: str
     version_description: Optional[str]
     prompt: PromptMeta
+    voice: VoiceIdentityConfig
 
 
 class ConfigMeta(BaseModel):
     """EVI configuration metadata."""
 
     id: Optional[str]
     version: Optional[int]
```

### Comparing `hume-0.5.0rc2/hume/_voice/voice_socket.py` & `hume-0.5.0rc3/hume/_voice/voice_socket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """Voice socket connection."""
 
 import json
 import logging
 from pathlib import Path
-from typing import Any, AsyncIterator, ClassVar
+from typing import Any, AsyncIterator, ClassVar, Optional
 
 from pydub import AudioSegment
 from websockets.client import WebSocketClientProtocol as WebSocket
 
+from hume._voice.session_settings import AudioSettings, SessionSettings
+
 logger = logging.getLogger(__name__)
 
 
 class VoiceSocket:
     """Voice socket connection."""
 
     DEFAULT_CUT_MS: ClassVar[int] = 250
-    DEFAULT_ENCODING: ClassVar[str] = "linear16"
     DEFAULT_NUM_CHANNELS: ClassVar[int] = 1
     DEFAULT_SAMPLE_RATE: ClassVar[int] = 44_100
 
     def __init__(self, protocol: WebSocket):
         """Construct a `VoiceSocket`.
 
         Args:
             protocol (WebSocketClientProtocol): Protocol instance from websockets library.
 
         Raises:
             HumeClientException: If there is an error processing media over the socket connection.
         """
         self._protocol = protocol
 
+        self._num_channels = self.DEFAULT_NUM_CHANNELS
+        self._sample_rate = self.DEFAULT_SAMPLE_RATE
+
     async def __aiter__(self) -> AsyncIterator[Any]:
         """Async iterator for the voice socket."""
         async for message in self._protocol:
             yield message
 
     async def send(self, byte_str: bytes) -> None:
         """Send a byte string over the voice socket.
@@ -46,35 +50,42 @@
     async def recv(self) -> Any:
         """Receive a message on the voice socket."""
         await self._protocol.recv()
 
     async def update_session_settings(
         self,
         *,
-        encoding: str,
-        sample_rate: int,
-        num_channels: int,
+        sample_rate: Optional[int] = None,
+        num_channels: Optional[int] = None,
     ) -> None:
         """Update the EVI session settings."""
-        session_settings = {
-            "type": "session_settings",
-            "audio": {
-                "encoding": encoding,
-                "channels": num_channels,
-                "sample_rate": sample_rate,
-            },
-        }
 
-        logger.info(f"Updating session settings to: {session_settings}")
-        message = json.dumps(session_settings).encode("utf-8")
+        if num_channels is not None:
+            self._num_channels = num_channels
+        if sample_rate is not None:
+            self._sample_rate = sample_rate
+
+        session_settings = SessionSettings(
+            audio=AudioSettings(
+                channels=num_channels,
+                sample_rate=sample_rate,
+            ),
+        )
+
+        settings_dict = session_settings.model_dump(exclude_none=True)
+
+        logger.info(f"Updating session settings to: {settings_dict}")
+        message = json.dumps(settings_dict)
         await self._protocol.send(message)
 
     async def send_file(self, filepath: Path) -> None:
         """Send a file over the voice socket.
 
         Args:
             filepath (Path): Filepath to the file to send over the socket.
         """
+
         with filepath.open("rb") as f:
             segment: AudioSegment = AudioSegment.from_wav(f)
+            segment = segment.set_frame_rate(self._sample_rate).set_channels(self._num_channels)
             audio_bytes = segment.raw_data
             await self._protocol.send(audio_bytes)
```

### Comparing `hume-0.5.0rc2/hume/error/hume_client_exception.py` & `hume-0.5.0rc3/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/config/__init__.py` & `hume-0.5.0rc3/hume/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/config/face_config.py` & `hume-0.5.0rc3/hume/models/config/face_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/config/language_config.py` & `hume-0.5.0rc3/hume/models/config/language_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/config/model_config_base.py` & `hume-0.5.0rc3/hume/models/config/model_config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/config/ner_config.py` & `hume-0.5.0rc3/hume/models/config/ner_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/config/prosody_config.py` & `hume-0.5.0rc3/hume/models/config/prosody_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/hume/models/model_type.py` & `hume-0.5.0rc3/hume/models/model_type.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc2/pyproject.toml` & `hume-0.5.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,29 +30,29 @@
   "communication",
   "learning",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.5.0rc2"
+version = "0.5.0rc3"
 
 [tool.poetry.dependencies]
 httpx = { extras = ["http2"], version = "^0.27.0" }
 jupyter = { version = "^1.0.0", optional = true }
 pydantic = "^2.6.4"
 pydub = "^0.25.1"
 python = ">=3.9,<4"
 simpleaudio = { version = "^1.0.4", optional = true }
 sounddevice = { version = "^0.4.6", optional = true }
 typing-extensions = "^4.3.0"
-websockets = "^10.3"
+websockets = "^12.0"
 
 [tool.poetry.dev-dependencies]
-black = "^24.3.0"
+black = "^24.4.0"
 covcheck = { version = "^0.4.3", extras = ["toml"] }
 flake8 = "^6.0.0"
 ipykernel = "^6.22.0"
 mypy = "^1.0.1"
 pydocstyle = "^6.1.1"
 pylint = "^2.16.2"
 pyproject-flake8 = "^6.0.0"
```

### Comparing `hume-0.5.0rc2/PKG-INFO` & `hume-0.5.0rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.5.0rc2
+Version: 0.5.0rc3
 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
 Keywords: hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev
 Author-email: dev@hume.ai
 Requires-Python: >=3.9,<4
@@ -22,15 +22,15 @@
 Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "examples"
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: simpleaudio (>=1.0.4,<2.0.0) ; extra == "microphone"
 Requires-Dist: sounddevice (>=0.4.6,<0.5.0) ; extra == "microphone"
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
-Requires-Dist: websockets (>=10.3,<11.0)
+Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Repository, https://github.com/HumeAI/hume-python-sdk
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://storage.googleapis.com/hume-public-logos/hume/hume-banner.png">
   <h1>Hume AI Python SDK</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hume Version: 0.5.0rc2 Summary: Hume AI Python SDK
+Metadata-Version: 2.1 Name: hume Version: 0.5.0rc3 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
 hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -10,15 +10,15 @@
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: examples Provides-Extra: microphone Provides-
 Extra: stream Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0) Requires-Dist:
 jupyter (>=1.0.0,<2.0.0) ; extra == "examples" Requires-Dist: pydantic
 (>=2.6.4,<3.0.0) Requires-Dist: pydub (>=0.25.1,<0.26.0) Requires-Dist:
 simpleaudio (>=1.0.4,<2.0.0) ; extra == "microphone" Requires-Dist: sounddevice
 (>=0.4.6,<0.5.0) ; extra == "microphone" Requires-Dist: typing-extensions
-(>=4.3.0,<5.0.0) Requires-Dist: websockets (>=10.3,<11.0) Project-URL:
+(>=4.3.0,<5.0.0) Requires-Dist: websockets (>=12.0,<13.0) Project-URL:
 Repository, https://github.com/HumeAI/hume-python-sdk Description-Content-Type:
 text/markdown
     [https://storage.googleapis.com/hume-public-logos/hume/hume-banner.png]
                        ************ HHuummee AAII PPyytthhoonn SSDDKK ************
            IInntteeggrraattee HHuummee AAPPIIss ddiirreeccttllyy iinnttoo yyoouurr PPyytthhoonn aapppplliiccaattiioonn
 
                           _[_D_o_c_s_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_P_I_]_[_C_I_]
```

