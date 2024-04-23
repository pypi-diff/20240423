# Comparing `tmp/tetos-0.1.1.tar.gz` & `tmp/tetos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetos-0.1.1.tar", last modified: Fri Apr 19 08:51:29 2024, max compression
+gzip compressed data, was "tetos-0.2.0.tar", last modified: Tue Apr 23 02:56:27 2024, max compression
```

## Comparing `tetos-0.1.1.tar` & `tetos-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      551 2024-04-19 08:51:26.404123 tetos-0.1.1/LICENSE
--rw-r--r--   0        0        0     2469 2024-04-19 08:51:26.404123 tetos-0.1.1/README.md
--rw-r--r--   0        0        0     1377 2024-04-19 08:51:29.376090 tetos-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/__init__.py
--rw-r--r--   0        0        0      928 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/__main__.py
--rw-r--r--   0        0        0     3777 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/azure.py
--rw-r--r--   0        0        0     5210 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/baidu.py
--rw-r--r--   0        0        0     3048 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/base.py
--rw-r--r--   0        0        0    20883 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/consts.py
--rw-r--r--   0        0        0     2473 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/edge.py
--rw-r--r--   0        0        0     4891 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/google.py
--rw-r--r--   0        0        0     2770 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/openai.py
--rw-r--r--   0        0        0     9002 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/volc.py
--rw-r--r--   0        0        0     1934 2024-04-19 08:51:26.408123 tetos-0.1.1/tests/test_speakers.py
--rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 tetos-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      551 2024-04-23 02:56:23.290477 tetos-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3277 2024-04-23 02:56:23.290477 tetos-0.2.0/README.md
+-rw-r--r--   0        0        0     1777 2024-04-23 02:56:27.806508 tetos-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/__init__.py
+-rw-r--r--   0        0        0      984 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/__main__.py
+-rw-r--r--   0        0        0     3776 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/azure.py
+-rw-r--r--   0        0        0     5210 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/baidu.py
+-rw-r--r--   0        0        0     3161 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/base.py
+-rw-r--r--   0        0        0    26479 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/consts.py
+-rw-r--r--   0        0        0     2471 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/edge.py
+-rw-r--r--   0        0        0     4891 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/google.py
+-rw-r--r--   0        0        0     4457 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/minimax.py
+-rw-r--r--   0        0        0     2770 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/openai.py
+-rw-r--r--   0        0        0     9090 2024-04-23 02:56:23.290477 tetos-0.2.0/src/tetos/volc.py
+-rw-r--r--   0        0        0     1934 2024-04-23 02:56:23.290477 tetos-0.2.0/tests/test_speakers.py
+-rw-r--r--   0        0        0     4402 1970-01-01 00:00:00.000000 tetos-0.2.0/PKG-INFO
```

### Comparing `tetos-0.1.1/LICENSE` & `tetos-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tetos-0.1.1/README.md` & `tetos-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 # TeToS
+<!--index start-->
+
+[![PyPI](https://img.shields.io/pypi/v/tetos)](https://pypi.org/project/tetos/)
+[![Python](https://img.shields.io/pypi/pyversions/tetos)](https://pypi.org/project/tetos/)
+[![License](https://img.shields.io/pypi/l/tetos)](https://www.apache.org/licenses/LICENSE-2.0)
+[![Downloads](https://pepy.tech/badge/tetos)](https://pepy.tech/project/tetos)
+[![Documentation Status](https://readthedocs.org/projects/tetos/badge/?version=latest)](https://tetos.readthedocs.io/latest/?badge=latest)
 
 A unified interface for multiple Text-to-Speech (TTS) providers.
 
 
 ## Supported TTS providers
 
 - [Edge-TTS](https://github.com/rany2/edge-tts)
@@ -39,14 +46,23 @@
   Required parameters:
 
   - `api_key`: Baidu API key
   - `secret_key`: Baidu secret key
 
   [Get both at the console](https://console.bce.baidu.com/ai/#/ai/speech/app/list)
 
+- [Minimax TTS](https://www.minimaxi.com/document/speech-synthesis-engine?id=645e034eeb82db92fba9ac20)
+
+  Required parameters:
+
+  - `api_key`: Minimax API key
+  - `group_id`: Minimax group ID
+
+  Get both at the [Minimax console](https://www.minimaxi.com/user-center/basic-information)
+
 
 ## Installation
 
 Requires Python 3.8 or higher.
 
 ```bash
 pip install tetos
@@ -90,7 +106,9 @@
 
 - [x] Google TTS
 - [ ] SSML support
 
 ## License
 
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
+
+<!--index end-->
```

### Comparing `tetos-0.1.1/src/tetos/__main__.py` & `tetos-0.2.0/src/tetos/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import click
 
 from .azure import AzureSpeaker
 from .baidu import BaiduSpeaker
 from .edge import EdgeSpeaker
 from .google import GoogleSpeaker
+from .minimax import MinimaxSpeaker
 from .openai import OpenAISpeaker
 from .volc import VolcSpeaker
 
 
 def setup_logger(debug: bool = False):
     logger = logging.getLogger("tetos")
     handler = logging.StreamHandler()
@@ -27,13 +28,14 @@
 for speaker in (
     OpenAISpeaker,
     EdgeSpeaker,
     AzureSpeaker,
     VolcSpeaker,
     GoogleSpeaker,
     BaiduSpeaker,
+    MinimaxSpeaker,
 ):
     tts.add_command(speaker.get_command())
 
 
 if __name__ == "__main__":
     tts()
```

### Comparing `tetos-0.1.1/src/tetos/azure.py` & `tetos-0.2.0/src/tetos/azure.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         self, text: str, out_file: str | Path, lang: str = "en-US"
     ) -> float:
         audio_config = speechsdk.audio.AudioOutputConfig(filename=str(out_file))
         speech_synthesizer = speechsdk.SpeechSynthesizer(
             speech_config=self.get_speech_config(lang), audio_config=audio_config
         )
         result = await anyio.to_thread.run_sync(speech_synthesizer.speak_text, text)
-
         if result.reason == speechsdk.ResultReason.SynthesizingAudioCompleted:
             return result.audio_duration.total_seconds()
         elif result.reason == speechsdk.ResultReason.Canceled:
             cancellation_details = result.cancellation_details
             if cancellation_details.reason == speechsdk.CancellationReason.Error:
                 errmsg = f"Error details: {cancellation_details.error_details}"
                 raise SynthesizeError(errmsg)
```

### Comparing `tetos-0.1.1/src/tetos/baidu.py` & `tetos-0.2.0/src/tetos/baidu.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.1/src/tetos/base.py` & `tetos-0.2.0/src/tetos/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,7 +104,11 @@
             is_eager=True,
             callback=list_voices,
             expose_value=False,
         )(func)
         return func
 
     return decorator
+
+
+def filter_none(d: dict[str, Any]) -> dict[str, Any]:
+    return {k: v for k, v in d.items() if v is not None}
```

### Comparing `tetos-0.1.1/src/tetos/consts.py` & `tetos-0.2.0/src/tetos/consts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-AZURE_SUPPORTED_VOICES = [
+MICROSOFT_SUPPORTED_VOICES = [
     "af-ZA-AdriNeural",
     "af-ZA-WillemNeural",
     "am-ET-AmehaNeural",
     "am-ET-MekdesNeural",
     "ar-AE-FatimaNeural",
     "ar-AE-HamdanNeural",
     "ar-BH-AliNeural",
@@ -314,14 +314,199 @@
     "zh-HK-WanLungNeural",
     "zh-TW-HsiaoChenNeural",
     "zh-TW-HsiaoYuNeural",
     "zh-TW-YunJheNeural",
     "zu-ZA-ThandoNeural",
     "zu-ZA-ThembaNeural",
 ]
+EDGE_SUPPORTED_VOICES = [*MICROSOFT_SUPPORTED_VOICES, "en-IN-NeerjaExpressiveNeural"]
+AZURE_SUPPORTED_VOICES = [
+    *MICROSOFT_SUPPORTED_VOICES,
+    "ca-ES-AlbaNeural",
+    "de-DE-BerndNeural",
+    "de-DE-ChristophNeural",
+    "de-DE-ElkeNeural",
+    "de-DE-GiselaNeural",
+    "de-DE-KasperNeural",
+    "de-DE-KlarissaNeural",
+    "de-DE-KlausNeural",
+    "de-DE-LouisaNeural",
+    "de-DE-MajaNeural",
+    "de-DE-RalfNeural",
+    "de-DE-TanjaNeural",
+    "en-AU-AnnetteNeural",
+    "en-AU-CarlyNeural",
+    "en-AU-DarrenNeural",
+    "en-AU-DuncanNeural",
+    "en-AU-ElsieNeural",
+    "en-AU-FreyaNeural",
+    "en-AU-JoanneNeural",
+    "en-AU-KenNeural",
+    "en-AU-KimNeural",
+    "en-AU-NeilNeural",
+    "en-AU-TimNeural",
+    "en-AU-TinaNeural",
+    "en-GB-AbbiNeural",
+    "en-GB-AlfieNeural",
+    "en-GB-BellaNeural",
+    "en-GB-ElliotNeural",
+    "en-GB-EthanNeural",
+    "en-GB-HollieNeural",
+    "en-GB-NoahNeural",
+    "en-GB-OliverNeural",
+    "en-GB-OliviaNeural",
+    "en-GB-MiaNeural",
+    "en-IN-AaravNeural",
+    "en-IN-AashiNeural",
+    "en-IN-AnanyaNeural",
+    "en-IN-KavyaNeural",
+    "en-IN-KunalNeural",
+    "en-IN-RehaanNeural",
+    "en-US-DavisNeural",
+    "en-US-JaneNeural",
+    "en-US-JasonNeural",
+    "en-US-SaraNeural",
+    "en-US-TonyNeural",
+    "en-US-NancyNeural",
+    "en-US-AmberNeural",
+    "en-US-AshleyNeural",
+    "en-US-BrandonNeural",
+    "en-US-CoraNeural",
+    "en-US-ElizabethNeural",
+    "en-US-JacobNeural",
+    "en-US-JennyMultilingualNeural",
+    "en-US-MonicaNeural",
+    "en-US-RyanMultilingualNeural",
+    "en-US-AIGenerate1Neural",
+    "en-US-AIGenerate2Neural",
+    "en-US-BlueNeural",
+    "es-ES-AbrilNeural",
+    "es-ES-ArnauNeural",
+    "es-ES-DarioNeural",
+    "es-ES-EliasNeural",
+    "es-ES-EstrellaNeural",
+    "es-ES-IreneNeural",
+    "es-ES-LaiaNeural",
+    "es-ES-LiaNeural",
+    "es-ES-NilNeural",
+    "es-ES-SaulNeural",
+    "es-ES-TeoNeural",
+    "es-ES-TrianaNeural",
+    "es-ES-VeraNeural",
+    "es-MX-BeatrizNeural",
+    "es-MX-CandelaNeural",
+    "es-MX-CarlotaNeural",
+    "es-MX-CecilioNeural",
+    "es-MX-GerardoNeural",
+    "es-MX-LarissaNeural",
+    "es-MX-LibertoNeural",
+    "es-MX-LucianoNeural",
+    "es-MX-MarinaNeural",
+    "es-MX-NuriaNeural",
+    "es-MX-PelayoNeural",
+    "es-MX-RenataNeural",
+    "es-MX-YagoNeural",
+    "eu-ES-AinhoaNeural",
+    "eu-ES-AnderNeural",
+    "fi-FI-SelmaNeural",
+    "fr-FR-AlainNeural",
+    "fr-FR-BrigitteNeural",
+    "fr-FR-CelesteNeural",
+    "fr-FR-ClaudeNeural",
+    "fr-FR-CoralieNeural",
+    "fr-FR-JacquelineNeural",
+    "fr-FR-JeromeNeural",
+    "fr-FR-JosephineNeural",
+    "fr-FR-MauriceNeural",
+    "fr-FR-YvesNeural",
+    "fr-FR-YvetteNeural",
+    "hi-IN-AaravNeural",
+    "hi-IN-AnanyaNeural",
+    "hi-IN-KavyaNeural",
+    "hi-IN-KunalNeural",
+    "hi-IN-RehaanNeural",
+    "hy-AM-AnahitNeural",
+    "hy-AM-HaykNeural",
+    "it-IT-BenignoNeural",
+    "it-IT-CalimeroNeural",
+    "it-IT-CataldoNeural",
+    "it-IT-FabiolaNeural",
+    "it-IT-FiammaNeural",
+    "it-IT-GianniNeural",
+    "it-IT-ImeldaNeural",
+    "it-IT-IrmaNeural",
+    "it-IT-LisandroNeural",
+    "it-IT-PalmiraNeural",
+    "it-IT-PierinaNeural",
+    "it-IT-RinaldoNeural",
+    "ja-JP-AoiNeural",
+    "ja-JP-DaichiNeural",
+    "ja-JP-MayuNeural",
+    "ja-JP-NaokiNeural",
+    "ja-JP-ShioriNeural",
+    "ja-JP-MasaruMultilingualNeural",
+    "ko-KR-BongJinNeural",
+    "ko-KR-GookMinNeural",
+    "ko-KR-JiMinNeural",
+    "ko-KR-SeoHyeonNeural",
+    "ko-KR-SoonBokNeural",
+    "ko-KR-YuJinNeural",
+    "nb-NO-IselinNeural",
+    "pl-PL-AgnieszkaNeural",
+    "pt-BR-BrendaNeural",
+    "pt-BR-DonatoNeural",
+    "pt-BR-ElzaNeural",
+    "pt-BR-FabioNeural",
+    "pt-BR-GiovannaNeural",
+    "pt-BR-HumbertoNeural",
+    "pt-BR-JulioNeural",
+    "pt-BR-LeilaNeural",
+    "pt-BR-LeticiaNeural",
+    "pt-BR-ManuelaNeural",
+    "pt-BR-NicolauNeural",
+    "pt-BR-ValerioNeural",
+    "pt-BR-YaraNeural",
+    "pt-PT-FernandaNeural",
+    "ru-RU-DariyaNeural",
+    "sr-Latn-RS-NicholasNeural",
+    "sr-Latn-RS-SophieNeural",
+    "sv-SE-HilleviNeural",
+    "th-TH-AcharaNeural",
+    "wuu-CN-XiaotongNeural",
+    "wuu-CN-YunzheNeural",
+    "yue-CN-XiaoMinNeural",
+    "yue-CN-YunSongNeural",
+    "zh-CN-XiaochenNeural",
+    "zh-CN-XiaohanNeural",
+    "zh-CN-XiaomengNeural",
+    "zh-CN-XiaomoNeural",
+    "zh-CN-XiaoqiuNeural",
+    "zh-CN-XiaoruiNeural",
+    "zh-CN-XiaoshuangNeural",
+    "zh-CN-XiaoxiaoMultilingualNeural",
+    "zh-CN-XiaoyanNeural",
+    "zh-CN-XiaoyouNeural",
+    "zh-CN-XiaozhenNeural",
+    "zh-CN-YunfengNeural",
+    "zh-CN-YunhaoNeural",
+    "zh-CN-YunyeNeural",
+    "zh-CN-YunzeNeural",
+    "zh-CN-XiaochenMultilingualNeural",
+    "zh-CN-XiaorouNeural",
+    "zh-CN-XiaoxiaoDialectsNeural",
+    "zh-CN-XiaoyuMultilingualNeural",
+    "zh-CN-YunjieNeural",
+    "zh-CN-YunyiMultilingualNeural",
+    "zh-CN-XiaoxuanNeural",
+    "zh-CN-guangxi-YunqiNeural",
+    "zh-CN-henan-YundengNeural",
+    "zh-CN-liaoning-YunbiaoNeural",
+    "zh-CN-shandong-YunxiangNeural",
+    "zh-CN-sichuan-YunxiNeural",
+]
 
 VOLC_SUPPORTED_VOICES = [
     "zh_female_qingxin",
     "zh_male_chunhou",
     "zh_female_zhixing",
     "zh_male_qinqie",
     "zh_female_qiaopi",
@@ -855,7 +1040,32 @@
     "DuXiaoLu": 5118,
     "DuBoWen": 106,
     "DuXiaoTong": 110,
     "DuMiDuo": 103,
     "DuXiaoJiao": 5,
     "DuXiaoMeng": 111,
 }
+
+MINIMAX_SUPPORTED_VOICES = [
+    "male-qn-qingse",
+    "male-qn-jingying",
+    "male-qn-badao",
+    "male-qn-daxuesheng",
+    "female-shaonv",
+    "female-yujie",
+    "female-chengshu",
+    "female-tianmei",
+    "presenter_male",
+    "presenter_female",
+    "audiobook_male_1",
+    "audiobook_male_2",
+    "audiobook_female_1",
+    "audiobook_female_2",
+    "male-qn-qingse-jingpin",
+    "male-qn-jingying-jingpin",
+    "male-qn-badao-jingpin",
+    "male-qn-daxuesheng-jingpin",
+    "female-shaonv-jingpin",
+    "female-yujie-jingpin",
+    "female-chengshu-jingpin",
+    "female-tianmei-jingpin",
+]
```

### Comparing `tetos-0.1.1/src/tetos/edge.py` & `tetos-0.2.0/src/tetos/edge.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 
 import anyio
 import click
 
 from .base import Speaker, SynthesizeError, common_options
-from .consts import AZURE_SUPPORTED_VOICES
+from .consts import EDGE_SUPPORTED_VOICES
 
 
 @dataclass
 class EdgeSpeaker(Speaker):
     """Edge TTS speaker.
 
     Args:
@@ -57,15 +57,15 @@
             return next(
                 (v for v in self.list_voices() if v.startswith(lang)),
                 "en-US-AriaNeural",
             )
 
     @classmethod
     def list_voices(cls) -> list[str]:
-        return AZURE_SUPPORTED_VOICES
+        return EDGE_SUPPORTED_VOICES
 
     @classmethod
     def get_command(cls) -> click.Command:
         @click.command()
         @click.option("--rate", default="+0%", help="The rate of speech.")
         @click.option("--pitch", default="+0Hz", help="The pitch of speech.")
         @click.option("--volume", default="+0%", help="The volume of speech.")
```

### Comparing `tetos-0.1.1/src/tetos/google.py` & `tetos-0.2.0/src/tetos/google.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.1/src/tetos/openai.py` & `tetos-0.2.0/src/tetos/openai.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.1/src/tetos/volc.py` & `tetos-0.2.0/src/tetos/volc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import base64
 import hashlib
 import hmac
 import json
 import logging
 import time
 from datetime import datetime, timezone
@@ -66,15 +68,18 @@
                 canonical_request_hash,
             ]
         )
         sign_key = self.secret_key.encode()
         for scope in credential_scope.split("/"):
             sign_key = self.hmac_sha256(sign_key, scope)
         signature = self.hmac_sha256(sign_key, string_to_sign).hex()
-        authorization = f"{self.ALGORITHM} Credential={self.access_key}/{credential_scope}, SignedHeaders={signed_headers}, Signature={signature}"
+        authorization = (
+            f"{self.ALGORITHM} Credential={self.access_key}/{credential_scope}"
+            f", SignedHeaders={signed_headers}, Signature={signature}"
+        )
         request.headers.update(
             {
                 "Authorization": authorization,
                 "X-Content-Sha256": x_content_sha256,
                 "X-Date": x_date,
             }
         )
@@ -90,15 +95,16 @@
         app_key (str): The app key.
         voice (str, optional): The voice to use.
         sample_rate (int, optional): The sample rate.
             Available values: [8000,16000,22050,24000,32000,44100,48000],
             Defaults to 24000.
         speech_rate (int, optional): The speech rate. It should be in range [-50,100].
             100 means 2x speed and -50 means half speed. Defaults to 0.
-        pitch_rate (int, optional): The pitch rate. It should be in range [-12,12]. Defaults to 0.
+        pitch_rate (int, optional): The pitch rate. It should be in range [-12,12].
+            Defaults to 0.
     """
 
     SERVICE_NAME = "sami"
     REGION = "cn-north-1"
     AUTH_VERSION = "volc-auth-v1"
     API_HOST = "open.volcengineapi.com"
     VERSION = "2021-07-27"
```

### Comparing `tetos-0.1.1/tests/test_speakers.py` & `tetos-0.2.0/tests/test_speakers.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.1/PKG-INFO` & `tetos-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: tetos
-Version: 0.1.1
+Version: 0.2.0
 Summary: Unified interface for multiple Text-to-Speech (TTS) providers
 Keywords: tts,text-to-speech,speech,audio,ai,nlp
 Author-Email: Frost Ming <me@frostming.com>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/frostming/tetos
+Project-URL: Documentation, https://tetos.readthedocs.io/latest/
 Requires-Python: >=3.8
 Requires-Dist: edge-tts>=6.1.10
 Requires-Dist: openai>=1.20.0
 Requires-Dist: mutagen>=1.47.0
 Requires-Dist: azure-cognitiveservices-speech>=1.37.0
 Requires-Dist: anyio>=4.3.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: google-cloud-texttospeech>=2.16.3
 Description-Content-Type: text/markdown
 
 # TeToS
+<!--index start-->
+
+[![PyPI](https://img.shields.io/pypi/v/tetos)](https://pypi.org/project/tetos/)
+[![Python](https://img.shields.io/pypi/pyversions/tetos)](https://pypi.org/project/tetos/)
+[![License](https://img.shields.io/pypi/l/tetos)](https://www.apache.org/licenses/LICENSE-2.0)
+[![Downloads](https://pepy.tech/badge/tetos)](https://pepy.tech/project/tetos)
+[![Documentation Status](https://readthedocs.org/projects/tetos/badge/?version=latest)](https://tetos.readthedocs.io/latest/?badge=latest)
 
 A unified interface for multiple Text-to-Speech (TTS) providers.
 
 
 ## Supported TTS providers
 
 - [Edge-TTS](https://github.com/rany2/edge-tts)
@@ -66,14 +74,23 @@
   Required parameters:
 
   - `api_key`: Baidu API key
   - `secret_key`: Baidu secret key
 
   [Get both at the console](https://console.bce.baidu.com/ai/#/ai/speech/app/list)
 
+- [Minimax TTS](https://www.minimaxi.com/document/speech-synthesis-engine?id=645e034eeb82db92fba9ac20)
+
+  Required parameters:
+
+  - `api_key`: Minimax API key
+  - `group_id`: Minimax group ID
+
+  Get both at the [Minimax console](https://www.minimaxi.com/user-center/basic-information)
+
 
 ## Installation
 
 Requires Python 3.8 or higher.
 
 ```bash
 pip install tetos
@@ -117,7 +134,9 @@
 
 - [x] Google TTS
 - [ ] SSML support
 
 ## License
 
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
+
+<!--index end-->
```

