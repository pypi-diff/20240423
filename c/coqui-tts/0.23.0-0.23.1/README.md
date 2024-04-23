# Comparing `tmp/coqui_tts-0.23.0.tar.gz` & `tmp/coqui_tts-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coqui_tts-0.23.0.tar", last modified: Fri Apr 19 12:26:04 2024, max compression
+gzip compressed data, was "coqui_tts-0.23.1.tar", last modified: Tue Apr 23 14:02:31 2024, max compression
```

## Comparing `coqui_tts-0.23.0.tar` & `coqui_tts-0.23.1.tar`

### file list

```diff
@@ -1,390 +1,390 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.784660 coqui_tts-0.23.0/TTS/
--rw-r--r--   0 runner    (1001) docker     (127)    44046 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/.models.json
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20591 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/collect_env_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/compute_attention_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/compute_embeddings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/compute_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/eval_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9602 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/extract_tts_spectrograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/find_unique_chars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/find_unique_phonemes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4433 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/remove_silence_using_vad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/resample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16672 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/synthesize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/train_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/train_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/train_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/tune_wavegrad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/config/shared_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.772660 coqui_tts-0.23.0/TTS/demos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/gpt_train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/xtts_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/encoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/encoder/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/configs/base_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/configs/emotion_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/configs/speaker_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/encoder/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/models/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/models/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/encoder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/prepare_voxceleb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/static/coqui-log-green-TTS.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/templates/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/align_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/bark_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/delightful_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/fast_pitch_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/fast_speech_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/fastspeech2_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/glow_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/neuralhmm_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/overflow_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/shared_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/speedy_speech_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/tacotron2_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/tacotron_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/tortoise_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/vits_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/xtts_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37839 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    28004 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/datasets/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/layers/align_tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/align_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/align_tts/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/align_tts/mdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/layers/bark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.800660 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/hubert_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/kmeans_hubert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26202 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/inference_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/model_fine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.800660 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/acoustic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23945 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conv_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/energy_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/kernel_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/pitch_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/variance_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.800660 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/aligner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/pos_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/res_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/time_depth_sep_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/wavenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/glow.py
--rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35686 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/overflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/common_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/neural_hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/plotting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/tacotron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/attentions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/capacitron_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/common_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/gst_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.808660 coqui_tts-0.23.0/TTS/tts/layers/tortoise/
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/arch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/audio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/clvp.py
--rw-r--r--   0 runner    (1001) docker     (127)    51012 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    72348 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/random_latent_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/wav2vec_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    41480 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/xtransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.808660 coqui_tts-0.23.0/TTS/tts/layers/vits/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/stochastic_duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.812660 coqui_tts-0.23.0/TTS/tts/layers/xtts/
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/dvae.py
--rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    25094 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/hifigan_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/latent_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/perceiver_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46561 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/stream_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    31005 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.812660 coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/gpt_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/xtts_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    59442 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/zh_num2words.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.816660 coqui_tts-0.23.0/TTS/tts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/align_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/bark.py
--rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/base_tacotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    20192 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/base_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    70351 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/delightful_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    35665 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/forward_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/glow_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17382 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/neuralhmm_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/overflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/tacotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (127)    42373 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/tortoise.py
--rw-r--r--   0 runner    (1001) docker     (127)    81986 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/vits.py
--rw-r--r--   0 runner    (1001) docker     (127)    32412 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/xtts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.816660 coqui_tts-0.23.0/TTS/tts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.776660 coqui_tts-0.23.0/TTS/tts/utils/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.816660 coqui_tts-0.23.0/TTS/tts/utils/assets/tortoise/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/assets/tortoise/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/fairseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   868695 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.c
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/speakers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/bangla/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/bangla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/bangla/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/characters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/cmudict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/english/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/number_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/time_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/french/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/french/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/french/abbreviations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/japanese/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/japanese/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/japanese/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/korean/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/ko_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/korean.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/punctuation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/utils/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15603 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/numpy_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/torch_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/capacitron_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/distribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/radam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22967 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.780660 coqui_tts-0.23.0/TTS/vc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/configs/freevc_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/configs/shared_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/models/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18826 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/models/base_vc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/models/freevc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/modules/freevc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/mel_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/wavlm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vocoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vocoder/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/fullband_melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/hifigan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/multiband_melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/parallel_wavegan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/shared_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/univnet_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/wavegrad_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/wavernn_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.836660 coqui_tts-0.23.0/TTS/vocoder/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/gan_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/wavegrad_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/wavernn_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.836660 coqui_tts-0.23.0/TTS/vocoder/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/lvc_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/melgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/parallel_wavegan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/pqmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/wavegrad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.840660 coqui_tts-0.23.0/TTS/vocoder/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/base_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/fullband_melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/hifigan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/hifigan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/melgan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/melgan_multiscale_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/multiband_melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/random_window_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/univnet_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/univnet_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/wavegrad.py
--rw-r--r--   0 runner    (1001) docker     (127)    25204 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/wavernn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.840660 coqui_tts-0.23.0/TTS/vocoder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/utils/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/utils/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/coqui_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.840660 coqui_tts-0.23.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/images/coqui-log-green-TTS.png
--rw-r--r--   0 runner    (1001) docker     (127)   474464 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/images/example_model_output.png
--rw-r--r--   0 runner    (1001) docker     (127)   149914 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/images/model.png
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.ja.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.536528 coqui_tts-0.23.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-23 14:02:31.536528 coqui_tts-0.23.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.476529 coqui_tts-0.23.1/TTS/
+-rw-r--r--   0 runner    (1001) docker     (127)    44046 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/.models.json
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20591 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.476529 coqui_tts-0.23.1/TTS/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/collect_env_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/compute_attention_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/compute_embeddings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/compute_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/eval_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9602 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/extract_tts_spectrograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/find_unique_chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/find_unique_phonemes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4433 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/remove_silence_using_vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16672 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/synthesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/train_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/train_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/train_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/bin/tune_wavegrad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.476529 coqui_tts-0.23.1/TTS/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/config/shared_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.464528 coqui_tts-0.23.1/TTS/demos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.476529 coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.476529 coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/utils/gpt_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/xtts_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/encoder/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/configs/base_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/configs/emotion_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/configs/speaker_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/encoder/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/models/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/models/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/encoder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/utils/prepare_voxceleb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/utils/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/encoder/utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/static/coqui-log-green-TTS.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.480528 coqui_tts-0.23.1/TTS/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.484528 coqui_tts-0.23.1/TTS/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.484528 coqui_tts-0.23.1/TTS/tts/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/align_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/bark_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/delightful_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/fast_pitch_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/fast_speech_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/fastspeech2_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/glow_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/neuralhmm_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/overflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/shared_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/speedy_speech_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/tacotron2_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/tacotron_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/tortoise_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/vits_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/configs/xtts_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.484528 coqui_tts-0.23.1/TTS/tts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37839 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28004 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/datasets/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.484528 coqui_tts-0.23.1/TTS/tts/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.488528 coqui_tts-0.23.1/TTS/tts/layers/align_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/align_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/align_tts/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/align_tts/mdn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.488528 coqui_tts-0.23.1/TTS/tts/layers/bark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.488528 coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/hubert_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/kmeans_hubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26202 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/inference_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/bark/model_fine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.492528 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/acoustic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23945 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/conv_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/energy_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/kernel_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/pitch_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/variance_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.492528 coqui_tts-0.23.1/TTS/tts/layers/feed_forward/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/feed_forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/feed_forward/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/feed_forward/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/feed_forward/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.492528 coqui_tts-0.23.1/TTS/tts/layers/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/pos_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/res_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/time_depth_sep_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/generic/wavenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.492528 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/glow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/glow_tts/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35686 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.496528 coqui_tts-0.23.1/TTS/tts/layers/overflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/overflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/overflow/common_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/overflow/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/overflow/neural_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/overflow/plotting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.496528 coqui_tts-0.23.1/TTS/tts/layers/tacotron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/capacitron_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/common_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/gst_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tacotron/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.500528 coqui_tts-0.23.1/TTS/tts/layers/tortoise/
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/arch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/audio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/clvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51012 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/diffusion_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72348 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/random_latent_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/wav2vec_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41480 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/tortoise/xtransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.500528 coqui_tts-0.23.1/TTS/tts/layers/vits/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/vits/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/vits/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/vits/stochastic_duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/vits/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.500528 coqui_tts-0.23.1/TTS/tts/layers/xtts/
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/dvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/gpt_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25094 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/hifigan_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/latent_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/perceiver_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46561 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/stream_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31005 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.500528 coqui_tts-0.23.1/TTS/tts/layers/xtts/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/trainer/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/trainer/gpt_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/xtts_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59442 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/layers/xtts/zh_num2words.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.504528 coqui_tts-0.23.1/TTS/tts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/align_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/bark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/base_tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20192 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/base_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70351 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/delightful_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35665 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/forward_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/glow_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17382 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/neuralhmm_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/overflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42373 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/tortoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81986 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/vits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32412 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/models/xtts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.508528 coqui_tts-0.23.1/TTS/tts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.468529 coqui_tts-0.23.1/TTS/tts/utils/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.508528 coqui_tts-0.23.1/TTS/tts/utils/assets/tortoise/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/assets/tortoise/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/fairseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.508528 coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   868695 2024-04-23 14:02:30.000000 coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/speakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.508528 coqui_tts-0.23.1/TTS/tts/utils/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/bangla/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/bangla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/bangla/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/belarusian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/belarusian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/belarusian/phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/characters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/cmudict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/english/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/english/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/english/abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/english/number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/english/time_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/french/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/french/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/french/abbreviations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/japanese/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/japanese/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/japanese/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.512528 coqui_tts-0.23.1/TTS/tts/utils/text/korean/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/korean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/korean/ko_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/korean/korean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/korean/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.516528 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/espeak_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/gruut_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/multi_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/text/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/tts/utils/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.516528 coqui_tts-0.23.1/TTS/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.520528 coqui_tts-0.23.1/TTS/utils/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15603 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/audio/numpy_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/audio/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/audio/torch_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/capacitron_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/radam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22967 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/utils/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.468529 coqui_tts-0.23.1/TTS/vc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.520528 coqui_tts-0.23.1/TTS/vc/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/configs/freevc_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/configs/shared_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.520528 coqui_tts-0.23.1/TTS/vc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18826 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/models/base_vc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/models/freevc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.520528 coqui_tts-0.23.1/TTS/vc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.520528 coqui_tts-0.23.1/TTS/vc/modules/freevc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/mel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.520528 coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.524528 coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/wavlm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.524528 coqui_tts-0.23.1/TTS/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.524528 coqui_tts-0.23.1/TTS/vocoder/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/fullband_melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/hifigan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/multiband_melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/parallel_wavegan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/shared_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/univnet_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/wavegrad_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/configs/wavernn_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.524528 coqui_tts-0.23.1/TTS/vocoder/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/datasets/gan_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/datasets/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/datasets/wavegrad_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/datasets/wavernn_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.528528 coqui_tts-0.23.1/TTS/vocoder/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/lvc_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/melgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/parallel_wavegan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/pqmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/layers/wavegrad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.528528 coqui_tts-0.23.1/TTS/vocoder/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/base_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/fullband_melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14527 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/hifigan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/hifigan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/melgan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/melgan_multiscale_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/multiband_melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/parallel_wavegan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/parallel_wavegan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/random_window_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/univnet_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/univnet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/wavegrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25204 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/models/wavernn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.532528 coqui_tts-0.23.1/TTS/vocoder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/utils/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/TTS/vocoder/utils/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.532528 coqui_tts-0.23.1/coqui_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-23 14:02:31.000000 coqui_tts-0.23.1/coqui_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-23 14:02:31.000000 coqui_tts-0.23.1/coqui_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:02:31.000000 coqui_tts-0.23.1/coqui_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 14:02:31.000000 coqui_tts-0.23.1/coqui_tts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:02:30.000000 coqui_tts-0.23.1/coqui_tts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 14:02:31.000000 coqui_tts-0.23.1/coqui_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 14:02:31.000000 coqui_tts-0.23.1/coqui_tts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:02:31.532528 coqui_tts-0.23.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/images/coqui-log-green-TTS.png
+-rw-r--r--   0 runner    (1001) docker     (127)   474464 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/images/example_model_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)   149914 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/images/model.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/requirements.ja.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/requirements.notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 14:02:31.536528 coqui_tts-0.23.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-23 14:02:21.000000 coqui_tts-0.23.1/setup.py
```

### Comparing `coqui_tts-0.23.0/CITATION.cff` & `coqui_tts-0.23.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/LICENSE.txt` & `coqui_tts-0.23.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/PKG-INFO` & `coqui_tts-0.23.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coqui-tts
-Version: 0.23.0
+Version: 0.23.1
 Summary: Deep learning for Text to Speech.
 Home-page: https://github.com/idiap/coqui-ai-TTS
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 Maintainer: Enno Hermann
 Maintainer-email: enno.hermann@gmail.com
 License: MPL-2.0
