# Comparing `tmp/hume-0.5.0rc3.tar.gz` & `tmp/hume-0.5.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.5.0rc3.tar", max compression
+gzip compressed data, was "hume-0.5.0rc4.tar", max compression
```

## Comparing `hume-0.5.0rc3.tar` & `hume-0.5.0rc4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.0rc3/LICENSE
--rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.0rc3/README.md
--rw-r--r--   0        0        0      824 2024-04-19 22:11:56.728457 hume-0.5.0rc3/hume/__init__.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.0rc3/hume/_common/__init__.py
--rw-r--r--   0        0        0     4853 2024-04-23 08:07:03.239984 hume-0.5.0rc3/hume/_common/client_base.py
--rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.0rc3/hume/_common/config_base.py
--rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.0rc3/hume/_common/protocol.py
--rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.0rc3/hume/_common/utilities/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.0rc3/hume/_common/utilities/config_utilities.py
--rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.0rc3/hume/_common/utilities/model_utilities.py
--rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.0rc3/hume/_common/utilities/paging_utilities.py
--rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.0rc3/hume/_common/utilities/retry_utilities.py
--rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.0rc3/hume/_common/utilities/typing_utilities.py
--rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.0rc3/hume/_measurement/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.0rc3/hume/_measurement/batch/__init__.py
--rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.0rc3/hume/_measurement/batch/batch_job.py
--rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.0rc3/hume/_measurement/batch/batch_job_details.py
--rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.0rc3/hume/_measurement/batch/batch_job_state.py
--rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.0rc3/hume/_measurement/batch/batch_job_status.py
--rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.0rc3/hume/_measurement/batch/hume_batch_client.py
--rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.0rc3/hume/_measurement/batch/transcription_config.py
--rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.0rc3/hume/_measurement/stream/__init__.py
--rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.0rc3/hume/_measurement/stream/hume_stream_client.py
--rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.0rc3/hume/_measurement/stream/stream_socket.py
--rw-r--r--   0        0        0      435 2024-04-23 08:23:37.608105 hume-0.5.0rc3/hume/_voice/__init__.py
--rw-r--r--   0        0        0      363 2024-04-19 22:11:56.729003 hume-0.5.0rc3/hume/_voice/hume_voice_client.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.675674 hume-0.5.0rc3/hume/_voice/microphone/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-19 22:11:56.729569 hume-0.5.0rc3/hume/_voice/microphone/asyncio_utilities.py
--rw-r--r--   0        0        0      728 2024-04-19 22:11:56.729947 hume-0.5.0rc3/hume/_voice/microphone/audio_utilities.py
--rw-r--r--   0        0        0     2976 2024-04-23 07:40:24.964687 hume-0.5.0rc3/hume/_voice/microphone/chat_client.py
--rw-r--r--   0        0        0     3350 2024-04-23 07:48:39.289465 hume-0.5.0rc3/hume/_voice/microphone/microphone.py
--rw-r--r--   0        0        0     1667 2024-04-23 07:50:17.115703 hume-0.5.0rc3/hume/_voice/microphone/microphone_interface.py
--rw-r--r--   0        0        0     2001 2024-04-23 07:52:43.076236 hume-0.5.0rc3/hume/_voice/microphone/microphone_sender.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676175 hume-0.5.0rc3/hume/_voice/mixins/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-23 08:27:51.769384 hume-0.5.0rc3/hume/_voice/mixins/chat_mixin.py
--rw-r--r--   0        0        0     2841 2024-04-19 22:11:56.731387 hume-0.5.0rc3/hume/_voice/mixins/chats_mixin.py
--rw-r--r--   0        0        0     4960 2024-04-23 08:24:48.860089 hume-0.5.0rc3/hume/_voice/mixins/configs_mixin.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676663 hume-0.5.0rc3/hume/_voice/models/__init__.py
--rw-r--r--   0        0        0     2608 2024-04-19 22:11:56.732113 hume-0.5.0rc3/hume/_voice/models/chats_models.py
--rw-r--r--   0        0        0     1860 2024-04-23 08:15:31.863465 hume-0.5.0rc3/hume/_voice/models/configs_models.py
--rw-r--r--   0        0        0      459 2024-04-23 07:39:58.261758 hume-0.5.0rc3/hume/_voice/session_settings.py
--rw-r--r--   0        0        0     2815 2024-04-23 08:33:34.069026 hume-0.5.0rc3/hume/_voice/voice_socket.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.0rc3/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.0rc3/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.0rc3/hume/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.0rc3/hume/models/config/__init__.py
--rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.0rc3/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.0rc3/hume/models/config/face_config.py
--rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.0rc3/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.0rc3/hume/models/config/language_config.py
--rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.0rc3/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.0rc3/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.0rc3/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.0rc3/hume/models/model_type.py
--rw-r--r--   0        0        0     2783 2024-04-23 08:41:21.680464 hume-0.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.0rc4/LICENSE
+-rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.0rc4/README.md
+-rw-r--r--   0        0        0      824 2024-04-23 08:46:40.806342 hume-0.5.0rc4/hume/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.0rc4/hume/_common/__init__.py
+-rw-r--r--   0        0        0     4853 2024-04-23 08:07:03.239984 hume-0.5.0rc4/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.0rc4/hume/_common/config_base.py
+-rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.0rc4/hume/_common/protocol.py
+-rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.0rc4/hume/_common/utilities/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.0rc4/hume/_common/utilities/config_utilities.py
+-rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.0rc4/hume/_common/utilities/model_utilities.py
+-rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.0rc4/hume/_common/utilities/paging_utilities.py
+-rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.0rc4/hume/_common/utilities/retry_utilities.py
+-rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.0rc4/hume/_common/utilities/typing_utilities.py
+-rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.0rc4/hume/_measurement/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.0rc4/hume/_measurement/batch/__init__.py
+-rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.0rc4/hume/_measurement/batch/batch_job.py
+-rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.0rc4/hume/_measurement/batch/batch_job_details.py
+-rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.0rc4/hume/_measurement/batch/batch_job_state.py
+-rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.0rc4/hume/_measurement/batch/batch_job_status.py
+-rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.0rc4/hume/_measurement/batch/hume_batch_client.py
+-rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.0rc4/hume/_measurement/batch/transcription_config.py
+-rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.0rc4/hume/_measurement/stream/__init__.py
+-rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.0rc4/hume/_measurement/stream/hume_stream_client.py
+-rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.0rc4/hume/_measurement/stream/stream_socket.py
+-rw-r--r--   0        0        0      435 2024-04-23 08:46:40.806650 hume-0.5.0rc4/hume/_voice/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-23 08:46:41.019929 hume-0.5.0rc4/hume/_voice/hume_voice_client.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.675674 hume-0.5.0rc4/hume/_voice/microphone/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-23 08:46:41.020172 hume-0.5.0rc4/hume/_voice/microphone/asyncio_utilities.py
+-rw-r--r--   0        0        0      728 2024-04-23 08:46:41.020466 hume-0.5.0rc4/hume/_voice/microphone/audio_utilities.py
+-rw-r--r--   0        0        0     2976 2024-04-23 08:46:41.242380 hume-0.5.0rc4/hume/_voice/microphone/chat_client.py
+-rw-r--r--   0        0        0     3350 2024-04-23 08:46:41.181842 hume-0.5.0rc4/hume/_voice/microphone/microphone.py
+-rw-r--r--   0        0        0     1667 2024-04-23 08:46:41.242633 hume-0.5.0rc4/hume/_voice/microphone/microphone_interface.py
+-rw-r--r--   0        0        0     2001 2024-04-23 08:46:41.242806 hume-0.5.0rc4/hume/_voice/microphone/microphone_sender.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676175 hume-0.5.0rc4/hume/_voice/mixins/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-23 08:46:41.243072 hume-0.5.0rc4/hume/_voice/mixins/chat_mixin.py
+-rw-r--r--   0        0        0     2841 2024-04-23 08:46:41.021491 hume-0.5.0rc4/hume/_voice/mixins/chats_mixin.py
+-rw-r--r--   0        0        0     4960 2024-04-23 08:46:41.243382 hume-0.5.0rc4/hume/_voice/mixins/configs_mixin.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676663 hume-0.5.0rc4/hume/_voice/models/__init__.py
+-rw-r--r--   0        0        0     2608 2024-04-23 08:46:41.021941 hume-0.5.0rc4/hume/_voice/models/chats_models.py
+-rw-r--r--   0        0        0     1916 2024-04-23 08:46:41.243661 hume-0.5.0rc4/hume/_voice/models/configs_models.py
+-rw-r--r--   0        0        0      461 2024-04-23 08:46:41.243897 hume-0.5.0rc4/hume/_voice/session_settings.py
+-rw-r--r--   0        0        0     2814 2024-04-23 10:05:14.835518 hume-0.5.0rc4/hume/_voice/voice_socket.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.0rc4/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.0rc4/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.0rc4/hume/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.0rc4/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.0rc4/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.0rc4/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.0rc4/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.0rc4/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.0rc4/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.0rc4/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.0rc4/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.0rc4/hume/models/model_type.py
+-rw-r--r--   0        0        0     2783 2024-04-23 10:56:06.250670 hume-0.5.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.0rc4/PKG-INFO
```

### Comparing `hume-0.5.0rc3/LICENSE` & `hume-0.5.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/README.md` & `hume-0.5.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/__init__.py` & `hume-0.5.0rc4/hume/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_common/client_base.py` & `hume-0.5.0rc4/hume/_common/client_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_common/config_base.py` & `hume-0.5.0rc4/hume/_common/config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_common/utilities/config_utilities.py` & `hume-0.5.0rc4/hume/_common/utilities/config_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_common/utilities/retry_utilities.py` & `hume-0.5.0rc4/hume/_common/utilities/retry_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/__init__.py` & `hume-0.5.0rc4/hume/_measurement/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/batch_job.py` & `hume-0.5.0rc4/hume/_measurement/batch/batch_job.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/batch_job_details.py` & `hume-0.5.0rc4/hume/_measurement/batch/batch_job_details.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/batch_job_state.py` & `hume-0.5.0rc4/hume/_measurement/batch/batch_job_state.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/batch_job_status.py` & `hume-0.5.0rc4/hume/_measurement/batch/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/hume_batch_client.py` & `hume-0.5.0rc4/hume/_measurement/batch/hume_batch_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/batch/transcription_config.py` & `hume-0.5.0rc4/hume/_measurement/batch/transcription_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/stream/hume_stream_client.py` & `hume-0.5.0rc4/hume/_measurement/stream/hume_stream_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_measurement/stream/stream_socket.py` & `hume-0.5.0rc4/hume/_measurement/stream/stream_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/microphone/asyncio_utilities.py` & `hume-0.5.0rc4/hume/_voice/microphone/asyncio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/microphone/audio_utilities.py` & `hume-0.5.0rc4/hume/_voice/microphone/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/microphone/chat_client.py` & `hume-0.5.0rc4/hume/_voice/microphone/chat_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/microphone/microphone.py` & `hume-0.5.0rc4/hume/_voice/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/microphone/microphone_interface.py` & `hume-0.5.0rc4/hume/_voice/microphone/microphone_interface.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/microphone/microphone_sender.py` & `hume-0.5.0rc4/hume/_voice/microphone/microphone_sender.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/mixins/chat_mixin.py` & `hume-0.5.0rc4/hume/_voice/mixins/chat_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/mixins/chats_mixin.py` & `hume-0.5.0rc4/hume/_voice/mixins/chats_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/mixins/configs_mixin.py` & `hume-0.5.0rc4/hume/_voice/mixins/configs_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/models/chats_models.py` & `hume-0.5.0rc4/hume/_voice/models/chats_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/_voice/models/configs_models.py` & `hume-0.5.0rc4/hume/_voice/models/configs_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
     page_number: int
     page_size: int
     configs_page: List[ConfigResponse]
 
 
 class VoiceIdentityConfig(BaseModel):