@@ -13,26 +13,27 @@
 Project-URL: Repository, https://github.com/idiap/coqui-ai-TTS
 Project-URL: Discussions, https://github.com/idiap/coqui-ai-TTS/discussions
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9.0, <3.12
+Requires-Python: >=3.9.0, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: cython>=0.29.30
 Requires-Dist: scipy>=1.11.2
 Requires-Dist: torch>=2.1
 Requires-Dist: torchaudio
@@ -43,15 +44,15 @@
 Requires-Dist: anyascii>=0.3.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fsspec[http]>=2023.6.0
 Requires-Dist: packaging>=23.1
 Requires-Dist: pysbd>=0.3.4
 Requires-Dist: umap-learn>=0.5.1
 Requires-Dist: matplotlib>=3.7.0
-Requires-Dist: trainer>=0.0.36
+Requires-Dist: coqui-tts-trainer>=0.1
 Requires-Dist: coqpit>=0.0.16
 Requires-Dist: jieba
 Requires-Dist: pypinyin
 Requires-Dist: hangul_romanize
 Requires-Dist: gruut[de,es,fr]==2.2.3
 Requires-Dist: jamo
 Requires-Dist: g2pkk>=0.1.1
@@ -66,30 +67,30 @@
 Provides-Extra: all
 Requires-Dist: black==24.2.0; extra == "all"
 Requires-Dist: coverage[toml]; extra == "all"
 Requires-Dist: nose2; extra == "all"
 Requires-Dist: ruff==0.3.0; extra == "all"
 Requires-Dist: bokeh==1.4.0; extra == "all"
 Requires-Dist: pandas<2.0,>=1.4; extra == "all"
-Requires-Dist: mecab-python3==1.0.6; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
 Requires-Dist: unidic-lite==1.0.8; extra == "all"
 Requires-Dist: cutlet; extra == "all"
 Requires-Dist: flask>=2.0.1; extra == "all"
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: nose2; extra == "dev"
 Requires-Dist: ruff==0.3.0; extra == "dev"
 Provides-Extra: notebooks
 Requires-Dist: bokeh==1.4.0; extra == "notebooks"
 Requires-Dist: pandas<2.0,>=1.4; extra == "notebooks"
 Provides-Extra: server
 Requires-Dist: flask>=2.0.1; extra == "server"
 Provides-Extra: ja
-Requires-Dist: mecab-python3==1.0.6; extra == "ja"
+Requires-Dist: mecab-python3; extra == "ja"
 Requires-Dist: unidic-lite==1.0.8; extra == "ja"
 Requires-Dist: cutlet; extra == "ja"
 
 
 ## 🐸Coqui TTS News
 - 📣 Fork of the [original, unmaintained repository](https://github.com/coqui-ai/TTS). New PyPI package: [coqui-tts](https://pypi.org/project/coqui-tts)
 - 📣 ⓍTTSv2 is here with 16 languages and better performance across the board.
@@ -218,15 +219,15 @@
 
 ### Voice Conversion
 - FreeVC: [paper](https://arxiv.org/abs/2210.15418)
 
 You can also help us implement more models.
 
 ## Installation
-🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.12.**.
+🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.13.**.
 
 If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the released 🐸TTS models, installing from PyPI is the easiest option.
 
 ```bash
 pip install coqui-tts
 ```
```

### Comparing `coqui_tts-0.23.0/README.md` & `coqui_tts-0.23.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 ### Voice Conversion
 - FreeVC: [paper](https://arxiv.org/abs/2210.15418)
 
 You can also help us implement more models.
 
 ## Installation
-🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.12.**.
+🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.13.**.
 
 If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the released 🐸TTS models, installing from PyPI is the easiest option.
 
 ```bash
 pip install coqui-tts
 ```
```

### Comparing `coqui_tts-0.23.0/TTS/.models.json` & `coqui_tts-0.23.1/TTS/.models.json`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/api.py` & `coqui_tts-0.23.1/TTS/api.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/collect_env_info.py` & `coqui_tts-0.23.1/TTS/bin/collect_env_info.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/compute_attention_masks.py` & `coqui_tts-0.23.1/TTS/bin/compute_attention_masks.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/compute_embeddings.py` & `coqui_tts-0.23.1/TTS/bin/compute_embeddings.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/compute_statistics.py` & `coqui_tts-0.23.1/TTS/bin/compute_statistics.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/eval_encoder.py` & `coqui_tts-0.23.1/TTS/bin/eval_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/extract_tts_spectrograms.py` & `coqui_tts-0.23.1/TTS/bin/extract_tts_spectrograms.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/find_unique_chars.py` & `coqui_tts-0.23.1/TTS/bin/find_unique_chars.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/find_unique_phonemes.py` & `coqui_tts-0.23.1/TTS/bin/find_unique_phonemes.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/remove_silence_using_vad.py` & `coqui_tts-0.23.1/TTS/bin/remove_silence_using_vad.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/resample.py` & `coqui_tts-0.23.1/TTS/bin/resample.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/synthesize.py` & `coqui_tts-0.23.1/TTS/bin/synthesize.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/train_encoder.py` & `coqui_tts-0.23.1/TTS/bin/train_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/train_tts.py` & `coqui_tts-0.23.1/TTS/bin/train_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/train_vocoder.py` & `coqui_tts-0.23.1/TTS/bin/train_vocoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/bin/tune_wavegrad.py` & `coqui_tts-0.23.1/TTS/bin/tune_wavegrad.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/config/__init__.py` & `coqui_tts-0.23.1/TTS/config/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/config/shared_configs.py` & `coqui_tts-0.23.1/TTS/config/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/formatter.py` & `coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/gpt_train.py` & `coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/utils/gpt_train.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/xtts_demo.py` & `coqui_tts-0.23.1/TTS/demos/xtts_ft_demo/xtts_demo.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/README.md` & `coqui_tts-0.23.1/TTS/encoder/README.md`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/configs/base_encoder_config.py` & `coqui_tts-0.23.1/TTS/encoder/configs/base_encoder_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/dataset.py` & `coqui_tts-0.23.1/TTS/encoder/dataset.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/losses.py` & `coqui_tts-0.23.1/TTS/encoder/losses.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/models/base_encoder.py` & `coqui_tts-0.23.1/TTS/encoder/models/base_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/models/lstm.py` & `coqui_tts-0.23.1/TTS/encoder/models/lstm.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/models/resnet.py` & `coqui_tts-0.23.1/TTS/encoder/models/resnet.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/utils/generic_utils.py` & `coqui_tts-0.23.1/TTS/encoder/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/utils/prepare_voxceleb.py` & `coqui_tts-0.23.1/TTS/encoder/utils/prepare_voxceleb.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/utils/training.py` & `coqui_tts-0.23.1/TTS/encoder/utils/training.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/encoder/utils/visual.py` & `coqui_tts-0.23.1/TTS/encoder/utils/visual.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/model.py` & `coqui_tts-0.23.1/TTS/model.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/server/README.md` & `coqui_tts-0.23.1/TTS/server/README.md`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/server/server.py` & `coqui_tts-0.23.1/TTS/server/server.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/server/static/coqui-log-green-TTS.png` & `coqui_tts-0.23.1/TTS/server/static/coqui-log-green-TTS.png`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/server/templates/details.html` & `coqui_tts-0.23.1/TTS/server/templates/details.html`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/server/templates/index.html` & `coqui_tts-0.23.1/TTS/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/__init__.py` & `coqui_tts-0.23.1/TTS/tts/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/align_tts_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/align_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/bark_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/bark_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/delightful_tts_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/delightful_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/fast_pitch_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/fast_pitch_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/fast_speech_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/fast_speech_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/fastspeech2_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/fastspeech2_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/glow_tts_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/glow_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/neuralhmm_tts_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/neuralhmm_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/overflow_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/overflow_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/shared_configs.py` & `coqui_tts-0.23.1/TTS/tts/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/speedy_speech_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/speedy_speech_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/tacotron2_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/tacotron2_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/tacotron_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/tacotron_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/tortoise_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/tortoise_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/vits_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/vits_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/configs/xtts_config.py` & `coqui_tts-0.23.1/TTS/tts/configs/xtts_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/datasets/__init__.py` & `coqui_tts-0.23.1/TTS/tts/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/datasets/dataset.py` & `coqui_tts-0.23.1/TTS/tts/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/datasets/formatters.py` & `coqui_tts-0.23.1/TTS/tts/datasets/formatters.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/align_tts/duration_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/align_tts/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/align_tts/mdn.py` & `coqui_tts-0.23.1/TTS/tts/layers/align_tts/mdn.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/hubert_manager.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/hubert_manager.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/kmeans_hubert.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/kmeans_hubert.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/tokenizer.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/hubert/tokenizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/inference_funcs.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/inference_funcs.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/load_model.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/load_model.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/model.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/model.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/bark/model_fine.py` & `coqui_tts-0.23.1/TTS/tts/layers/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/acoustic_model.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/acoustic_model.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conformer.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/conformer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conv_layers.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/conv_layers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/encoders.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/encoders.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/energy_adaptor.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/energy_adaptor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/kernel_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/kernel_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/networks.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/networks.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/pitch_adaptor.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/pitch_adaptor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/variance_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/delightful_tts/variance_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/feed_forward/decoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/feed_forward/decoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/feed_forward/duration_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/feed_forward/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/feed_forward/encoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/feed_forward/encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/aligner.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/aligner.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/gated_conv.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/gated_conv.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/normalization.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/normalization.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/pos_encoding.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/pos_encoding.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/res_conv_bn.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/res_conv_bn.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/time_depth_sep_conv.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/time_depth_sep_conv.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/transformer.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/transformer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/generic/wavenet.py` & `coqui_tts-0.23.1/TTS/tts/layers/generic/wavenet.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/decoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/glow_tts/decoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/duration_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/glow_tts/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/encoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/glow_tts/encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/glow.py` & `coqui_tts-0.23.1/TTS/tts/layers/glow_tts/glow.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/transformer.py` & `coqui_tts-0.23.1/TTS/tts/layers/glow_tts/transformer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/losses.py` & `coqui_tts-0.23.1/TTS/tts/layers/losses.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/overflow/common_layers.py` & `coqui_tts-0.23.1/TTS/tts/layers/overflow/common_layers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/overflow/decoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/overflow/decoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/overflow/neural_hmm.py` & `coqui_tts-0.23.1/TTS/tts/layers/overflow/neural_hmm.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/overflow/plotting_utils.py` & `coqui_tts-0.23.1/TTS/tts/layers/overflow/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tacotron/attentions.py` & `coqui_tts-0.23.1/TTS/tts/layers/tacotron/attentions.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tacotron/capacitron_layers.py` & `coqui_tts-0.23.1/TTS/tts/layers/tacotron/capacitron_layers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tacotron/common_layers.py` & `coqui_tts-0.23.1/TTS/tts/layers/tacotron/common_layers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tacotron/gst_layers.py` & `coqui_tts-0.23.1/TTS/tts/layers/tacotron/gst_layers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron.py` & `coqui_tts-0.23.1/TTS/tts/layers/tacotron/tacotron.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron2.py` & `coqui_tts-0.23.1/TTS/tts/layers/tacotron/tacotron2.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/arch_utils.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/arch_utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/audio_utils.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/audio_utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/autoregressive.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/autoregressive.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/classifier.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/classifier.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/clvp.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/clvp.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/diffusion.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion_decoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/diffusion_decoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/dpm_solver.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/random_latent_generator.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/random_latent_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/tokenizer.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/tokenizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/transformer.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/transformer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/utils.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/vocoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/vocoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/wav2vec_alignment.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/wav2vec_alignment.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/tortoise/xtransformers.py` & `coqui_tts-0.23.1/TTS/tts/layers/tortoise/xtransformers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/vits/discriminator.py` & `coqui_tts-0.23.1/TTS/tts/layers/vits/discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/vits/networks.py` & `coqui_tts-0.23.1/TTS/tts/layers/vits/networks.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/vits/stochastic_duration_predictor.py` & `coqui_tts-0.23.1/TTS/tts/layers/vits/stochastic_duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/vits/transforms.py` & `coqui_tts-0.23.1/TTS/tts/layers/vits/transforms.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/dvae.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/dvae.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/gpt.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt_inference.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/gpt_inference.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/hifigan_decoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/hifigan_decoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/latent_encoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/latent_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/perceiver_encoder.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/perceiver_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/stream_generator.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/stream_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/tokenizer.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/tokenizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/dataset.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/trainer/dataset.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/gpt_trainer.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/trainer/gpt_trainer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/xtts_manager.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/xtts_manager.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/layers/xtts/zh_num2words.py` & `coqui_tts-0.23.1/TTS/tts/layers/xtts/zh_num2words.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/__init__.py` & `coqui_tts-0.23.1/TTS/tts/models/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/align_tts.py` & `coqui_tts-0.23.1/TTS/tts/models/align_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/bark.py` & `coqui_tts-0.23.1/TTS/tts/models/bark.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/base_tacotron.py` & `coqui_tts-0.23.1/TTS/tts/models/base_tacotron.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/base_tts.py` & `coqui_tts-0.23.1/TTS/tts/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/delightful_tts.py` & `coqui_tts-0.23.1/TTS/tts/models/delightful_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/forward_tts.py` & `coqui_tts-0.23.1/TTS/tts/models/forward_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/glow_tts.py` & `coqui_tts-0.23.1/TTS/tts/models/glow_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/neuralhmm_tts.py` & `coqui_tts-0.23.1/TTS/tts/models/neuralhmm_tts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/overflow.py` & `coqui_tts-0.23.1/TTS/tts/models/overflow.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/tacotron.py` & `coqui_tts-0.23.1/TTS/tts/models/tacotron.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/tacotron2.py` & `coqui_tts-0.23.1/TTS/tts/models/tacotron2.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/tortoise.py` & `coqui_tts-0.23.1/TTS/tts/models/tortoise.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/vits.py` & `coqui_tts-0.23.1/TTS/tts/models/vits.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/models/xtts.py` & `coqui_tts-0.23.1/TTS/tts/models/xtts.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/assets/tortoise/tokenizer.json` & `coqui_tts-0.23.1/TTS/tts/utils/assets/tortoise/tokenizer.json`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/data.py` & `coqui_tts-0.23.1/TTS/tts/utils/data.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/fairseq.py` & `coqui_tts-0.23.1/TTS/tts/utils/fairseq.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/helpers.py` & `coqui_tts-0.23.1/TTS/tts/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/languages.py` & `coqui_tts-0.23.1/TTS/tts/utils/languages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 import fsspec
 import numpy as np
 import torch
 from coqpit import Coqpit
 
 from TTS.config import check_config_and_model_args
@@ -81,26 +81,26 @@
 
         Args:
             file_path (str): Path to the output file.
         """
         self._save_json(file_path, self.name_to_id)
 
     @staticmethod
-    def init_from_config(config: Coqpit) -> "LanguageManager":
+    def init_from_config(config: Coqpit) -> Optional["LanguageManager"]:
         """Initialize the language manager from a Coqpit config.
 
         Args:
             config (Coqpit): Coqpit config.
         """
-        language_manager = None
         if check_config_and_model_args(config, "use_language_embedding", True):
             if config.get("language_ids_file", None):
-                language_manager = LanguageManager(language_ids_file_path=config.language_ids_file)
-            language_manager = LanguageManager(config=config)
-        return language_manager
+                return LanguageManager(language_ids_file_path=config.language_ids_file)
+            # Fall back to parse language IDs from the config
+            return LanguageManager(config=config)
+        return None
 
 
 def _set_file_path(path):
     """Find the language_ids.json under the given path or the above it.
     Intended to band aid the different paths returned in restored and continued training."""
     path_restore = os.path.join(os.path.dirname(path), "language_ids.json")
     path_continue = os.path.join(path, "language_ids.json")
```

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/managers.py` & `coqui_tts-0.23.1/TTS/tts/utils/managers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/measures.py` & `coqui_tts-0.23.1/TTS/tts/utils/measures.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.c` & `coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/core.c`

 * *Files 2% similar despite different names*

```diff
@@ -1110,177 +1110,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":688
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":695
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":702
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":712
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1311,42 +1311,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3244,15 +3244,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_t_xs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_t_ys, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3261,29 +3261,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":732
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3294,15 +3294,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3311,29 +3311,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3344,15 +3344,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3361,29 +3361,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3394,15 +3394,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3411,29 +3411,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3444,15 +3444,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3461,29 +3461,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3494,89 +3494,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":748
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3584,33 +3584,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":927
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3618,96 +3618,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":933
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3723,15 +3723,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3739,53 +3739,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":940
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -3793,30 +3793,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3831,15 +3831,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3855,15 +3855,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3871,53 +3871,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":946
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -3925,30 +3925,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3963,15 +3963,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3987,15 +3987,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4003,53 +4003,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":952
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -4057,30 +4057,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
+    /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4095,176 +4095,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":964
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":976
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":964
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":979
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":991
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":994
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1001
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1004
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1008
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1011
+/* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1015
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18201,26 +18201,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-pb4l9q1q/lib/python3.9/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 948, __pyx_L1_error)
```

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.pyx` & `coqui_tts-0.23.1/TTS/tts/utils/monotonic_align/core.pyx`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/speakers.py` & `coqui_tts-0.23.1/TTS/tts/utils/speakers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/ssim.py` & `coqui_tts-0.23.1/TTS/tts/utils/ssim.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/synthesis.py` & `coqui_tts-0.23.1/TTS/tts/utils/synthesis.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/bangla/phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/bangla/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/belarusian/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/characters.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/characters.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/numbers.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/numbers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/cleaners.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/cmudict.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/cmudict.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/english/abbreviations.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/english/abbreviations.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/english/number_norm.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/english/number_norm.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/english/time_norm.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/english/time_norm.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/french/abbreviations.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/french/abbreviations.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/japanese/phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/japanese/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/korean/ko_dictionary.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/korean/ko_dictionary.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/korean/korean.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/korean/korean.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/korean/phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/korean/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/__init__.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/base.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/base.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/espeak_wrapper.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/gruut_wrapper.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/multi_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/punctuation.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/punctuation.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/text/tokenizer.py` & `coqui_tts-0.23.1/TTS/tts/utils/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/tts/utils/visual.py` & `coqui_tts-0.23.1/TTS/tts/utils/visual.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/audio/numpy_transforms.py` & `coqui_tts-0.23.1/TTS/utils/audio/numpy_transforms.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/audio/processor.py` & `coqui_tts-0.23.1/TTS/utils/audio/processor.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/audio/torch_transforms.py` & `coqui_tts-0.23.1/TTS/utils/audio/torch_transforms.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/callbacks.py` & `coqui_tts-0.23.1/TTS/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/capacitron_optimizer.py` & `coqui_tts-0.23.1/TTS/utils/capacitron_optimizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/distribute.py` & `coqui_tts-0.23.1/TTS/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/download.py` & `coqui_tts-0.23.1/TTS/utils/download.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/downloaders.py` & `coqui_tts-0.23.1/TTS/utils/downloaders.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/generic_utils.py` & `coqui_tts-0.23.1/TTS/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/io.py` & `coqui_tts-0.23.1/TTS/utils/io.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/manage.py` & `coqui_tts-0.23.1/TTS/utils/manage.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/radam.py` & `coqui_tts-0.23.1/TTS/utils/radam.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/samplers.py` & `coqui_tts-0.23.1/TTS/utils/samplers.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/synthesizer.py` & `coqui_tts-0.23.1/TTS/utils/synthesizer.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/training.py` & `coqui_tts-0.23.1/TTS/utils/training.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/utils/vad.py` & `coqui_tts-0.23.1/TTS/utils/vad.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/configs/freevc_config.py` & `coqui_tts-0.23.1/TTS/vc/configs/freevc_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/configs/shared_configs.py` & `coqui_tts-0.23.1/TTS/vc/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/models/__init__.py` & `coqui_tts-0.23.1/TTS/vc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/models/base_vc.py` & `coqui_tts-0.23.1/TTS/vc/models/base_vc.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/models/freevc.py` & `coqui_tts-0.23.1/TTS/vc/models/freevc.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/commons.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/commons.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/mel_processing.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/mel_processing.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/modules.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/modules.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/audio.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/audio.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/hparams.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/hparams.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/__init__.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/config.json` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/config.json`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/modules.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/modules.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/wavlm.py` & `coqui_tts-0.23.1/TTS/vc/modules/freevc/wavlm/wavlm.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/README.md` & `coqui_tts-0.23.1/TTS/vocoder/README.md`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/__init__.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/fullband_melgan_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/fullband_melgan_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/hifigan_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/hifigan_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/melgan_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/melgan_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/multiband_melgan_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/multiband_melgan_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/parallel_wavegan_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/parallel_wavegan_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/shared_configs.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/univnet_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/univnet_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/wavegrad_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/wavegrad_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/configs/wavernn_config.py` & `coqui_tts-0.23.1/TTS/vocoder/configs/wavernn_config.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/datasets/__init__.py` & `coqui_tts-0.23.1/TTS/vocoder/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/datasets/gan_dataset.py` & `coqui_tts-0.23.1/TTS/vocoder/datasets/gan_dataset.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/datasets/preprocess.py` & `coqui_tts-0.23.1/TTS/vocoder/datasets/preprocess.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/datasets/wavegrad_dataset.py` & `coqui_tts-0.23.1/TTS/vocoder/datasets/wavegrad_dataset.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/datasets/wavernn_dataset.py` & `coqui_tts-0.23.1/TTS/vocoder/datasets/wavernn_dataset.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/hifigan.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/hifigan.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/losses.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/losses.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/lvc_block.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/lvc_block.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/melgan.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/melgan.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/parallel_wavegan.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/parallel_wavegan.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/pqmf.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/pqmf.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/upsample.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/layers/wavegrad.py` & `coqui_tts-0.23.1/TTS/vocoder/layers/wavegrad.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/__init__.py` & `coqui_tts-0.23.1/TTS/vocoder/models/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/base_vocoder.py` & `coqui_tts-0.23.1/TTS/vocoder/models/base_vocoder.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/fullband_melgan_generator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/fullband_melgan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/gan.py` & `coqui_tts-0.23.1/TTS/vocoder/models/gan.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/hifigan_discriminator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/hifigan_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/hifigan_generator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/hifigan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/melgan_discriminator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/melgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/melgan_generator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/melgan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/melgan_multiscale_discriminator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/melgan_multiscale_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/multiband_melgan_generator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/multiband_melgan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_discriminator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/parallel_wavegan_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_generator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/parallel_wavegan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/random_window_discriminator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/random_window_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/univnet_discriminator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/univnet_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/univnet_generator.py` & `coqui_tts-0.23.1/TTS/vocoder/models/univnet_generator.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/wavegrad.py` & `coqui_tts-0.23.1/TTS/vocoder/models/wavegrad.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/models/wavernn.py` & `coqui_tts-0.23.1/TTS/vocoder/models/wavernn.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/utils/distribution.py` & `coqui_tts-0.23.1/TTS/vocoder/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/TTS/vocoder/utils/generic_utils.py` & `coqui_tts-0.23.1/TTS/vocoder/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/coqui_tts.egg-info/PKG-INFO` & `coqui_tts-0.23.1/coqui_tts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coqui-tts
-Version: 0.23.0
+Version: 0.23.1
 Summary: Deep learning for Text to Speech.
 Home-page: https://github.com/idiap/coqui-ai-TTS
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 Maintainer: Enno Hermann
 Maintainer-email: enno.hermann@gmail.com
 License: MPL-2.0
@@ -13,26 +13,27 @@
 Project-URL: Repository, https://github.com/idiap/coqui-ai-TTS
 Project-URL: Discussions, https://github.com/idiap/coqui-ai-TTS/discussions
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9.0, <3.12
+Requires-Python: >=3.9.0, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: cython>=0.29.30
 Requires-Dist: scipy>=1.11.2
 Requires-Dist: torch>=2.1
 Requires-Dist: torchaudio
@@ -43,15 +44,15 @@
 Requires-Dist: anyascii>=0.3.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fsspec[http]>=2023.6.0
 Requires-Dist: packaging>=23.1
 Requires-Dist: pysbd>=0.3.4
 Requires-Dist: umap-learn>=0.5.1
 Requires-Dist: matplotlib>=3.7.0
-Requires-Dist: trainer>=0.0.36
+Requires-Dist: coqui-tts-trainer>=0.1
 Requires-Dist: coqpit>=0.0.16
 Requires-Dist: jieba
 Requires-Dist: pypinyin
 Requires-Dist: hangul_romanize
 Requires-Dist: gruut[de,es,fr]==2.2.3
 Requires-Dist: jamo
 Requires-Dist: g2pkk>=0.1.1
@@ -66,30 +67,30 @@
 Provides-Extra: all
 Requires-Dist: black==24.2.0; extra == "all"
 Requires-Dist: coverage[toml]; extra == "all"
 Requires-Dist: nose2; extra == "all"
 Requires-Dist: ruff==0.3.0; extra == "all"
 Requires-Dist: bokeh==1.4.0; extra == "all"
 Requires-Dist: pandas<2.0,>=1.4; extra == "all"
-Requires-Dist: mecab-python3==1.0.6; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
 Requires-Dist: unidic-lite==1.0.8; extra == "all"
 Requires-Dist: cutlet; extra == "all"
 Requires-Dist: flask>=2.0.1; extra == "all"
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: nose2; extra == "dev"
 Requires-Dist: ruff==0.3.0; extra == "dev"
 Provides-Extra: notebooks
 Requires-Dist: bokeh==1.4.0; extra == "notebooks"
 Requires-Dist: pandas<2.0,>=1.4; extra == "notebooks"
 Provides-Extra: server
 Requires-Dist: flask>=2.0.1; extra == "server"
 Provides-Extra: ja
-Requires-Dist: mecab-python3==1.0.6; extra == "ja"
+Requires-Dist: mecab-python3; extra == "ja"
 Requires-Dist: unidic-lite==1.0.8; extra == "ja"
 Requires-Dist: cutlet; extra == "ja"
 
 
 ## 🐸Coqui TTS News
 - 📣 Fork of the [original, unmaintained repository](https://github.com/coqui-ai/TTS). New PyPI package: [coqui-tts](https://pypi.org/project/coqui-tts)
 - 📣 ⓍTTSv2 is here with 16 languages and better performance across the board.
@@ -218,15 +219,15 @@
 
 ### Voice Conversion
 - FreeVC: [paper](https://arxiv.org/abs/2210.15418)
 
 You can also help us implement more models.
 
 ## Installation
-🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.12.**.
+🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.13.**.
 
 If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the released 🐸TTS models, installing from PyPI is the easiest option.
 
 ```bash
 pip install coqui-tts
 ```
```

### Comparing `coqui_tts-0.23.0/coqui_tts.egg-info/SOURCES.txt` & `coqui_tts-0.23.1/coqui_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/coqui_tts.egg-info/requires.txt` & `coqui_tts-0.23.1/coqui_tts.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 anyascii>=0.3.0
 pyyaml>=6.0
 fsspec[http]>=2023.6.0
 packaging>=23.1
 pysbd>=0.3.4
 umap-learn>=0.5.1
 matplotlib>=3.7.0
-trainer>=0.0.36
+coqui-tts-trainer>=0.1
 coqpit>=0.0.16
 jieba
 pypinyin
 hangul_romanize
 gruut[de,es,fr]==2.2.3
 jamo
 g2pkk>=0.1.1
@@ -34,27 +34,27 @@
 [all]
 black==24.2.0
 coverage[toml]
 nose2
 ruff==0.3.0
 bokeh==1.4.0
 pandas<2.0,>=1.4
-mecab-python3==1.0.6
+mecab-python3
 unidic-lite==1.0.8
 cutlet
 flask>=2.0.1
 
 [dev]
 black==24.2.0
 coverage[toml]
 nose2
 ruff==0.3.0
 
 [ja]
-mecab-python3==1.0.6
+mecab-python3
 unidic-lite==1.0.8
 cutlet
 
 [notebooks]
 bokeh==1.4.0
 pandas<2.0,>=1.4
```

### Comparing `coqui_tts-0.23.0/images/coqui-log-green-TTS.png` & `coqui_tts-0.23.1/images/coqui-log-green-TTS.png`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/images/example_model_output.png` & `coqui_tts-0.23.1/images/example_model_output.png`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/images/model.png` & `coqui_tts-0.23.1/images/model.png`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/pyproject.toml` & `coqui_tts-0.23.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coqui_tts-0.23.0/requirements.txt` & `coqui_tts-0.23.1/requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # deps for inference
 pysbd>=0.3.4
 # deps for notebooks
 umap-learn>=0.5.1
 # deps for training
 matplotlib>=3.7.0
 # coqui stack
-trainer>=0.0.36
+coqui-tts-trainer>=0.1
 # config management
 coqpit>=0.0.16
 # chinese g2p deps
 jieba
 pypinyin
 # korean
 hangul_romanize
```

### Comparing `coqui_tts-0.23.0/setup.py` & `coqui_tts-0.23.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,18 @@
 import subprocess
 import sys
 
 import numpy
 import setuptools.command.build_py
 import setuptools.command.develop
 from Cython.Build import cythonize
-from packaging.version import Version
 from setuptools import Extension, find_packages, setup
 
-python_version = sys.version.split()[0]
-if Version(python_version) < Version("3.9") or Version(python_version) >= Version("3.12"):
-    raise RuntimeError("TTS requires python >= 3.9 and < 3.12 " "but your Python version is {}".format(sys.version))
-
+if sys.version_info < (3, 9) or sys.version_info >= (3, 13):
+    raise RuntimeError("Trainer requires python >= 3.6 and <3.13 " "but your Python version is {}".format(sys.version))
 
 cwd = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(cwd, "TTS", "VERSION")) as fin:
     version = fin.read().strip()
 
 
 class build_py(setuptools.command.build_py.build_py):  # pylint: disable=too-many-ancestors
@@ -117,22 +114,23 @@
     extras_require={
         "all": requirements_all,
         "dev": requirements_dev,
         "notebooks": requirements_notebooks,
         "server": requirements_server,
         "ja": requirements_ja,
     },
-    python_requires=">=3.9.0, <3.12",
+    python_requires=">=3.9.0, <3.13",
     entry_points={"console_scripts": ["tts=TTS.bin.synthesize:main", "tts-server = TTS.server.server:main"]},
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Operating System :: POSIX :: Linux",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