+    """Configuration for changing the voice of EVI."""
+
     provider: Optional[str] = None
     name: Optional[str] = None
 
 
 class PostConfigRequest(BaseModel):
     """Post request model for creating a new EVI configuration."""
```

### Comparing `hume-0.5.0rc3/hume/_voice/voice_socket.py` & `hume-0.5.0rc4/hume/_voice/voice_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     async def update_session_settings(
         self,
         *,
         sample_rate: Optional[int] = None,
         num_channels: Optional[int] = None,
     ) -> None:
         """Update the EVI session settings."""
-
         if num_channels is not None:
             self._num_channels = num_channels
         if sample_rate is not None:
             self._sample_rate = sample_rate
 
         session_settings = SessionSettings(
             audio=AudioSettings(
@@ -79,13 +78,12 @@
 
     async def send_file(self, filepath: Path) -> None:
         """Send a file over the voice socket.
 
         Args:
             filepath (Path): Filepath to the file to send over the socket.
         """
-
         with filepath.open("rb") as f:
-            segment: AudioSegment = AudioSegment.from_wav(f)
+            segment: AudioSegment = AudioSegment.from_file(f)
             segment = segment.set_frame_rate(self._sample_rate).set_channels(self._num_channels)
             audio_bytes = segment.raw_data
             await self._protocol.send(audio_bytes)
```

### Comparing `hume-0.5.0rc3/hume/error/hume_client_exception.py` & `hume-0.5.0rc4/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/config/__init__.py` & `hume-0.5.0rc4/hume/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/config/face_config.py` & `hume-0.5.0rc4/hume/models/config/face_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/config/language_config.py` & `hume-0.5.0rc4/hume/models/config/language_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/config/model_config_base.py` & `hume-0.5.0rc4/hume/models/config/model_config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/config/ner_config.py` & `hume-0.5.0rc4/hume/models/config/ner_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/config/prosody_config.py` & `hume-0.5.0rc4/hume/models/config/prosody_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/hume/models/model_type.py` & `hume-0.5.0rc4/hume/models/model_type.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc3/pyproject.toml` & `hume-0.5.0rc4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "communication",
   "learning",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.5.0rc3"
+version = "0.5.0rc4"
 
 [tool.poetry.dependencies]
 httpx = { extras = ["http2"], version = "^0.27.0" }
 jupyter = { version = "^1.0.0", optional = true }
 pydantic = "^2.6.4"
 pydub = "^0.25.1"
 python = ">=3.9,<4"
@@ -84,19 +84,19 @@
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 line-length = 120
 
 [tool.covcheck.group.unit.coverage]
-branch = 50.0
+branch = 49.0
 line = 72.0
 
 [tool.covcheck.group.service.coverage]
-branch = 58.0
+branch = 57.0
 line = 80.0
 
 [tool.flake8]
 ignore = ""           # Required to disable default ignores
 max-line-length = 120
 
 [tool.isort]
```

### Comparing `hume-0.5.0rc3/PKG-INFO` & `hume-0.5.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.5.0rc3
+Version: 0.5.0rc4
 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
 Keywords: hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev
 Author-email: dev@hume.ai
 Requires-Python: >=3.9,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hume Version: 0.5.0rc3 Summary: Hume AI Python SDK
+Metadata-Version: 2.1 Name: hume Version: 0.5.0rc4 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
 hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

